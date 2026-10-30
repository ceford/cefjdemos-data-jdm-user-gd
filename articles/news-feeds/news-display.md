<!--
{
    "source": "https://docs.joomla.org/jdocmanual?manual=user&heading=news&filename=news-display.md",
    "title": "Taisbeanadh Naidheachdan",
    "description": " ",
    "author": ""
}
-->

## Am Modal Taisbeanaidh Inbhir

Tha modal bunaiteach *Taisbeanadh Inbhir* ri fhaighinn gus naidheachdan bho
làraichean eile a thaisbeanadh. Tha an dealbh-sgrìn a leanas a’ sealltainn an
fhoirm airson dàta a chur a-steach le URL inbhir naidheachdan Sanasan Joomla.
Thoir fa-near gu bheil Cunntas nam Faclan suidhichte aig 100. Air neo, faodaidh
fad sanas a bhith ro mhòr airson modal bàr-taoibh.

![Dàta air a chur a-steach airson modal taisbeanaidh inbhir](../../../gd/images/news-feeds/news-display/01-news-joomla-news-form.png)

Faodaidh an toradh a bhith grànda ach faodar a leasachadh le cuid de stoidhlichean
gnàthaichte ann an user.css:

![Dàta air a chur a-steach airson modal taisbeanaidh inbhir](../../../gd/images/news-feeds/news-display/02-news-joomla-news-display.png)

## Duilleagan Taisbeanaidh Inbhir

Mar roghainn eile seach naidheachdan a thaisbeanadh ann am modal, faodaidh tu
nì clàr-taice a chruthachadh gus inbhir naidheachdan a thaisbeanadh ann an
duilleag-lìn. Bho chlàr-taice an Rianaire:

* Tagh **Co-phàirtean / Inbhirean Naidheachdan / Inbhirean**. Dh’fhaodadh tu
  Roinn-seòrsa a chruthachadh an toiseach airson naidheachdan.
* Tagh am putan **Ùr** sa *Bhàr-inneal*.
* Lìon a-steach am foirm **Inbhirean Naidheachdan: Deasaich**:
    - ’S e an **Ceangal** an ceangal RSS a chaidh a chopaigeadh bho thùs iomallach.
    - Tha an **Tuairisgeul** roghainneil.
    - Tha nithean anns an taba **Roghainnean** gus smachd a chumail air an *Taisbeanadh* inbhir.
* **Sàbhail & Dùin**

![Dàta air a chur a-steach airson co-phàirt inbhir naidheachdan](../../../gd/images/news-feeds/news-display/03-news-feed-data-entry.png)

Cruthaich nì clàr-taice a’ tòiseachadh bho chlàr-taice an Rianaire:

* Tagh **Clàran-taice / Prìomh Chlàr-taice** no clàr-taice sam bith eile airson an nì seo.
* Tagh **Ùr** à Bhàr-inneal *Clàran-taice: Nithean*.
* Ann an **Seòrsa Nì Clàr-taice**, cleachd am putan **Tagh** gus
*Inbhirean Naidheachdan / Aon Inbhir Naidheachdan* a lorg agus a thaghadh.
* Lìon a-steach a’ chòrr den fhoirm mar a tha iomchaidh.
* **Sàbhail & Dùin**

![Dàta air a chur a-steach airson nì clàr-taice inbhir naidheachdan](../../../gd/images/news-feeds/news-display/04-news-feed-menu-form.png)

Dèan deuchainn air: rach gu clàr-taice na Làraich agus tagh nì clàr-taice an Inbhir.

![Taisbeanadh inbhir naidheachdan](../../../en/images/news-feeds/news-display/05-news-feed-display.png)

Tha gach nì san inbhir na `<li>` taobh a-staigh taga `<ul>`, agus mar sin
nochdaidh e le peilear mar bhun-roghainn. Chan eil seo cho follaiseach ma tha
na nithean fada. Faodaidh tu na stoidhlichean agad fhèin a chur an sàs ann an
*user.css*. Cuiridh na leanas gach nì ann am bogsa air leth:

```
ul.com-newsfeeds-newsfeed__items {
  list-style-type: none;
  padding-left: 0;
}

ul.com-newsfeeds-newsfeed__items > li {
  padding: 1rem;
  margin-bottom: 1rem;
  border: 2px solid navy;
}
```

A nochdas mar seo:

![Taisbeanadh gnàthaichte inbhir naidheachdan](../../../gd/images/news-feeds/news-display/06-news-feed-custom-display.png)

## Liostaich Inbhirean Naidheachdan ann an Roinn-seòrsa

Tha duilleag *Inbhirean Naidheachdan RSS Joomla!* a’ liostadh ochd inbhirean
naidheachdan fa leth. Dh’fhaodadh tu inbhir a chruthachadh airson cuid dhiubh
no airson nan uile agus an sònrachadh do Roinn-seòrsa, canaidh sinn
*Naidheachdan Joomla*. An uair sin faodaidh tu nì clàr-taice a chruthachadh le
*Seòrsa Nì Clàr-taice* suidhichte gu *Liostaich Inbhirean Naidheachdan ann an
Roinn-seòrsa* agus an Roinn-seòrsa suidhichte gu *Naidheachdan Joomla*.

![Foirm clàr-taice inbhir naidheachdan a rèir roinn-seòrsa](../../../gd/images/news-feeds/news-display/07-news-feed-menu-category-form.png)

Feuch e gus an toradh fhaicinn!
*Air eadar-theangachadh le openai.com*