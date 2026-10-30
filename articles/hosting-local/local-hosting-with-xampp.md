<!--
{
    "source": "https://docs.joomla.org/",
    "title": "Cl\u00e0rachadh Ionadail le XAMPP",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

’S e pasgan furasta a stàladh a th’ ann an XAMPP a tha a’ gabhail a-steach
frithealaiche-lìn Apache, PHP, XDEBUG agus stòr-dàta MySQL. Leigidh seo leat
an àrainneachd a chruthachadh a dh’fheumas tu gus Joomla! a ruith air a’ choimpiutair
ionadail agad. Tha an tionndadh as ùire de XAMPP ri fhaighinn air làrach-lìn
[Apache Friends](https://www.apachefriends.org/index.html). Tha luchdachadh a-nuas
ri fhaighinn airson Linux, Windows agus Mac OS X. Luchdaich a-nuas am pasgan
airson an àrd-ùrlair agad.

*Nota Chudromach mu XAMPP agus Skype:* Bidh Apache agus Skype le chèile a’ cleachdadh
port 80 mar roghainn eile airson ceanglaichean a-steach. Ma chleachdas tu Skype, rach
chun phannail Tools-Options-Advanced-Connection agus cuir dheth an roghainn
*Use 80 and 443 as alternatives for incoming connections*. Ma thòisicheas Apache
mar sheirbheis, gabhaidh e port 80 mus tòisich Skype agus chan fhaic thu duilgheadas.
Ach, airson a bhith sàbhailte, cuir à comas an roghainn ann an Skype.

## Stàladh

Tha an stàladh air àrd-ùrlar sam bith glè shìmplidh - cleachd an stàlaichear. Chan eil
leabhar-làimhe no leabhar-iùil ceart ann airson XAMPP. Tha na sgrìobhainnean ann an cruth
Ceistean Bitheanta a tha ceangailte bhon duilleag Luchdaich a-nuas.

### Stàladh air Windows

Airson Windows, thathar a’ moladh XAMPP a stàladh ann an "c:\xampp" (chan ann an
"c:\program files"). Ma nì thu seo, thèid na pasganan Joomla! agad (agus pasganan
làraichean-lìn ionadail sam bith eile) dhan phasgan "c:\xampp\htdocs". (A rèir
gnàthais, thèid gach susbaint-lìn fon phasgan "htdocs".)

Ma tha iomadh frithealaiche http agad (mar IIS), ’s urrainn dhut port èisteachd xampp
atharrachadh. Ann an \apache\conf\httpd.conf, atharraich an loidhne Listen 80 gu
Listen \[portnumber\] (m.e.: "Listen 8080").

<div class="alert alert-info">

### Oideachadh Iris Coimhearsnachd Joomla

Gheibh thu oideachadh mionaideach mu stàladh XAMPP air Windows, còmhla ri
Joomla 4 Beta, Deuchainn Pàistean Joomla agus Git san [artaigil seo ann an Iris Coimhearsnachd Joomla](https://magazine.joomla.org/all-issues/june-2020/github-installing-git).
</div>

Gus XDebug a stàladh: [XAMPP - XDebug Setup for PHP 8](https://odan.github.io/2020/12/03/xampp-xdebug-setup-php8.html)

### Stàladh air Linux

#### Stàlaich XAMPP

Luchdaichidh an duilleag Luchdaich a-nuas stàlaichear xampp-linux-x64-8.2.12-0-installer.run
far a bheil 8.2.12 mar an tionndadh as ùire. Ruith faidhle an stàlaicheir gus Apache2,
MySQL agus PHP a stàladh.

An dèidh an stàlaidh, cleachd na h-àitheantan a leanas gus na seirbheisean a thòiseachadh agus a stad:
```sh
    sudo /opt/lampp/lampp start
    sudo /opt/lampp/lampp stop
```

#### Dèan deuchainn air an fhrithealaiche localhost XAMPP agad

Fosgail do bhrobhsair agus comharraich e gu

    http://localhost

Ath-stiùiridh an index.php thu gu

    http://localhost/xampp

An sin gheibh thu stiùireadh air mar a dh’atharraicheas tu na h-ainmean-cleachdaiche
agus na faclan-faire bunaiteach. Air PC nach eil a’ frithealadh fhaidhlichean dhan eadar-lìon
no dhan LAN, ’s e co-dhùnadh pearsanta a th’ ann na roghainnean bunaiteach atharrachadh.

#### Faigh Joomla

* Luchdaich a-nuas an zip stàlaidh Joomla as ùire
* Dì-dhùmhlachd e dhan chlàr-chruaidh agad
* Ceangail ri localhost le cliant FTP Bunaiteach
* Cruthaich pasgan airson Joomla air an fhrithealaiche localhost
* FTP na faidhlichean stàlaidh Joomla neo-dhùmhlaichte dhan phasgan Joomla a chaidh a chruthachadh.

##### Cudromach:

- Bidh stàladh xammp a’ suidheachadh Seilbh cheart nam faidhlichean agus nan ceadan.
- Bidh cleachdadh na **h-àithne CHOWN** ag **adhbharachadh dhuilgheadasan Seilbhe le xampp**.
- Bidh **cleachdadh nautilus** gus pasganan/faidhlichean air localhost a làimhseachadh
  **ag adhbharachadh dhuilgheadasan Seilbhe le xampp**.

#### Fiosrachadh mun stòr-dàta

- Òstair: localhost
- Ainm bunaiteach an stòir-dhàta: test
- Cleachdaiche bunaiteach an stòir-dhàta: root
- Facal-faire bunaiteach: Chan eil **facal-faire** bunaiteach ann.
- Facal-faire an rianaire: do roghainn fhèin.

Thathar a’ moladh Dàta Sampall a stàladh do chleachdaiche ùr.

An dèidh an stàlaidh, sguab às an eòlaire stàlaidh agus comharraich do
bhrobhsair gu: `http://localhost/yournewjoomlafolder` no
`http://localhost/yournewjoomlafolder/administrator`.

#### A’ cruthachadh ceangal ann an clàr-taice Ubuntu

##### Gus GUI a chruthachadh airson xammp ceangailte ri clàr-taice Ubuntu

Fosgail an Terminal agus sgrìobh

    sudo nano /usr/share/applications/xampp-control-panel.desktop

An uair sin dèan lethbhreac de na leanas a-steach don deasaiche nano agus sàbhail e.

    [Desktop Entry]
    Encoding=UTF-8
    Name=XAMPP Control Panel
    Comment=Start and Stop XAMPP
    Exec=gksudo "python /opt/lampp/share/xampp-control-panel/xampp-control-panel.py"
    Icon=/usr/share/icons/Tango/scalable/devices/network-wired.svg
    Terminal=false
    Type=Application
    Categories=GNOME;Application;Network;
    StartupNotify=true

Ma dh’fhàillig leis a’ phannal-smachd tòiseachadh, feuch an àithne Exec a ruith
gu dìreach san terminal:

    gksudo "python /opt/lampp/share/xampp-control-panel/xampp-control-panel.py"

Ma gheibh thu a’ mhearachd:

    Error importing pygtk2 and pygtk2-libglade

Stàlaich na leabharlannan a tha a dhìth:

    sudo apt-get install python-glade2

#### Dì-bhugadair PHP XDebug

Chan eil pasgan XAMPP airson Linux a’ gabhail a-steach dì-bhugadair PHP XDebug.
Gus XDebug a stàladh air Debian no Ubuntu:

- Stàlaich am pasgan *build-essential*:

    sudo apt-get update
    sudo apt-get install build-essential
    sudo apt-get install autoconf

- Luchdaich a-nuas am [pasgan leasachaidh](http://www.apachefriends.org/en/xampp-linux.html)
airson an tionndaidh agad de XAMPP agus thoir a-mach e thairis air an stàladh a th’ agad mu thràth:

    sudo tar xvfz xampp-linux-devel-1.7.7.tar.gz -C /opt

- Tog XDebug:

    wget http://xdebug.org/files/xdebug-2.1.3.tgz
    tar xzf xdebug-2.1.3.tgz
    cd xdebug-2.1.3/
    /opt/lampp/bin/phpize

Às dèidh seo, chì thu an toradh a leanas air a’ chonsal agad…

    Configuring for:
    PHP Api Version:         20090626
    Zend Module Api No:      20090626
    Zend Extension Api No:   20090626

    ./configure --with-php-config=/opt/lampp/bin/php-config
    make
    sudo make install

An uair sin bidh an toradh seo ann... thoir sùil air an eòlaire ainmichte.

    Installing shared extensions:     /opt/lampp/lib/php/extensions/no-debug-non-zts-20090626/

Cruthaich pasgan sa phasgan temp agad a chumas am faidhle dàta
a ghineas XDebug:

    sudo mkdir /opt/lampp/tmp/xdebug
    sudo chmod a+rwx -R /opt/lampp/tmp/xdebug

Stàlaidhean eile:

Stàlaich a’ cleachdadh leabharlann coimhearsnachd nan leudachan PHP (PECL) a tha air a phasgadh le
xampp:

    sudo /opt/lampp/bin/pecl install xdebug

Air Ubuntu/Debian faodaidh tu stàladh le:

    apt-get install php5-xdebug

(rabhadh: stàlaichidh seo Apache agus PHP cuideachd à stòran apt).

##### Rabhadh do luchd-cleachdaidh 64-bit

Nuair a bhios tu a’ cur ri chèile XDebug no ga stàladh tro apt-get, gheibh thu
mearachd nuair a thòisicheas tu XAMPP às ùr:

    /opt/lampp/lib/php/extensions/no-debug-non-zts-20090626/xdebug.so: wrong ELF class: ELFCLASS64

Tha seo air sgàth ’s gu bheil xampp a’ ruith 32-bit ach gu bheil XDebug 64-bit. Gus faighinn seachad air an
duilgheadas seo, cruthaich xdebug.so air inneal 32-bit no luchdaich a-nuas e bho:

    http://code.activestate.com/komodo/remotedebugging/

Luchdaich a-nuas am faidhle: "PHP Remote Debugging Client" airson "Linux (x86)"
Thoir a-mach susbaint an fhaidhle air a’ choimpiutair agad; tha grunn phasganan anns an fhaidhle dhlùthaichte seo le àireamhan tionndaidh, me: 4.4, 5.0, 5.1 ... 5.3
agus mar sin air adhart. Rach a-steach don phasgan leis an àireamh tionndaidh as àirde no
am fear a tha ag obair dhut, agus an uair sin dèan lethbhreac làimhe den fhaidhle "xdebug.so" dhan
ionad a leanas, agus sgrìobh thairis air an t-seann fhaidhle ma bhios feum air:

    /opt/lampp/lib/php/extensions/no-debug-non-zts-20090626/

Cuimhnich gum faodadh an t-ionad seo a bhith eadar-dhealaichte air a’ choimpiutair agad

### Stàladh air Mac OS X

Tha frithealaiche Apache ann am Mac OS X mu thràth, ach is fheàrr leis a’ mhòr-chuid
de luchd-leasachaidh na h-innealan amalaichte agus an sùbailteachd rèiteachaidh
a tha XAMPP a’ toirt seachad a chleachdadh.

Coltach ris a’ mhòr-chuid de phrògraman air Mac, tha an stàladh glè fhurasta. Tadhail air làrach-lìn
[Apache Friends](https://www.apachefriends.org/) agus luchdaich a-nuas an
stàlaichear (xampp-osx-8.2.4-0-installer.dmg). Briog dùbailte air an stàlaichear a luchdaich thu a-nuas gus pròiseas
na stàlaidh a thòiseachadh.

Gus am frithealaiche a thòiseachadh, fosgail "XAMPP Control.app" agus brùth air a’ phutan tòiseachaidh
ri taobh Apache.

#### Beagan fhuasglaidhean dhuilgheadasan

Bidh duilgheadas beag aig mòran de luchd-cleachdaidh Mac aig an ìre seo nuair a tha iad a’ feuchainn ri
eisimpleir eile de Apache a chur air dòigh air an inneal aca. Mura h-urrainn dhut Apache XAMPP a thòiseachadh, tha dà roghainn agad:
**Faodaidh tu port èisteachd XAMPP atharrachadh.** Ann an
\Applications\XAMPP\xamppfiles\etc\httpd.conf, atharraich an loidhne a
tha ag ràdh, "Listen 80" gu Listen \[portNumber\]. Mar eisimpleir:

    Listen 8080

**Faodaidh tu port èisteachd an fhrithealaiche Apache a chaidh a stàladh ro-làimh atharrachadh.** Ann an Finder, rach gu "/etc" (CMD+SHIFT+G); às an seo bidh e comasach dhut
seòladh tro na faidhlichean Apache a tha falaichte mar as àbhaist. Lorg am
pasgan leis an ainm Apache2, agus deasaich am faidhle "http.conf". Atharraich an loidhne
a tha ag ràdh, "Listen 80" gu Listen \[portNumber\]. Mar eisimpleir:

    Listen 8080

*Nota: Ma roghnaicheas tu port an fhrithealaiche Apache a chaidh a stàladh ro-làimh atharrachadh,
is dòcha gum feum thu an coimpiutair agad ath-thòiseachadh gus am bi na h-atharrachaidhean èifeachdach. Feumaidh tu cuideachd
dearbhadh mar rianaire gus na faidhlichean seo atharrachadh.*

### Dèan deuchainn air stàladh XAMPP

Aon uair ’s gu bheil XAMPP air a stàladh agus gu bheil thu air seirbheis Apache a thòiseachadh leis an
inneal Pannal Smachd XAMPP, faodaidh tu deuchainn a dhèanamh air le bhith a’ fosgladh do bhrobhsair agus a’ seòladh gu `http://localhost`. Bu chòir dhut sgrìn fàilte XAMPP
fhaicinn coltach ris an fhear gu h-ìosal.

![Duilleag tòiseachaidh xampp](../../../en/images/hosting-local/local-hosting-with-xampp/01-local-hosting-xampp.png)

Tagh an ceangal air a bheil `phpinfo()` sa chlàr-taice aig a’ mhullach. Seallaidh seo sgrìn fhada
de dh’fhiosrachadh mu rèiteachadh PHP, mar a chithear gu h-ìosal.

![Duilleag fiosrachaidh tionndaidh php xampp](../../../en/images/hosting-local/local-hosting-with-xampp/02-local-hosting-xampp-php.png)

Aig an ìre seo tha XAMPP air a stàladh gu soirbheachail. Thoir fa-near am *Faidhle rèiteachaidh
luchdaichte*. Bidh sinn a’ deasachadh an fhaidhle seo san ath earrainn gus XDebug a rèiteachadh.

*Air eadar-theangachadh le openai.com*

