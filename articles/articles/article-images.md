<!--
{
    "source": "https://docs.joomla.org/Adding_an_image_to_an_article",
    "title": "Artaigil: Deasaich - \u00ccomhaighean",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Tha e cudromach tuigsinn gu bheil ìomhaighean airson sgrìobhainnean lìn air an stòradh
fa leth bho theacsa HTML. Nuair a thèid duilleag-lìn iarraidh, gheibh am brabhsair an toiseach
an teacsa agus faidhlichean taice fa leth leithid siotaichean stoidhle agus
sgriobtaichean JavaScript. Gheibhear na h-ìomhaighean nas fhaide air adhart. Gu tric bidh am brabhsair agus
frithealaiche-lìn a’ rèiteachadh dè an tionndadh de dh’ìomhaigh a gheibhear gus freagairt air meud
agus rùn sgrìn a’ bhrabhsair. Tha fiù ’s leudachan Joomla ri fhaighinn 
a chruthaicheas grunn thionndaidhean de phrìomh ìomhaigh ann an diofar mheudan agus
fhòrmatan gus astar lìbhrigidh agus tairgse a leasachadh.

Tha ìomhaighean air an neadachadh ann an duilleagan-lìn le bhith a’ cur a-steach ceanglaichean ann an cruth iomchaidh.
Tha dà dhòigh eadar-dhealaichte ann airson ìomhaighean a chur a-steach ann an artaigilean:

- Tha taba *Susbaint* na foirm deasachaidh a’ leigeil le aon cheangal ìomhaigh no barrachd a chur a-steach
  dìreach ann an teacsa an artaigil. ’S e sin cuspair an artaigil seo.
- Tha taba *Ìomhaighean agus Ceanglaichean* na foirm deasachaidh a’ solarachadh airson ìomhaigh a chur a-steach mar
  *Ìomhaigh tòiseachaidh* no *Ìomhaigh an artaigil slàn*, no an dà chuid. Tha sin air a chòmhdach ann an
  artaigil fa leth mu [Ìomhaighean agus Ceanglaichean](jdocmanual?article=user/articles/article-images-and-links).

’S fhiach eadar-dhealachadh a dhèanamh eadar ìomhaighean ionadail agus ìomhaighean iomallach:

- Tha **Ìomhaighean Ionadail** suidhichte air an aon làrach ris an stàladh Joomla,
  mar as trice sa phasgan *images*. Chan fheum na ceanglaichean ìomhaigh am
  pròtacal agus ainm an àrainn a ghabhail a-steach oir tha iad air an toirt bho roghainnean na làraich.
- Tha **Ìomhaighean Iomallach** suidhichte ann an àite eile air an eadar-lìon. Feumaidh iad
  am pròtacal agus ainm an àrainn a ghabhail a-steach sa cheangal. Dh’fhaodadh cleachdadh ìomhaighean iomallach tro
  *hot-linking* a bhith ceadaichte an-diugh ach gun a bhith ceadaichte a-màireach. Thathar a’ meas cleachdadh
  ìomhaighean iomallach gun chead mar mhodhalachd no eadhon mar ghoid.

## A’ cur ìomhaigh ionadail ris

’S e an dòigh as fheàrr air ìomhaighean ionadail a chur a-steach a bhith a’ cleachdadh a’ phutan **Susbaint CMS → Meadhanan** 
ann am bàr-inneal deasachaidh TinyMCE. Fosglaidh e còmhradh nam Meadhanan a leigeas
leat ìomhaigh sam bith ann am pasgan ìomhaighean na làraich a thaghadh.

**Cudromach:** An toiseach cuir an cursair san àite far a bheil thu airson gun nochd an ìomhaigh. Dh’fhaodadh
sin a bhith aig toiseach no deireadh paragraf, no ann am paragraf falamh.

![An còmhradh priob-uinneig nam meadhanan](../../../gd/images/articles/article-images/01-articles-edit-images-media.png)

Anns a’ chòmhradh priob-uinneig, seòl chun na h-ìomhaigh a tha thu airson a chleachdadh agus tagh i. Nuair
a thèid a taghadh, nochdaidh foirm ag iarraidh dàta a bharrachd.

- **Tuairisgeul na h-Ìomhaigh (Teacsa Alt)** Tha seo cudromach airson adhbharan ruigsinneachd
  agus gèilleadh ri inbhean lìn.
- **Clas na h-Ìomhaigh** Ma thèid ìomhaigh a chleachdadh gun cheann-sgrìobhadh, faodar cuid de
  chlasaichean gnàthaichte a chur an sàs an seo. Mar eisimpleir, nì *float-end ms-2 mb-1*
  an ìomhaigh co-thaobhadh ris an taobh dheas agus cuiridh e teacsa timcheall oirre le beàrnan
  air an taobh chlì agus gu h-ìosal gus nach bi an teacsa a’ beantainn ris an ìomhaigh.
- **Clas an Fhigear** Ma tha ceann-sgrìobhadh air a shuidheachadh, faodar clas co-thaobhachaidh, ma tha
  gin ann, a chur an sàs san Fhigear. Thoir an aire, ann an Cassiopeia, gu bheil beàrnan air an cur an sàs
  san fhigear le siota stoidhle na teamplaide, agus mar sin tha *float-start* no *float-end*
  gu leòr.
- **Ceann-sgrìobhadh an Fhigear** Cuiridh seo an comas an ceann-sgrìobhadh, a sheallas susbaint an
  raoin seo mar cheann-sgrìobhadh fon ìomhaigh.

**Cudromach:** Ma tha raon *Ceann-sgrìobhadh an Fhigear* falamh, thèid an ìomhaigh a chur a-steach
taobh a-staigh taga `<img...>` agus cha tèid an raon *Clas an Fhigear* a chleachdadh. Ma tha
teacsa ann an raon *Ceann-sgrìobhadh an Fhigear*, thèid an taga `<img...>` a chuairteachadh ann an
tagaichean `<figure>...</figure>`. ’S iad na clasaichean as fheumaile ri chur ris *float-start*
agus *float-end* gus an ìomhaigh a chur air taobh chlì no deas na duilleige, leis an
teacsa a’ sruthadh timcheall oirre.

Tagh am putan *Cuir Meadhan a-steach* gus an ìomhaigh a chur a-steach. Dùinidh an sgrìn Cuir Ìomhaigh a-steach
agus nochdaidh an ìomhaigh san deasaiche. No
tagh am putan *Sguir dheth* gus an sgrìn Cuir Ìomhaigh a-steach fhàgail.

**Gliocas:** Tagh am putan Toglaich an Deasaiche gus na stoidhlichean Ìomhaigh agus
Figear a chaidh an cur an sàs fhaicinn. Dh’fhaodadh gum feum thu figear no img a ghearradh agus a
phasgadh gus a ghluasad.

### A’ cleachdadh Slaod agus Leig airson ìomhaighean ionadail

Faodaidh tu ìomhaigh a shlaodadh bhon deasg no bho bhrabhsair fhaidhlichean gu dìreach a-steach do
theacsa an artaigil, agus thèid an ìomhaigh a luchdadh suas don phasgan mheadhanan agus a chur
san artaigil. ’S e an aon dhuilgheadas gun tèid na h-ìomhaighean uile a luchdaichear suas mar seo a chur
san aon phasgan mheadhanan.

Tha suidheachadh an *Eòlaire Ìomhaighean* a thèid a chleachdadh airson luchdachadh suas agus co-dhiù a tha am feart seo
an comas (air a chomasachadh gu bunaiteach) air an suidheachadh ann an Roghainnean rèiteachaidh TinyMCE.

## A’ cur ceangal ri ìomhaigh iomallach ris

Mura h-eil an ìomhaigh a tha thu airson a chleachdadh ann am pasgan images an stàlaidh Joomla agad,
tha modh-obrach beagan eadar-dhealaichte a dhìth.

- Tagh **Cuir a-steach → Ìomhaigh** bho bhàr-inneal TinyMCE gus bogsa còmhraidh fhosgladh.
- Anns an raon **Tùs**, cuir a-steach URL na h-ìomhaigh.
- Lìon na raointean eile mar a tha riatanach.
- Tha taba **Adhartach** a’ solarachadh roghainnean cruthachaidh a thèid an cur an sàs mar
  stoidhlichean in-loidhne. Feuch le 1rem, 2, groove.

![An còmhradh priob-uinneig airson ìomhaigh a chur a-steach](../../../gd/images/articles/article-images/02-articles-edit-images-external-image.png)

### A’ cleachdadh Slaod is Leig às gus ceanglaichean gu dealbhan iomallach a chur a-steach

’S urrainn dhut ceangal dealbh a shlaodadh is a leigeil às bho làrach-lìn iomallach gu dìreach ann an teacsa an artaigil agad. Ach bi mothachail gum faodadh seo HTML soitheach an deilbh a chopaigeadh cuideachd, le aithrisean clas nach eil dligheach airson na làraich agad.

## A’ luchdachadh suas dhealbhan a’ cleachdadh a’ chòmhraidh Meadhanan

’S urrainn dhut dealbhan ùra a luchdachadh suas dhan phasgan dhealbhan agad bhon duilleag 
*Susbaint CMS -> Meadhanan*.

- Fosgail còmhradh Meadhanan agus rach dhan phasgan far a bheil thu airson
  dealbhan ùra a stòradh airson an artaigil làithrich.
- Tagh am putan Luchdaich suas aig mullach clì sgrìn nam Meadhanan gus
  brabhsair fhaidhlichean fhosgladh.
- Tagh na faidhlichean dhealbhan a tha thu airson luchdachadh suas. Tagh Fosgail ann am brabhsair
  nam faidhlichean gus an taghadh a dhearbhadh. Nota: Tha stoidhle agus
  cruth a’ bhrabhsair fhaidhlichean an urra ris a’ bhrabhsair agus an t-siostam-obrachaidh a tha thu a’ cleachdadh.
- Nochdaidh na faidhlichean taghte ann an òrdugh na h-aibideil ann an sgrìn
  Meadhanan/Ìomhaigh.
- Nuair a bhios an luchdachadh suas deiseil, nochdaidh brath dearbhaidh uaine
  aig mullach na sgrìn.

’S urrainn dhut a-nis an dealbh a chaidh a luchdachadh suas a thaghadh agus a chur a-steach mar a bha roimhe.

*Eadar-theangaichte le openai.com*