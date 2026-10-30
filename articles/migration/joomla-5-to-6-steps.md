<!--
{
    "source": "https://docs.joomla.org/https:",
    "title": "Joomla 5 gu 6 Ceum air Cheum",
    "description": " ",
    "author": ""
}
-->

<div class="alert alert-warning">
<p class="h3">Rabhadh</p>

Tha an iùl seo a’ gabhail ris gu bheil thu a’ tòiseachadh le Joomla 5.4.x. Ma tha thu air tionndadh nas tràithe, dèan cinnteach gun dèan thu imrich no ùrachadh gu Joomla 5.4.x mus ùraich thu gu Joomla 6.x.
</div>

## Ro-ràdh

Deagh naidheachd airson Joomla 5.4.x gu 6.x: ’s e ùrachadh a th’ ann, chan e imrich. Carson? Dà phrìomh adhbhar:

- Obraichidh leudachain Joomla 5 (J5) a thug air falbh a h-uile còd nach eilear a’ moladh tuilleadh, a tha a’ cleachdadh còd Joomla ùraichte, agus nach eil feumach air am plugan Behaviour - Backward Compatibility a bhith an comas, ann an Joomla 6 (J6)
- Obraichidh a’ mhòr-chuid den fheadhainn eile leis a’ phlugain ùr Behaviour - Backward Compatibility 6 air a chomasachadh

Tha an sgrìobhainn seo a’ nochdadh a’ phròiseis as sìmplidhe le bhith a’ cur a’ phlanaidh agus na ceumannan air cheum còmhla ann an aon sgrìobhainn. Ach, bidh feum agad fhathast air cuid de sgilean. Faic an [[Migration Step by Step Self Assessment|Fèin-mheasadh]] gus faighinn a-mach am bu chòir dhut an ùrachadh a dhèanamh leat fhèin no nach bu chòir.

<div class="alert alert-info">
<p class="h3">Sgrìobhainnean leasachaidh 5.4 gu 6.0 airson luchd-leasachaidh leudachain treas-phàrtaidh.</p>

- [A chaidh a thoirt air falbh agus Neo-fhreagarrachd air ais](https://manual.joomla.org/60/removed-backward-incompatibility)
- [Deachaidhean ùra](https://manual.joomla.org/60/new-deprecations)
- [Mu dheidhinn sgrìobhainnean imrich](https://manual.joomla.org/migrations)
- [Feartan ùra](https://manual.joomla.org/60/new-features/)
</div>

## Planadh 5.4.x gu 6.x

### Sònrachadh aoigheachd/teicnigeach

1. Faigh a-mach a bheil an àrainneachd aoigheachd agad a’ coinneachadh ris na riatanasan. Cha bhith e comasach dhut ùrachadh gu Joomla 6 mura coinnich àrainneachd an fhrithealaiche agad ris na [riatanasan teicnigeach](https://manual.joomla.org/docs/get-started/technical-requirements/) as lugha. Cha nochd an roghainn ùrachaidh ann am pàirt Joomla Update.
    - PHP 8.3
    - MySQL 8.0.13
    - MariaDB 10.6.x
    - PostgreSQL 14.0

’S urrainn dhut fiosrachadh an t-siostaim agad a sgrùdadh ann an làrach Joomla 5 le bhith a’ briogadh air System -> System Information. Cuir fios chun t-solaraiche aoigheachd agad mura coinnich an frithealaiche agad ris na riatanasan.

![Deas-bhòrd an t-siostaim leis a’ cheangal Fiosrachadh an t-Siostaim air a chomharrachadh](../../../en/images/migration/joomla-5-to-6-steps/01-steps-5-to-6-system-dashboard.png)

Seo eisimpleir de dh’àrainneachd a tha a’ coinneachadh ris na riatanasan teicnigeach. Tha e a’ sealltainn MySQL 8.0.43, PHP 8.3, Joomla 5.4.x, agus am Plugan Co-fhreagarrachd Air Ais à comas.

![Fiosrachadh an t-siostaim a’ sealltainn Tionndadh Joomla, Tionndadh PHP, Seòrsa DB, Tionndadh DB agus am Plugan Co-fhreagarrachd Air Ais à comas](../../../en/images/migration/joomla-5-to-6-steps/02-steps-5-to-6-system-information.png)

2. Thoir sùil air na leudachain agad uile airson co-fhreagarrachd ri Joomla 6. Tha grunn shuidheachaidhean ann le leudachain treas-phàrtaidh airson an ùrachaidh seo.

    1. Dh’fhaodadh an leudachan a bhith co-fhreagarrach ri J5 agus J6 GUN am plugan co-fhreagarrachd air ais a chleachdadh.
    2. Dh’fhaodadh an leudachan a bhith co-fhreagarrach ri J5 agus J6 LE am plugan co-fhreagarrachd air ais a chleachdadh.
    3. Dh’fhaodadh coltas a bhith air gu bheil an leudachan ag obair ann an J6, ach nuair a dh’fheuchas tu ri a chleachdadh, tha e briste.
    4. Dh’fhaodadh an leudachan an làrach gu lèir a bhriseadh.

Na gabh dragh! Chan eil e cho dona ’s a tha e coltach! An toiseach, bruidhnidh sinn mu na plugain co-fhreagarrachd air ais.

<div class="alert alert-warning">
<p class="h3">Rabhadh</p>

Gus ùrachadh bho Joomla 5.4.x gu 6.x, FEUMAIDH am Plugan Co-fhreagarrachd Air Ais airson Joomla 5 a bhith À COMAS.
</div>

### Na Plugain Co-fhreagarrachd air Ais

Tha am plugan [Giùlan - Co-fhreagarrachd air ais 6](https://manual.joomla.org/60/compat-plugin/) a tha air a ghabhail a-steach le Joomla 5.4.x ann gus co-fhreagarrachd air ais eadar Joomla 5 agus Joomla 6 a neartachadh. Bidh am plugan a’ cuideachadh leudachain treas-phàrtaidh gus clasaichean nach eil tuilleadh air an gabhail a-steach ann an Joomla 6 a chleachdadh. Tha e air a chur an gnìomh mar sheòrsa plugain “Giùlan” gus dèanamh cinnteach gu bheil e air a luchdadh mus tèid plugan sam bith eile a luchdadh.

![Duilleag nam plugan a’ sealltainn nam plugan co-fhreagarrachd air ais](../../../en/images/migration/joomla-5-to-6-steps/03-steps-5-to-6-bc-plugins.png)

Tha an dealbh gu h-àrd a’ sealltainn dà phlugain Co-fhreagarrachd air Ais:

1. Giùlan - Co-fhreagarrachd air ais agus
2. Giùlan - Co-fhreagarrachd air ais 6

Tha am plugan Giùlan - Co-fhreagarrachd air ais (gun àireamh ann an Ainm a’ Phlugain) air a sholarachadh le Joomla 4.4.x gus còmhdach co-fhreagarrachd air ais a chruthachadh airson leudachain Joomla 5. **Feumar am plugan seo a chur à comas mus dèanar ùrachadh gu J6**.

Tha am plugan Giùlan - Co-fhreagarrachd air ais 6 air a sholarachadh le Joomla 5.4.x gus còmhdach co-fhreagarrachd air ais a chruthachadh airson leudachain Joomla 6.

Chan fhaod an dithis aca a bhith an comas fhad ’s a thathar ag ùrachadh gu J6.

Mus dèanar ùrachadh bho Joomla 5 gu Joomla 6, feumar am plugan Giùlan - Co-fhreagarrachd air ais (gun àireamh ann an Ainm a’ Phlugain) a chur à comas. Feumaidh tu dèanamh cinnteach gun urrainn do na leudachain treas-phàrtaidh agad uile ruith air an làrach-lìn agad gun am plugan Giùlan - Co-fhreagarrachd air ais a bhith an comas mus urrainn dhut ùrachadh gu J6.

Às dèidh dhut dearbhadh gu bheil gach aon de na leudachain treas-phàrtaidh agad a’ gèilleadh agus ag obair gu h-iomlan ann an J5 gun am plugan Giùlan - Co-fhreagarrachd air ais a bhith an comas, faodaidh tu a chur à comas. A dh’aindeoin sin, tha sinn a’ moladh a bhith faiceallach. Mus cuir thu am plugan co-fhreagarrachd air ais à comas, thathar a’ moladh aon den dà rud a leanas a dhèanamh:

1. Dèan e air làrach leasachaidh/deuchainn. San dòigh sin, ma chaill thu gun fhiosta aon leudachan a tha a’ fàgail nach eil an deireadh-cùil agad ruigsinneach, cha toir e do làrach riochdachaidh sìos.
2. Dèan cinnteach gu bheil cothrom agad air an db. San dòigh sin, faodaidh tu am plugan a chur an comas a-rithist gu luath tron db ma bhios feum air. Barrachd mu dheidhinn seo gu h-ìosal.

Nuair a thathar ag ùrachadh gu J5.4.x, thèid am plugan Giùlan - Co-fhreagarrachd air ais 6 a chur an comas gu fèin-obrachail. Ann an stàlaidhean ùra de J6, bidh am plugan co-fhreagarrachd air ais à comas a ghnàth.

Bidh am plugan Giùlan - Co-fhreagarrachd air ais 6, a tha a’ toirt taic do leudachain a tha ag obair ann an J5, an sàs tro J6. Ann an J7, cha tèid na leudachain J5 a dhèanamh co-fhreagarrach air ais leis a’ phlugain. Bheir seo dà bhliadhna a bharrachd do luchd-leasachaidh leudachan gus na leudachain aca a dhèanamh co-fhreagarrach ri J6 gun a’ phlugain co-fhreagarrachd air ais. ’S e an rùn, le gach sgaoileadh cearcall-beatha, gum bi plugan co-fhreagarrachd air ais a’ toirt taic don chearcall-beatha a bha roimhe gus an tèid an ath chearcall-beatha a ruighinn.

An urrainn dhut am plugan Giùlan - Co-fhreagarrachd air ais 6 a chur à comas ann an J6 a-riamh? Ceist mhath. Às dèidh dhut dearbhadh gu bheil gach aon de na leudachain treas-phàrtaidh agad a’ gèilleadh agus ag obair gu h-iomlan gun am plugan co-fhreagarrachd air ais a bhith an comas, faodaidh tu am plugan Giùlan - Co-fhreagarrachd air ais 6 a chur à comas. A dh’aindeoin sin, tha sinn a’ moladh a bhith faiceallach. Mus cuir thu am plugan Giùlan - Co-fhreagarrachd air ais 6 à comas, thathar a’ moladh aon den dà rud a leanas a dhèanamh:

1. Dèan e air làrach leasachaidh/deuchainn. San dòigh sin, ma chaill thu gun fhiosta aon leudachan a tha a’ fàgail nach eil an deireadh-cùil agad ruigsinneach, cha toir e do làrach riochdachaidh sìos.
2. Dèan cinnteach gu bheil cothrom agad air an db. San dòigh sin, faodaidh tu am plugan a chur an comas a-rithist gu luath ma bhios feum air. Barrachd mu dheidhinn seo gu h-ìosal.

### Sgrùdadh ro-ùrachaidh no Stiùirich leudachain

Gu teòiridheach, innsidh an sgrùdadh ro-ùrachaidh dhut a bheil na leudachain treas-phàrtaidh agad co-fhreagarrach ri J6. Ach, chan eil an sgrùdadh ro-ùrachaidh feumail ach ma tha gach leasaiche leudachain air an leudachan aca ùrachadh gus co-fhreagarrachd nan leudachan aca a nochdadh. Ann an saoghal foirfe, innsidh an earrann **Leudachain** den sgrùdadh ro-ùrachaidh dhut a bheil leudachan:

* Gabhaidh ùrachadh às aonais am plugan co-fhreagarrachd air ais air a chur an comas
* Gabhaidh ùrachadh leis a’ phlugan co-fhreagarrachd air ais air a chur an comas
* A bheil feum air ùrachadh an leudachain mus tèid ùrachadh bho J5 gu J6
* Neo-fhreagarrach gu tur

Tha deuchainnean air neo-chunbhalachdan a nochdadh eadar leudachain a tha co-fhreagarrach agus feadhainn nach eil co-fhreagarrach. Chan eil seo na dhuilgheadas leis an eileamaid sgrùdaidh ro-ùrachaidh. An àite sin, bidh leasaichean leudachain a’ cur fiosrachadh tron leudachan aca a bhiodh a’ lìonadh an sgrùdaidh ro-ùrachaidh gu ceart. Mura h-eil na leudachain aca air an còdadh gus am fiosrachadh ceart innse don sgrùdadh ro-ùrachaidh, chan eil mòran (no dad) as urrainn don sgrùdadh ro-ùrachaidh, no do Phròiseact Joomla!, a dhèanamh mu dheidhinn. Bhiodh làrach-lìn leasaiche an leudachain treas-phàrtaidh na thùs fiosrachaidh math airson dearbhadh mar a bu chòir dèiligeadh ris an leudachan shònraichte rè an ùrachaidh bho J5 gu J6.

Tha an dealbh nas fhaide sìos san earrainn seo a’ sealltainn eisimpleir de dh’eileamaid sgrùdaidh ro-ùrachaidh Joomla 5.4.x anns an earrainn Leudachain.

Seallaidh an earrann aig a’ mhullach na leudachain a dh’fheumas ùrachadh. Rach gu System -> Update -> Extensions agus ùraich na leudachain agad.  
Tha an earrann sa mheadhan a’ sealltainn leudachain far nach eil fiosrachadh ùrachaidh ri fhaighinn bhon leasaiche leudachain. Cha bhi fios agad a bheil iad sin co-fhreagarrach no nach eil gun deuchainn a dhèanamh orra no gun fios a chur chun an leasaiche.

Tha an earrann aig a’ bhonn a’ sealltainn nan leudachan nach eil feumach air ùrachadh. Tha seo a’ ciallachadh gu bheil na leudachain ag innse do Joomla gu bheil iad co-fhreagarrach ri Joomla 6. Chan eil e air a shònrachadh a bheil feum aca air a’ phlugan co-fhreagarrachd air ais no nach eil.

Thoir an aire nach eil na leudachain seo air am moladh le Pròiseact Joomla. Tha na leudachain seo air an sealltainn mar eisimpleir a-mhàin. Chaidh an taghadh air thuaiream bhon JED mar dheuchainn.

![Earrann Leudachain an Sgrùdaidh ro-ùrachaidh](../../../en/images/migration/joomla-5-to-6-steps/04-steps-5-to-6-pre-update-check.png)

Thathar a’ moladh nach cleachd thu ach an earrann **Leudachain** den eileamaid sgrùdaidh ro-ùrachaidh mar shealladh farsaing aig ìre air leth àrd, ach chan ann mar an aon thùs fìrinn 100%. Ann an dòigh eile, is dòcha nach urrainn dhut earbsa a chur anns an eileamaid sgrùdaidh ro-ùrachaidh a rèir nan leudachan a tha thu a’ cleachdadh.

*Dè an fhìor thùs fiosrachaidh ma-thà?* Systems -> Manage Extensions

![Deas-bhòrd an t-siostaim le Manage Extensions air a chomharrachadh](../../../en/images/migration/joomla-5-to-6-steps/05-steps-5-to-6-system-dashboard-manage.png)

Bhon sgrìn Extensions: Manage, chì thu na leudachain treas-phàrtaidh uile a tha thu a’ cleachdadh air an làrach. San dealbh-sgrìn gu h-ìosal chì thu am prìomh sgrìn. Sa cholbh Author, chì thu ainm leasaiche leudachain mòr-chòrdte ann an grunn shreathan. Chì thu cuideachd Ùghdar Pròiseact Joomla ann an grunn shreathan.

![Prìomh dhuilleag Manage Extensions](../../../en/images/migration/joomla-5-to-6-steps/06-steps-5-to-6-extensions-manage.png)

Thoir sùil air na leudachain treas-phàrtaidh agad. An ath rud, feumaidh tu dearbhadh a bheil iad co-fhreagarrach ri J6 (leis a’ phlugan co-fhreagarrachd air ais no às aonais) no nach eil. Mura h-eil iad co-fhreagarrach, cha soirbhich leis an ùrachadh.

### Trì dòighean gus na leudachain treas-phàrtaidh agad a sgrùdadh airson co-chòrdalachd le J6

1. Thoir sùil air làrach-lìn an leasaiche.
2. Dèan lethbhreac-glèidhidh/lethbhreac den làrach J5 agad, aisig e air fo-àrainn, cuir an gnìomh dì-bhugachadh, agus lean na ceumannan ceum air cheum (gu h-ìosal) gus ùrachadh gu J6. Faic a bheil dad a’ briseadh. Ma bhriseas, cuir à comas gach leudachan a thilgeas mearachd agus dèan nota den leudachan. Feumaidh tu fios a chur chun an leasaiche mu dheidhinn, leis nach eil e co-chòrdail ri J6.
3. Stàlaich pasgan J6 glan air fo-àrainn, cuir an gnìomh am Plugan Giùlain - Co-fhreagarrachd air Ais, stàlaich na leudachain uile a chleachdas tu agus faic a bheil iad ag obair.

NOTA: Seallaidh Directory Leudachain Joomla! (JED) bràistean co-chòrdalachd Joomla 6 airson leudachain a tha co-chòrdail, leis a’ phlugan co-fhreagarrachd air ais no às aonais.

Dh’fhaodadh tu measgachadh de na dòighean gu h-àrd a dhèanamh. Tòisich le stàladh glan agus dèan deuchainn air na leudachain agad. Nuair a bhios fios agad dè na leudachain a tha ag obair agus dè na leudachain nach eil, faodaidh tu obrachadh leis na leasaichean gus faighinn a-mach dè an ìre sa bheil iad leis an leasachadh aca airson J6. AN UTAIR, nuair a bhios na leudachain agad uile ag obair air làrach glan, bidh fios agad gun urrainn dhut **deuchainn** a dhèanamh air ùrachadh slàn bho J5.4.x gu 6.x.

’S dòcha gum bi thu airson faighinn a-mach a bheil leudachan ag obair gun am plugan co-fhreagarrachd air ais a bhith an gnìomh. Mas e sin a’ chùis, bidh feum agad air cothrom air an stòr-dàta. Dèan planadh air a shon. Dèan cinnteach gu bheil cothrom agad air an stòr-dàta.

Às dèidh dhut stàladh ùr de J6 a dhèanamh, bidh am plugan co-fhreagarrachd air ais à comas. Stàlaich gach leudachan aon aig aon àm. Ma chuireas e an làrach agad à comas, cuir an gnìomh am plugan co-fhreagarrachd air ais tron stòr-dàta.

Gheibhear am Plugan Co-fhreagarrachd air Ais san stòr-dàta sa chlàr #__extensions. ’S e plg_behaviour_compat6 an t-ainm a th’ air. Suidhich an raon Enabled gu 0 gus am plugan a chur à comas. Suidhich gu 1 e gus am plugan a chur an gnìomh. Le bhith a’ cur a’ phlugain co-fhreagarrachd air ais an gnìomh a-rithist, dh’fhaodadh gum faigh thu cothrom a-rithist air backend Joomla (cho fad ’s a tha an leudachan ag obair leis a’ phlugain co-fhreagarrachd air ais).

NO

Faodaidh tu leudachain fa leth a chur à comas san stòr-dàta gus leantainn ort a’ dèanamh deuchainn air na leudachain eile agad agus faicinn an obraich iad gun am plugan co-fhreagarrachd a bhith an gnìomh. Bidh na h-inntrigidhean seo sa chlàr #__extensions. Atharraich an raon Enabled gu 0 gus an leudachan a chur à comas.

Ann an cuid de chùisean, nuair a stàlaicheas tu leudachan ann an J6 nach eil co-chòrdail, leis a’ phlugain co-fhreagarrachd air ais an gnìomh no às aonais, feumaidh tu na h-inntrigidhean san stòr-dàta airson an leudachain sin a lorg (’s dòcha nach bi ann ach beagan dhiubh no gum bi mòran dhiubh ann) agus an cur à comas gus am faigh thu cothrom air a’ backend a-rithist. Bidh na h-inntrigidhean seo sa chlàr #__extensions. Atharraichidh tu an raon Enabled gu 0 gus an leudachan a chur à comas. Nuair a gheibh thu cothrom air backend Joomla a-rithist, faodaidh tu a dhì-stàladh gu ceart bho System -> Manage -> Extensions. An uair sin, faighnich don leasaiche.

### Cassiopeia agus Weblinks

#### Cassiopeia

Fuirichidh Cassiopeia mar theamplaid an frontend airson Joomla 6. Bu chòir do na gnàthachaidhean agad a bhith ceart, ach tha sinn fhathast a’ moladh deuchainn a dhèanamh air làrach leasachaidh gus dèanamh cinnteach.

#### com_weblinks

Bidh an leudachan Weblinks ag obair ann an J6 gun am plugan co-fhreagarrachd air ais a bhith an gnìomh ann an tionndadh 5.4.0+:

- [Weblinks Evolved in the JCM](https://magazine.joomla.org/all-issues/september-2025/joomla-weblinks-evolved-insights-from-gsoc-2025). 
- [Weblinks on the JED](https://extensions.joomla.org/extension/weblinks/).

### Ruith Deuchainn

Mar phàirt den phlanadh agad, thathar a’ moladh gun dèan thu deuchainn air an ùrachadh agad air fo-àrainn no gu h-ionadail gus dearbhadh gu bheil e ag obair gu foirfe. Dèan cinnteach gun cùm thu sùil air ceumannan sam bith a dh’fheumas tu a ghabhail gus an tachair an ùrachadh agad **gu foirfe**.

Aon uair ’s gu bheil thu air an ùrachadh agad fheuchainn air fo-àrainn no localhost, agus gu bheil e ag obair **gu foirfe**, faodaidh tu lethbhreac-glèidhidh den làrach riochdachaidh agad a dhèanamh agus an ùrachadh a chur an gnìomh oirre. Tha stiùireadh ceum air cheum gu h-ìosal.

## Ùrachadh Ceum air Cheum

Feumaidh an làrach a tha thu gu bhith ag ùrachadh na riatanasan theicnigeach uile a choileanadh agus a bhith a’ ruith Joomla 5.4.x gus an tèid ùrachadh a dhèanamh. Mura h-eil an làrach agad fhathast a’ ruith Joomla 5.4.x, ùraich gu 5.4.x mus ùraich thu gu J6.

1. Lean a h-uile stiùireadh anns an earrann Dealbhaidh (gu h-àrd) mus dèan thu an t-ùrachadh.
2. **Dèan lethbhreac-glèidhidh den làrach-lìn agad.**
3. Ùraich leudachain sam bith a dh’fheumas ùrachadh.
4. Cuir à comas no dì-stàlaich leudachain sam bith nach eil co-chòrdail ri J6.
5. Cuir Debug air (Rèiteachadh Cruinneil -> taba an t-Siostaim -> suidheachadh Debug an t-Siostaim gu Tha).
6. **Dèan lethbhreac-glèidhidh den làrach-lìn agad a-rithist.**
7. **Dèan deuchainn air an lethbhreac-glèidhidh agad gus dèanamh cinnteach gun gabh ath-stèidheachadh.** (Seadh, dèan seo. Bidh thu a’ faireachdainn nas fheàrr.)
8. Rach gu Siostam -> Ùrachadh -> Joomla
![Deas-bhòrd an t-siostaim leis an roghainn ùrachadh Joomla air a chomharrachadh](../../../en/images/migration/joomla-5-to-6-steps/07-steps-5-to-6-system-dashboard-joomla.png)

9. Briog air a’ phutan Roghainnean anns a’ Bhàr-inneal Uachdarach air an taobh cheart.
![Duilleag ùrachaidh Joomla leis a’ phutan Roghainnean air a chomharrachadh](../../../en/images/migration/joomla-5-to-6-steps/08-steps-5-to-6-joomla-update.png)

10. Atharraich an Sianal Ùrachaidh gu Joomla Next.
![Roghainnean ùrachaidh Joomla leis an t-sianal ùrachaidh air a chomharrachadh](../../../en/images/migration/joomla-5-to-6-steps/09-steps-5-to-6-joomla-update-options.png)

11. Briog air Sàbhail & Dùin anns a’ Bhàr-inneal Uachdarach.
12. Ma choileanas an frithealaiche agad na sònrachaidhean theicnigeach, chì thu an sgrìn a leanas le ceanglaichean air a’ bhàr-taoibh chlì airson Roghainnean Riatanach, Roghainnean Molta, agus Leudachain.
![Sgrùdadh ro-ùrachaidh leis a’ bhàr-taoibh air a chomharrachadh](../../../en/images/migration/joomla-5-to-6-steps/10-steps-5-to-6-pre-update-check-for-6.png)

13. Tha deagh chothrom ann gum bi na Roghainnean Riatanach agus na Roghainnean Molta agad ceart, oir cha nochd an sgrìn seo mura coilean an àrainneachd agad na riatanasan theicnigeach. Is dòcha nach bi na Leudachain ceart. Faic an earrann ann an Dealbhadh (gu h-àrd) mun sgrùdadh ro-ùrachaidh agus carson is dòcha nach bi comharra-seic uaine ann ged a tha na leudachain uile co-chòrdail. Tha thu air do dheuchainn a dhèanamh mu thràth (nach eil?), agus mar sin tha fios agad mu thràth a bheil iad co-chòrdail no nach eil.
14. Tha am plugan Co-chòrdalachd Air Ais 6 air a chur an comas ann an Joomla 5.4.x. Gus ùrachadh gu J6, feumar am plugan Giùlan - Co-chòrdalachd Air Ais a chur à comas.
15. **Mura lean thu an stiùireadh ann an Dealbhadh (gu h-àrd) mun Ruith Dheuchainneach, stad an-dràsta agus till don earrann Dealbhaidh agus lean an stiùireadh. Is e Dealbhadh am pàirt as cudromaiche den ùrachadh seo.**
16. Nuair a bhios tu cinnteach gu bheil na leudachain agad uile co-chòrdail ri J6 agus gu bheil thu air an t-ùrachadh fheuchainn agus gun robh an toradh foirfe, faodaidh tu briogadh air a’ bhogsa gus gabhail ris na rabhaidhean mu leudachain a dh’fhaodadh a bhith neo-chòrdail agus leantainn air adhart leis an ùrachadh, briog air OK sa bhogsa uinneagail, agus an uair sin briog air a’ phutan Ùraich.
![Sanas airson gabhail ris na Rabhaidhean](../../../en/images/migration/joomla-5-to-6-steps/11-steps-5-to-6-pre-update-warnings.png)

17. An uair sin, iarraidh an làrach agad ort a-rithist dearbhadh gu bheil thu air lethbhreac-glèidhidh a dhèanamh (rud a rinn thu agus a dhearbh thu gun gabh ath-stèidheachadh).
![Duilleag Luchdaich suas agus Ùraich gu Joomla 6](../../../en/images/migration/joomla-5-to-6-steps/12-steps-5-to-6-upload-and-update.png)

18. Nì an làrach agad an t-ùrachadh gu J6.
![Duilleag adhartais an ùrachaidh](../../../en/images/migration/joomla-5-to-6-steps/13-steps-5-to-6-joomla-update-progress.png)

19. Seallaidh ùrachadh soirbheachail dhut sgrìn mar seo:
![Duilleag Inbhe an Ùrachaidh a’ sealltainn soirbheachas](../../../en/images/migration/joomla-5-to-6-steps/14-steps-5-to-6-joomla-update-success.png)

20. Chì thu gu bheil an làrach agad a’ ruith Joomla 6 anns an oisean gu h-àrd air an làimh dheis den sgrìn.
21. Dèan deuchainn air aghaidh na làraich agad.
22. Dèan deuchainn air cùlaibh na làraich agad.
23. Cuir Debug dheth ann an Siostam -> Rèiteachadh Cruinneil -> taba an Fhrithealaiche.
24. Ceartaich an Lorg Glic ùr agad ma tha feum air.
25. Tlachd a ghabhail air deoch mhath agus iongnadh a dhèanamh air cho mìorbhaileach ’s a tha thu.

## Dè ma thèid rudeigin ceàrr?

Ma rinn thu deuchainn air a h-uile càil ro làimh, cha bu chòir dha tachairt. Ach tha e comasach gun do dh’atharraich rudeigin san àrainneachd no gun do dh’atharraich cuid de chòd ann an leudachan eadar àm na deuchainn agad agus an t-ùrachadh agad.

Leis gun do chuir thu Debug an comas mus do thòisich thu, bu chòir dhut a bhith comasach air an leudachan a tha ag adhbharachadh na cùise fhaicinn agus a chur à comas (is dòcha gum feumar seo a dhèanamh bhon stòr-dàta mura h-urrainn dhut tuilleadh faighinn chun chùlaibh gus a chur à comas). Mar sin, bidh an làrach agad ag obair fhad ’s a tha thu a’ faighinn a-mach dè chaidh ceàrr agus ga chàradh.

Anns an t-suidheachadh as miosa, ath-stèidhich an lethbhreac-glèidhidh agad gus am bi ùine agad dèiligeadh ris na thachair ann an àrainneachd deuchainn.

Dh’fhaodadh Ceartachadh an Stòr-dàta cuid de na cùisean agad fhuasgladh. Seòl gu Deas-bhòrd an t-Siostaim agus briog air Stòr-dàta.

![Deas-bhòrd an t-Siostaim leis a’ cheangal Stòr-dàta air a chomharrachadh](../../../en/images/migration/joomla-5-to-6-steps/15-steps-5-to-6-system-dashboard-database.png)

Air duilleag Stòr-dàta a’ Chàraidh, seallaidh e cùisean sam bith le structar an stòr-dàta a dh’fhaodadh a bhith aig an làrach agad. Cuir comharra sa bhogsa iomchaidh agus an uair sin briog air a’ phutan Ùraich Structar anns a’ Bhàr-inneal Uachdarach.

![Duilleag stòr-dàta a’ chàraidh a’ sealltainn aon duilgheadas](../../../en/images/migration/joomla-5-to-6-steps/16-steps-5-to-6-maintenance-database.png)

## Àiteachan eile airson cuideachadh fhaighinn

- [Fòram Joomla: Bòrd Imrich & Ùrachaidh 6.x](https://forum.joomla.org/viewforum.php?f=866&sid=47959551fb677ee3690f8b61eece277b)
- [Coimhearsnachd Joomla air Mattermost](https://joomlacommunity.cloud.mattermost.com/main/channels/town-square)

*Air eadar-theangachadh le openai.com*