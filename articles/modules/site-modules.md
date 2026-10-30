<!--
{
    "source": "https://docs.joomla.org/J4.x:Site_Modules",
    "title": "Modalan na L\u00e0raich",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Tha modalan nan leudachain aotrom agus shùbailte a thathar a’ cleachdadh gus pìosan
fiosrachaidh a thaisbeanadh ann an **bogsaichean** air an cur air dòigh timcheall
air co-phàirt air duilleag. ’S e am modal logaidh a-steach eisimpleir ainmeil.
Tha modalan air an sònrachadh a rèir gach nì clàr-taice, agus mar sin faodaidh tu
co-dhùnadh am bi modal ri fhaicinn no falaichte a rèir na duilleige a tha an
cleachdaiche a’ coimhead oirre an-dràsta.

Tha cuid de mhodalan ceangailte ri co-phàirtean. Mar eisimpleir, tha am modal
**Naidheachdan as ùire** ceangailte ris a’ cho-phàirt susbaint gus ceanglaichean
ris na h-artaigilean as ùire a thaisbeanadh. Chan fheum modalan a bhith ceangailte
ri co-phàirtean. Chan fheum iad eadhon a bhith ceangailte ri dad agus faodaidh
iad a bhith dìreach nan HTML statach no nan teacsa.

Faodaidh iomadh eisimpleir den aon mhodal a bhith ann. Mar eisimpleir, faodaidh tu
aon eisimpleir den mhodal Dealbh Air Thuaiream a chleachdadh airson cuid de
dhuilleagan agus eisimpleir eile airson duilleagan eile, gach fear a’ cleachdadh
pasgan dhealbhan eadar-dhealaichte gus dealbhan a thaghadh às.

## Suidheachaidhean nam Modal

Tha modalan air an sònrachadh do shuidheachadh air duilleag a tha air a mhìneachadh
leis an teamplaid a thathar a’ cleachdadh. Tha an dealbh a leanas a’ sealltainn
cruth sgeamach na teamplaide Cassiopeia:

![Diagram de shuidheachaidhean na teamplaide Cassiopeia](../../../en/images/modules/site-modules/01-cassiopeia-template-positions.png)

Agus tha an liosta a leanas a’ sealltainn nan suidheachaidhean modal a tha rim
faighinn a rèir an ainm:

```xml
    <positions>
        <position>topbar</position>
        <position>below-top</position>
        <position>menu</position>
        <position>search</position>
        <position>banner</position>
        <position>top-a</position>
        <position>top-b</position>
        <position>main-top</position>
        <position>main-bottom</position>
        <position>breadcrumbs</position>
        <position>sidebar-left</position>
        <position>sidebar-right</position>
        <position>bottom-a</position>
        <position>bottom-b</position>
        <position>footer</position>
        <position>debug</position>
    </positions>
```

## Cuir Modal Bunaiteach ris

Is iad modalan bunaiteach na modalan a thig le stàladh ùr de Joomla. Tha
mìltean de mhodalan a bharrachd rim faighinn bho sholaraichean treas-phàrtaidh.
Can gun bu toil leat dealbh air thuaiream a shealltainn gus an làrach agad a dhèanamh
nas inntinniche do luchd-tadhail. Bhon chlàr Rianadair, tagh
**Susbaint → Modalan na Làraich** gus liosta nam modal làraich a tha gan
cleachdadh mar-thà fhaicinn:

![Liosta nam Modal Làraich](../../../gd/images/modules/site-modules/02-cassiopeia-modules-list.png)

Tagh am putan Ùr gus liosta nam modal làraich a tha rim faighinn airson an
stàladh fhaicinn:

![Modalan Làraich rim faighinn](../../../gd/images/modules/site-modules/03-cassiopeia-modules-available.png)

Sgrolaich sìos agus tagh am modal Dealbh Air Thuaiream. Fosglaidh sin am foirm
deasachaidh **Modalan: Dealbh Air Thuaiream** deiseil dhut a lìonadh.

![Modal de dhealbh air thuaiream](../../../gd/images/modules/site-modules/04-cassiopeia-module-random-image.png)

- **Tiotal** ’S e raon èigneachail a tha seo.
- **Seòrsa Dhealbhan** ’S e jpg an roghainn bhunaiteach.
- **Pasgan Dhealbhan** Cuir a-steach slighe gu pasgan anns a bheil dealbhan den
  t-seòrsa a thagh thu dha-rìribh.
- **Ceangal** URL gus ath-stiùireadh thuige ma thèid an dealbh a thaghadh.
- **Leud** Bheir seo air a h-uile dealbh a bhith air a thaisbeanadh leis an leud
  seo ann am piogsail.
- **Àirde** Fàg falamh e gus co-mheas taobh an deilbh a chumail.
- **Suidheachadh** Tagh suidheachadh modal gus am modal nochdadh dha-rìribh air
  duilleag. Anns an dealbh, chaidh sidebar-right a thaghadh.
- **Sàbhail & Dùin** No cleachd am putan Cobhair anns a’ Chrann-inneal gus faighinn
  a-mach dè nì na raointean eile.

## Òrdugh nam Modal

An dèidh sàbhaladh, ’s dòcha gum feum thu òrdugh nam modal san t-suidheachadh
a thagh thu atharrachadh. Dèan na leanas:

- anns an liosta Mhodalan, tagh an ìomhaigheag Òrdugh nan Colbhan ann an ceann a’ chlàir
  mhodal; ’s e triantan co-cheangailte suas/sìos a th’ ann. Cuiridh sin an clàr
  ann an òrdugh agus seallaidh e samhlaidhean glacaidh nan nithean, ellipsis
  inghearach. Tagh a-rithist e gus òrdugh an t-seòrsachaidh atharrachadh! Bidh
  samhla seòrsachaidh a’ cholbh ag atharrachadh: triantan suas gus òrdugh
  àbhaisteach an t-seòrsachaidh a chomharrachadh, agus triantan sìos gus òrdugh
  cùil an t-seòrsachaidh a chomharrachadh.
- Glac agus slaod ellipsis an Dealbh Air Thuaiream gus a ghluasad suas no sìos.
  Leig às e nuair a bhios e san t-suidheachadh as fheàrr leat.

## Seall an Làrach

![Sealladh na làraich leis a’ mhodal de dhealbh air thuaiream](../../../gd/images/modules/site-modules/05-cassiopeia-module-random-image-site.png)

Thoir sùil air coltas na Làraich. Anns a’ chùis seo, ’s dòcha gur e deagh bheachd a
bhiodh ann an dealbh a chur sa mheadhan. Faodar sin a dhèanamh mar a leanas:

- Till don fhoirm deasachaidh agus tagh an taba Adhartach.
- Ann an raon Clas a’ Mhodail, cuir a-steach text-center agus Sàbhail.
- Seall an toradh le bhith ag ath-luchdachadh duilleag na Làraich.

A bheil sin deiseil?

## Liosta nam Prìomh Mhodalan

- **Artaigilean - Tasglannaichte** Seallaidh am modal seo liosta de na
  mìosan mìosachain anns a bheil Artaigilean Tasglannaichte. Às dèidh dhut
  inbhe Artaigil atharrachadh gu Tasglannaichte, thèid an liosta seo a
  chruthachadh gu fèin-obrachail.
- **Artaigilean - Roinnean** Seallaidh am modal seo liosta de roinnean
  bho aon phrìomh-roinn.
- **Artaigilean - Roinn** Seallaidh am modal seo liosta de dh’artaigilean
  bho aon roinn no barrachd.
- **Artaigilean - As Ùire** Seallaidh am modal seo liosta de na
  h-Artaigilean as ùire a chaidh fhoillseachadh agus a tha làithreach.
- **Artaigilean - As Leughta** Seallaidh am modal seo liosta de na
  h-Artaigilean foillsichte aig a bheil an àireamh as motha de
  sheallaidhean dhuilleagan.
- **Artaigilean - Naidheachdan Goirid** Seallaidh am Modal Naidheachdan
  Goirid àireamh shònraichte de dh’artaigilean bho roinn shònraichte.
- **Artaigilean - Co-cheangailte** Seallaidh am modal seo Artaigilean eile
  a tha co-cheangailte ris an fhear a thathar a’ coimhead. Tha na
  ceanglaichean seo air an stèidheachadh leis na Prìomh-fhaclan. Thèid
  prìomh-fhacal uile an Artaigil làithich a lorg an aghaidh nan uile...
- **Brataichean** Seallaidh am Modal Brataichean na Brataichean gnìomhach
  bhon Cho-phàirt.
- **Breadcrumbs** Seallaidh am modal seo na Breadcrumbs.
- **Gnàthaichte** Leigidh am modal seo leat am Modal agad fhèin a chruthachadh
  a’ cleachdadh deasaiche WYSIWYG.
- **Taisbeanadh Inbhir** Leigidh am modal seo le inbhir siondacaichte a
  thaisbeanadh.
- **Bun-coise** Seallaidh am modal seo fiosrachadh dlighe-sgrìobhaidh
  Joomla!.
- **Atharrachadh Cànain** Seallaidh am modal seo inneal-atharrachaidh
  cànain air an làrach-lìn agad airson nan cànanan susbaint a tha rim
  faighinn.
- **An Luchd-cleachdaidh as Ùire** Seallaidh am modal seo an luchd-cleachdaidh
  as ùire a chaidh a chlàradh.
- **Logadh a-steach** Seallaidh am modal seo foirm logaidh a-steach le
  ainm-cleachdaidh agus facal-faire. Seallaidh e cuideachd ceangal gus
  facal-faire a chaidh a dhìochuimhneachadh fhaighinn air ais. Ma tha
  clàradh luchd-cleachdaidh air a chomasachadh (ann an Users → Manage →
  Options),...
- **Clàr-taice** Seallaidh am modal seo clàr-taice air an Aghaidh-lìn.
- **Ìomhaigh Air Thuaiream** Seallaidh am modal seo ìomhaigh air thuaiream
  bhon phasgan a thagh thu.
- **Lorg Glic** Seo modal-lorgaidh airson siostam an Lorg Glic.
- **Staitistig** Seallaidh am Modal Staitistig fiosrachadh mun stàladh
  frithealaiche agad còmhla ri staitistig mu luchd-cleachdaidh na làraich
  agus an àireamh de dh’Artaigilean san stòr-dàta agad.
- **Inbhirean Siondacaidh** Modal Siondacaidh Glic a chruthaicheas
  Inbhir Siondacaichte airson na duilleige far a bheil am Modal air a
  thaisbeanadh.
- **Tagaichean - As Motha-chòrdte** Seallaidh am modal seo tagaichean a
  thathar a’ cleachdadh air an làrach ann an liosta no ann an cruth
  neòil. Faodar tagaichean òrdachadh a rèir tiotail no a rèir àireamh nan
  nithean tagaichte, agus an cuingealachadh ri ùine shònraichte.
- **Tagaichean - Coltach** Seallaidh am Modal Tagaichean Coltach ceanglaichean
  gu nithean eile aig a bheil tagaichean coltach. Faodar cho faisg ’s a
  tha an coimeas a shònrachadh.
- **Cò tha Air Loidhne** Seallaidh am Modal Cò tha Air Loidhne an àireamh
  de Luchd-cleachdaidh Neo-ainmichte (Aoighean) agus Luchd-cleachdaidh
  Clàraichte (luchd-cleachdaidh a tha air logadh a-steach) a tha a’ faighinn
  cothrom air an làrach-lìn an-dràsta.
- **Còmhdach** Seallaidh am modal seo uinneag iframe gu àite ainmichte.

*Air eadar-theangachadh le openai.com*