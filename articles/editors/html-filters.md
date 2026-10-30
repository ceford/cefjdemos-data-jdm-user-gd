<!--
{
    "source": "https://docs.joomla.org/Entering_raw_HTML_in_editors",
    "title": "Criathragan HTML",
    "description": " ",
    "author": ""
}
-->

## Taga HTML Textarea

Ann an HTML, canar textarea ri raon ion-chuir ioma-loidhne. Tha teacsa sam bith
eadar na tagaichean fosglaidh agus dùnaidh air a thaisbeanadh mar theacsa anns
faod markup HTML a bhith.
Eisimpleir:
```
<textarea><p class="poem">The quick brown fox<br>
jumps over the lazy dog.</textarea>
```

Bidh luchd-deasachaidh, leithid TinyMCE no Code Mirror, a’ cleachdadh JavaScript
gus textarea a chòmhdachadh le taisbeanadh eadar-dhealaichte, a’ leigeil le
dàta WYSIWYG a chur a-steach agus/no soilleireachadh co-chàradh. Bidh am putan
Toggle fon raon deasachaidh ag atharrachadh eadar sealladh an textarea agus
sealladh WYSIWYG.

Bithear a’ cleachdadh seallaidhean deasachaidh airson susbaint Artaigilean agus
cuid de Mhodalan. Ach, feumaidh tu a bhith mothachail nach eil a h-uile taga
HTML agus feart (leithid class="xyz") ceadaichte do gach neach-cleachdaidh.
Dh’fhaodadh cuid no iad uile a dhol à sealladh nuair a shàbhaileas tu susbaint
textarea no raoin deasachaidh.

Tha seo air adhbhrachadh le uidheaman criathraidh, an dara cuid ann an
Rèiteachadh Coitcheann Joomla! no ann an rèiteachadh an deasaiche. Faodar
criathrag deasaiche a sheachnadh le bhith a’ taghadh *No Editor* ann an
roghainnean a’ *Phròifil Chleachdaiche* agad. Chan urrainn dhut na criathragan
coitcheann a sheachnadh, ach faodaidh tu an atharrachadh gus freagairt air
adhbharan na làraich agad.

## Taghadh Deasaiche a’ Chleachdaiche

Faodaidh tu aon de na deasaichean a tha rim faighinn a thaghadh, a’ gabhail a-steach None, bhon
Phròifil Chleachdaiche agad, a gheibhear tron chlàr Cunntas Cleachdaiche /
Deasaich Pròifil aig bàrr deas sgrìn an Rianaire. Tha taba Roghainnean
Bunaiteach anns an fhoirm Deasaich: Pròifil, le raon airson Deasaiche a
thaghadh. Mar as trice tha e air a shuidheachadh gu *- Use Default -*, a tha
mar as trice TinyMCE. Faodaidh tu *Editor None* a thaghadh. Seachnaidh sin
criathradh sam bith de thagaichean HTML agus fheartan nach eil ceadaichte le
roghainnean rèiteachaidh TinyMCE.

**Rabhadh:** ma thaghas tu *Editor - None* gus susbaint anns a bheil tagaichean HTML
a chruthachadh nach eil ceadaichte le criathrag deasaiche, agus an uairsin
tilgeas tu air ais chun deasaiche bhunaiteach, bu chòir dhut a bhith faiceallach
gun a bhith a’ deasachadh agus a’ sàbhaladh an t-susbaint sin a-rithist, air neo
caillidh tu tagaichean agus feartan sam bith a chaidh a chriathradh. Tha e furasta
seo a dhèanamh le mearachd agus chan eil rabhadh ann.

## Rèiteachadh Coitcheann: Criathragan Teacsa

Bhon Deas-bhòrd Dachaigh, tagh Rèiteachadh Coitcheann agus an uair sin an taba
Criathragan Teacsa. Tha na roghainnean bunaiteach air *No HTML* a thaghadh
airson na buidhnean cleachdaiche Guest, Public agus Registered. Dh’fhaodadh
cothrom a bhith aig gin de na buidhnean seo raon textarea a lìonadh, mar eisimpleir
ann am foirm conaltraidh a tha ag iarraidh fiosrachadh a bharrachd mu dhuilgheadas,
agus mar sin tha toirt air falbh nan tagaichean HTML uile gu fèin-obrachail
mar as trice iomchaidh. Tha buidhnean eile, ach a-mhàin Super Users, air an
cuingealachadh leis an Default Forbidden List. Chan eil criathradh sam bith aig
Super Users.

![rèiteachadh coitcheann nan criathragan teacsa](../../../gd/images/editors/html-filters/01-global-configuration-filters-tab.png)

Tha na notaichean a’ mìneachadh dè tha anns an liosta thoirmeasgach bhunaiteach
agus mar a chleachdas tu na liostaichean eile.

## Rèiteachadh TinyMCE airson Criathragan Teacsa

Tha deasaichean air an cur an gnìomh mar Phluganan ann an Joomla. Chan eil
roghainnean criathraidh teacsa aig deasaiche CodeMirror. Gus deasaiche TinyMCE
a ghnàthachadh, lorg agus tagh e ann an liosta nam plugan. Mu letheach slighe
sìos an liosta fhada de roghainnean, chì thu raon leis an leubail *Use Joomla
Text Filter*, a tha **Off** gu bunaiteach. ’S iad na trì raointean a leanas
* **Prohibited Elements** liosta de thagaichean a thèid an-còmhnaidh a thoirt air falbh. Tha draghan tèarainteachd aig an liosta bhunaiteach *script,applet,iframe* uile.
* **Valid Elements** cleachd an liosta seo gus tagaichean dligheach a chuingealachadh gu fo-sheata de na tagaichean HTML cumanta uile. Eisimpleir: `a[href|target=_blank],strong/b,div[align],br`
* **Extended Valid Elements** cleachd an liosta seo gus eileamaid a chur ris an t-seata riaghailtean bhunaiteach a th’ ann mar-thà, no gus eileamaid atharrachadh san t-seata riaghailtean bhunaiteach. Eisimpleir:
`img[class|src|border=0|alt|title|hspace|vspace|width|height|align|onmouseover|onmouseout|name]`

Faic Sgrìobhainnean TinyMCE airson barrachd mìneachaidh.

Gus criathragan teacsa TinyMCE a sheachnadh agus criathragan teacsa Joomla a
chleachdadh, suidhich *Use Joomla Text Filter* gu **On**. Thèid na trì
raointean a bharrachd a chaidh a mhìneachadh gu h-àrd à sealladh, oir chan eil
iad gan cleachdadh.

*Air eadar-theangachadh le openai.com*