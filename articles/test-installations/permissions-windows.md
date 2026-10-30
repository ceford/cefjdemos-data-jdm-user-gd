<!--
{
    "source": "https://docs.joomla.org/How_do_Windows_file_permissions_work?",
    "title": "Ceadan Fhaidhlichean: Windows",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Dhaibhsan agaibh a tha an dàrna cuid a’ leasachadh no a’ lìbhrigeadh nan làraichean-lìn Joomla! agaibh à àrainneachd Windows, faodaidh e a bhith doirbh uaireannan fiosrachadh iomchaidh fhaighinn mu cheadan. Gu mì-fhortanach, ’s e fìrinn a th’ ann gu bheil a’ mhòr-chuid de sheirbheis-lìn air a thabhann fo Unix agus gu bheil Unix air a dheagh chlàradh san àrainneachd seo. Tha sinn an dòchas gun cuidich am fiosrachadh a leanas le mì-chinnt sam bith a shoilleireachadh agus gun toir e beagan stiùiridh cuideachd. 

## Sealladh farsaing air frithealaichean-lìn Windows

An toiseach, bruidhnidh sinn mu na h-eadar-dhealachaidhean eadar frithealaichean. San fharsaingeachd, tha coltas ann gu bheil a’ mhòr-chuid de luchd-cleachdaidh Windows a’ cleachdadh Apache (Win32) no Microsoft IIS. Tha an dà fhrithealaiche-lìn seo ag obrachadh ann an dòighean glè eadar-dhealaichte agus a’ cleachdadh mhodalan lìbhrigidh a tha beagan eadar-dhealaichte. Mar as trice, bidh Apache (Win32) a’ ruith air a’ choimpiutair aoigheachd mar an Cleachdaiche fon deach a stàladh, ach bidh IIS ga stàladh fo chleachdaiche shònraichte ach a’ ruith fo chleachdaiche a chaidh a stàladh às ùr *IUSR_*. 

## Roghainnean bunaiteach nan ceadan

Gu bunaiteach, chan àbhaist do Unix làn chothrom a thoirt ach don chleachdaiche *sealbhach* air faidhlichean agus pasgain. An coimeas ri sin, bheir Windows, gu bunaiteach, làn cheadan don bhuidheann *Everyone* cuideachd. Is e a’ chiad rud a nì rianaire math Windows còraichean na buidhne *Everyone* a thoirt air falbh gus tèarainteachd a leasachadh. Airson deuchainn air PC ionadail, is dòcha nach eil seo riatanach, ach tha e a’ mìneachadh carson, mura tèid *Everyone* a thoirt air falbh agus ma ruitheas tu sgriobt de sheòrsa air choreigin airson ceadan a sgrùdadh no sgrùdadh Ro-stàlaidh Joomla!, gum bi làn cheadan *Leugh, Sgrìobh agus Cuir an gnìomh* agad. Tha thu a’ faighinn còraichean na buidhne *Everyone*. 

## Microsoft Internet Information Server (IIS)

Tha IIS a’ tighinn ann an dà phrìomh sheòrsa, PWS (Personal WebServer), agus IIS (Internet Information Server). Gu bunaiteach, ’s e an aon aplacaid a th’ annta. Chan eil ann am PWS ach dreach lùghdaichte de IIS a chaidh a dhealbhadh airson àrainneachdan deasg, agus chaidh IIS a dhealbhadh airson àrainneachdan frithealaiche. Chan eil PWS a’ leigeil leat ach aon phrìomh làrach-lìn a bhith agad, agus mar sin bidh stàlaidhean nan aplacaidean agad mar as trice ann am fo-phasganan na prìomh làraich-lìn. Tha IIS, air an làimh eile, a’ toirt seachad na comasan airson Òstairean Brìgheil a ruith às na pasganan seo, a’ lìbhrigeadh comas ioma-làraich.

Air sgàth nan diofar chuingealachaidhean gnìomh, chan eil an *Permissions Wizard* aig PWS oir chaidh a dhearbhadh nach eil feum air. Cha bhi ach aon chleachdaiche a’ cleachdadh an Fhrithealaiche PWS. Ann an IIS, bidh mòran chleachdaichean a’ cleachdadh an Fhrithealaiche, agus mar sin tha feum air sònrachaidhean cheadan eadar-dhealaichte.

Aon uair ’s gu bheil an cunntas *Everyone* air a thoirt air falbh, chan eil air fhàgail aig Windows IIS ach an cunntas *IUSR_** le còraichean aig an ìre as àirde air pasganan an Fhrithealaiche-lìn. Bu chòir do sgrùdadh cheadan a-nis toraidhean eadar-dhealaichte a shealltainn. Chan eil ach làn cheadan aig a’ chunntas *IUSR_** agus bu chòir do chleachdaichean eile *Leugh a-mhàin* no gun chòraichean idir fhaighinn. Tha na còraichean air an dearbhadh leis na cleachdaichean eile a chaidh na còraichean iomchaidh a shònrachadh dhaibh le làimh air pasganan IIS. 

### Sònrachadh cheadan

Tha sònrachadh cheadan ann an Windows reusanta sìmplidh, ach faodaidh e a bhith beagan troimh-chèile aig amannan. Dèan briogadh deas air a’ phasgan no air an fhaidhle iomchaidh. Le bhith a’ taghadh *Properties* no *Sharing and Security* thèid thu a-steach do phana Stiùireadh Tèarainteachd Windows. Ma thaghas tu (le aon bhriogadh) ainm-cleachdaiche sam bith a tha air a liostadh, nochdaidh na còraichean a th’ aig a’ chleachdaiche sin anns an leth ìosal den phana. Dh’fhaodadh cuid de chòraichean a bhith *liath*. Chan eil iad sin rim faighinn, an dara cuid air sgàth ’s nach eil ceadan àrd gu leòr aig a’ chleachdaiche làithreach (fon deach logadh a-steach agad) airson an atharrachadh, no seach gu bheil iad air an sealbhadh bhon phasgan gu h-àrd agus air an suidheachadh gus ceadan a’ phasgain aig an ìre as àirde sin a chleachdadh. (Mar as trice, ’s e seo an uidheam bunaiteach.) 

Mar a chì thu, tha Windows a’ cleachdadh an sgeama Ceadan/Còraichean a leanas: 

| # | Smachd | A’ ceadachadh #     |
| :---:        |:----   | :--- |
| 1.|  Smachd slàn | A’ ceadachadh: 1, 2, 3, 4, 5, 6, 7 |
| 2.| Atharraich | A’ ceadachadh: 2, 3, 4, 5, 6 |- |
| 3.| Leugh & Cuir an gnìomh | A’ ceadachadh: 3, 4  |- | 
| 4.| Liostaich susbaint a’ phasgain | A’ ceadachadh: 4 (ach chan urrainn dha prògraman a ruith)  |- |
| 5.| Leugh | A’ ceadachadh: 5 (A’ ciallachadh: 4) |- |
| 6.| Sgrìobh | A’ ceadachadh: 6 (A’ ciallachadh:4 ) |- |
| 7.| Ceadan sònraichte | A’ ceadachadh: Measgachaidhean |

### Feartan cheadan fhaidhlichean Windows

Faodar ceadan fhaidhlichean Windows fhaicinn mar fheartan coltach ri ceadan fhaidhlichean (Modhan) UNIX no Linux. Chan eil iad air an riochdachadh ach san aon dòigh. Mar eisimpleir, ma tha thu gu h-àraidh nad neach-cleachdaidh Unix/Linux, is dòcha gu bheil thu cleachdte ri ceadan air an riochdachadh mar 644/666 755/777, an àite a bhith air an cur an cèill anns na teirmean gu h-àrd. Mar sin, nuair a chleachdas tu 644, tha seo a’ ciallachadh: 

- Faodaidh sealbhadair an fhaidhle seo leughadh agus sgrìobhadh ann.
- Faodaidh buidheann an t-sealbhadair am faidhle a leughadh.
- Faodaidh a h-uile duine eile am faidhle a leughadh.

**Nota:** Chan eil ceadan Windows agus Unix (Liostaichean Smachd Ruigsinneachd) dìreach co-ionann; chan eil Windows a’ cleachdadh an uidheamachd *Buidhnean* san aon dòigh. Airson a’ chòmhraidh seo agus a thaobh na h-àrainneachd aoigheachd lìn, faodar an coimeas ri chèile. Ach, ann an Windows chan eilear a’ cleachdadh *Buidhnean* agus bu chòir *A h-uile duine* a bhith air a thoirt air falbh. Seo far nach eil Windows agus Unix buileach co-ionann, ach ’s e na ghabhas dèanamh na brìghtean co-ionann a *cho-fhreagairt* no a *cheangal* ri chèile. 

Chan eil an geàrr-chunntas seo dha-rìribh a’ dol a thoirt dhut stiùireadh air ceadan a tha sònraichte do Windows no NTFS, ach tuigse air mar a tha na ceadan ann an stoidhle UNIX/Linux, a tha air an ainmeachadh gu cumanta le àireamhan, a’ co-fhreagairt air inneal le siostam fhaidhlichean NTFS. Bu chòir na faidhlichean a chuirear ann am pasgan freumha `www` no `public_html`, no ann an ge bith dè an eòlaire ris a bheil an làrach agad (`www.domain.com` no `localhost`) a’ comharrachadh air a’ chlàr-chruaidh agad, a bhith fo sheilbh a’ chunntais chleachdaiche agad, ach dìreach mura h-eil an cleachdaiche sin na chleachdaiche sochairichte, leithid *Rianaire* ann an Windows no *root* ann an UNIX/Linux. Tha na cunntasan seo a’ ceadachadh cus ruigsinneachd agus cha bu chòir an cleachdadh gu bràth airson cleachdadh làitheil. 

### Cleachdaidhean as Fheàrr

Tha cleachdaidhean tèarainteachd a thathar a’ cleachdadh gu cumanta a’ moladh gum bu chòir na **faidhlichean** uile na ceadan a leanas a bhith aca.

- **Sealbhadair** Leughadh & Sgrìobhadh
- **Buidheann** Leughadh a-mhàin
- **Càch** Leughadh a-mhàin

Bu chòir na ceadan a leanas a bhith aig a h-uile **eòlaire/pasgan**.

- **Sealbhadair** Leughadh, Sgrìobhadh & Cur an gnìomh
- **Buidheann** Leughadh & Cur an gnìomh
- **Càch** Leughadh & Cur an gnìomh

Dh’fhaodadh argamaid a bhith ann nach e tèarainteachd *as fheàrr* a tha seo riatanach, ach feumar cothromachadh a lorg eadar tèarainteachd, comas-gnìomh agus comas cumail suas. 

Chan eil Windows, eu-coltach ri Unix, a’ cumail aon ACL airson *Cur an gnìomh*, ach tha e dìreach a’ toirt seachad *Leughadh & Cur an gnìomh* còmhla, rud nach eil a’ ciallachadh *Sgrìobhadh*. Ach tha an ACL *Leughadh & Cur an gnìomh* a’ ciallachadh *Liosta de Shusbaint an Eòlaire*. Mar sin, mura h-eil agad ach ceadan *Leughadh & Sgrìobhadh* air eòlaire ach gun *Cur an gnìomh*, chan urrainn dhut susbaint an eòlaire fhaicinn agus dh’fhaodadh duilgheadasan a bhith agad cuideachd nuair a dh’fheuchas tu ris an fhaidhle a ruith tro bhrobhsair-lìn. Tha feum air beagan tuigse air ceadan UNIX/Linux gus an co-fhreagairt gu h-iomlan ri ceadan Windows. Bu chòir don chlàr a leanas cuideachadh: 

| Modh Unix   | ACL Windows | Beachdan|
|:-----------:| :----   | :--- |
| 7 | Atharraich| Leughadh, Sgrìobhadh & Cur an gnìomh; bu chòir dhut a bhith nad shealbhadair an fhaidhle seo | 
| 6 | Leughadh & Sgrìobhadh | | 
| 5 | Leughadh & Cur an gnìomh| air a chleachdadh airson a’ mhòr-chuid de thagraidhean | 
| 4 | Leughadh a-mhàin | chan eil tèarainteachd tro dhorchadas na dheagh chleachdadh | 
| 3 | Sgrìobhadh & Cur an gnìomh | chan eil e ri fhaighinn tro Windows, mura cleachdar *Ceadan Sònraichte*; chan eil e air a chleachdadh gu cumanta | 
| 2 | Sgrìobhadh a-mhàin | chan eil e ri fhaighinn tro Windows, mura cleachdar *Ceadan Sònraichte*; chan eil e air a chleachdadh gu cumanta | 
| 1 | Cur an gnìomh a-mhàin | (chan eil e ri fhaighinn tro Windows, mura cleachdar *Ceadan Sònraichte*; chan eil e air a chleachdadh gu cumanta) |

An coimeas ri modhan Unix, nuair a chì thu rudeigin mar 644, roinn sin ann an trì eileamaidean: 

Tha a’ chiad àireamh a’ riochdachadh ceadan an t-sealbhadair, tha an dàrna fear a’ riochdachadh ceadan na buidhne agus tha an treas fear a’ riochdachadh ceadan chàich. Bhiodh an co-ionann Windows mar a leanas: 

- **Sealbhadair** (6) Leughadh & Sgrìobhadh
- **Buidheann** (4) Leughadh a-mhàin
- **Càch** (4) Leughadh a-mhàin

Tha sinn an dòchas gu bheil an t-eisimpleir seo a’ toirt beagan tuigse air mar a ghabhas Modhan/Ceadan Unix a cho-fhreagairt ri Ceadan/ACLs Windows. Chan eil an sgrìobhainn seo a’ gabhail a-steach cuspairean nas iom-fhillte leithid ceadan *Èifeachdach*, *Sealbhaichte* no *Sònraichte*. A dh’aindeoin cho furasta ’s a tha Windows a chleachdadh, tha uidheaman Ceadan agus ACL Microsoft gu dearbh caran iom-fhillte agus farsaing, ach dh’fhaodadh seo iomradh luath a thoirt dhut gus feuchainn ri cuid den troimh-chèile mu eadar-theangachaidhean Ceadan Unix agus Windows a lùghdachadh. 

*Air eadar-theangachadh le openai.com*

