<!--
{
    "source": "https://docs.joomla.org/Installing_Joomla_on_a_Raspberry_Pi",
    "title": "St\u00e0ladh Raspberry Pi",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

**Nòta: Chan eil an sgrìobhainn seo coileanta no làn dheuchainn fhathast.**

Tha an <a href="https://www.raspberrypi.org/"
rel="nofollow noreferrer noopener">Raspberry Pi</a> na
choimpiutair beag air aon bhòrd a chaidh a leasachadh an toiseach gus
teagasg saidheans coimpiutaireachd bunaiteach a bhrosnachadh ann an sgoiltean
agus dùthchannan fo leasachadh. Air sgàth a shùbailteachd, tha e air fàs gu
math mòr-chòrdte agus tha e air a chleachdadh mar chluicheadair mheadhanan,
frithealaiche beag neo-eisimeileach, msaa. Faodaidh tu a chleachdadh mar
fhrithealaiche-lìn agus Joomla! a stàladh air. Tha an duilleag seo a’ sealltainn
dhut mar a chuireas tu làrach-lìn Joomla! agad ag obair air an Raspberry Pi.

## Bathar-cruaidh

- **Raspberry Pi tionndadh 3 Model B** - Tha diofar mhodailean de
  Raspberry Pi ann. Faodaidh tu a’ mhòr-chuid de na modailean aig a bheil
  port Ethernet (na seòrsaichean Model B) a chleachdadh. Ach airson
  coileanadh nas fheàrr, cleachdaidh sinn an tionndadh as ùire leis a’ mhòr-chuid
  de chuimhne RAM.
- **Cairt micro SD** - Airson an t-siostaim-obrachaidh + an fhrithealaiche-lìn
  + Joomla. (Cleachdaidh RPi tionndadh 3 model B micro SD; dh’fhaodadh gun
  cleachd tionndaidhean eile cairtean SD àbhaisteach)
- **Adaptair 5 Volt (1 Amp)** - Gus cumhachd a thoirt don Raspberry Pi,
  feumaidh tu cumhachd an lìonraidh (230V no 110V) atharrachadh gu 5 Volt.
  Feumaidh an Raspberry Pi mu 1 Amp, agus ’s dòcha barrachd ma cheanglas tu
  uidheaman USB ris.
- **Càball Ethernet àbhaisteach** - gus an RPi a cheangal ris an Lìonra
  Sgìre Ionadail agad / an rothaiche / an t-eadar-lìon.

## A’ Stàladh an t-Siostaim-Obrachaidh

Tha an siostam-obrachaidh Raspbian na dhreach de Debian Linux a chaidh a
chruinneachadh gu sònraichte airson an Raspberry Pi. Tha dà dhreach de
<a href="https://www.raspberrypi.com/software/"
rel="nofollow noreferrer noopener">Raspbian</a> rim faighinn: **Raspbian
Jessie le Pixel Lite** (dreach leis an deasg PIXEL stèidhichte air Debian
Jessie) agus **Raspbian Jessie Lite** (dreach as lugha stèidhichte air Debian
Jessie). Leis gu bheil sinn a’ cleachdadh an Raspberry Pi mar fhrithealaiche-lìn
airson Joomla, cha bhi feum againn air an GUI.

**Luchdaich a-nuas** <a href="https://www.raspberrypi.org/downloads/raspbian/"
rel="nofollow noreferrer noopener">Raspbian Jessie Lite</a> agus dì-dhùmhlaich
am faidhle a luchdaich thu a-nuas, m.e. **2016-09-23-raspbian-jessie-lite.zip**
(306 MB) gu **2016-09-23-raspbian-jessie-lite.img** (1.4 GB).

A-nis feumaidh sinn am faidhle .img a chopaigeadh dhan chairt SD (micro).
Faodaidh tu inneal le eadar-aghaidh grafaigeach a chleachdadh leithid
<a href="https://unetbootin.github.io/"
rel="nofollow noreferrer noopener">UNetbootin</a> (airson
Windows, Mac OS X agus Linux) no a dhèanamh air an loidhne-àithne).

**Bi faiceallach** nuair a sgrìobhas tu ìomhaigh diosc *.img* gu diosg eile.
Ma shònraicheas tu an diosg cheann-uidhe cheàrr, sgrìobhaidh tu thairis air
an diosg sin leis an *.img*, rud a nì an diosg sin do-dhèanta a chleachdadh,
agus a dh’adhbhraicheas call dàta.

### Windows

Ann an terminal (CMD), dèan sgrùdadh air dè an t-inneal a tha a’ freagairt ris
a’ Chairt SD agus dèan rudeigin mar:

```
    dd bs=1M if=c:\temp\2016-09-23-raspbian-jessie-lite.img od=[the device of your SD Card]
```

Faic cuideachd <a
href="https://www.raspberrypi.org/documentation/installation/installing-images/windows.md"
rel="nofollow noreferrer noopener">A’ Stàladh Ìomhaighean an t-Siostaim-
Obrachaidh a’ cleachdadh Windows</a>

### Apple OSX

Dèan sgrùdadh air dè an t-inneal a thathar a’ cleachdadh airson do Chairt SD.
Anns a’ chùis againn ’s e *disk1s1* a th’ ann agus nì sinn seo ann an
Terminal:

```
    sudo dd bs=1M if=~/Downloads/2016-09-23-raspbian-jessie-lite.img of=/dev/disk1s1
```

Faic cuideachd: <a
href="https://www.raspberrypi.org/documentation/installation/installing-images/mac.md"
rel="nofollow noreferrer noopener">A’ Stàladh Ìomhaighean an t-Siostaim-
Obrachaidh air MacOS</a>

### Linux

Ceanglaidh sinn leughadair Chairtean SD le a’ Chairt SD (micro) ri coimpiutair.
Le *dmesg* gheibh sinn ainm inneil na Cairte SD. Anns a’ chùis againn, tha
dmesg a’ sealltainn rudeigin mar `[xxxxxx.xxxxxxx]  sdd: sdd1 sdd2`, a’ ciallachadh
gu bheil Cairt SD againn le 2 phàirteachadh. Na sgrìobh ìomhaigh Raspbian gu
pàirteachadh ach dhan diosg slàn **sdd**.

Cleachdaidh sinn *dd* ("Dump Diosg") gus Faidhle In-chuir (*if*) a sgrìobhadh
gu Faidhle Toraidh (*of*) a’ cleachdadh Meud Bloc (*bs*) sònraichte.

**Bi faiceallach**: sgrìobhaidh *dd* gu inneal gun rabhadh sam bith.
Dèan sgrùdadh dùbailte gu bheil thu a’ sgrìobhadh dhan inneal cheart! Ma
sgrìobhas tu dhan diosg cheàrr, bidh cuimhne agad gu bràth air an àithne
*dd* mar an "Milleadair Diosg".

```bash
    sudo dd if=~/Downloads/2016-09-23-raspbian-jessie-lite.img of=/dev/sdd bs=4M
```

Faic cuideachd <a
href="https://www.raspberrypi.org/documentation/installation/installing-images/linux.md"
rel="nofollow noreferrer noopener">A’ Stàladh Ìomhaighean an t-Siostaim-
Obrachaidh air Linux</a>

**RABHADH airson tionndadh Raspbian Stretch** : gus am bi frithealaiche
SSH ag obair bhon bhròg, feumaidh tu faidhle falamh *ssh* a chruthachadh air
a’ phàirteachadh freumhaich.

## A’ Ceangal Raspberry Pi ri LAN

Nuair a bhios sinn air Siostam-Obrachaidh Raspbian a stàladh air a’ Chairt SD,
nì sinn na leanas:

- Cuir a’ chairt micro SD ann an slot na Cairt SD air an Raspberry Pi.
- Ceangail càball Ethernet ris an Raspberry Pi agus ris an Lìonra Sgìre
  Ionadail (ceangail ris an router againn e).
- Ceangail an solar cumhachd 5V ris an Raspberry Pi.

Bheir tòiseachadh an Raspberry Pi mu 30 diog. Feumaidh sinn an seòladh
IP a lorg gus ceangal ris a’ cleachdadh SSH. ’S urrainn dhuinn diofar
dhòighean a chleachdadh airson sin:

- log a-steach do dh’eadar-aghaidh-lìn an router agad agus coimhead suas
  na h-innealan ceangailte;
- cleachd fòn-làimhe a tha ceangailte ris an router wi-fi a’ cleachdadh
  App sganadh lìonra air a bheil **Fing Overlook**;
- cleachd àithne mar **nmap**. A’ gabhail ris gur e **192.168.0**.25 an
  seòladh IP aig a’ PC againn, ’s urrainn dhuinn a h-uile inneal eile san
  aon raon lìonraidh a lorg le bhith a’ dèanamh na leanas:
```
    sudo nmap -sP 192.168.0/24
```

A dh’fhaodadh am mion-fhiosrachadh a leanas a shealltainn:

    Starting Nmap 6.47 ( http://nmap.org ) at 2016-10-22 17:42 CEST
    Nmap scan report for 192.168.0.35
    Host is up (0.00042s latency).
    MAC Address: 42:42:42:42:42:42 (Raspberry Pi Foundation)

Gus logadh a-steach don Raspberry Pi againn, cleachdaidh sinn an àithne
**ssh**.

```
    ssh pi@192.168.0.35
```

A’ chiad turas a nì thu ceangal ris, seallaidh e rudeigin mar:

    The authenticity of host '192.168.0.35 (192.168.0.35)' can't be established.
    ECDSA key fingerprint is 42:42:42:42:42:42:42:42:42:42:42:42:42:42:42:42.
    Are you sure you want to continue connecting (yes/no)?

Taghaidh sinn **Yes**

    Warning: Permanently added 192.168.0.35 (ECDSA) to the list of known hosts.
    pi@192.168.0.35's password:

agus cleachdaidh sinn am *facal-faire bunaiteach*: *raspberry*, agus ma
shoirbhicheas leis an logadh a-steach seallaidh e:

    The programs included with the Debian GNU/Linux system are free software;
    the exact distribution terms for each program are described in the
    individual files in /usr/share/doc/*/copyright.

    Debian GNU/Linux comes with ABSOLUTELY NO WARRANTY, to the extent
    permitted by applicable law.
    pi@raspberrypi:~ $

’S urrainn dhuinn an Raspberry Pi a rèiteachadh a’ cleachdadh eadar-aghaidh
teacsa tro:

    sudo raspi-config

### Inneal Rèiteachaidh Bathar-bog Raspberry Pi (raspi-config)

Leis an inneal rèiteachaidh seo cha dèan sinn ach na roghainnean a leanas
atharrachadh.

#### 1 Leudaich an siostam-fhaidhlichean

Gu bunaiteach, tha an t-àite diosga air a’ Chairt SD den aon mheud ris an
fhaidhle .img 1.4GB a chleachd thu gus a’ chairt SD airson an Raspberry Pi
agad a chruthachadh. ’S urrainn dhut an roghainn seo a chleachdadh gus an
còrr den àite diosga fhaighinn.

#### 2 Atharraich Facal-faire a’ Chleachdaiche

Air sgàth adhbharan tèarainteachd, ’s fheàrr am **facal-faire bunaiteach**
"raspberry" atharrachadh cho luath ’s a ghabhas.

#### 3 Roghainnean Bròg

Bu toil leinn gun tòisicheadh an Raspberry Pi air a’ chonsòl Teacsa

##### B2 Logadh a-steach fèin-obrachail air a’ Chonsòl, consol teacsa, air logadh a-steach gu fèin-obrachail mar chleachdaiche 'pi'

#### 9 Roghainnean Adhartach

##### A3 Sgaradh na Cuimhne

Leis gum bi sinn a’ cleachdadh an Raspberry Pi mar fhrithealaiche gun
cheann-uidhe, gun a cheangal ri monitor, ’s urrainn dhuinn an cuimhne a
chleachdas an GPU a lùghdachadh bho 64 gu **16**

#### 5 Roghainnean Eadar-nàiseantachd

##### I2 Atharraich an Sòn-ama

Atharraichidh sinn an Sòn-ama chun an t-sòn-ama againn fhèin (m.e.
Europe/Amsterdam)

Às dèidh nan atharrachaidhean uile, nì sinn Ath-thòiseachadh air an
Raspberry Pi, agus logaidh sinn a-steach a-rithist leis an fhacal-faire ùr
againn.

    ssh pi@192.168.0.35

A-nis tha an t-àm ann a h-uile càil eile a stàladh.

## Ùraich am bathar-bog

Mus stàlaich sinn dad sam bith eile, nì sinn na leanas:

- **ùraich** liosta nan tionndaidhean bathar-bog bho na stòran
  taobh a-muigh uile
    sudo apt-get update

- **àrdaich** am bathar-bog stàlaichte uile
    sudo apt-get upgrade

**Bu chòir liosta nan tionndaidhean ùrachadh agus am bathar-bog uile
àrdachadh gu cunbhalach.**

## Frithealaiche-lìn Nginx

’S e roghainn luath agus aotrom eile an àite frithealaiche-lìn Apache am
frithealaiche-lìn **Nginx**, a tha a’ sìor fhàs mòr-chòrdte.

### Stàladh Nginx

Stàlaichidh sinn nginx agus a h-uile eisimeileachd (’s e sin: bathar-bog
a dh’fheumas nginx gus obrachadh) le

    sudo apt-get install nginx

Gheibh sinn teachdaireachd mar seo:

    Reading package lists... Done
    Building dependency tree
    Reading state information... Done
    The following extra packages will be installed:
     fontconfig-config fonts-dejavu-core libfontconfig1 libgd3 libjbig0 libtiff5 libvpx1 libxpm4 libxslt1.1 nginx-common nginx-full
    Suggested packages:
     libgd-tools fcgiwrap nginx-doc ssl-cert
    The following NEW packages will be installed:
     fontconfig-config fonts-dejavu-core libfontconfig1 libgd3 libjbig0 libtiff5 libvpx1 libxpm4 libxslt1.1 nginx nginx-common nginx-full
    0 upgraded, 12 newly installed, 0 to remove and 0 not upgraded.
    Need to get 3,550 kB of archives.
    After this operation, 8,666 kB of additional disk space will be used.
    Do you want to continue? [Y/n] y

Le bhith a’ taghadh “y”, thèid nginx agus na pacaidean riatanach uile a stàladh.

Faodaidh tu an stàladh a dhearbhadh le brabhsair. Rach gu seòladh IP
do Raspberry pi; nar cùis-ne,
<a href="http://192.168.0.35/"
rel="nofollow noreferrer noopener">http://192.168.0.35/</a> Bu chòir dhuinn
teachdaireachd mar seo fhaicinn:

    Welcome to nginx on Debian!
    If you see this page, the nginx web server is successfully installed and working on Debian. Further configuration is required.
    For online documentation and support please refer to nginx.org
    Please use the reportbug tool to report bugs in the nginx package with Debian.
    However, check existing bug reports before reporting a  new bug.
    Thank you for using debian and nginx.

#### A’ tòiseachadh agus a’ stad Nginx

Às dèidh an stàlaidh, tòisichear Nginx gu fèin-obrachail. Faodaidh tu:

- Stad Nginx: sudo service nginx stop
- Tòisich Nginx: sudo service nginx start
- Ath-thòisich Nginx: sudo service nginx restart

### Rèitich Nginx

#### Rèiteachadh cruinneil Nginx

Ann an rèiteachadh cruinneil Nginx, is urrainn dhuinn tasgadh bunaiteach
agus eile a rèiteachadh. Tha pròiseasar ARM Cortex-A53 **ceithir-chridheach**
64-bit aig 1.2 GHz aig an Raspberry Pi 3. Ma tha tionndadh nas tràithe
agad le nas lugha de chridheachan CPU, bu chòir dhut

    sudo nano /etc/nginx/nginx.conf

a chleachdadh gus na “worker_processes” atharrachadh a rèir na tha de
CPUan san uidheam agad. A ghnàth, tha e air a rèiteachadh mar

    worker_processes 4;

mar sin chan fheum thu atharrachadh airson Raspberry Pi 3.

Às dèidh dhut rèiteachadh Nginx no rèiteachadh àrainn bhiortail
atharrachadh, feumaidh tu

    sudo nginx reload

a ruith gus na h-atharrachaidhean a chur an gnìomh.

#### Àrainnean Bhiortail

Tha e comasach iomadh làrach-lìn Joomla a ruith air an aon fhrithealaiche
a’ cleachdadh àrainnean bhiortail.

Cuir gach làrach-lìn ann am pasgan fa leth anns an fhreumh-lìn bhunaiteach /var/www/,
mar eisimpleir:

- /var/www/example.com/
- /var/www/voorbeeld.nl/
    sudo mkdir /var/www/example.com
    sudo mkdir /var/www/voorbeeld.nl

Airson gach làrach, cruthaichidh sinn àrainn bhiortail, a tha gu bunaiteach na
fhaidhle teacsa le fiosrachadh sònraichte don àrainn:

- /etc/nginx/sites-available/example.com
    server {
    listen 80;
    server_name example.com www.example.com;
    root /var/www/example.com;

    access_log /var/log/nginx/example.com.access_log;
    error_log /var/log/nginx/example.com.error_log info;

    location / {
      index index.php index.html index.htm;
      }
    }

- /etc/nginx/sites-available/voorbeeld.nl
    server {
    listen 80;
    server_name voorbeeld.nl www.voorbeeld.nl;
    root /var/www/voorbeeld.nl;

    access_log /var/log/nginx/voorbeeld.nl.access_log;
    error_log /var/log/nginx/voorbeeld.nl.error_log info;

    location / {
      index index.php index.html index.htm;
      }
    }

Feumaidh sinn gach làrach a chur an comas le ceangal bho /etc/nginx/sites-enabled/
gu ruige na h-àrainn bhiortail ann an “sites-available”. Cruthaichidh sinn
ceangal samhlachail airson gach àrainn bhiortail:

    sudo ln -s /etc/nginx/sites-available/example.com /etc/nginx/sites-enabled/example.com
    sudo ln -s /etc/nginx/sites-available/voorbeeld.nl /etc/nginx/sites-enabled/voorbeeld.nl

Gus an rèiteachadh àrainn bhiortail seo a chur an gnìomh, ruithidh sinn

    sudo nginx reload

agus nuair a bhios a h-uile càil air a rèiteachadh mar bu chòir, freagraidh e:

    Reloading nginx configuration: nginx.

## Stòr-dàta

Is urrainn dhuinn MariaDB no MySQL a stàladh; obraichidh Joomla leis an dà
chlàr. Stàlaichidh sinn MariaDB le:

    sudo apt-get install mariadb-server

Rè an stàlaidh, feumaidh tu facal-faire a chur ris airson a’ chleachdaiche
**root**. Cruthaicheamaid **facal-faire an stòir-dhàta**, mar eisimpleir
**correcthorsebatterystaple**.

Mu dheireadh, leasaichidh sinn tèarainteachd an stàlaidh MariaDB againn le
bhith a’ toirt air falbh cunntasan root a tha ruigsinneach bhon taobh a-muigh
den òstair ionadail, cunntasan luchd-cleachdaidh gun ainm agus an stòr-dàta
deuchainn. Is urrainn dhuinn sin a dhèanamh le

    mysql_secure_installation

## PHP

Airson PHP, stàlaichidh sinn **php-fpm** (Manaidsear Pròiseasan FastCGI) a
bhios a’ ruith mar daemon agus a’ faighinn iarrtasan Fast/CGI. A bharrachd air
sin, stàlaichidh sinn **php5-mysql**, a tha na mhodal airson ceanglaichean ri
stòran-dàta MySQL gu dìreach bho sgriobtaichean PHP.

bu chòir php7 nas ùire a bhith air a stàladh le

    sudo apt-get install php-fpm php-mysql

A-nis feumaidh sinn innse do Nginx gum bu chòir dha php-fpm a chleachdadh
airson faidhlichean .php. Cuiridh sinn dà loidhne ris na raointean mas-fhìor
againn:

    sudo nano /etc/nginx/sites-available/example.com

cuir ris:

    location ~ \.php$ {
    fastcgi_pass unix:/var/run/php/php7.0-fpm.sock;
    fastcgi_index index.php;
    include fastcgi_params;
    }

Dèan deuchainn air le bhith a’ cruthachadh an fhaidhle PHP a leanas

    sudo nano /var/www/example.com/test.php

Cleachdaidh sinn brabhsair gus dearbhadh a bheil sinn a’ faicinn duilleag
rèiteachaidh PHP aig
<a href="http://192.168.0.35/example.com/test.php"
rel="nofollow noreferrer noopener">http://192.168.0.35/example.com/test.php</a>

## Joomla!

- ri dhèanamh
```
    sudo wget https://github.com/joomla/joomla-cms/releases/download/3.6.3/Joomla_3.6.3-Stable-Full_Package.zip
    sudo unzip -x Joomla_3.6.3-Stable-Full_Package.zip
```

## A’ ceangal Raspberry Pi ris an Eadar-lìon

Tha sinn airson ’s gum bi daoine air an Eadar-lìon comasach air tadhal air an
làrach-lìn Joomla againn air an Raspberry Pi againn. Gus sin a dhèanamh,
feumaidh sinn an **rothadair Eadar-lìn againn a rèiteachadh** gus a h-uile
**trafaig a-steach** air port 80 a chur air adhart **chun Raspberry Pi
againn**.

Cleachd am brabhsair-lìn agad gus ceangal ri Eadar-aghaidh Lìn an rothadair
agad. Mar as trice tha rothadair suidhichte air a’ chiad àireamh den raon IP
agad; nar cùis-ne, air 192.168.0.1. Anns an rothadair againn, rèitichidh sinn
**Ath-chur air adhart phuirt**:

- Seòladh IP taobh a-muigh: 0.0.0.0
- Port tòiseachaidh taobh a-muigh: 80
- Port crìochnachaidh taobh a-muigh: 80
- Seòladh IP taobh a-staigh: 192.168.0.35 ( = an Raspberry Pi againn)
- Port tòiseachaidh taobh a-staigh: 80
- Port crìochnachaidh taobh a-staigh: 80
- Pròtacal: TCP

Dèan cinnteach gu bheil e air a chomasachadh.

Ma tha a h-uile càil ag obair mar bu chòir, bu chòir dhut an làrach-lìn Joomla
agad fhèin fhaicinn air an Raspberry Pi le bhith a’ tadhal air an t-seòladh IP
taobh a-muigh agad (Lorg an seòladh IP taobh a-muigh agad le inneal mar
<a href="http://www.whatsmyip.org/"
rel="nofollow noreferrer noopener">whatsmyip.org</a>).

### A’ cleachdadh ainm àrainn

Canamaid gur e 42.42.42.42 an seòladh IP taobh a-muigh againn. Canamaid cuideachd
gu bheil sinn air ainm àrainn leis an ainm example.com a chlàradh. Bu mhath
leinn an làrach Joomla againn a fhrithealadh air an Raspberry Pi againn do
luchd-tadhail a bhios a’ tadhal air example.com. Ma bheir neach-clàraidh an
ainm àrainn agad cothrom dhuinn frithealaiche an **t-Siostaim Ainmean Àrainn
(DNS)** a rèiteachadh, feumaidh sinn **clàr MX** a chruthachadh san DNS a
phointeas an **ainm àrainn againn gu** ar **seòladh IP**, 42.42.42.42. Thoir
fa-near gum faod e suas ri 24 uairean a thoirt gus an ath-stiùirich a h-uile
solaraiche Eadar-lìn trafaig an luchd-ceannach aca chun a’ chlàir MX a chaidh
a rèiteachadh.

### Seòladh IP statach

Cumaidh a’ mhòr-chuid de rothadairean orra a’ sònrachadh an aon sheòladh IP
taobh a-staigh dhan Raspberry Pi agad. Uaireannan tha e nas fheàrr an
Raspberry Pi agad a rèiteachadh gus seòladh IP statach a chleachdadh:

    sudo nano /etc/network/interfaces

atharraich

    iface eth0 inet static

gu

    iface eth0 inet static
    address 192.168.0.35
    netmask 255.255.255.0
    gateway 192.168.0.1

Is e an geata seòladh IP an rothadair agad. Gheibh thu e cuideachd le bhith a’
cleachdadh

    route

# Ceanglaichean taobh a-muigh

- <a href="https://raspberrypi.org"
  rel="nofollow noreferrer noopener">Bun-stèidh Raspberry Pi</a> (RPF) -
  làrach-lìn oifigeil agus fòraman
- <a href="http://elinux.org/RaspberryPiBoard"
rel="nofollow noreferrer noopener">Uicipeid Raspberry Pi</a>,
  le taic bhon RPF
- Bhidio den taisbeanadh
  <a href="https://youtu.be/u2MFQCoexD0"
  rel="nofollow noreferrer noopener">Joomla air Raspberry
  Pi (le Nginx)</a> aig Joomladay sa Ghearmailt 2013 ann an Nuremberg, sa
  Ghearmailt

*Air eadar-theangachadh le openai.com*