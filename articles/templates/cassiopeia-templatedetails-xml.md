<!--
{
    "source": "https://docs.joomla.org/J4.x:Cassiopeia_templateDetails.xml",
    "title": "templateDetails.xml Cassiopeia",
    "description": " ",
    "author": ""
}
-->

## Àite agus Adhbhar

Chì thu eisimpleir de fhaidhle `templateDetails.xml` air a liostadh ann an
**Siostam → Teamplaidean Làraich → Mion-fhiosrachadh agus Faidhlichean Cassiopeia**. Faodaidh tu
a dheasachadh an sin cuideachd ma tha adhbhar math agad airson sin a dhèanamh. Air neo, fàg
mar a tha e! Tha faidhle mar seo aig gach teamplaid agus tha teamplaid pàiste
an toiseach air a dhèanamh suas de structar fhaidhlichean anns nach eil ach am faidhle seo.

Tha am faidhle `templateDetails.xml` a’ gabhail a-steach an dàta a tha a dhìth air Joomla! gus
an teamplaid a stiùireadh agus a thaisbeanadh. Tha seo a’ gabhail a-steach meata-dàta a
thathar a’ cleachdadh gus fiosrachadh mun teamplaid a thoirt seachad, àiteachan nam
pasganan agus nam faidhlichean, suidheachaidhean nam mòdan teamplaid agus na roghainnean
rèiteachaidh a thaghas an cleachdaiche. Bidh susbaint an fhaidhle templateDetails.xml
eadar-dhealaichte bho theamplaid gu teamplaid.

## templateDetails.xml Cassiopeia

Tha structar air a dheagh mhìneachadh aig faidhlichean ann an cruth xml. Feumaidh faidhle xml
an co-chòrdadh cheart a bhith aige no chan obraich e!

### Cruth XML

Feumaidh a’ chiad loidhne de gach `templateDetails.xml` tòiseachadh le mìneachadh
doctype XML.

Tha an ath loidhne ag innse do Joomla! gu bheil an dàta san fhaidhle seo airson leudachan
teamplaide làraich. Tha dàta an teamplaide gu lèir taobh a-staigh nan tagaichean fosglaidh
agus dùnaidh.

```xml
<extension type="template" client="site">
...
</extension>
```

### Meata-dàta

Mar as trice bidh a’ chiad earrann de dhàta an teamplaide a’ mìneachadh fiosrachadh mun
teamplaid, mar eisimpleir: ainmean, cinn-latha, fiosrachadh conaltraidh, dlighe-sgrìobhaidh,
àireamh an tionndaidh agus tuairisgeul.

```xml
<extension version="3.1" type="template" client="site">
    <name>cassiopeia</name>
    <version>1.0</version>
    <creationDate>2017-02</creationDate>
    <author>Joomla! Project</author>
    <authorEmail>admin@joomla.org</authorEmail>
    <copyright>(C) 2017 Open Source Matters, Inc.</copyright>
    <description>TPL_CASSIOPEIA_XML_DESCRIPTION</description>
    <inheritable>1</inheritable>
```

Thoir an aire gu bheil an luach inheritable aig 1 aig teamplaid a dh’fhaodas teamplaidean
pàiste a bhith aige. Tha an luach seo aig 0 aig teamplaidean pàiste. Tha an dàta seo
air a chleachdadh anns an liosta Teamplaidean: Teamplaidean (Làrach), mar a chithear gu h-ìosal.

![liosta theamplaidean làraich](../../../en/images/templates/cassiopeia-templatedetails-xml/01-templates-list.png)

Tha iuchair cànain anns an tuairisgeul agus chan eil an t-sreang teacsa fhìor ann.
Thèid an iuchair a chur an àite an teacsa a gheibhear bho fhaidhle cànain aig àm ruith.
Tha na faidhlichean cànain air am mìneachadh ann an earrann a’ chànain de `templateDetails.xml`.

![foirm deasachaidh stoidhle nan teamplaidean](../../../en/images/templates/cassiopeia-templatedetails-xml/02-templates-edit-style.png)

### Pasganan agus Faidhlichean

Tha pasganan agus faidhlichean teamplaide Cassiopeia air an stòradh ann an dà àite
fa leth. Tha na faidhlichean php agus na faidhlichean co-cheangailte riutha air an stòradh
sa phasgan site/templates. Tha na faidhlichean mheadhanan (css, images, js agus scss)
air an stòradh sa phasgan site/media. Tha na h-àiteachan sin air am mìneachadh san
fhaidhle xml mar a leanas:

```xml
    <files>
        <filename>component.php</filename>
        <filename>error.php</filename>
        <filename>index.php</filename>
        <filename>joomla.asset.json</filename>
        <filename>offline.php</filename>
        <filename>templateDetails.xml</filename>
        <folder>html</folder>
    </files>
    <media destination="templates/site/cassiopeia" folder="media">
        <folder>js</folder>
        <folder>css</folder>
        <folder>scss</folder>
        <folder>images</folder>
    </media>
```

Seo am pàtran a chithear anns na teamplaidean Joomla 4 agus 5 ùr-nodha uile. Chithear an
structar anns an fhoirm Teamplaidean: Gnàthaich (Cassiopeia):

![duilleag gnàthachaidh teamplaidean Cassiopeia](../../../en/images/templates/cassiopeia-templatedetails-xml/03-templates-customise-cassiopeia.png)

### Suidheachaidhean nam Mòdan

Tha na suidheachaidhean mòdan a tha rim faighinn air am mìneachadh mar a leanas:

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

Cruthaichidh gach taga suidheachadh mòdan a bhios ri fhaighinn bhon liosta shuidheachaidhean
ann an fhoirm deasachaidh mòdan. Tha cruth sìmplidh na liosta shuidheachaidhean a’ ciallachadh
gun gabh a ghnàthachadh gu furasta. Mar eisimpleir, gus suidheachadh mòdan ùr a chur ris
an liosta **ann an teamplaid pàiste**, dìreach cuir taga ùr am broinn an taga
le ainm àraid a’ cleachdadh litrichean beaga a-mhàin gun bheàrnan. Cuimhnich nach eil seo
ach a’ cur an t-suidheachaidh ris na foirmean deasachaidh mòdan agus gu bheil feum air
barrachd leasachaidh ann am faidhlichean teamplaide eile gus an suidheachadh ùr a
thaisbeanadh air an aghaidh.

Tha suidheachaidhean teamplaide gu leòr aig Cassiopeia! Ma shaoileas tu gu bheil feum agad
air fear a bharrachd, tha coltas ann gu bheil thu ceàrr. Cuimhnich gun gabh àireamh sam bith
de mhòdan a shònrachadh do aon suidheachadh agus an cur ann an òrdugh air duilleag liosta
nam Mòdan. Suidheachaidhean a tha rim faighinn:

![diagram de shuidheachaidhean teamplaide Cassiopeia](../../../en/images/templates/cassiopeia-templatedetails-xml/04-cassiopeia-template-positions.png)

Chì thu suidheachaidhean nam mòdan ann an teamplaid sam bith cuideachd: bho
**Siostam → Teamplaidean Làraich**, tagh am putan Roghainnean sa Bhàr-inneal.
Anns an fhoirm Roghainnean, suidhich an raon Seall Suidheachaidhean Mòdan gu Comasach.
Sàbhail agus Dùin. Rach dhan làrach agad agus cuir ?tp=1 ri deireadh URL sam bith (no
&tp=1 ma tha ? ann san URL mu thràth). Seallaidh Joomla na suidheachaidhean teamplaide
a tha rim faighinn uile, fiù ’s an fheadhainn nach deach a chleachdadh:

![suidheachaidhean teamplaide Cassiopeia](../../../en/images/templates/cassiopeia-templatedetails-xml/05-templates-template-positions-by-tp.png)

### Cànanan

Leigidh faidhlichean cànain le teacsa stèidhichte san teamplaid a bhith air eadar-theangachadh.
Tha am faidhle tpl_cassiopeia.ini a’ gabhail a-steach eadar-theangachaidhean bho iuchraichean
gu teacsa airson an teacsa a chì an Cleachdaiche. Tha am faidhle tpl_cassiopeia.sys.ini a’
gabhail a-steach eadar-theangachaidhean bho iuchraichean gu teacsa airson an teacsa a chì
an Rianaire.

```xml
    <languages folder="language">
        <language tag="en-GB">en-GB/tpl_cassiopeia.ini</language>
        <language tag="en-GB">en-GB/tpl_cassiopeia.sys.ini</language>
    </languages>
```

Tha na faidhlichean cànain airson na Beurla bunaichte GB air an stòradh ann an
site/language/en-GB/. Bhiodh cànanan eile air an stòradh san aon dòigh ann am faidhlichean
leis a’ chòd cànain ISO iomchaidh, mar eisimpleir fr-FR airson Fraingis san Fhraing no
de-DE airson Gearmailtis sa Ghearmailt (a dh’fhaodadh a bhith eadar-dhealaichte bho
Ghearmailtis na h-Eilbheis agus Ghearmailtis na h-Ostaire).

### Roghainnean

Faodaidh teamplaid roghainnean taisbeanaidh a thabhann a ghabhas taghadh leis an
Rianaire anns an fhoirm Teamplaid: Deasaich an Stoidhle. Mar eisimpleir, tha
taba Adhartach teamplaid Cassiopeia a’ leigeil le Rianaire am Brannd atharrachadh,
Suaicheantas a chur ris, Sgeama Chruthan-clò a thaghadh, agus barrachd.

![foirm deasachaidh stoidhle teamplaide taba adhartach](../../../en/images/templates/cassiopeia-templatedetails-xml/06-templates-edit-style-advanced.png)

Tha roghainnean na teamplaide air am mìneachadh taobh a-staigh structair a chruthaicheas raointean
taobh a-staigh sheataichean raoin. Nochdaidh gach seata raoin mar taba anns an fhoirm
deasachaidh. Seo an structair a chruthaicheas an taba Adhartach a chithear gu h-àrd.

```xml
    <config>
        <fields name="params">
            <fieldset name="advanced">
                <field
                    name="brand"
                    type="radio"
                    label="TPL_CASSIOPEIA_BRAND_LABEL"
                    default="1"
                    layout="joomla.form.field.radio.switcher"
                    filter="boolean"
                    >
                    <option value="0">JNO</option>
                    <option value="1">JYES</option>
                </field>
                ...
            </fieldset>
        </fields>
    </config>
```

Tha roghainnean fa leth air am mìneachadh leis an taga `<field>`. Feumaidh gach `<fieldset>`,
agus gach paramadair `<field>` taobh a-staigh `<fieldset>`, ainm àraidh a tha air a mhìneachadh
le feart **name**. Tha an t-ainm seo a’ mìneachadh a’ pharamadair fhèin agus
ga chleachdadh gus roghainnean a chur gu na faidhlichean aghaidh.
Tha feart **label** agus feart **description** aig gach paramadair cuideachd.
Nochdaidh teacsa na leubail leis a’ pharamadair ann an sgrìn nan roghainnean gus
comharrachadh carson a thathar a’ cleachdadh an roghainn, agus faodar fiosrachadh nas mionaidiche
a chur san tuairisgeul.

Faodaidh raon paramadair a bhith cha mhòr na sheòrsa sam bith de chur-a-steach foirm le
roghainnean co-fhreagarrach. Tha seo air a thaghadh leis an fheart **type**. Tha roghainnean riatanach sam bith,
leithid putanan rèidio no roghainnean taghaidh, air am mìneachadh ann an tagaichean
`<option>`. Faodar ainmean chlasaichean CSS a mhìneachadh leis an fheart **class**, agus
faodar luach bunaiteach a mhìneachadh leis an fheart **default**.

Gu h-ìosal tha mìneachaidhean nan roghainnean ann an teamplaid bunaiteach Cassiopeia. San
eisimpleir seo, tha na Leubailean, na Tuairisgeulan agus na Roghainnean uile a’ cleachdadh
mìneachaidhean shreangan cànain bho na faidhlichean Cànain a chaidh a mhìneachadh san earrann
roimhe, a bharrachd air cuid bho chridhe Joomla!, gus an gabh an
eadar-theangachadh gu cànanan eadar-dhealaichte mar a bhios riatanach.

```xml
    <config>
        <fields name="params">
            <fieldset name="advanced">
                <field
                    name="brand"
                    type="radio"
                    label="TPL_CASSIOPEIA_BRAND_LABEL"
                    default="1"
                    layout="joomla.form.field.radio.switcher"
                    filter="boolean"
                    >
                    <option value="0">JNO</option>
                    <option value="1">JYES</option>
                </field>

                <field
                    name="logoFile"
                    type="media"
                    default=""
                    label="TPL_CASSIOPEIA_LOGO_LABEL"
                    showon="brand:1"
                />

                <field
                    name="siteTitle"
                    type="text"
                    default=""
                    label="TPL_CASSIOPEIA_TITLE"
                    filter="string"
                    showon="brand:1"
                />

                <field
                    name="siteDescription"
                    type="text"
                    default=""
                    label="TPL_CASSIOPEIA_TAGLINE_LABEL"
                    description="TPL_CASSIOPEIA_TAGLINE_DESC"
                    filter="string"
                    showon="brand:1"
                />

                <field
                    name="useFontScheme"
                    type="groupedlist"
                    label="TPL_CASSIOPEIA_FONT_LABEL"
                    default="0"
                    >
                    <option value="0">JNONE</option>
                    <group label="TPL_CASSIOPEIA_FONT_GROUP_LOCAL">
                        <option value="media/templates/site/cassiopeia/css/global/fonts-local_roboto.css">Roboto (local)</option>
                    </group>
                    <group label="TPL_CASSIOPEIA_FONT_GROUP_WEB">
                        <option value="https://fonts.googleapis.com/css2?family=Fira+Sans:wght@100;300;400;700&amp;display=swap">Fira Sans (web)</option>
                        <option value="https://fonts.googleapis.com/css2?family=Noto+Sans:wght@100;300;400;700&amp;family=Roboto:wght@100;300;400;700&amp;display=swap">Roboto + Noto Sans (web)</option>
                    </group>
                </field>

                <field
                    name="noteFontScheme"
                    type="note"
                    description="TPL_CASSIOPEIA_FONT_NOTE_TEXT"
                    class="alert alert-warning"
                />

                <field
                    name="colorName"
                    type="filelist"
                    label="TPL_CASSIOPEIA_COLOR_NAME_LABEL"
                    default="colors_standard"
                    fileFilter="^custom.+[^min]\.css$"
                    exclude="^colors.+"
                    stripext="true"
                    hide_none="true"
                    hide_default="true"
                    directory="media/templates/site/cassiopeia/css/global/"
                    validate="options"
                    >
                    <option value="colors_standard">TPL_CASSIOPEIA_COLOR_NAME_STANDARD</option>
                    <option value="colors_alternative">TPL_CASSIOPEIA_COLOR_NAME_ALTERNATIVE</option>
                </field>

                <field
                    name="fluidContainer"
                    type="radio"
                    layout="joomla.form.field.radio.switcher"
                    default="0"
                    label="TPL_CASSIOPEIA_FLUID_LABEL"
                    >
                    <option value="0">TPL_CASSIOPEIA_STATIC</option>
                    <option value="1">TPL_CASSIOPEIA_FLUID</option>
                </field>

                <field
                    name="stickyHeader"
                    type="radio"
                    label="TPL_CASSIOPEIA_STICKY_LABEL"
                    layout="joomla.form.field.radio.switcher"
                    default="0"
                    filter="integer"
                    >
                    <option value="0">JNO</option>
                    <option value="1">JYES</option>
                </field>

                <field
                    name="backTop"
                    type="radio"
                    label="TPL_CASSIOPEIA_BACKTOTOP_LABEL"
                    layout="joomla.form.field.radio.switcher"
                    default="0"
                    filter="integer"
                    >
                    <option value="0">JNO</option>
                    <option value="1">JYES</option>
                </field>
            </fieldset>
        </fields>
    </config>
```

San eisimpleir seo, tha an taga `<fieldset name="advanced">` a’ cuairteachadh nam paramadairean uile,
agus tha e a’ cleachdadh an fheart **name** gus an taba *Adhartach* a chruthachadh san eadar-aghaidh.
Chan eil feum ach air taga `<fieldset>` eile le feart **name** eadar-dhealaichte
gus taba eile a chruthachadh san eadar-aghaidh. Le seo san amharc, tha e
gu math furasta na h-uimhir de thabaichean is pharamadairean a bharrachd a chruthachadh ’s a
tha riatanach ann an teamplaid.

’S e aon chleachdadh a dh’fhaodadh a bhith aig paramadairean a bharrachd ann an tar-chuiridhean no
cruthan airson teamplaidean pàrant no pàiste.

## Geàrr-chunntas

Seo am faidhle templateDetails.xml a tha Cassiopeia a’ cleachdadh:

```xml
<?xml version="1.0" encoding="utf-8"?>
<extension type="template" client="site">
    <name>cassiopeia</name>
    <version>1.0</version>
    <creationDate>2017-02</creationDate>
    <author>Joomla! Project</author>
    <authorEmail>admin@joomla.org</authorEmail>
    <copyright>(C) 2017 Open Source Matters, Inc.</copyright>
    <description>TPL_CASSIOPEIA_XML_DESCRIPTION</description>
    <inheritable>1</inheritable>
    <files>
        <filename>component.php</filename>
        <filename>error.php</filename>
        <filename>index.php</filename>
        <filename>joomla.asset.json</filename>
        <filename>offline.php</filename>
        <filename>templateDetails.xml</filename>
        <folder>html</folder>
    </files>
    <media destination="templates/site/cassiopeia" folder="media">
        <folder>js</folder>
        <folder>css</folder>
        <folder>scss</folder>
        <folder>images</folder>
    </media>
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
    <languages folder="language">
        <language tag="en-GB">en-GB/tpl_cassiopeia.ini</language>
        <language tag="en-GB">en-GB/tpl_cassiopeia.sys.ini</language>
    </languages>
    <config>
        <fields name="params">
            <fieldset name="advanced">
                <field
                    name="brand"
                    type="radio"
                    label="TPL_CASSIOPEIA_BRAND_LABEL"
                    default="1"
                    layout="joomla.form.field.radio.switcher"
                    filter="boolean"
                    >
                    <option value="0">JNO</option>
                    <option value="1">JYES</option>
                </field>

                <field
                    name="logoFile"
                    type="media"
                    default=""
                    label="TPL_CASSIOPEIA_LOGO_LABEL"
                    showon="brand:1"
                />

                <field
                    name="siteTitle"
                    type="text"
                    default=""
                    label="TPL_CASSIOPEIA_TITLE"
                    filter="string"
                    showon="brand:1"
                />

                <field
                    name="siteDescription"
                    type="text"
                    default=""
                    label="TPL_CASSIOPEIA_TAGLINE_LABEL"
                    description="TPL_CASSIOPEIA_TAGLINE_DESC"
                    filter="string"
                    showon="brand:1"
                />

                <field
                    name="useFontScheme"
                    type="groupedlist"
                    label="TPL_CASSIOPEIA_FONT_LABEL"
                    default="0"
                    >
                    <option value="0">JNONE</option>
                    <group label="TPL_CASSIOPEIA_FONT_GROUP_LOCAL">
                        <option value="media/templates/site/cassiopeia/css/global/fonts-local_roboto.css">Roboto (local)</option>
                    </group>
                    <group label="TPL_CASSIOPEIA_FONT_GROUP_WEB">
                        <option value="https://fonts.googleapis.com/css2?family=Fira+Sans:wght@100;300;400;700&amp;display=swap">Fira Sans (web)</option>
                        <option value="https://fonts.googleapis.com/css2?family=Noto+Sans:wght@100;300;400;700&amp;family=Roboto:wght@100;300;400;700&amp;display=swap">Roboto + Noto Sans (web)</option>
                    </group>
                </field>

                <field
                    name="noteFontScheme"
                    type="note"
                    description="TPL_CASSIOPEIA_FONT_NOTE_TEXT"
                    class="alert alert-warning"
                />

                <field
                    name="colorName"
                    type="filelist"
                    label="TPL_CASSIOPEIA_COLOR_NAME_LABEL"
                    default="colors_standard"
                    fileFilter="^custom.+[^min]\.css$"
                    exclude="^colors.+"
                    stripext="true"
                    hide_none="true"
                    hide_default="true"
                    directory="media/templates/site/cassiopeia/css/global/"
                    validate="options"
                    >
                    <option value="colors_standard">TPL_CASSIOPEIA_COLOR_NAME_STANDARD</option>
                    <option value="colors_alternative">TPL_CASSIOPEIA_COLOR_NAME_ALTERNATIVE</option>
                </field>

                <field
                    name="fluidContainer"
                    type="radio"
                    layout="joomla.form.field.radio.switcher"
                    default="0"
                    label="TPL_CASSIOPEIA_FLUID_LABEL"
                    >
                    <option value="0">TPL_CASSIOPEIA_STATIC</option>
                    <option value="1">TPL_CASSIOPEIA_FLUID</option>
                </field>

                <field
                    name="stickyHeader"
                    type="radio"
                    label="TPL_CASSIOPEIA_STICKY_LABEL"
                    layout="joomla.form.field.radio.switcher"
                    default="0"
                    filter="integer"
                    >
                    <option value="0">JNO</option>
                    <option value="1">JYES</option>
                </field>

                <field
                    name="backTop"
                    type="radio"
                    label="TPL_CASSIOPEIA_BACKTOTOP_LABEL"
                    layout="joomla.form.field.radio.switcher"
                    default="0"
                    filter="integer"
                    >
                    <option value="0">JNO</option>
                    <option value="1">JYES</option>
                </field>
            </fieldset>
        </fields>
    </config>
</extension>
```

*Air eadar-theangachadh le openai.com*