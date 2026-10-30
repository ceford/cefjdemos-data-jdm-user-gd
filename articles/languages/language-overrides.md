<!--
{
    "source": "https://docs.joomla.org/J4.x:Language_Overrides",
    "title": "Searrachaidhean C\u00e0nain",
    "description": " ",
    "author": ""
}
-->

## Àiteachan nam Faidhlichean Cànain

Tha a’ mhòr-chuid de fhaidhlichean cànain Joomla! ann am pasganan cànain, fear
ann am freumh na làraich agus fear eile ann am pasgan an rianaire. Tha
fo-phasgan fhèin aig gach cànan stèidhichte air còdan cànain inbhe RFC3066.
Bidh gach leudachan a’ stòradh a chuid eadar-theangachaidhean le ainm a tha
a’ tighinn à ainm an leudachain. Seo eisimpleirean:

    siteroot/language/en-GB/com_content.ini
    siteroot/administrator/language/en-GB/com_content.ini
    siteroot/administrator/language/en-GB/com_content.sys.ini

Tha loidhnichean anns na faidhlichean anns a bheil iuchair agus a
h-eadar-theangachadh:

    COM_CONTENT="Articles"
    COM_CONTENT_ADD_NEW_MENU_ITEM="New Menu Item"
    COM_CONTENT_ARTICLE_CONTENT="Content"
    COM_CONTENT_ARTICLES_TABLE_CAPTION="Table of Articles"
    COM_CONTENT_ARTICLES_TITLE="Articles"

Bidh còd PHP Joomla a’ cleachdadh na h-iuchrach. Thèid teacsa an
eadar-theangachaidh a chur na h-àite aig àm ruith. Tha eadar-theangachaidhean
anns an fhaidhle .ini a bhios an leudachan a’ cleachdadh. Tha
eadar-theangachaidhean anns na faidhlichean sys.ini a bhios Joomla a’
cleachdadh gus an leudachan a stiùireadh. Dh’fhaodadh ceudan de loidhnichean
a bhith ann am faidhle cànain.

Thathar a’ moladh do leudachain treas-phàrtaidh na faidhlichean cànain aca a
stòradh ann am pasganan cànain taobh a-staigh an leudachain. An sin, bidh iad
sàbhailte bho bhith air an sguabadh às ma cho-dhùnas rianaire cànan a
dhì-stàladh. Eisimpleir:

    siteroot/components/com_countrybase/language/en-GB/com_countrybase.ini
    siteroot/administrator/components/com_countrybase/language/en-GB/com_countrybase.ini
    siteroot/administrator/components/com_countrybase/language/en-GB/com_countrybase.sys.ini

**Na deasaich faidhle cànain bunaiteach Joomla! no faidhle cànain treas-phàrtaidh
a-chaoidh! Thèid atharrachadh sam bith a nì thu a chall aig an ath-ùrachadh.
Ma tha thu airson briathrachas nì cànain sam bith atharrachadh, cleachd an
co-phàirt oifigeil Searrachaidhean Cànain.**

Is e na tha anns na searrachaidhean cànain na h-ath-chuiridhean agad airson
eadar-theangachaidhean iuchraichean cànain bunaiteach no leudachain. ’S e
eadar-theangachaidhean fa leth a tha annta, aon no dhà, chan e faidhle slàn!
Tha na searrachaidhean cànain airson cànan sònraichte uile air an stòradh ann
an aon fhaidhle:

    siteroot/language/overrides/en-GB.override.ini
    siteroot/language/overrides/fr-FR.override.ini
    siteroot/language/overrides/de-DE.override.ini

    siteroot/administrator/language/overrides/en-GB.override.ini
    siteroot/administrator/language/overrides/fr-FR.override.ini
    siteroot/administrator/language/overrides/de-DE.override.ini

### Òrdugh Luchdaidh nan Cànan

Aig gach luchdadh duilleige, thèid eadar-theangachaidhean cànan en-GB a
luchdadh an toiseach. Nì seo cinnteach nach fhaic luchd-cleachdaidh na
làraich iuchraichean sam bith. Ma tha cànan eile ga chleachdadh, thèid
eadar-theangachaidhean a’ chànain sin a luchdadh an ath rud, a’ cur
eadar-theangachaidhean en-GB nan àite. Tha cànanan eile buailteach a bhith
air dheireadh air en-GB ann a bhith a’ cruthachadh eadar-theangachaidhean,
mar sin is dòcha gum faic luchd-cleachdaidh faclan no abairtean ann am
Beurla bho àm gu àm am measg an cànain fhèin.

Mu dheireadh, thèid eadar-theangachaidhean a luchdadh bhon fhaidhle
searrachdan cànain. Leigidh seo leis an làraich faclan no abairtean eile a
chleachdadh a fhreagras air suidheachaidhean ionadail.

## Searrachaidhean Cànain

Uaireannan, is dòcha gum bi thu airson aon nì cànain eadar-theangaichte
a chur an àite rudeigin a tha nas freagarraiche do shuidheachaidhean
ionadail. ’S e cùis chumanta a tha seo nuair a chruthaicheas tu
searrachadh teamplaide no cruth agus nuair a tha thu airson susbaint a
chur ris a chleachdas iuchair cànain ùr. Tha an eisimpleir a leanas a’
sealltainn cùis far an deach teacsa a chur ri cruth fàgail a’ mhodail
logaidh a-steach, mar a chaidh a mhìneachadh san artaigil mu Chruthan
Teamplaide. Tha an còd seo aig a’ chruth eile:

```html
<p class="text-center">
Your session will expire at <br><?php echo $endTime; ?>
</p>
```

Airson làrach ioma-chànanach a chleachdas Beurla, Fraingis agus Gearmailtis,
feumaidh an còd atharrachadh:

```html
<p class="text-center">
<?php echo Text::_('TPL_CASSIOPEIA_MOD_LOGIN_SESSION_EXPIRES_AT')?><br><?php echo $endTime; ?>
</p>
```

Nota: ma lean thu an oideachadh mu Chruthan Teamplaide, is dòcha gu bheil
iuchair TPL_CASSIOPEIA_MOD_LOGIN_LAYOUT_EXPIRES agad mu thràth a tha ag
eadar-theangachadh mar Expires. Ach tha sin air a chleachdadh ann an
siteroot/administrator/language/overrides.

Faodar an iuchair ùr eadar-theangachadh a-nis do gach cànan. Thèid na
h-eadar-theangachaidhean a shàbhaladh ann an siteroot/language/overrides.

- Tagh **System **→** Manage panel **→** Language Overrides**
- Tagh do chànan agus àite na Làraich.
- Tagh am putan **New** agus lìon am foirm. San eisimpleir seo, ’s e
  **TPL_CASSIOPEIA_MOD_LOGIN_SESSION_EXPIRES_AT** iuchair a’ chànain agus
  dh’fhaodadh an teacsa a bhith **Your session will expire at**
- Sàbhail agus Dùin am foirm.
- Dèan ath-aithris air a’ phròiseas eadar-theangachaidh airson gach cànan.

![foirm deasachaidh searrachadh chànanan](../../../gd/images/languages/language-overrides/01-language-overrides-edit.png)

Mu dheireadh, dèan cinnteach gun deach an t-eadar-theangachadh a chur an
gnìomh.

![Toradh an t-searrachaidh ann am foirm logaidh a-steach na làraich](../../../en/images/languages/language-overrides/02-language-overrides-custom-logout.png)

*Air eadar-theangachadh le openai.com*

