<!--
{
    "source": "https://docs.joomla.org/Adding_www_to_a_url",
    "title": "A' cur www ri URL",
    "description": " ",
    "author": ""
}
-->

## Abairtean cunbhalach Apache .htaccess

Airson fuasgladh sìmplidh, cuir na leanas ris an fhaidhle `.htaccess` agad:

```bash
    RewriteEngine On
    RewriteCond %{HTTP_HOST} !^(www\.example\.com)?$ [NC]
    RewriteRule (.*) https://www.example.com/$1 [R=301,L]
```

Anns a' chùis seo, thèid URL den chruth `https://example.com/index.php?item=1` ath-stiùireadh gu `https://www.example.com/index.php?item=1`.

Anns an eisimpleir gu h-àrd:

* Tha `RewriteCond` a' mìneachadh cumha deuchainn.
* Bidh `%{HTTP_HOST}` a' cleachdadh caochladair an òstair bhon iarrtas (example.com).
* Tha `!` a' ciallachadh CHAN EIL agus tha `^` a' ciallachadh TOISEACH - mar sin, chan eil e a' tòiseachadh le www.example.com
* Bidh `(` agus `)` a' glacadh rud sam bith a tha eadar na camagan airson a chleachdadh ann an iomradh air ais.
* Bidh `\` a' tionndadh an ath charactair bho charactar smachd gu fìor charactar.
* Mar as trice tha `.` a' ciallachadh caractar sam bith, ach nuair a tha \ roimhe tha e a' ciallachadh puing.
* Bidh `?` a' dèanamh a' mhaidseadh roghainneil.
* Tha `$` a' ciallachadh CRÌOCH (a' mhaidseadh roghainneil).
* Tha `[NC]` a' seasamh airson No Case, a' ciallachadh nach eil e mothachail do chùis-litrichean.
* Tha `RewriteRule` dligheach mura tòisich an URL le www.
* Tha `(.*)` na phàtran; sa chùis seo, caractar singilte air ath-aithris 0 no barrachd
    thursan, a' ciallachadh pàirt na slighe den URL. Tha e air a ghlacadh mar $1.
* `https://www.example.com/` na àite an àite pàirt an òstair den URL.
* Is e `$1` an t-slighe a chaidh a ghlacadh.
* Tha `[]` a' gabhail a-steach brataichean - stiùiridhean air dè nì thu.
* Tha `R=301` na stiùireadh airson bann-cinn Moved Permanently a chur.
* Tha `L` a' ciallachadh Last san t-seata - leis gun deach maids a lorg, leig seachad riaghailtean sam bith a thig às a dhèidh.

Fuasgladh nas coileanta a bhios a' ceartachadh grunn chùisean canonaigeach eile
aig an aon àm:

    RewriteEngine On
    #
    RewriteCond %{THE_REQUEST} ^[A-Z]{3,9}\ /([^/]+/)*index\.html?\ HTTP/
    RewriteRule ^(([^/]+/)*)index\.html?$ http://www.example.com/$1 [R=301,L]
    #
    RewriteCond %{THE_REQUEST} !^POST
    RewriteCond %{THE_REQUEST} ^[A-Z]{3,9}\ /([^/]+/)*index\.php\ HTTP/
    RewriteCond %{SERVER_PORT}>s ^(443>(s)|[0-9]+>s)$
    RewriteRule ^(([^/]+/)*)index\.php$ http%2://www.example.com/$1 [R=301,L]
    #
    RewriteCond %{HTTP_HOST} !^(www\.example\.com)?$
    RewriteRule (.*) http://www.example.com/$1 [R=301,L]

Ma tha thu airson tuigsinn dè tha seo uile a' ciallachadh, faodaidh tu na
h-artaigilean seo a leughadh:

* [Ro-ràdh do Apache mod_rewrite](https://httpd.apache.org/docs/2.4/rewrite/intro.html)
* [Ro-ràdh do dh'ath-stiùiridhean .htaccess](https://www.danielmorell.com/guides/htaccess-seo/redirects/introduction-to-redirects)

*Air eadar-theangachadh le openai.com*