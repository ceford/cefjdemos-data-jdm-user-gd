<!--
{
    "source": "https://docs.joomla.org/J4.x:Favicons",
    "title": "Faviconan",
    "description": " ",
    "author": ""
}
-->

## Faviconan Joomla!

Is e faviconan na h-ìomhaighean beaga a nochdas ann an taba a’ bhrabhsair ri taobh
ainm na làraich agad. Faisg air mullach teamplaid index.php tha trì
stiùiridhean gus faviconan a luchdadh a-steach don duilleag:
```php
    // Browsers support SVG favicons
    $this->addHeadLink(HTMLHelper::_('image', 'joomla-favicon.svg', '', [], true, 1), 'icon', 'rel', ['type' => 'image/svg+xml']);
    $this->addHeadLink(HTMLHelper::_('image', 'favicon.ico', '', [], true, 1), 'alternate icon', 'rel', ['type' => 'image/vnd.microsoft.icon']);
    $this->addHeadLink(HTMLHelper::_('image', 'joomla-favicon-pinned.svg', '', [], true, 1), 'mask-icon', 'rel', ['color' => '#000']);
```

Airson teamplaid Cassiopeia, seallaidh Joomla airson na faviconan anns na
h-àiteachan a leanas:

1.  **media/templates/site/cassiopeia/images** - chan eil iad ann, agus mar sin
    seallaidh Joomla san ath àite.
2.  **media/system/images** - tha iad ann, agus mar sin cleachdaidh Joomla iad
    às an sin.

Ma tha thu airson na faviconan agad fhèin a chleachdadh an àite faviconan Joomla,
luchdaich suas iad chun chiad àite:
**media/templates/site/cassiopeia/images**. Faodaidh tu sin a dhèanamh a’ cleachdadh
foirm Teamplaidean: Gnàthaich. Cha toir ùrachadh sam bith air
teamplaid Cassiopeia buaidh orra.

Bithear uaireannan a’ cleachdadh faviconan aig meudan nas motha agus ann an àiteachan
eile seach taba a’ bhrabhsair. Mar eisimpleir, seo glacadh-sgrìn de phàirt de
dhuilleag tòiseachaidh Firefox a’ sealltainn cuid de na h-àiteachan as fheàrr leis an
neach-cleachdaidh:

![eisimpleirean de faviconan bho dhuilleag tòiseachaidh firefox](../../../en/images/templates/favicons/01-favicons-firefox-start-collection.png)

Tha na brabhsairean ùra uile a’ cur taic ri h-ìomhaighean SVG, agus mar sin bu chòir dhut
prìomhachas a thoirt do chruthachadh ìomhaigh SVG.

## Mu SVG

Is e SVG giorrachadh de Scalable Vector Graphics. Tha faidhle SVG a’ gabhail a-steach
teacsa ann an cruth a mhìnicheas suidheachadh agus cumaidhean nan loidhnichean le
dathan loidhne, dathan lìonaidh agus mar sin air adhart. Tha an glacadh-sgrìn a leanas a’ sealltainn
faidhle *joomla-favicon.svg* fosgailte ann an deasaiche teacsa. Tha àireamhan nan loidhnichean air
an cruthachadh leis an deasaiche teacsa. Chan eil iad an làthair san fhaidhle. Tha na loidhnichean
fada a’ riochdachadh lùban agus tha iad air an giorrachadh an seo airson adhbharan taisbeanaidh.

![susbaint teacsa favicon joomla](../../../en/images/templates/favicons/02-favicons-joomla-favicon-svg-text.png)

Gus faidhle SVG a chruthachadh, feumaidh tu aplacaid iomchaidh leithid
Inkscape a chleachdadh. Cha dèan aplacaidean grafaigeachd raster leithid Photoshop no The GIMP
a’ chùis. Nam b’ fheàrr leat ìomhaigh a dhealbhadh ann an aplacaid grafaigeachd raster,
no ma tha suaicheantas grafaigeachd raster agad mu thràth a ghabhas atharrachadh airson ìomhaigh,
faodaidh tu am faidhle PNG a thig às a thoirt a-steach do Inkscape agus an uair sin lorg a dhèanamh
air gus faidhle SVG a chruthachadh. Feumar an ìomhaigh a chaidh a lorg a sguabadh às an dèidh an
lorg a dhèanamh!

Tha cruthachadh favicon SVG fhèin taobh a-muigh raon an artaigil seo.
Tha cruthachadh faidhle àbhaisteach *favicon.ico* a’ tòiseachadh le faidhle
*joomla-favicon.svg* glè shìmplidh—bidh iomadh làrach ga dhèanamh air loidhne
an-asgaidh.

## Mar a Chruthaicheas Tu Faviconan

Ma tha thu airson na faviconan agad fhèin a chruthachadh, ’s e an dòigh as fheàrr air sin a dhèanamh
favicon SVG a chruthachadh agus an uair sin inneal air loidhne a chleachdadh gus na cruthan eile
uile a ghineadh leis mar chur-a-steach. Anns an eisimpleir seo, tha feum air ìomhaigh a fhreagras air
teamplaid pàiste leis an ainm Cassiopeia Green. Feumaidh ìomhaigh a bhith ceàrnagach
agus gun a bhith ro mhionaideach, oir ’s e 16x16 piogsail am meud taisbeanaidh as lugha.
Feumaidh cuid de dh’uidheaman rùintean nas àirde, leithid 32x32 no 180x180, agus tha Google
a’ moladh iomadan de 48x48 piogsail. Ma thòisicheas tu le SVG, cha leig thu leas dragh a ghabhail
mu dheidhinn sin idir—dìreach cruthaich ìomhaigh cha mhòr ceàrnagach
le dealbhadh freagarrach. Anns an eisimpleir seo, bidh an favicon na litrichean
*J4* ann an uaine dhorch.

### Inkscape

Tha Inkscape na aplacaid grafaigeachd vector an-asgaidh, le Stòr Fosgailte agus thar-àrd-ùrlar,
a thathar a’ cleachdadh airson obrachadh le faidhlichean SVG. Bidh e ag obair air Linux, Mac agus
Windows. Tadhail air làrach Inkscape (inkscape.org) gus lethbhreac a luchdadh a-nuas
airson an àrd-ùrlair agad. Tha na dealbhan a leanas a’ sealltainn sgrìn Inkscape
letheach slighe tro na stiùiridhean a leanas.

![inkscape le favicon ga ullachadh](../../../en/images/templates/favicons/03-favicons-inkscape-favicon.png)

### Cruthaich SVG

1.  Tòisich Inkscape agus dèan uinneag de mheud chofhurtail: tagh View /
    Zoom / Zoom Page
2.  Tagh an t-Inneal Teacsa, air a chomharrachadh leis an litir A sa
    Chrann-Inneal chlì
3.  Tagh Arial, Normal, 48 agus px
4.  Slaod gus bogsa a mhìneachadh àite sam bith air an duilleag
5.  Sgrìobh an Teacsa: J4
6.  Tagh View / Zoom Selection
7.  Tagh Path / Object to Path - chan eil atharrachadh follaiseach ann ach
    chan eil na faclan nan teacsa tuilleadh
8.  Tagh File / Document Properties
9.  Tagh Resize to Content
10. Sùm a-mach airson sealladh nas fheàrr - ach dèan cinnteach gu bheil na
    litrichean uile fhathast air an taghadh
11. Suidhich am bogsa àirde chun an aon luach ris a’ bhogsa leud. Taidhp a-steach e!
12. Dùin còmhradh Document Properties
13. View / Zoom Page a-rithist - feumaidh na caractaran a bhith sa mheadhan
14. Edit / Select All
15. Objects / Align and Distribute
16. Gluais an taghadh mar bhuidheann / Relative to Page / Center on horizontal
    axis - bu chòir dhut J4 fhaicinn a’ gluasad gu meadhan puing dìreach
17. Tagh Fill and Stroke air an taobh cheart - tha liosta-tharraing sìos aig a’
    phannal air an làimh dheis, air a chomharrachadh le saighead sìos
18. Anns a’ phannal Fill and Stroke, tagh Fill agus a’ chiad cheàrnag làn
19. Anns a’ phannal RGB cuir a-steach 006400ff san raon RGBA faisg air a’ bhonn
    cheart - an còd airson an stoidhle CSS *darkgreen*
20. File / Save
21. Anns a’ chòmhradh Save, cuir a-steach ainm faidhle iomchaidh, mar eisimpleir
    green-favicon-j4.svg
22. Tagh àite iomchaidh, mar eisimpleir
    *~/Documents/joomla-dev/svgs*
23. Tagh Optimised SVG (*.svg*) bhon liosta-tharraing sìos aig bonn
    na foirm.
24. Tagh *Save*
25. Tagh *OK* airson na Defaults uile san fhoirm Optimised SVG Output
26. Dùin an SVG air a bheil thu ag obair - bidh cothrom ann an
    dealbh a shàbhaladh ann an cruth Inkscape ach chan eil sin dha-rìribh
    riatanach.

### Deasaich an SVG le Deasaiche Teacsa

Tòisich an deasaiche teacsa as fheàrr leat gus atharrachaidhean a dhèanamh
nach robh comasach ann an Inkscape.

1.  Fosgail am faidhle SVG a chruthaich thu às ùr - mothaich gur e
    sònrachadh XML a th’ anns a’ chiad loidhne
2.  Faodaidh tu an dàrna loidhne a sguabadh às - beachd anns a bheil Created with
    Inkscape
3.  Ma tha i an làthair, faodaidh tu an loidhne anns a bheil a sguabadh às oir
    chan eil teacsa ann
4.  Fosgail am faidhle tùsail joomla-favicon.svg - tha e ann an
    *joomla_root/media/system/images*
5.  Dèan lethbhreac den bhloc stoidhle agus cuir a-steach e don SVG agad air an loidhne
    dìreach às dèidh na h-aithris SVG
6.  Dùin am faidhle tùsail *joomla-favicon-svg* gus atharrachaidhean
    tubaisteach a sheachnadh
7.  Ann am bloc stoidhle an fhaidhle SVG agad fhèin, atharraich path {fill: \#000;}
    gu path {fill: \#006400;}, an luach san loidhne
8.  Thoir air falbh *fill="#006400"* on loidhne
9.  Sàbhail
10. Fosgail an dealbh sa bhrobhsair agad. Airson Firefox ’s e sin File / Open
    File...

Bu chòir dhut an dealbh fhaicinn sa bhrobhsair agad. Tha an t-eisimpleir a’ sealltainn
J4 aig 47 piogsail ceàrnagach. ’S e an ath cheum na seòrsaichean eile de dh’ìomhaigheagan
a dh’fheumas tu a chruthachadh, a’ cleachdadh an SVG ùr agad mar phrìomh theamplaid.

### Giullachd Air Loidhne

Rach gu làrach Real Favicon Generator.
Tha làraichean eile rim faighinn ach tha coltas gu bheil an tè seo gu sònraichte coileanta.

1.  Tagh am putan leis an leubail *Select your Favicon image*
2.  Seallaidh an làrach dhut am Prìomh Dhealbh agad. Tha i cuideachd ag ràdh *Your picture
    is not square (688x512). We can fix this by adding transparent
    margins*
3.  Tagh am putan *Continue with this picture* fon Phrìomh Dhealbh.
4.  Tha fo-fhoirmean le cùlaibhean gorma bàn ann airson grunn sheòrsaichean de
    dh’ìomhaigheagan - lìon gach fear dhiubh, a’ dèanamh cinnteach gu bheil an ro-shealladh
    freagarrach dhut.
5.  Tha e nas fheàrr cumail ri roghainnean bunaiteach Favicon Generator Options mura
    h-eil fios nas fheàrr agad. Ach:
6.  Path, tagh an roghainn I cannot ... agus cuir a-steach:
    *media/templates/site/cassiopeia-green/images*
7.  Tagh am putan *Generate your Favicons and HTML Code*
8.  Às dèidh greiseag bheag, nochdaidh foirm ùr; tagh am putan Download your
    package: *Favicon* package
9.  Sàbhail an luchdachadh a-nuas ...
10. Tagh agus dèan lethbhreac den bhloc cheanglaichean gus a shàbhaladh an àiteigin.
11. Dùin an làrach giullachd air loidhne

’S e faidhle *zip* a th’ anns an luchdachadh a-nuas anns a bheil 10 nithean: *favicon.ico*,
*safari-pinned-tab.svg*, sia faidhlichean PNG, *browserconfig.xml* agus
*site.webmanifest*.

### Cur an Gnìomh

Gus an seata àbhaisteach de favicons Joomla a chleachdadh, feumaidh tu na h-ìomhaigheagan
ath-ainmeachadh agus a ghluasad gu *joomla_root/media/templates/site/yourtemplate/images*:

- Feumaidh an dealbh SVG prìomhach agad, *green-favicon-j4.svg*, a bhith air ath-ainmeachadh
  gu *joomla-favicon.svg*
- Feumaidh am faidhle *safari-pinned-tab.svg* a chaidh a luchdachadh a-nuas a bhith air ath-ainmeachadh gu
  *joomla-favicon-pinned.svg*
- Chan fheum am faidhle *favicon.ico* a chaidh a luchdachadh a-nuas ach a bhith air a ghluasad

### Am Bloc Cheanglaichean

Tha na leantainnean a chaidh a chopaigeadh roimhe seo anns a’ bhloc cheanglaichean:

```html
<link rel="apple-touch-icon" sizes="180x180" href="media/templates/site/cassiopeia-green/images/apple-touch-icon.png">
<link rel="icon" type="image/png" sizes="32x32" href="media/templates/site/cassiopeia-green/images/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="media/templates/site/cassiopeia-green/images/favicon-16x16.png">
<link rel="manifest" href="media/templates/site/cassiopeia-green/images/site.webmanifest">
<link rel="mask-icon" href="media/templates/site/cassiopeia-green/images/safari-pinned-tab.svg" color="#5bbad5">
<link rel="shortcut icon" href="media/templates/site/cassiopeia-green/images/favicon.ico">
<meta name="msapplication-TileColor" content="#ffc40d">
<meta name="msapplication-config" content="media/templates/site/cassiopeia-green/images/browserconfig.xml">
<meta name="theme-color" content="#ffffff">
```

Is dòcha nach fheum thu feum a dhèanamh dheth!

*Air eadar-theangachadh le openai.com*