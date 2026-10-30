<!--
{
    "source": "https://docs.joomla.org/Setting_up_Apache,_PHP_and_MySQL_manually",
    "title": "A\u2019 st\u00e8idheachadh Apache, PHP agus MySQL le l\u00e0imh",
    "description": " ",
    "author": ""
}
-->

## Sealladh farsaing

Seo sealladh farsaing goirid air na ceumannan gus Apache, PHP agus MySQL a
stèidheachadh ann an àrainneachd Windows, agus cuideachd iomradh a thoirt air
diofar innealan co-cheangailte airson a’ mhòr-chuid de na gnìomhan co-cheangailte
ri Joomla! a chumail suas agus obrachadh leotha.

Gus an stiùireadh a dhèanamh soilleir agus pongail, gabhaidh sinn ris, mura
h-eil sinn ag innse stiùireadh sònraichte, gun tèid na slighean bunaiteach
stèidheachaidh a chleachdadh gun atharrachadh.

### Rabhadh

Ma tha gin de na cruachan AMP ro-phacaichte air an stàladh air an inneal agad mu thràth:

- Bidh e doirbh tilleadh chun chruaich AMP agad. Bidh na diofar
  stàlaidhean a nì sinn gu h-ìosal a’ sgrìobhadh thairis air luachan a’ chlàraidh
  agus a’ dèanamh atharrachaidhean coitcheann air an àrainneachd. (Tha seo a’
  buntainn co-dhiù ris an àrainneachd PC/Windows.)
- Ma dh’fheumas tu rèiteachadh sam bith (Apache, MySQL no PHP) no dàta
  (na làraichean-lìn agad agus na stòran-dàta co-cheangailte riutha) a chumail
  suas, dèan lethbhreacan-glèidhidh iomchaidh mus feuch thu ris an stiùireadh
  seo a leantainn.

(feumar seo a leudachadh le comhairle shònraichte air mar a choileanar na
rudan gu h-àrd...)

## Stèidheachadh MySQL

1.  Luchdaich sìos an <a href="https://dev.mysql.com/downloads/mysql/"
    rel="nofollow noreferrer noopener">stàlaichear MySQL</a> iomchaidh airson an àrd-ùrlair agad.
2.  Tòisich an stàladh agus tagh slighe stàlaidh Gnàthaichte.
3.  Briog tron phròiseas stàlaidh gu lèir agus briog air Crìochnaich.
4.  Chì thu a-nis *MySQL Server Instance
    Configuration Wizard*.
    1.  Dèan cinnteach gu bheil *Standard Configuration* air a thaghadh agus
        rach gu Air adhart.
    2.  Ma tha MySQL air a stàladh agad mu thràth, is dòcha gum faigh thu an
        teachdaireachd *A Windows service with the name MySQL already exists. Please
        uninstall this service correctly or choose a different name for
        the new service.* Ma thachras seo, tagh ainm seirbheis eile.
    3.  San ath-uinneag, tagh *Include Bin Directory in Windows
        PATH*. Le bhith a’ dèanamh seo, bidh e comasach dhut cothrom fhaighinn
        air na diofar ghoireasan MySQL bhon loidhne-àithne.
    4.  San ath-uinneag, bidh e comasach dhut facal-faire a chruthachadh airson
        an cleachdaiche root MySQL agad, an cleachdaiche aig a bheil an ìre
        inntrigidh as àirde air an fhrithealaiche agad.
    5.  San uinneag mu dheireadh, thèid na h-atharrachaidhean uile a tha
        thu air rèiteachadh gu ruige seo a shàbhaladh nuair a bhrùthas tu am
        putan *Execute*, agus tòisichear seirbheis Windows na h-eisimpleir seo.

### Notaichean

1.  Gus an stiùireadh a dhèanamh cho ruigsinneach ’s a ghabhas, dh’fhàg sinn
    a-mach grunn shuidheachaidhean rèiteachaidh den eisimpleir MySQL agad,
    leithid comas na faidhlichean stòir-dhàta agad ath-shuidheachadh.
2.  Bidh MySQL air a stàladh gu bunaiteach le modh STRICT, a dh’fhaodadh
    mearachdan adhbhrachadh nuair a thathar a’ cleachdadh leudachain no
    aplacaidean nach do ghabh seo a-steach.

### Goireasan MySQL

- <a href="https://www.heidisql.com/" class="external text"
   rel="nofollow noreferrer noopener">HeidiSQL</a> Neach-àite làn-chleachdaiche
  furasta a chleachdadh agus a ghabhas leudachadh airson phpMyAdmin, ga
  leasachadh gu cunbhalach.
- <a href="https://dev.mysql.com/downloads/workbench/"
  class="external text"
  rel="nofollow noreferrer noopener">MySQL Workbench</a> Diofar innealan,
  nam measg an Rianaire, a chuidicheas tu le rèiteachadh na h-eisimpleir MySQL
  agad. Feumaidh e am
  <a href="https://dotnet.microsoft.com/en-us/" class="external text"
   rel="nofollow noreferrer noopener">frèam-obrach .Net</a>.
- <a href="https://www.phpmyadmin.net/" class="external text"
   rel="nofollow noreferrer noopener">phpMyAdmin</a> Neach-dèiligidh MySQL
  cumhachdach stèidhichte air an lìon airson rud sam bith co-cheangailte ri
  MySQL a rianachd.
- <a href="https://dev.mysql.com/doc/" class="external text"
   rel="nofollow noreferrer noopener">sgrìobhainnean
  MySQL</a>

## Suidheachadh Apache

1.  <a href="https://httpd.apache.org/download.cgi" class="external text"
     rel="nofollow noreferrer noopener">Luchdaich a-nuas an
    stàlaichear</a> as fheàrr leat.
2.  Ruith draoidh an stàlaicheir agus cliog tro gach ceum gus an ruig thu uinneag Fiosrachadh an Fhrithealaiche. Thoir na roghainnean gu h-ìosal fa leth agus san òrdugh ainmichte anns gach raon, mura h-eil riatanasan sònraichte agad a thaobh mar a tha am frithealaiche-lìn agad air a rèiteachadh:
    1.  localhost,
    2.  localhost agus
    3.  admin@localhost
3.  Cliog troimh an draoidh, a stàlaicheas agus a thòisicheas frithealaiche-lìn Apache mar sheirbheis Windows.
4.  Ann am bàr inbhe Windows chì thu a-nis iteag phinc le putan cluiche uaine, a’ sealltainn gu bheil Apache ag obair. Seòl do bhrobhsair gu
    <a href="http://localhost/"
    rel="nofollow noreferrer noopener">http://localhost/</a> agus bu chòir dhut duilleag fhaighinn a tha a’ sealltainn gu bheil e ag obair.
5.  Rachamaid a-nis don àite far a bheil Apache air a stàladh, a tha mar as trice aig *C:\Program Files\Apache Software
    Foundation\Apache2.2*, agus rachamaid tro na diofar phasganan:
    1.  *bin* - tha na diofar fhaidhlichean dà-chànaraich ann, agus tha cuid dhiubh air an liostadh gu h-ìosal. Gus cothrom fhaighinn air na h-aplacaidean seo, a’ mhòr-chuid dhiubh stèidhichte air àitheantan, feumaidh sinn an t-slighe dhan phasgan *bin* a chur ris a’ chaochladair PATH chruinneil againn. Gus sin a dhèanamh, dèan briogadh deas air My Computer \> Properties \> Advanced \> Environments
        Variables agus anns an liosta System Variables lorg agus tagh an caochladair PATH, briog air Edit agus cuir leth-chòilean aig an deireadh, mura h-eil fear ann mu thràth, agus an uair sin an t-slighe iomlan dhan phasgan bin agad. Dùin còmhradh System Properties le bhith a’ gabhail ris.
        1.  *httpd.exe*, is e sin frithealaiche-lìn Apache fhèin, a thèid a ghineadh gu grunn phròiseasan cloinne fhad ’s a tha e a’ frithealadh na h-uimhir de dh’iarrtasan luchd-dèiligidh a thig a-steach aig an aon àm ’s a tha riatanach a rèir stiùiridh MaxClients;
        2.  ’S e inneal tomhais coileanaidh a th’ ann an *ab.exe* a thig le Apache, a’ leigeil leat faicinn dè cho math ’s as urrainn don aplacaid agad coileanadh gach aonad ùine
    2.  *conf* - pasgan far a bheil diofar fhaidhlichean rèiteachaidh suidhichte, agus ’s iad na leanas an fheadhainn as cudromaiche dhuinn:
        1.  *httpd.conf* - tha a’ mhòr-chuid de stiùiridhean an fhrithealaiche suidhichte san fhaidhle seo agus, airson cothrom furasta, bu chòir dhut an seòrsa faidhle *.conf* a cheangal ri deasaiche a tha furasta a chleachdadh, i.e. rud sam bith seach an Notepad bunaiteach.
        2.  *extra\httpd-vhosts.conf* - tha stiùiridhean ann a leigeadh leat am frithealaiche ionadail agad a chleachdadh mar òstair bhrìgheil, i.e. comasach air grunn fhrithealaichean a ruith air a’ PC agad. ’S e aon shuidheachadh cleachdaidh, rè ìre leasachaidh, ma tha thu airson an àrainn fhìor air a bheil thu ag obair a mhapadh dhan lethbhreac ionadail agad, gum biodh e comasach dhut sin a dhèanamh le bhith a’ dèanamh atharrachaidhean beaga san fhaidhle seo. Bruidhnidh sinn air seo ann am barrachd mionaideachd gu h-ìosal.
    3.  *htdocs* - freumh bunaiteach an fhrithealaiche-lìn; seo far a bheil
        <a href="http://localhost/"
        rel="nofollow noreferrer noopener">http://localhost/</a> air a mhapadh, i.e. mura dèan thu ath-rèiteachadh air ann an *httpd.conf* gu h-àrd.
    4.  *logs* - logaichean ruigsinneachd agus mhearachdan, nuair a tha thu a’ feuchainn ri dèiligeadh ri diofar chùisean co-cheangailte ris an fhrithealaiche agad no fiù ’s ris an aplacaid agad

### Goireasan Apache

- An
  <a href="https://httpd.apache.org/docs/current/" class="external text"
   rel="nofollow noreferrer noopener">sgrìobhainnean iomraidh Apache</a>

## Suidheachadh PHP

1.  <a href="https://windows.php.net/download/" class="external text"
     rel="nofollow noreferrer noopener">Luchdaich a-nuas PHP</a>
    agus tagh mar as trice VC6 x86 Thread Safe ann an cruth Zip. Tha na diofar roghainnean co-cheangailte ri mar a chaidh bun-chòd PHP a chur ri chèile gu faidhle dà-chànarach, agus is dòcha nach fheum thu dragh a ghabhail mu dheidhinn seo an-dràsta.
2.  Cruthaich pasgan fon C:\Program Files\\ (no ge bith càit a bheil am pasgan phrògraman agad suidhichte), agus ainmich e PHP.
3.  Lorg am faidhle Zip a luchdaich thu a-nuas, gluais e dhan phasgan ùr agus dì-phacaich e gu dìreach sa phasgan.
4.  Cuiridh sinn a-nis slighe PHP ris a’ chaochladair PATH chruinneil againn le bhith a’ leantainn an stiùiridh gu h-àrd.

### Rèiteachadh PHP

Tha an rèiteachadh a’ ciallachadh am faidhle *php.ini* a dheasachadh. Tha
faidhle sampall airson diofar shuidheachaidhean mu thràth sa phasgan PHP
agad. Nach ath-ainmich sinn *php.ini-development* gu *php.ini* agus fosgail
sinn e san deasaiche teacsa as fheàrr leat. Seo na luachan cumanta a
dh’fhaodar atharrachadh, agus tha na caochladairean seo uile air an
sgrìobhadh gu mionaideach anns an fhaidhle *php.ini*. (Thoir an aire gur e
suidheachadh a tha seo a tha a’ buntainn ris an fhrithealaiche air fad agus
ris na pròiseactan agad uile.):

- *max_execution_time* - nuair a bhios sgriobtaichean agad a’ ruith ro fhada
  agus am frithealaiche a’ tilleadh diofar thoraidhean ris nach robh dùil,
  agus a tha thu a’ smaoineachadh gur e an t-adhbhar nach urrainn dha a dhol
  tron phròiseas air fad
- *memory_limit*
- *error_reporting*
- *display_errors*
- *log_errors* - caochladair air am feum thu aire a thoirt ann an
  suidheachaidhean riochdachaidh
- *upload_tmp_dir*
- *upload_max_filesize*
- *extension_dir' - gus duilgheadasan a sheachnadh, comharraichidh sinn
  am pasgan far a bheil na leudachain a leanas suidhichte le bhith a’
  toirt air falbh a’ bheachd bhon chaochladair seo agus a’ sònrachadh
  làrach iomlan a’ phasgain. Bu chòir don loidhne iomlan a bhith mar a leanas*
    extension_dir = "C:\Program Files\PHP\ext"

- Tha grunn mhodalan a bharrachd anns an earrann Dynamic extensions a
  tha thu airson an luchdachadh, agus ’s iad na feadhainn le beachd
  ro-làimh an fheadhainn a thig am broinn PHP agus a gheibhear sa phasgan
  *ext* sa phasgan PHP agad. Ma tha thu airson gin dhiubh a chur an
  gnìomh, dìreach thoir air falbh a’ bheachd, mar a bu chòir dhut a dhèanamh
  leis na leudachain a leanas:
  - php_curl.dll
  - php_gd2.dll
  - php_mbstring.dll
  - php_mysql.dll
  - php_mysqli.dll
  - php_pdo.dll
  - php_pdo_mysql.dll
  - php_xsl.dll
- session.save_path

### Rèiteachadh Apache gus Obrachadh le PHP

A-nis gu bheil sinn air PHP a rèiteachadh gus obrachadh mar a tha sinn
ag iarraidh, rachamaid gu Apache agus dèanamaid an aon rud.

- Fosgail *httpd.conf* agus anns an earrann "Dynamic Shared Object (DSO) Support"
  cuir na stiùiridhean a leanas ris. (Ma tha thu air am pasgan PHP agad a
  lorg ann an àite eile, dèan an t-atharrachadh iomchaidh airson
  php5apache2_2.dll gu h-ìosal.):
    LoadModule php5_module "C:/Program Files/PHP/php5apache2_2.dll"
    AddType application/x-httpd-php .php

- Ann an DirectoryIndex cuir *index.php* agus *index.htm* ris mar
  fhaidhlichean a ghabhas frithealadh nuair a thèid pasgan iarraidh, mar a
  leanas:
    DirectoryIndex index.html index.htm index.php

- Aig deireadh an fhaidhle cuir an loidhne a leanas ris, a chomharraicheas
  càit a bheil am faidhle *php.ini* suidhichte:
    PHPIniDir "C:/Program Files/PHP"

### Ath-thòiseachadh agus Deuchainn PHP

Cho luath ’s a nì thu atharrachadh sam bith air *php.ini*, *httpd.conf* no
faidhlichean rèiteachaidh sam bith eile, feumaidh tu Apache ath-thòiseachadh
gus buaidh nan atharrachaidhean fhaicinn. Mar sin, ath-thòisichidh sinn
Apache a-nis le bhith a’ cleachdadh inneal Apache Monitor a gheibhear ann am
bàr inbhe Windows. Tha sinn an dòchas nach nochd còmhradh sam bith agus gun
lean Apache Monitor air adhart a’ ruith ann an uaine.

Nì sinn deuchainn a-nis gus dèanamh cinnteach gu bheil PHP ag obair. Rach gu
freumh sgrìobhainnean an fhrithealaiche-lìn agad (anns a’ chùis bhunaiteach
*C:\Program Files\Apache Software
Foundation\Apache2.2\htdocs*) agus cuir faidhle ris air a bheil
*phpinfo.php*, leis an t-susbaint a leanas:

Seallaidh seo duilleag anns a bheil fiosrachadh mu rèiteachadh PHP agad agus
mu na diofar mhodalan/leudachain a tha air an luchdachadh an-dràsta. Seòl
do bhrobhsair gu
<a href="http://localhost/phpinfo.php"

rel="nofollow noreferrer noopener">http://localhost/phpinfo.php</a>.

### A’ Stàladh agus a’ Rèiteachadh *xdebug*

1.  Seòl do bhrobhsair gu
    <a href="https://xdebug.org/wizard" class="external text"
     rel="nofollow noreferrer noopener">Xdebug Installation
    Wizard</a>. Cuidichidh an duilleag seo thu gus tionndadh iomchaidh de
    Xdebug a lorg.
2.  Dèan lethbhreac de dhuilleag iomlan na duilleige *phpinfo* a ruith sinn
    gu h-àrd agus cuir a-steach e don raon teacsa, agus lean an stiùireadh a
    chaidh a thoirt seachad airson a stàladh.

### Goireasan XDebug

- Tha an <a href="https://www.php.net/docs.php" class="external text"
   rel="nofollow noreferrer noopener">PHP Manual</a>
  na sgrìobhainnean sàr-mhath agus ùraichte, le beachdan a bharrachd luachmhor
  bho luchd-cleachdaidh. Tha tionndaidhean a ghabhas luchdachadh a-nuas rim
  faighinn.
- An
  <a href="https://xdebug.org/docs/" class="external text"
  rel="nofollow noreferrer noopener">Xdebug 3 Documentation</a>

*Air eadar-theangachadh le openai.com*