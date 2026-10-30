<!--
{
    "source": "https://docs.joomla.org/No_original_yet",
    "title": "Ostadh Ionadail air Linux",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Tha an t-artaigil seo a’ dèiligeadh ri bhith a’ cur Joomla air aoigheachd
air coimpiutair pearsanta stèidhichte air Linux airson adhbharan deuchainn agus
leasachaidh. Tha na tionndaidhean de Linux air an còmhdach à teaghlach
Debian-Ubuntu, agus gu sònraichte Linux Mint. Tha sgaoilidhean eile
coltach ris ach tha co-chàradh àitheantan agus àiteachan fhaidhlichean
eadar-dhealaichte aca.

Feumaidh tu seata de phacaidean bathair-bhog a stàladh ris an canar gu tric
cruach LAMP. Tha na litrichean a’ seasamh airson Linux, Apache, MySQL agus
PHP. ’S urrainn dhut bathar-bog a stàladh an dàrna cuid a’ cleachdadh an
Eadar-aghaidh Grafaigeach Cleachdaiche (GUI) no an loidhne-àithne ann an
uinneag Crìochnachaidh. ’S e dòighean eadar-dhealaichte a tha annta airson
Manaidsear Phacaidean Synaptic a chleachdadh.

## Stàlaich Apache leis an GUI

Bhon chlàr-taice Siostaim, air a chomharrachadh le suaicheantas LM, tagh
Rianachd / Manaidsear Phacaidean Synaptic. Thèid iarraidh ort am facal-faire
agad. Cuir a-steach am facal-faire logaidh a-steach agad gus an GUI fhosgladh.
Aig a’ mhullach air an làimh dheis tha putan `Lorg`. Tagh e agus
cuir a-steach **apache**, agus tagh `Lorg`. Tagh am bogsa `apache2` agus
anns an leubail uinneag-nochdte tagh `Comharraich airson stàladh`. Nochdaidh
bogsa-nochdte eile le liosta de phacaidean a bharrachd a tha riatanach gus
apache a chur an comas. Tagh `Comharraich`:

![manaidsear phacaidean synaptic](../../../en/images/hosting-local/local-hosting-on-linux/01-synaptic-package-manager-gui.png)

Tagh am putan `Cuir an gnìomh` anns a’ Chrann-inneal gu h-àrd agus am putan
`Cuir an gnìomh` anns a’ chòmhradh Geàrr-chunntais. Thèid Apache a stàladh
agus a rèiteachadh, agus thig am pròiseas gu crìch le **còmhradh Atharrachaidhean
air an cur an gnìomh**. Tagh `Dùin`.

’S urrainn dhut dearbhadh gu bheil Apache air a stàladh agus ag obair le bhith
a’ fosgladh do bhrobhsair, Firefox mar as àbhaist ann an stàladh ùr de
Linux Mint, agus a’ cur **localhost** a-steach sa bhàr URL. Bu chòir dhut
Duilleag Bhunaiteach Ubuntu Apache2 fhaicinn:

![duilleag bhunaiteach apache](../../../en/images/hosting-local/local-hosting-on-linux/02-apache-default-page.png)

Tha beagan fiosrachaidh fheumail air an duilleig mu àiteachan fhaidhlichean
a dh’fhaodadh nach bi cho furasta faighinn thuige nas fhaide air adhart, agus
mar sin ’s dòcha gum bu toil leat an duilleag seo a chlò-bhualadh air
pàipear no ann am faidhle PDF.

## Stàlaich PHP leis an CLI

’S dòcha gur fheàrr PHP a stàladh a’ cleachdadh na loidhne-àithne. ’S e aon
adhbhar airson seo, aig àm sgrìobhaidh, nach eil Manaidsear Phacaidean
Synaptic a’ tabhann ach PHP8.1, ged a tha PHP8.2 air a bhith ri fhaighinn
fad greis agus gun gabh a stàladh à tasg-lann treas-phàrtaidh. Tha deagh
thuairisgeul air a’ mhodh-obrach anns an oideachadh seo le earrannan
Quickstart agus Mion-fhiosrachadh.

An toiseach dùin GUI Manaidsear Phacaidean Synaptic agus an uair sin fosgail
uinneag Crìochnachaidh agus cuir a-steach na h-àitheantan a leanas aon aig
aon àm:

```bash
sudo add-apt-repository ppa:ondrej/php
sudo apt update
sudo apt install php8.2 php8.2-cli php8.2-{bz2,curl,mbstring,intl}
sudo apt install php8.2-fpm
sudo a2enconf php8.2-fpm
sudo systemctl reload apache2
```

Sa bhrobhsair agad, dèan cinnteach gu bheil an duilleag bhunaiteach localhost
fhathast ag obair.

## Stàlaich MySQL no MariaDb

’S urrainn dhut an lìon a rannsachadh airson fiosrachadh mu gach aon de na
pacaidean stòr-dàta seo. ’S e MySQL an roghainn thraidiseanta ach chaidh a
ghabhail thairis le Oracle agus chan eil e cho measail a-nis. ’S e roghainn
Open Source a th’ ann am MariaDB a ghabhas cur na àite gu dìreach, le
feartan a bharrachd. Bidh an dà chuid ag obair le Joomla! 5 ach chan eil e
furasta gluasad bho fhear dhiubh chun fhear eile. Feumar na clàir a
às-phortadh agus a thoirt a-steach. Tha Joomla! 5 ag iarraidh tionndaidhean
as ìsle sònraichte a tha Linux Mint a’ tabhann tro Mhanaidsear Phacaidean
Synaptic.

Fosgail GUI Manaidsear Phacaidean Synaptic agus rannsaich airson mysql-server
no mariadb-server. Tagh am bogsa airson an nì a tha a’ crìochnachadh ann an
-server. Tagh `Comharraich airson stàladh` agus an uair sin `Cuir an gnìomh`
anns a’ Chrann-inneal gu h-àrd. ’S urrainn dhut am pannal Mion-fhiosrachaidh
fhosgladh gus faicinn dè tha a’ tachairt rè an stàlaidh. Tagh `Dùin`
nuair a bhios e deiseil.

’S urrainn dhut deuchainn a dhèanamh a dh’fhaicinn a bheil an stòr-dàta agad
ag obair le bhith a’ cur `mysql` a-steach san loidhne-àithne. Tha seo mar an
ceudna airson MySQL agus MariaDB. Bu chòir dhut teachdaireachd mearachd
`Ruigsinneachd air a dhiùltadh` fhaicinn, rud a tha ceart gu leòr oir tha e
a’ sealltainn gu bheil stàladh an stòir-dhàta agad ag obair dha-rìribh.

## Stàlaich phpMyAdmin

'S e inneal riaghlaidh stòr-dàta GUI a th’ ann am phpMyAdmin a bhios a dhìth ort gus na stòran-dàta agad a chruthachadh agus a riaghladh. Ann an GUI Manaidsear nam Pasgan Synaptic, rannsaich airson **phpmyadmin**. Tagh a bhogsa-sgrùdaidh agus `Mark for Installation`. Às dèidh an luchdachaidh a-nuas, nochdaidh iarrtas gus an `Webserver to reconfigure automatically` a thaghadh. Tagh am bogsa-sgrùdaidh airson `apache2` agus an uair sin am putan `Next`. Air an ath-sgrìn rèiteachaidh, fàg am bogsa-sgrùdaidh `Configure database...` air a thaghadh agus tagh `Next`.

Tagh facal-faire aplacaid airson a’ chleachdaiche phpmyadmin. Deuchainn: sa bhàr URL sa bhrobhsair agad, cuir a-steach localhost/phpmyadmin. Bu chòir dhut sgrìn logaidh a-steach phpMyAdmin fhaicinn. Leis an ainm-chleachdaiche phpmyadmin agus am facal-faire a chuir thu a-steach rè an stàlaidh, bidh e comasach dhut logadh a-steach. Ach cha bhi e comasach dhut stòran-dàta sam bith a chruthachadh! Gus an duilgheadas fhuasgladh, feumaidh tu am faidhle rèiteachaidh a dheasachadh mar root ann an uinneag an Terminal:

```bash
sudo nano /etc/phpmyadmin/config.inc.php
```

Lorg an dà loidhne anns a bheil // $cfg['Servers'][$i]['AllowNoPassword'] = TRUE; agus thoir air falbh na sliasaidean tòiseachaidh gus an dì-iomradhachadh. An dà chuid dhiubh!

An uair sin log a-steach do mysql bhon loidhne-àithne agus cruthaich cleachdaiche ùr, agus thoir na sochairean uile don chleachdaiche sin:
```bash
sudo mysql
CREATE USER 'admin'@'localhost' IDENTIFIED BY '';
GRANT ALL PRIVILEGES ON *.* TO 'admin'@'localhost' WITH GRANT OPTION;
exit
```

An uair sin till air ais gu phpMyAdmin agus feuch ri logadh a-steach leis an ainm-chleachdaiche **admin** agus gun fhacal-faire. Bu chòir dhut na stòran-dàta uile fhaicinn agus a bhith comasach air stòran-dàta ùra a chruthachadh.

## Prìomhachas an Fhaidhle-innse

'S e /var/www/html an t-àite bunaiteach airson duilleagan-lìn air Ubuntu/Linux Mint. Ma nì thu liosta de shusbaint an eòlaire sin, chì thu gu bheil index.html ann, anns a bheil susbaint Duilleag Bhunaiteach Ubuntu Apache2. Cruthaich faidhle air a bheil index.php san eòlaire sin leis an t-susbaint a leanas:

```php
<?php echo phpinfo();
```

Ath-luchdaich localhost. Chan eil atharrachadh sam bith ann! Cuir a-steach **localhost/index.php** sa bhàr URL agus chì thu duilleag anns a bheil fiosrachadh mun Tionndadh PHP. Tha an giùlan seo fo smachd rèiteachadh bunaiteach Apache, agus faodar atharrachadh le bhith a’ comasachadh modal Apache `dir` agus a’ deasachadh a rèiteachaidh:

```bash
sudo a2enmod dir
sudo nano /etc/apache2/mods-enabled/dir.conf
```

Gluais index.php gu beulaibh na liosta. An uair sin ath-thòisich Apache:

```bash
sudo systemctl restart apache2
```

An turas seo, le **localhost** leis fhèin sa bhàr URL, bu chòir dhut susbaint an fhaidhle index.php fhaicinn, duilleag Fiosrachadh PHP.

## Òstairean Mas-fhìor

Ann an stàladh bunaiteach Linux, tha faidhlichean an t-siostaim sa phasgan root (/) agus tha faidhlichean dàta nan cleachdaichean sa phasgan dachaigh (/home/myusername). Tha seo na chunnart a dh’fhaodadh a bhith ann oir is dòcha nach bi na ceadan iomchaidh aig a’ chleachdaiche bunaiteach Apache, www-data, gus faidhlichean a chruthachadh ann an àite fhaidhlichean nan cleachdaichean. ’S e Òstairean Mas-fhìor a chruthachadh am fuasgladh as fheàrr.

An toiseach, tha feum air modal a leigeas le Apache a chleachdaiche agus a bhuidheann atharrachadh gus freagairt air gach cleachdaiche:

```bash
sudo apt-get install libapache2-mpm-itk
sudo a2enmod mpm_itk
```

An ath rud, dèan lethbhreac de fhaidhle rèiteachaidh na làraich bhunaiteach agus deasaich e:

```bash
cd /etc/apach2/sites-available
sudo cp 000-default.conf username.localhost.conf
sudo nano username.localhost.conf
```

Tha beachdan ann am faidhle rèiteachaidh na làraich bhunaiteach a mhìnicheas an t-susbaint aige. Tha iad air am fàgail a-mach san dealbh gu h-ìosal. Dèan dì-iomradhachadh air loidhne ServerName agus atharraich gach eisimpleir de `username` dhan ainm-chleachdaiche agad fhèin.

```xml
<VirtualHost *:80>
        ServerName username.localhost
        ServerAdmin webmaster@localhost
        DocumentRoot /home/username/public_html
        <IfModule mpm_itk_module>
                AssignUserId username username
        </IfModule>
        <Directory /home/username/public_html/ >
                Options Indexes FollowSymLinks
                AllowOverride None
                Require all granted
        </Directory>
        ErrorLog ${APACHE_LOG_DIR}/error.log
        CustomLog ${APACHE_LOG_DIR}/access.log combined
</VirtualHost>
```

Comasaich an làrach ùr agus ath-thòisich Apache:

```bash
sudo a2ensite username.localhost
sudo systemctl reload apache
```

Dèan inntrigeadh san fhaidhle /etc/hosts gus inntrigeadh a chur ris airson an òstair mas-fhìor ùr. Mur dèan thu sin, bidh am brabhsair agad ga lorg air an eadar-lìon.

```bash
sudo nano /etc/hosts
```

Nuair a bhios e deiseil, seallaidh e rudeigin mar seo:

```bash
127.0.0.1       localhost
127.0.0.1       username.localhost
127.0.1.1       hostname

# The following lines are desirable for IPv6 capable hosts
::1     ip6-localhost ip6-loopback
fe00::0 ip6-localnet
ff00::0 ip6-mcastprefix
ff02::1 ip6-allnodes
ff02::2 ip6-allrouters
```

**Hostname:** Seo an t-ainm a thug thu dhan choimpiutair agad nuair a stàlaich thu Linux. Bidh feum agad air goirid. Faodaidh tu atharrachadh ma thogras tu — ach ’s fheàrr tuilleadh leughaidh a dhèanamh mu dheidhinn agus a dhèanamh an toiseach.

Ma thèid a h-uile càil gu math, le URL den chruth username.localhost chì thu liosta eòlaire an eòlaire public_html agad. Thathar a’ meas gur e droch chleachdadh agus cunnart tèarainteachd a th’ ann a bhith a’ taisbeanadh liostaichean eòlaire gu poblach, agus mar as trice tha e air a thoirmeasg le suidheachadh rèiteachaidh Apache eile. Ach, airson làrach phearsanta air coimpiutair pearsanta a thathar a’ cleachdadh airson leasachadh agus deuchainn, tha e glè fheumail. Faodar iomadh làrach eadar-dhealaichte a stèidheachadh ann am fo-eòlairean eadar-dhealaichte. Mar eisimpleir, làraichean Joomla 4 agus Joomla 5, Bùird-fiosrachaidh, Wikis agus mar sin air adhart. Nuair a bhios mòran làraichean deuchainn agad, tha e doirbh cuimhneachadh air ainmean nan fo-eòlairean uile!

## Cothrom air Lìonra na Dachaigh

Ma tha coimpiutair eile agad air an lìonra dachaigh agad, is dòcha gum bu toil
leat cothrom fhaighinn air an làrach Linux agad às an sin cuideachd. Gus sin a
chur an gnìomh, feumaidh tu aoigheachd bhrìgheil eile. Dèan lethbhreac den
fhear a chaidh a chruthachadh agus deasaich e:

```bash
cd /etc/apache2/sites-available
sudo cp username.localhost.conf username.conf
sudo nano username.conf
```

Atharraich an ServerName bho username.localhost gu username.hostname agus
an uair sin cuir an làrach bhrìgheil ùr an comas agus ath-thòisich Apache.

```bash
sudo a2ensite username
sudo apachectl restart
```

Rach chun choimpiutair eile agad air an lìonra dachaigh agus deasaich am faidhle
hosts pearsanta aige. Mar eisimpleir, air Mac deasaich
/private/etc/hosts agus cuir an loidhne a leanas ris aig a’ bhonn:

```bash
192.168.178.20 username.hostname www.username.hostname
```

Far a bheil 192.168.178.20 na sheòladh IP aig a’ choimpiutair Linux agad.

A-nis, air an dàrna coimpiutair agad, bu chòir dhut a bhith comasach air cothrom
fhaighinn air an fhrithealaiche-lìn air a’ choimpiutair Linux agad le bhith a’
cur username.hostname ann am bàr URL a’ bhrabhsair agad.

## Notaichean mu Phàirteanan

Mar as trice tha bathar-bog a chaidh a stàladh a’ cleachdadh Manaidsear
Phasgan Synaptic san eòlaire freumha Linux (/). Tha dàta a’ chleachdaiche san
eòlaire dachaigh (/home). Ann an stàladh shìmplidh, tha na h-eòlairean seo san
aon phàirt chorporra den diosg.

Ann an stàladh nas iom-fhillte, ’s dòcha le roghainn diofar shiostaman-obrachaidh
(Windows no Linux) no diofar thionndaidhean den aon shiostam-obrachaidh a
thòiseachadh, tha an eòlaire freumha agus dàta a’ chleachdaiche gu tric ann am
pàirtean fa leth. Leigidh seo le cothrom fhaighinn air an aon dàta cleachdaiche
bho gach siostam-obrachaidh.

Tha duilgheadas ann: feumaidh làrach Joomla a tha suidhichte ann an eòlaire
/home/username dàta stòr-dàta a tha mar as trice san eòlaire freumha, gu
sònraichte ann an /var/lib/mysql. Faodaidh tu eòlaire dàta MySQL/MariaDB a
ghluasad gu àite a tha ri fhaighinn don dà shiostam-obrachaidh, an dara cuid
anns a’ phàirt /home no ann am pàirt fa leth. Tha an oideachadh seo a’ mìneachadh
mar a nì thu
Atharraich Eòlaire Dàta MySQL
ann an Ubuntu agus Debian Linux. Feumar sin a dhèanamh airson gach siostam-obrachaidh,
ach chan eil e air a chòmhdach an seo.

*Air eadar-theangachadh le openai.com*