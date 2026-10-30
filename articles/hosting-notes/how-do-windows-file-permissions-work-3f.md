<!--
{
    "source": "https://docs.joomla.org/How_do_Windows_file_permissions_work%3F",
    "title": "Ceadan fhaidhlichean Windows",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Dhaibhsan agaibh a tha an dàrna cuid a’ leasachadh no a’ lìbhrigeadh nan
làraichean-lìn Joomla! agaibh à àrainneachd Windows, tha e uaireannan
doirbh fiosrachadh iomchaidh fhaighinn mu cheadan. Gu mì-fhortanach, ’s e
fìrinn a th’ ann gu bheil a’ mhòr-chuid de sheirbheis-lìn ga tabhann fo
Unix agus gu bheil Unix air a dheagh chlàradh san àrainneachd seo. Tha
dòchas agam gun cuidich am fiosrachadh a leanas le mì-thuigse sam bith a
shoilleireachadh agus gun toir e beagan stiùiridh cuideachd.

### Sealladh farsaing air frithealaichean-lìn Windows

An toiseach, bruidhnidh sinn mu na h-eadar-dhealachaidhean eadar
frithealaichean. San fharsaingeachd, tha coltas ann gu bheil a’ mhòr-chuid
de luchd-cleachdaidh Windows a’ cleachdadh Apache(Win32) no Microsoft IIS.
Tha an dà fhrithealaiche-lìn seo ag obrachadh ann an dòighean gu math
eadar-dhealaichte agus a’ cleachdadh mhodailean lìbhrigidh beagan
eadar-dhealaichte. Mar as trice, bidh Apache(Win32) a’ ruith air a’
choimpiutair-aoigheachd mar an Cleachdaiche fon deach a stàladh, ach bidh
IIS ga stàladh fo chleachdaiche sònraichte agus an uair sin a’ ruith fo
chleachdaiche ùr-stàlaichte *IUSR_*.

### Ceadan bunaiteach

Gu gnàthach, chan àbhaist do Unix ach làn-inntrigeadh a thoirt don
chleachdaiche *leis an t-seilbh* airson faidhlichean agus pasganan. An
coimeas ris an dòigh seo, sònraichidh Windows gu gnàthach cuideachd làn
cheadan don Bhuidheann *Everyone*. ’S e a’ chiad rud a nì deagh
Rianaire Windows sam bith còraichean na buidhne *Everyone* a thoirt air
falbh, gus tèarainteachd a leasachadh. Airson deuchainnean air PC ionadail,
’s dòcha nach eil seo riatanach, ach tha e a’ mìneachadh carson, mura tèid
*Everyone* a thoirt air falbh agus ma ruitheas tu seòrsa air choreigin de
sgriobt sgrùdaidh cheadan no sgrùdadh Ro-stàlaidh Joomla!, gum bi làn
cheadan *Leughaidh, Sgrìobhaidh agus Cur an Gnìomh* agad san fharsaingeachd,
oir tha thu a’ faighinn còraichean na Buidhne *Everyone*.

### Microsoft Internet Information Server (IIS)

Tha IIS a’ tighinn ann an dà phrìomh chruth, PWS (Personal WebServer), agus
IIS (Internet Information Server). Gu bunaiteach, ’s e an aon aplacaid a
th’ annta. Chan eil ann am PWS ach tionndadh lùghdaichte de IIS a chaidh a
dhealbhadh airson àrainneachdan deasg, agus tha IIS air a dhealbhadh airson
àrainneachdan frithealaiche. Tha PWS gad chuingealachadh gu aon phrìomh
làrach-lìn, agus mar sin bidh na stàlaidhean aplacaidean agad mar as trice
ann am fo-phasganan na prìomh làraich-lìn. Air an làimh eile, tha IIS a’
toirt seachad comas airson Òstairean Mas-fhìor a ruith às na pasganan seo,
a’ lìbhrigeadh comas ioma-làraich.

Air sgàth nan cuingealachaidhean eadar-dhealaichte ann an comas, chan eil
an *Permissions Wizard* aig PWS oir chaidh a dhearbhadh nach eil feum air.
Cha bhi ach aon chleachdaiche a’ cleachdadh Frithealaiche PWS. Ann an IIS,
bidh mòran chleachdaichean a’ cleachdadh an Fhrithealaiche, agus mar sin
tha feum air sònrachaidhean cheadan eadar-dhealaichte.

Nuair a thèid cunntas *Everyone* a thoirt air falbh, bidh Windows IIS a-nis
air fhàgail leis a’ chunntas *IUSR_* aig a bheil còraichean aig an ìre as
àirde airson pasganan an Fhrithealaiche-lìn. Bu chòir do sgrùdadh cheadan a-nis
toraidhean eadar-dhealaichte a thoirt seachad. Chan eil làn cheadan aig
ach a’ chunntas *IUSR_* agus bu chòir do chleachdaichean eile *Leughadh a-mhàin*
no gun chòraichean idir fhaighinn. Tha na còraichean air an dearbhadh leis
na cleachdaichean eile a chaidh na còraichean iomchaidh a shònrachadh dhaibh
le làimh airson pasganan IIS.

### Sònrachadh Cheadan

Tha sònrachadh cheadan ann an Windows gu math sìmplidh, ach faodaidh e a
bhith beagan troimh-chèile aig amannan. Dèan briogadh deas air a’ phasgan
no air an fhaidhle iomchaidh. Le bhith a’ taghadh *Properties* no *Sharing
and Security* thèid thu a-steach do phana Riaghladh Tèarainteachd Windows.
Ma thaghas tu (le aon bhriogadh) ainm-cleachdaiche sam bith a tha air a
liostadh, nochdaidh na còraichean a th’ aig a’ chleachdaiche sin anns an
leth ìosal den phana. Dh’fhaodadh cuid de chòraichean a bhith
*liath-dhathte*. Chan eil iad sin rim faighinn, an dara cuid air sgàth
nach eil ceadan àrd gu leòr aig a’ chleachdaiche làithreach (fon do rinn
thu logadh a-steach) airson an atharrachadh, no gun deach an sealbhachadh
bhon phasgan gu h-àrd agus gun deach an suidheachadh gus ceadan na
pasgain aig an ìre as àirde sin a chleachdadh (is e seo an dòigh àbhaisteach
san fharsaingeachd).

Mar a chì thu, bidh Windows a’ cleachdadh an sgeama Ceadan/Còraichean a
leanas:

| # | Ceadan | Còraichean |
|:-----:|:----------|:---------|
| 1 | Làn-smachd | A’ ceadachadh: 1, 2, 3, 4, 5, 6, 7 |
| 2 | Atharraich | A’ ceadachadh: 2, 3, 4, 5, 6 |
| 3 | Leughadh & Cur an Gnìomh | A’ ceadachadh: 3, 4 |
| 4 | Liostaich Susbaint na Pasgain | A’ ceadachadh: 4 (ach chan urrainn dha prògraman a ruith) |
| 5 | Leughadh | A’ ceadachadh: 5 (A’ ciallachadh: 4) |
| 6 | Sgrìobhadh | A’ ceadachadh: 6 (A’ ciallachadh:4) |
| 7 | Ceadan Sònraichte | A’ ceadachadh: Measgachaidhean |

### Feartan ceadan fhaidhlichean Windows

Faodar ceadan fhaidhlichean Windows fhaicinn mar cheadan aig a bheil
feartan **coltach** ri ceadan fhaidhlichean (Modhan) UNIX no Linux; chan eil
iad ach air an riochdachadh ann an dòigh eadar-dhealaichte. Mar eisimpleir, ma
tha thu gu sònraichte nad chleachdaiche Unix/Linux, is dòcha gu bheil thu
cleachdte ri ceadan a bhith air an riochdachadh mar 644/666 755/777,
seach a bhith air am mìneachadh anns na briathran gu h-àrd. Mar sin, nuair
a thèid innse dhut 644 a chleachdadh, tha seo co-ionann ri:

* Faodaidh sealbhadair an fhaidhle seo leughadh agus sgrìobhadh ann.
* Faodaidh buidheann an t-sealbhadair am faidhle a leughadh.
* Faodaidh a h-uile duine eile am faidhle a leughadh.

**Nòta:** Chan eil ceadan Windows agus Unix (Liostaichean Smachd Ruigsinneachd)
co-ionann gu tur, oir chan eil Windows a’ cleachdadh an uidheamachd
*Buidhnean* san aon dòigh. Ach, airson na deasbaireachd seo agus a thaobh
àrainneachd aoigheachd-lìn, faodar an coimeas ri chèile ann an dòigh
shìmplidh. Ach, ann an Windows chan eilear a’ cleachdadh ***Buidhnean***
agus bu chòir ***A h-uile duine*** a bhith air a thoirt air falbh.
Seo an t-àite far nach eil Windows agus Unix buileach co-ionann, ach ’s e
na ghabhas dèanamh a bhith a’ *maidseadh* no a’ *cho-cheangal* bhrìgh
cho-ionnan.

Chan eil an geàrr-chunntas seo dha-rìribh a’ dol a thoirt dhut stiùireadh
ceadan sònraichte do Windows no NTFS, ach tuigse nas fheàrr air mar a tha
na ceadan stoidhle UNIX/Linux le àireamhan, a thathar ag ainmeachadh gu
tric, a’ co-cheangal ri coimpiutair le siostam fhaidhlichean NTFS. Bu chòir
na faidhlichean a chuirear sa phasgan freumhaich www no public_html,
no ann an ge bith dè am pasgan air a bheil an làrach agad
(www.domain.com.au no localhost) a’ comharrachadh air a’ chlàr-chruaidh agad,
a bhith fo sheilbh a’ chunntais chleachdaiche agad, ach dìreach mura h-eil
an cleachdaiche sin na chleachdaiche le sochairean sònraichte, leithid
*Rianaire* air Windows no *root* air UNIX/Linux. Bheir na cunntasan seo
cus ruigsinneachd agus cha bu chòir an cleachdadh airson cleachdadh làitheil.

### Deagh chleachdaidhean

Tha cleachdaidhean tèarainteachd a thathar a’ cleachdadh gu tric a’ moladh
gum bu chòir na ceadan a leanas a bhith aig gach **faidhle**.

* **Sealbhadair:** Leughadh & Sgrìobhadh
* **Buidheann:** Leughadh a-mhàin
* **Càch:** Leughadh a-mhàin

Bu chòir na ceadan a leanas a bhith aig gach **eòlaire/pasgan**:

* **Sealbhadair:** Leughadh, Sgrìobhadh & Cur an gnìomh
* **Buidheann:** Leughadh & Cur an gnìomh
* **Càch:** Leughadh & Cur an gnìomh

Dh’fhaodadh argamaid a bhith ann nach e tèarainteachd *as fheàrr* a tha
seo gu riatanach, ach feumar cothromachadh a lorg eadar tèarainteachd,
comas-gnìomh agus furasta cumail suas. Chan eil Windows, eu-coltach ri Unix,
a’ cumail ACL singilte airson *Cur an gnìomh*, ach tha e dìreach a’ toirt
seachad *Leughadh & Cur an gnìomh* còmhla, rud nach eil a’ ciallachadh
* Sgrìobhadh*. Tha an ACL *Leughadh & Cur an gnìomh* ge-tà a’ ciallachadh
*Liosta Susbaint an Eòlaire*. Mar sin, ma tha ceadan *Leughadh & Sgrìobhadh*
agad air eòlaire ach gun *Cur an gnìomh*, chan urrainn dhut susbaint an
eòlaire fhaicinn agus dh’fhaodadh duilgheadasan a bhith agad cuideachd nuair
a dh’fheuchas tu ris an fhaidhle a ruith tro bhrabhsair-lìn. Tha feum air
beagan tuigse air ceadan UNIX/Linux gus an coimeas/co-cheangal gu h-iomlan
ri ceadan Windows. Bu chòir don chlàr a leanas cuideachadh;

| Modh Unix | ACL Windows | Beachdan |
|:-----:|:----------|:---------|
| 7 | Atharraich | Leughadh, Sgrìobhadh & Cur an gnìomh; bu chòir dhut a bhith nad shealbhadair an fhaidhle seo |
| 6 | Leughadh & Sgrìobhadh |  |
| 5 | Leughadh & Cur an gnìomh | air a chleachdadh airson a’ mhòr-chuid de thagraidhean |
| 4 | Leughadh a-mhàin | chan eil tèarainteachd tro neo-shoilleireachd na dheagh chleachdadh |
| 3 | Sgrìobhadh & Cur an gnìomh | chan eil e ri fhaighinn tro Windows, mura cleachdar ceadan “Sònraichte”; chan eil e air a chleachdadh gu tric |
| 2 | Sgrìobhadh a-mhàin | chan eil e ri fhaighinn tro Windows, mura cleachdar ceadan “Sònraichte”; chan eil e air a chleachdadh gu tric |
| 1 | Cur an gnìomh a-mhàin | chan eil e ri fhaighinn tro Windows, mura cleachdar ceadan “Sònraichte”; chan eil e air a chleachdadh gu tric |

An coimeas ri Modhan Unix, nuair a chì thu rudeigin mar 644, bhiodh tu ga
bhriseadh sìos ann an trì eileamaidean:

**6**  :  **4**  : **4**

Tha a’ chiad àireamh a’ riochdachadh ceadan an **t-Sealbhadair***, tha an
dàrna fear a’ riochdachadh ceadan na ***Buidhne*** agus an treas fear ceadan
***Chàich***. Bhiodh an co-ionnan Windows mar a leanas;

* **Sealbhadair** (6) : **Leughadh & Sgrìobhadh**
* **Buidheann** (4) : **Leughadh a-mhàin**
* **Càch** (4) : **Leughadh a-mhàin**

Tha sinn an dòchas gun toir an eisimpleir seo beagan tuigse air mar a nì thu
co-cheangal eadar Modhan/Ceadan Unix agus Ceadan/ACLan Windows. Chan eil an
sgrìobhainn seo a’ gabhail a-steach cuspairean nas iom-fhillte leithid
ceadan *Èifeachdach*, *Oighreachail* no *Sònraichte*. A dh’aindeoin cho
furasta ’s a tha Windows a chleachdadh, tha uidheaman Ceadan agus ACL
Microsoft gu dearbh caran iom-fhillte agus farsaing, ach dh’fhaodadh seo
iomradh luath a thoirt dhut gus cuid den troimh-chèile mu eadar-theangachaidhean
Ceadan Unix agus Windows a lùghdachadh.

*Eadar-theangaichte le openai.com*

