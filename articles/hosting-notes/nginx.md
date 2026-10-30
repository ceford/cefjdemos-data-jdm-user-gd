<!--
{
    "source": "https://docs.joomla.org/Nginx",
    "title": "Nginx",
    "description": " ",
    "author": ""
}
-->

<a href="http://nginx.org/"
rel="nofollow noreferrer noopener">Is e frithealaiche-lìn aotrom a th’ ann an Nginx</a>
a tha a’ cumhachdachadh
<a href="https://en.wikipedia.org/wiki/Nginx"
rel="nofollow noreferrer noopener">mu 33%</a> de na
frithealaichean-lìn thar gach àrainn. Mura h-eil riatanasan sònraichte agad a
dh’iarras frithealaiche-lìn trom mar Apache, tha e fada nas fheàrr dhut
Nginx a chleachdadh.

Gu h-ìosal tha stiùireadh air mar a gheibh thu Joomla! ag obrachadh le <a
href="https://www.nginx.com/resources/wiki/start/topics/examples/phpfcgi/"
rel="nofollow noreferrer noopener">Eisimpleir PHP FastCGI</a>.

## Stàlaich Nginx

Air Ubuntu, ruith *aptitude install Nginx*. Airson sgaoilidhean eile, ruith
manaidsear nam pasganan iomchaidh no faic <a
href="https://www.nginx.com/resources/wiki/start/topics/tutorials/install/"
rel="nofollow noreferrer noopener">duilleag stàlaidh Nginx</a>.

## Stàlaich PHP FastCGI

Air Ubuntu, leugh <a
href="https://www.nginx.com/resources/wiki/start/topics/examples/phpfcgi/"
rel="nofollow noreferrer noopener">Eisimpleir PHP FastCGI</a>.

Air Gentoo, ruithidh PHP mar sheirbheis FastCGI (FPM), agus mar sin
ruithidh frithealaiche Nginx PHP mar phròiseas air leth:

    # echo "dev-lang/php gd gd2 curl simplexml tokenizer dom tidy sqlite xml fpm cgi" >> /etc/portage/package.use
    # emerge php

Tha na roghainnean bunaiteach aig PHP-FPM math airson a’ mhòr-chuid de na
frithealaichean. Airson rèiteachaidhean sònraichte, tadhail air an
<a href="http://php.net/manual/en/install.fpm.php"
rel="nofollow noreferrer noopener">làrach PHP FPM</a>.

## Rèitich Nginx

Tha faidhlichean rèiteachaidh Nginx ann an:

- `/etc/nginx/sites-available/` air Ubuntu (airson làraichean a tha a’ ruith air an
  eisimpleir Nginx sin)
- `/etc/nginx/nginx.conf` air Gentoo agus Raspbian (Debian air a
  leasachadh airson Raspberry Pi)

Seo faidhle rèiteachaidh sampall Nginx, *joomla.conf*, a ghabhas
ath-chleachdadh thar nan làraichean agad uile aig a bheil Nginx an comas.

    server {
      listen 80;
        server_name YOUR_DOMAIN;
        server_name_in_redirect off;

        access_log /var/log/nginx/localhost.access_log;
        error_log /var/log/nginx/localhost.error_log info;

        root PATH_ON_SERVER;
        index index.php index.html index.htm default.html default.htm;
        # Support Clean (aka Search Engine Friendly) URLs
        location / {
            try_files $uri $uri/ /index.php?$args;
        }

        # add global x-content-type-options header
        add_header X-Content-Type-Options nosniff;

        # deny running scripts inside writable directories
        location ~* /(images|cache|media|logs|tmp)/.*\.(php|pl|py|jsp|asp|sh|cgi)$ {
            return 403;
            error_page 403 /403_error.html;
        }

        location ~ \.php$ {
          fastcgi_pass  127.0.0.1:9000;
          fastcgi_index index.php;
          include fastcgi_params;
          fastcgi_param SCRIPT_FILENAME $document_root$fastcgi_script_name;
          include /etc/nginx/fastcgi.conf;
        }

        # caching of files
        location ~* \.(ico|pdf|flv)$ {
            expires 1y;
        }

        location ~* \.(js|css|png|jpg|jpeg|gif|swf|xml|txt)$ {
            expires 14d;
        }

    }

Thoir aire do ghrunn rudan:

1.  Tha am paramadair *fastcgi_pass* suidhichte aig *127.0.0.1:9000*,
    a’ freagairt ris a’ phort air a bheil FPM air a rèiteachadh gus èisteachd. Tha
    seo a’ ciallachadh gun urrainn dhut pròiseasan PHP a ruith air
    frithealaichean fa leth. Air Gentoo, gheibh thu an rèiteachadh seo san
    fhaidhle */etc/php/fpm-php5.3/php-fpm.conf/*.
2.  Na dìochuimhnich YOUR_DOMAIN agus PATH_ON_SERVER gu h-àrd a chur nan àite,
    a rèir d’ àrainn agus slighe Joomla air an fhrithealaiche agad.

## Taic GZip

Ma tha feum agad air taic airson dùmhlachadh GZip, cuir an earrann a leanas
ris an earrann *http* de phrìomh fhaidhle rèiteachaidh Nginx:

    gzip on;
    gzip_http_version 1.1;
    gzip_comp_level 6;
    gzip_min_length 1100;
    gzip_buffers 4 8k;
    gzip_types text/plain application/xhtml+xml text/css application/xml application/xml+rss text/javascript application/javascript application/x-javascript
    gzip_proxied any;
    gzip_disable "MSIE [1-6]\.";

## Tùsan

- <a href="https://wiki.gentoo.org/wiki/Nginx"
rel="nofollow noreferrer noopener">Nginx ann an Gentoo</a>
- <a href="https://kevinworthington.com/nginx-for-windows/"
  rel="nofollow noreferrer noopener">Nginx airson Windows</a>
- <a
  href="https://ubuntu.com/tutorials/install-and-configure-nginx#1-overview"
  rel="nofollow noreferrer noopener">Nginx ann an Ubuntu</a>
- <a
  href="https://www.debianadmin.com/howto-install-nginx-webserver-in-debian.html"
  rel="nofollow noreferrer noopener">Nginx ann an Debian</a>
- <a href="https://www.php.net/manual/en/install.fpm.php"
  rel="nofollow noreferrer noopener">Stàladh agus rèiteachadh PHP-FPM</a>
- <a
  href="https://docs.nginx.com/nginx/admin-guide/web-server/compression/"
  rel="nofollow noreferrer noopener">Dùmhlachadh agus dì-dhùmhlachadh</a>
- <a href="https://www.nginx.com/blog/creating-nginx-rewrite-rules/"
  rel="nofollow noreferrer noopener">Cruthachadh riaghailtean ath-sgrìobhaidh NGINX</a>
- <a href="http://nginx.org/en/docs/http/request_processing.html"
  rel="nofollow noreferrer noopener">Mar a làimhsicheas Nginx iarrtas</a>

*Air eadar-theangachadh le openai.com*