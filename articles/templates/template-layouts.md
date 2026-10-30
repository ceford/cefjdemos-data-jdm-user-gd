<!--
{
    "source": "https://docs.joomla.org/J4.x:Template_Layouts",
    "title": "Cruthan nan Teamplaidean",
    "description": " ",
    "author": ""
}
-->

## Structaran nam Faidhlichean Crutha

Ann an **teamplaid**, bidh gach leudachan a chruthaicheas toradh html a’ cur a’ chòd toraidh ann am faidhle teamplaide taobh a-staigh structar fhaidhlichean an leudachain, gu tric ann am pasgan air a bheil tmpl. Seo eisimpleirean:

- /modules/mod_login/tmpl/default.php
- /modules/mod_login/tmpl/default_logout.php
- /components/com_content/tmpl/article/default.php
- /plugins/content/vote/tmpl/vote.php

Ann an **tar-sgrìobhadh teamplaide**, thèid faidhle leis an aon ainm a chruthachadh taobh a-staigh structar fhaidhlichean na teamplaide, agus thèid sin a chleachdadh an àite an fhaidhle ann an structar fhaidhlichean an leudachain. Eisimpleirean co-fhreagarrach:

- /templates/cassiopeia/html/mod_login/default.php
- /templates/cassiopeia/html/mod_login/default_logout.php
- /templates/cassiopeia/html/com_content/article/default.php
- /templates/cassiopeia/html/plg_content_vote/vote.php

Leigidh seo leat an toradh a ghnàthachadh a rèir do fheumalachdan. Ach, chan eil roghainn agad co-dhùnadh am bu chòir dhut an tar-sgrìobhadh agad a chleachdadh no nach bu chòir. Tha e an-còmhnaidh ga chleachdadh.

Ann an **cruth eile teamplaide**, cruthaichidh tu faidhle le ainm eadar-dhealaichte bhon fhear thùsail ach anns an aon phasgan teamplaide. Chan fhaod caractar fo-loidhne a bhith san ainm ùr. Cruthaichidh tu cuideachd faidhle sam bith a tha a’ co-roinn a’ chiad phàirt de ainm an fhaidhle thùsail. Eisimpleir:

- /templates/cassiopeia/html/mod_login/expires.php
- /templates/cassiopeia/html/mod_login/expires_logout.php

Bidh e comasach an uair sin taghadh am bu chòir an cruth bunaiteach tùsail no an cruth eile a chleachdadh. Thèid an roghainn a dhèanamh ann am foirm deasachaidh a’ mhòidil no a’ cho-phàirt (an taba Adhartach airson mhodalan, agus an taba Roghainnean airson Artaigilean). Thoir fa-near nach eil gach leudachan a’ ceadachadh tar-sgrìobhaidhean no cruthan eile.

**Bi faiceallach:** chan eil uidheamachd aig plugain airson cruthan eile a thaghadh.

## Cruthan Eile nam Modal

Tha cruth eile a chruthachadh airson modal coltach ri tar-sgrìobhadh teamplaide a chruthachadh airson modal. Anns an dà chùis, cruthaichidh tu pasgan air a bheil `templates/.../html/`. Mar eisimpleir, bhiodh am pasgan airson tar-sgrìobhadh teamplaide no cruth eile de `mod_login` airson teamplaid cassiopeia mar `templates/cassiopeia/html/mod_login/`.

Tha dà phrìomh eadar-dhealachadh eadar tar-sgrìobhadh teamplaide agus cruth eile. ’S e ainm an fhaidhle a’ chiad fhear. Airson tar-sgrìobhadh teamplaide, bheireadh tu `default.php` mar ainm air an fhaidhle gus a bhith co-ionann ri ainm an fhaidhle bhunaidh. Airson cruth eile, cleachdaidh tu ainm eadar-dhealaichte. ’S e an aon riaghailt nach bu chòir **fo-loidhnichean sam bith a bhith ann an ainm an fhaidhle**.

’S e an dàrna eadar-dhealachadh cudromach, eu-coltach ri faidhlichean tar-sgrìobhaidh teamplaide a thèid an cleachdadh gu fèin-obrachail gach uair a thèid am modal a thaisbeanadh leis an teamplaid anns a bheil an tar-sgrìobhadh, nach tèid faidhle cruth eile a chleachdadh ach ma thaghas tu e mar pharamadair ann an roghainnean pharamadairean a’ mhòidil.

### Eisimpleir obrach - mod_login

- Rach gu **Siostam **→** Teamplaidean na Làraich **→** Mion-fhiosrachadh agus Faidhlichean Cassiopeia**
- Tagh an taba **Cruthaich Tar-sgrìobhaidhean**.
- Bho liosta nam Modal, tagh an nì **mod_login**.
- Anns an taba Deasaiche, tagh **html **→** mod_login** gus na lethbhreacan ùra de theamplaidean toraidh mod_login agad fhaicinn.
- Ath-ainmich **default.php** gu rudeigin eile gun fho-loidhne, **expires.php** san eisimpleir seo.
- Ath-ainmich **default_logout.php** gu **expires_logout.php**.

Tha dà fhaidhle agad a-nis leis an aon susbaint cheart ris na faidhlichean tùsail. Atharraich susbaint expires_logout.php gus teachdaireachd a chur ris a bheir fios don chleachdaiche dè an uair a thig an seisean gu crìch às dèidh gach luchdadh duilleige.

Air loidhne 16, dìreach fon fheadhainn a th’ ann de na h-aithrisean use, cuir na leanas ris:

    use Joomla\CMS\Factory;

    date_default_timezone_set('Europe/London');
    $config = Factory::getContainer()->get('config');
    $lifetime = $config->get('lifetime', 0);
    $time = time() + $lifetime * 60;
    $endTime = date('H:i:s', $time); // time() returns a time in seconds already

Agus air loidhne 36, dìreach às dèidh na loidhne anns a bheil aithris endif, cuir an còd seo ris:

```html
<p class="text-center">
Your session will expire at <br><?php echo $endTime; ?>
</p>
```

Dùin faidhlichean Cassiopeia. Tagh **Susbaint **→** Modalan na Làraich** agus fosgail am modal Log a-steach. Anns an taba Adhartach, ann an nì Cruth, chì thu gu bheil roghainn agad eadar **-- Bhon Mhòidil -- / Bunaiteach** agus **-- Bho Teamplaid cassiopeia -- / expires**.

![modal log a-steach a’ sealltainn cruthan eile](../../../en/images/templates/template-layouts/01-layouts-module-login.png)

’S e aon dòigh anns am faodadh tu an gleus seo a chleachdadh dà fhoirm Log a-steach a bhith agad, aon le inntrigeadh Poblach agus am fear eile le inntrigeadh Luchd-cleachdaidh Sàr-ìre. Anns an fhear mu dheireadh, tagh an roghainn **expires**, agus chan fhaic ach Luchd-cleachdaidh Sàr-ìre an cuimhneachan mun àm a thig an seisean gu crìch.

Tha e cudromach tuigsinn, ma thèid a shònrachadh ann an sgrìn pharamadairean a’ mhòidil, gun tèid faidhle cruth eile airson modal a chleachdadh airson a’ mhòidil sin ge bith dè an teamplaid a thèid a chleachdadh gus an duilleag far a bheil am modal ri fhaicinn a thaisbeanadh. Mar sin, ’s e uallach an rianaire dèanamh cinnteach gun obraich am faidhle crutha mar a thathar ag iarraidh ann an teamplaidean sam bith far am faodadh am modal seo a bhith ri fhaicinn.

### Eadar-theangachadh

Faodaidh tu ainm an fhaidhle eadar-theangachadh a’ cleachdadh Tar-chuiridhean
Cànain. Feuch an dòigh-obrach a leanas:

- Tagh **Siostam **→** Pannal stiùiridh **→** Tar-chuiridhean Cànain**
- Tagh do chànan agus ionad an Rianaire.
- Tagh am putan **Ùr** agus lìon am foirm. San eisimpleir seo,
  ’s e **TPL_CASSIOPEIA_MOD_LOGIN_LAYOUT_EXPIRES** iuchair a’ chànain agus
  dh’fhaodadh an teacsa a bhith **Log a-steach / Log a-mach le ùine crìochnachaidh**
- Sàbhail agus Dùin agus till dhan fhoirm mhodal Log a-steach.

![foirm tar-chuiridh cànain deasachaidh](../../../en/images/templates/template-layouts/02-layouts-language-override-form.png)

Foirm raoin taghaidh cruth a’ mhodail le **expires**
eadar-theangaichte:

![tagh cruthan eile a’ mhodail](../../../en/images/templates/template-layouts/03-layouts-example-translated.png)

## Cruthan Eile airson Cho-phàirtean

Bidh cruthan eile airson cho-phàirtean ag obair san aon dòigh ri cruthan
mhodailean. Cuiridh tu faidhle sa phasgan cheudna far an cuireadh tu
faidhle tar-chuiridh teamplaide. Mar eisimpleir, gus cruth eile a chruthachadh
airson artaigil airson an teamplaide "cassiopeia", chuireadh tu faidhle sa
phasgan `templates/cassiopeia/html/com_content/article/`. Coltach ri cruthan
mhodailean, chan fhaod an aon ainm a bhith air an fhaidhle ’s a tha air
faidhle bunaiteach, agus chan fhaod fo-loidhnichean a bhith san ainm.
A bharrachd air sin, cha bu chòir faidhle XML leis an aon ainm a bhith sa
phasgan seo. (Bruidhnidh sinn mu fhaidhlichean XML gu h-ìosal fo Chruthan
Eile airson Nithean Clàir-thaice.)

Faodaidh tu luach uile-choitcheann a shuidheachadh airson cruthan
cho-phàirtean ann an uinneag nan Roghainnean den cho-phàirt. Mar eisimpleir,
ann an uinneag Artaigil: Roghainnean, tha paramadair *Tagh cruth* mar a
chithear gu h-ìosal:

![foirm roghainnean artaigilean le liosta de chruthan eile](../../../en/images/templates/template-layouts/04-layouts-articles-options.png)

Coltach ri cruthan mhodailean, tha cruthan nan co-phàirtean air an sealltainn
mar roghainnean paramadair ann an sgrìn deasachaidh fa leth a’ cho-phàirte.
Mar eisimpleir, airson artaigil, tha am paramadair ri fhaicinn ann an taba
Artaigilean: Deasaich Roghainnean mar a chithear gu h-ìosal.

![foirm deasachaidh artaigil a’ sealltainn liosta de chruthan eile](../../../en/images/templates/template-layouts/05-layout-article-edit.png)

Coltach ri paramadairean eile, cleachdaidh an suidheachadh Cleachd
Roghainnean Cruinneil an suidheachadh bhon pharamadair Roghainnean. Bidh an
suidheachadh Bho Chruth Bunaiteach a’ Cho-phàirte a’ cleachdadh cruth
bunaiteach a’ cho-phàirte. Tha cruthan eile a chruthaich thu airson teamplaidean
eadar-dhealaichte air an sealltainn fo cheann gach teamplaid.

Faodar ainmean fhaidhlichean eadar-theangachadh. An loidhne gu h-ìosal:
```ini
    TPL_CASSIOPEIA_COM_CONTENT_ARTICLE_LAYOUT_MYLAYOUT="Title Only No XML"
```

eadar-theangaichidh i faidhle air a bheil "mylayout.php" mar "Tiotal a-mhàin gun XML".

Faodaidh barrachd air aon fhaidhle a bhith agad airson cruth. Feumaidh an
t-ainm a bhith air a’ chiad fhaidhle gun fho-loidhnichean agus feumaidh
fo-loidhnichean a bhith anns na faidhlichean a bharrachd.

Faodar cruthan eile airson cho-phàirtean a chleachdadh le artaigilean,
luchd-conaltraidh no inbhir naidheachdan.

Cha chleachdar cruthan eile airson cho-phàirtean ach nuair a thèid dà
chumha a choileanadh:
(1) tha iad air an sònrachadh ann am paramadairean a’ cho-phàirte; agus
(2) chan eil nì clàr-taice ann airson a’ cho-phàirt shònraichte seo. Mar
eisimpleir, ma tha aon nì clàr-taice no barrachd den t-seòrsa "Artaigil Singilte"
air an stèidheachadh airson artaigil shònraichte, cha chleachdar an cruth eile
airson an artaigil sin. An àite sin, cleachdaidh e an cruth a chaidh a shònrachadh
san nì clàr-taice. Tha seo co-chòrdail ris an dòigh choitcheann sa bheil
paramadairean cho-phàirtean ag obair, far a bheil an nì as sònraichte (sa chùis
seo, nì clàr-taice airson aon artaigil) a’ dol thairis air an fhear nach eil
cho sònraichte (sa chùis seo, paramadairean an artaigil).

## Cruthan Eile airson Roinnean

Bidh cruthan eile airson roinnean ag obair mar chruthan cho-phàirtean. Tha na
riaghailtean airson faidhlichean cruth a shònrachadh co-ionann. ’S e an aon
eadar-dhealachadh gu bheil am pasgan na phasgan roinne, chan e pasgan
a’ cho-phàirte. Mar eisimpleir, chuireadh cruth eile airson roinn luchd-
conaltraidh airson cassiopeia sa phasgan
`templates/cassiopeia/html/com_contact/category`.

Faodaidh tu cruthan roinne a shuidheachadh gu h-uile-choitcheann, ann an
sgrìn nan Roghainnean de gach co-phàirt. Gu h-ìosal tha eisimpleir bhon fhoirm
Luchd-conaltraidh: Roghainnean / Roinn:

![foirm roghainnean co-phàirt luchd-conaltraidh a’ sealltainn chruthan eile](../../../en/images/templates/template-layouts/06-layouts-contacts-options.png)

Nochdaidh cruthan eile airson roinnean nuair a chuireas tu roinn ris no nuair
a dheasaicheas tu tè ann am foirm Co-phàirt: Deasaich Roinn / Roghainnean, mar
a chithear gu h-ìosal.

![foirm roghainnean co-phàirt luchd-conaltraidh a’ sealltainn chruthan eile](../../../en/images/templates/template-layouts/07-layouts-contacts-category-options.png)

Faodar cruthan eile airson roinnean a chleachdadh airson artaigilean, brataichean,
luchd-conaltraidh agus inbhirean naidheachdan.

Coltach ri cruthan cho-phàirtean, cha chleachdar cruth roinne ach ma tha:

1.  e air a thaghadh sna paramadairean uile-choitcheann no roinne.
2.  chan eil nì clàr-taice ann gu sònraichte airson na roinne.

Ma tha nì clàr-taice air a stèidheachadh airson roinn shònraichte, cleachdar an
cruth sin a chaidh a thaghadh sa chlàr-taice an àite cruth eile na roinne.

## Blog agus Liosta Roinnean Artaigilean

Airson artaigilean, tha dà phrìomh chruth-roinne ri fhaighinn: Blog agus
Liosta. Nochdaidh gach fear de na cruthan seo ann an taba Roinn fo
cheann-sgrìobhadh “Bho Cho-phàirt” san fhoirm Roghainnean
Artaigilean. Nochdaidh cruthan eile cuideachd san liosta, a’ leigeil
leat Blog no Liosta, no cruthan teamplaid eile, a thaghadh mar an cruth
roinne bunaiteach an dàrna cuid gu cruinneil no nuair a bhios tu a’
deasachadh roinn artaigil shingilte.

![foirm roghainnean co-phàirt luchd-aithne a’ sealltainn chruthan eile](../../../en/images/templates/template-layouts/08-layouts-articles-options-category.png)

Tha seo a’ ciallachadh, mar le roghainnean cruth eile, gun urrainn dhut
smachd a chumail air co-dhiù a chleachdas ceanglaichean roinne
artaigilean cruth blog no liosta. Tha e cudromach tuigsinn, mar le
paramadairean cruth eile, nach bi an roghainn seo èifeachdach ach nuair
nach eil nì clàr-taice airson na roinne singilte ann.

## Nithean Clàr-taice Eile

Tha aon eadar-dhealachadh cudromach aig Nithean Clàr-taice Eile bho
na càch. Gus cruth nì clàr-taice eile a chruthachadh, feumaidh tu faidhle
XML a thoirt a-steach aig a bheil ainm a tha a’ maidseadh ainm an
fhaidhle chrutha thùsail. Mar eisimpleir, gus nì clàr-taice eile leis an
ainm “myarticle” a chruthachadh airson artaigil san teamplaid
cassiopeia, chruthaicheadh tu dà fhaidhle sa phasgan
`templates/cassiopeia/html/com_content/article` leis na h-ainmean
`myarticle.php` agus `myarticle.xml`. Nam biodh tu airson barrachd
fhaidhlichean crutha a thoirt a-steach, chuireadh tu na faidhlichean
seo ris le fo-loidhnichean anns na h-ainmean fhaidhlichean.

Cleachdaidh am faidhle XML an aon fhòrmat ri prìomh fhaidhlichean XML
Nithean Clàr-taice. Leigidh seo leat chan ann a-mhàin cruth gnàthaichte a
chruthachadh airson an nì clàr-taice seo, ach cuideachd paramadairean
gnàthaichte a chruthachadh. Mar eisimpleir, dh’fhaodadh tu cuid de
paramadairean fhalach no paramadairean ùra a chur ris.

Nochdaidh Nithean Clàr-taice Eile nuair a thaghas tu Seòrsa Nì Clàr-taice
mar a chithear gu h-ìosal.

![liosta taghaidh nì clàr-taice](../../../en/images/templates/template-layouts/09-layouts-menu-blog-menu-creation.png)

Tha Nithean Clàr-taice Eile gan cleachdadh agus ag obair san aon dòigh
ri nithean clàr-taice àbhaisteach. Leis gu bheil iad stèidhichte mar
-thà air cruthan gnàthaichte, chan eil tar-sgrìobhainnean teamplaid a’
buntainn ri nithean clàr-taice eile.

Mar a chaidh ainmeachadh gu h-àrd, tha prìomhachas aig cruthan nithean
clàr-taice air cruthan eile cho-phàirtean no roinnean.

Tha eadar-theangachadh nithean clàr-taice eile air a dhèanamh leis na
tagaichean a leanas anns na faidhlichean XML. ’S e fòrmat nan tagaichean
`"TPL_"<template name>_<component>_<view>_<menu item name>_<tag type>`. Mar
eisimpleir, eadar-theangaichidh na loidhnichean gu h-ìosal an tiotal, an
roghainn agus an tuairisgeul airson nì clàr-taice eile leis an ainm
“catmenuitem”.
```
    TPL_CASSIOPEIA_COM_CONTENT_CATEGORY_VIEW_CATMENUITEM_TITLE="cassiopeia Custom Category Layout"
    TPL_CASSIOPEIA_COM_CONTENT_CATEGORY_VIEW_CATMENUITEM_OPTION="cassiopeia Custom"
    TPL_CASSIOPEIA_COM_CONTENT_CATEGORY_VIEW_CATMENUITEM_DESC="Description for cassiopeia custom category layout."
```

Feumar na sreangan seo a chur ri
`administrator/language/overrides/en-GB.override.ini`, ach faodaidh tu
an fhoirm Tar-sgrìobhaidhean Cànain a tha air a mhìneachadh gu h-àrd a
chleachdadh.

Thòisicheadh catmenuitem.xml le:

```xml
<?xml version="1.0" encoding="utf-8"?>
<metadata>
   <layout title="TPL_CASSIOPEIA_COM_CONTENT_CATEGORY_VIEW_CATMENUITEM_TITLE" option="TPL_CASSIOPEIA_COM_CONTENT_CATEGORY_VIEW_CATMENUITEM_OPTION">
      <help
         key = "JHELP_MENUS_MENU_ITEM_ARTICLE_SINGLE_ARTICLE"
      />
      <message>
         <![CDATA[TPL_CASSIOPEIA_COM_CONTENT_CATEGORY_VIEW_CATMENUITEM_DESC]]>
      </message>
   </layout>
```

## Smachd air an Teamplaid airson Nithean Clàr-taice Eile

Mar a chaidh a dheasbad gu h-àrd, tha faidhle XML ann a’ dèanamh cruth
eile na nì clàr-taice. Tha fòrmat an fhaidhle XML co-ionann ri fòrmat
nam prìomh fhaidhlichean XML airson nithean clàr-taice. Leis an fhaidhle
XML seo, faodaidh tu na paramadairean a tha thu airson a chur a-steach
airson an nì clàr-taice seo a chur ris. Faodaidh iad a bhith co-ionann ri
paramadairean aon de na prìomh nithean clàr-taice, no faodaidh tu
paramadairean bunaiteach fhàgail air falbh no feadhainn ùra a chur ris.
Thoir fa-near, ma chuireas tu paramadairean ùra ris, gum faodar an
cleachdadh san fhaidhle chrutha ach nach tèid an cleachdadh anns na
faidhlichean prìomh-mhodail no seallaidh.

Tha e comasach cuideachd roghainnean pharamadairean airson
paramadairean bunaiteach a sgrìobhadh thairis. ’S e aon eisimpleir de
seo smachd a chumail air dè na teamplaidean leis am faodar cruth nì
clàr-taice eile a thaisbeanadh. Ann an cuid de chùisean, ’s dòcha gum
bi thu airson leigeil le nì clàr-taice gnàthaichte a bhith air a
thaisbeanadh le teamplaid sam bith air an làrach. Ann an cùisean eile,
’s dòcha gum bi thu airson cruth an nì clàr-taice sin a chuingealachadh
gu teamplaid shònraichte. Anns an t-suidheachadh seo, cha leig thu ach
am paramadair a leanas a chur ri faidhle XML an nì clàr-taice:

```xml
<fields>
  <field
    name="template_style_id"
    type="templatestyle"
    label="COM_MENUS_ITEM_FIELD_TEMPLATE_LABEL"
    description="COM_MENUS_ITEM_FIELD_TEMPLATE_DESC"
    filter="int"
    template="cassiopeia"
    class="inputbox">
  </field>
 </fields>
 ```

Sgrìobhaidh seo thairis air a’ pharamadair bunaiteach
`template_style_id`. Le bhith a’ suidheachadh na teamplaide gu
“cassiopeia” sa chùis seo, cha leigear leis an neach-cleachdaidh ach
stoidhlichean teamplaid airson na teamplaide “cassiopeia” a thaghadh.

## Barrachd Fiosrachaidh

-  Teamplaid
  Bunaitean
-  Pasganan is
  Faidhlichean Teamplaid Cassiopeia
-  Gnàthachadh
  Teamplaid Cassiopeia
-  Tar-sgrìobhaidhean
  Teamplaid
-  Cruthan
  Teamplaid
-  Teamplaid Cassiopeia Shimplichte - Sgrùdadh
  Cùise -
  teamplaid shìmplidh stèidhichte air Cassiopeia

*Air eadar-theangachadh le openai.com*