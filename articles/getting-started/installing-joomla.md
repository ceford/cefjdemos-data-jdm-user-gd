<!--
{
    "source": "https://docs.joomla.org/J4.x:Installing_Joomla",
    "title": "A\u2019 St\u00e0ladh Joomla",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Tha stàladh Joomla! airson a’ chiad uair glè fhurasta. Às dèidh dhut
na ceumannan tòiseachaidh a chrìochnachadh, àrainneachd aoigheachd a
shuidheachadh agus stòr-dàta a chruthachadh, suidhichidh stàlaichear lìn
togte Joomla an làrach ùr agad ann am beagan mhionaidean. Na ceumannan
roimhe:

### Suidheachadh na h-aoigheachd

Mura h-eil thu air àrainneachd aoigheachd a shuidheachadh fhathast, feumaidh
tu sin a dhèanamh a-nis, an dara cuid air seirbheis aoigheachd no air a’
choimpiutair ionadail agad.

Cuideachd, tha cuid de shuidheachaidhean PHP ann a dh’fheumas a bhith
iomchaidh airson Joomla a stàladh. Mar as trice tha na suidheachaidhean ann am
faidhle rèiteachaidh *php.ini* no *user.ini* air an fhrithealaiche. Ma tha thu
air aoigheachd cho-roinnte, bruidhinn ris an t-seirbheis aoigheachd agad mu
mar a dh’atharraicheas tu na suidheachaidhean seo, ma ghabhas sin dèanamh. Ma
tha thu ag obair air localhost, mar eisimpleir le XAMPP, no air
VPS no aoigheachd shònraichte, cha bu chòir na suidheachaidhean seo
do chuingealachadh agus ’s urrainn dhut an suidheachadh thu fhèin.

Tha na luachan as lugha airson an fhaidhle *php.ini* air an sealltainn gu
h-ìosal:

- *memory_limit:* 256M
- *upload_max_filesize:* 64M
- *post_max_size:* 64M
- *max_execution_time:* 30

Tha e comasach obrachadh le luachan nas ìsle airson upload_max_filesize agus
post_max_size, ach fàilligidh leudachain nas motha an luchdachadh suas agus
adhbharaichidh iad duilgheadasan nach gabh ro-innse.

### Suidheachadh an Stòir-dhàta

Mura h-eil thu air stòr-dàta a shuidheachadh fhathast, dèan sin a-nis. Tha
seo air a mhìneachadh airson seirbheis aoigheachd cPanel anns an oideachadh
[aoigheachd cPanel](jdocmanual?article=user/hosting/cpanel-hosting). Tha
oideachadh *A’ Cruthachadh Stòr-dàta airson Joomla!* ann cuideachd a tha a’
còmhdach dhòighean localhost agus phpMyAdmin.

Feumaidh tu nota a dhèanamh den fhiosrachadh bhunaiteach mun stòr-dàta a
dh’fheumar nuair a thòisichear air fìor stàladh Joomla.

- Suidheachadh an stòir-dhàta, mar as trice *localhost* eadhon air seirbheis
  aoigheachd. Faodaidh e bhith na fhrithealaiche aig òstair shònraichte mar
  *`dbserver1.yourhost.com`*.
- Ainm an stòir-dhàta
- Ainm-cleachdaiche an stòir-dhàta
- Facal-faire neach-cleachdaidh an stòir-dhàta

## Ullachadh airson Stàladh

### Luchdadh a-nuas agus Luchdadh suas Pacaidean Faidhlichean Joomla!

Luchdaich a-nuas an tionndadh làithreach de Joomla! bhon cheangal air an
duilleag [Luchdaich a-nuas Joomla](https://downloads.joomla.org/)

Gluais am faidhle zip pacaid stàlaidh Joomla a luchdaich thu a-nuas chun
fhrithealaiche. Airson seirbheis aoigheachd, faodaidh tu an gnìomh Luchdaich
suas aig Manaidsear Fhaidhlichean cPanel a chleachdadh, no faodaidh tu
Cliant FTP a chleachdadh gus am faidhle zip Joomla 5.x a luchdaich thu a-nuas
a ghluasad chun fhrithealaiche agad. Tha grunn Chliaint FTP rim faighinn.
Seo [Coimeas de bhathar-bog cliant FTP](https://en.wikipedia.org/wiki/Comparison_of_FTP_client_software)
mionaideach. Ma tha teagamh ort, cleachd FileZilla.

Tha e nas fheàrr am pasgan zip a luchdaich thu a-nuas a ghluasad chun
fhrithealaiche agad agus a dhì-phasgadh an sin na bhith ga dhì-phasgadh gu
h-ionadail agus an uair sin craobh nam faidhlichean a ghluasad. Mar as trice
luchdaicheas tu na faidhlichean-lìn agad suas gu pasgan freumha na seirbheis
aoigheachd agad. Mar as trice canar `public_html` ris an seo, ach tha
caochladh eile ann leithid `htdocs`, agus tha seo an urra ri mar a shuidhich
an t-òstair agad am frithealaiche. Airson adhbharan Joomla, faodaidh tu na
faidhlichean a luchdadh dìreach a-steach do *public_html* no do fho-phasgan a
chruthaich thu na bhroinn.

**Rabhadh:** Ma dhì-phasgadh tu na faidhlichean air a’ choimpiutair agad fhèin
agus ma nì thu lethbhreac dhiubh chun fhrithealaiche agad, dèan cinnteach
nach gluais thu ach na pasganan agus na faidhlichean a tha **taobh a-staigh**
a’ phacaid Joomla. Ma dhì-phasgadh tu na pasganan agus na faidhlichean ann am
pasgan, canaidh sinn *`Joomla`* ris, agus ma luchdaicheas tu am pasgan sin
suas, feumar inntrigeadh dhan làrach agad aig
*`yoursitename.com/Joomla`* an àite *`yoursitename.com`*. Faodaidh tu
an fho-eòlaire ath-ainmeachadh bho Joomla gu rudeigin a tha nas freagarraiche
don làrach, leithid jblog, agus dh’fhaodadh sin a bhith goireasach dhut.
**Nota:** bu chòir ainmean nan eòlairean a bhith ann an litrichean beaga,
gun bheàrnan, agus soidhnichean minus a chleachdadh an àite fo-loidhnichean
gus faclan a sgaradh.

Faodar faidhlichean a’ phacaid zip a thoirt a-mach dìreach air an òstair le
diofar innealan loidhne-àithne (m.e. unzip), a dh’fheumas a bhith air an
stàladh air an fhrithealaiche. Ma chleachdas an t-seirbheis aoigheachd agad
an t-inneal rianachd cPanel, faodar am putan Thoir a-mach a bhrùthadh ann am
Manaidsear nam Faidhlichean. A bharrachd air sin, faodar an t-inneal saor
treas-phàrtaidh Akeeba Kickstart a chleachdadh airson an adhbhair seo
cuideachd. Thèid na faidhlichean agus na h-eòlairean gun phasgadh a chur sa
phasgan làithreach. Tha toirt a-mach air a’ choimpiutair ionadail agad an urra
ris an t-siostam-obrachaidh agad. Feuch briogadh deas agus faic a bheil clàr
toirt-a-mach ann. Anns a’ chùis seo, dh’fhaodadh an siostam-obrachaidh agad
na faidhlichean a chur ann am pasgan leis an aon ainm ris an fhaidhle zip.
Às dèidh an toirt a-mach, faodaidh tu am faidhle zip a sguabadh às agus am
pasgan às-tharraingidh ath-ainmeachadh gu rudeigin goirid agus freagarrach
airson a chleachdadh ann an url.

## Tòisich air an stàladh

Nuair a bhios na riatanasan gu h-àrd air an coileanadh, stòr-dàta air a chruthachadh agus na faidhlichean Joomla riatanach nan àite, tha thu deiseil airson Joomla a stàladh. Tòisich stàlaichear-lìn Joomla le bhith a’ fosgladh a’ bhrabhsair as fheàrr leat agus a’ dol gu ainm àrainn na làraich. Air stàladh aoigheachd, cleachdaidh tu *`https://www.yoursitename.com`*. Ma tha thu a’ stàladh Joomla gu h-ionadail, cleachdaidh tu *`http://localhost/`* agus bu chòir dhut an sgrìn stàlaidh fhaicinn.

![Stàlaichear Joomla pàirt 1, cànan an stàlaidh agus ainm na làraich](../../../en/images/getting-started/installing-joomla/01-site-name.png)

Feuchaidh Joomla ri raon *Tagh cànan* aithneachadh gu fèin-obrachail a rèir cànan a’ bhrabhsair agad. Faodaidh tu seo atharrachadh ma tha feum air.

Lìon a-steach am fiosrachadh a leanas.

- **Ainm na làraich** Ainm na làraich-lìn agad — faodar seo atharrachadh aig àm sam bith nas fhaide air adhart air duilleag Rèiteachadh Cruinneil na Làraich.

Nuair a bhios a h-uile càil air a’ chiad duilleag deiseil, tagh am putan *Suidhich dàta an logaidh a-steach* airson leantainn air adhart.

## Dàta an logaidh a-steach

Bu chòir dhut a-nis sgrìn dàta an logaidh a-steach fhaicinn.

![Stàlaichear Joomla pàirt 2, dàta an logaidh a-steach](../../../en/images/getting-started/installing-joomla/02-login-data.png)

Lìon a-steach am fiosrachadh a leanas.

- **Fìor ainm** Ainm an Super User. Seo mar a chuireas Joomla fàilte ort nuair a nì thu logadh a-steach.
- **Ainm-cleachdaiche cunntas Super User** An t-ainm-cleachdaiche airson an *Super User*. Seachain *admin* a chleachdadh mar ainm an Rianaire!
- **Facal-faire an rianaire** Cuimhnich gu bheil làn smachd aig Super User air eadar-aghaidhean na Làraich agus an Rianaire, mar sin cleachd facal-faire doirbh. Cleachd **Mo phròifil** san eadar-aghaidh *Rianachd* gus atharrachadh nas fhaide air adhart.
- **Seòladh puist-d Super User** Seòladh puist-d an Super User. Cuir a-steach post-d dligheach gun fhios nach dìochuimhnich thu am facal-faire agad. Seo an seòladh puist-d far am faigh thu ceangal airson facal-faire an Super User atharrachadh.

Nuair a bhios a h-uile càil air an dàrna duilleag deiseil, tagh am putan *Suidhich ceangal an stòir-dhàta* airson leantainn air adhart.

## Rèiteachadh an stòir-dhàta

Cuir a-steach am fiosrachadh mun stòr-dàta a sgrìobh thu sìos nuair a chruthaich thu an stòr-dàta airson an stàlaidh seo.

![Stàlaichear Joomla pàirt 3, rèiteachadh an stòir-dhàta](../../../en/images/getting-started/installing-joomla/03-database.png)

Airson sìmplidheachd, tha na stiùiridhean seo a’ toirt iomradh air stàladh le stòr-dàta MySQLi. Tha na stiùiridhean air duilleag an stàlaidh fèin-mhìneachail, ach seo iad a-rithist:

- **Seòrsa stòir-dhàta** ’S e MySQLi an stòr-dàta cumanta a thathar a’ cleachdadh
- **Ainm an òstair** Far a bheil an stòr-dàta agad suidhichte. ’S e *localhost* an t-àite cumanta, eadhon air seirbheisean aoigheachd. Ach bidh cuid de dh’òstairean a’ cleachdadh frithealaiche stòir-dhàta sònraichte leithid *dbserver1.yourhost.com*.
- **Ainm-cleachdaiche** An t-ainm-cleachdaiche a thathar a’ cleachdadh gus ceangal ris an stòr-dàta
- **Facal-faire** Facal-faire neach-cleachdaidh an stòir-dhàta (chan e am facal-faire Rianaire agad)
- **Ainm an stòir-dhàta** Ainm an stòir-dhàta
- **Ro-leasachan nan clàr** Tha seo air a chruthachadh gu fèin-obrachail mar fheart tèarainteachd. Faodaidh tu gabhail ris an roghainn bhunaiteach a chaidh a chruthachadh air thuaiream no atharrachadh. Na dìochuimhnich ach an caractar fo-loidhne (`_`) a chur aig deireadh an ro-leasain.
- **Crioptachadh a’ cheangail** Sònraichidh seo mar a bu chòir an ceangal ris an stòr-dàta a bhith air a chrioptachadh. Mura h-eil fios agad, ’s fheàrr cumail ris an roghainn bhunaiteach. Ach leigidh seo le buidhnean a bhios a’ cleachdadh dearbhadh aon-shligheach no dà-shligheach airson ceangal an stòir-dhàta sin a thoirt seachad.

Faodar na roghainnean seo uile agus barrachd a dheasachadh air duilleag Rèiteachadh Cruinneil na Làraich, fo *Roghainnean an fhrithealaiche* às dèidh crìoch a chur air an stàladh. Thoir an aire gum bris thu an stàladh agad ma dh’atharraicheas tu na roghainnean seo às dèidh an stàlaidh, mura h-eil lethbhreac slàn agad den stòr-dàta làithreach a tha stàladh Joomla a’ cleachdadh. Bhiodh cleachdaidhean cumanta a’ gabhail a-steach ainm-cleachdaiche agus facal-faire an stòir-dhàta ùrachadh, no gluasad stàlaidh a tha ann mu thràth gu òstair ùr le paramadairean eadar-dhealaichte a choileanadh.

Às dèidh dhut am putan *Stàlaich Joomla* a thaghadh, bu chòir dhut bàr adhartais stàlaidh Joomla fhaicinn.

![Stàlaichear Joomla pàirt 4, bàr adhartais an stàlaidh](../../../en/images/getting-started/installing-joomla/04-installer-progress.png)

Nuair a bhios an stàladh deiseil, bu chòir dhut duilleag na soirbheachais fhaicinn.

## A’ cur crìoch air

### Soirbheachas agus crìoch a chur air an stàladh

Meal do naidheachd! Tha an làrach Joomla agad deiseil.

![Stàlaichear Joomla pàirt 5, tha an làrach Joomla agad deiseil](../../../en/images/getting-started/installing-joomla/05-site-ready.png)

Tha an dealbh-sgrìn gu h-àrd a’ sealltainn stàladh leasaiche. Bidh stàladh riochdachaidh a’ toirt air falbh am pasgan Installation gu fèin-obrachail.

Ma tha thu airson tòiseachadh air Joomla a chleachdadh sa bhad gun chànanan a bharrachd a stàladh, faodaidh tu *Fosgail an Rianaire* a thaghadh airson a dhol gu *Deas-bhòrd an Rianaire*, no *Fosgail an Làrach* a thaghadh airson a dhol gu duilleag-dhachaigh na Làraich. Is dòcha gum faic thu earrann le roghainnean PHP a thathar a’ moladh.

- **Roghainnean a thathar a’ moladh** Tha na roghainnean seo air am moladh ann an rèiteachadh PHP agad, ach cha chuir iad casg air Joomla! a bhith air a stàladh. Faodaidh tu sùil a thoirt air na stiùiridhean gu h-àrd gus faicinn mar a dh’fhaodar an atharrachadh ma tha feum air.

### Cànanan a bharrachd

Mar phàirt de phròiseas stàlaidh Joomla gheibh thu cothrom
cànanan a bharrachd a stàladh mus cuir thu crìoch air an stàladh.

Gus seo a dhèanamh, tagh am putan Stàlaich cànanan a bharrachd.

Bheir seo thu gu duilleag stàlaidh a bharrachd far an urrainn dhut
na cànanan a tha a dhìth ort a thaghadh.

#### Stàlaich cànanan a bharrachd

Tha liosta de phacaidean cànain air a shealltainn.

![Stàlaichear Joomla pàirt 6, stàlaich cànanan a bharrachd](../../../en/images/getting-started/installing-joomla/06-additional-languages.png)

Tagh suas ri 3 cànanan a tha thu airson a stàladh. (Faodaidh barrachd
na 3 aig an aon àm duilgheadasan ùine-tìm a chruthachadh; faodaidh tu
barrachd a stàladh nas fhaide air adhart.)

Cuimhnich air na leanas:

- Cha tèid pacaidean cànain a tha ann an sgaoilidhean gnàthaichte a
  shealltainn aig an ìre seo, oir tha iad air an stàladh mu thràth.
- Bidh dreach nam pacaidean a thathar a’ moladh a’ freagairt ri prìomh
  dhreach Joomla (5.0.x, 5.1.x, msaa). Is dòcha nach bi mion-dreach a’
  phacaid a’ freagairt, mar eisimpleir ma tha thu a’ stàladh dreach
  5.0.3 agus gu bheil pasgan cànain 5.0.2 air a shealltainn.
- Is dòcha gum bi teudan nach deach eadar-theangachadh anns na pacaidean
  cànain nach eil a’ freagairt san eisimpleir gu h-àrd.
- Thèid na pacaidean cànain nach eil a’ freagairt a thabhann mar
  ùrachadh nuair a thèid na pacaidean ùrachadh leis na sgiobaidhean
  eadar-theangachaidh clàraichte. Thèid an t-ùrachadh a tha ri fhaighinn
  a shealltainn anns a’ Phannal-smachd a bharrachd air ann an
  **Leudachain → Ùraich**.
  Tha an giùlan seo coltach ri **Leudachain → Stàlaich cànanan**.

Tagh *Air adhart* agus thèid bàr adhartais a shealltainn fhad ’s a tha
am pasgan cànain no na pacaidean cànain gan stàladh.

#### Tagh an cànan bunaiteach

Nuair a bhios stàladh nan cànanan deiseil, thèid scrion coltach ri
*Meal do naidheachd! Tha an làrach Joomla agad deiseil.* a shealltainn
dhut a-nis. Is e an diofar gum bi liosta de na cànanan a chaidh a
stàladh ann, a’ leigeil leat an cànan bunaiteach airson an Làraich agus
an eadar-aghaidh Rianaire a thaghadh.

![Stàlaichear Joomla pàirt 7, tagh an cànan bunaiteach](../../../en/images/getting-started/installing-joomla/07-choose-default-language.png)

- Tagh an cànan bunaiteach a tha thu airson a chleachdadh.
- Nuair a bhios tu air an cànan bunaiteach a thaghadh, tagh am putan
  *Suidhich an cànan bunaiteach* gus dearbhadh.
- Thèid teachdaireachd siostaim a shealltainn a dhearbhas gu bheil Joomla
  air cànan bunaiteach an RIANAIRE agus na LÀRAICH a shuidheachadh. Faodar
  an teachdaireachd sin a dhùnadh.

#### Cuir crìoch air

Faodaidh tu a-nis gluasad chun *Deas-bhòrd an Rianaire*. Clàraich a-steach
le bhith a’ taghadh *Fosgail an Rianaire*, no rach dìreach gu duilleag
Dachaigh na làraich agad le bhith a’ taghadh *Fosgail an Làrach*.

*Eadar-theangaichte le openai.com*