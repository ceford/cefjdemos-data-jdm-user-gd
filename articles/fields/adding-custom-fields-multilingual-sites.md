<!--
{
    "source": "https://docs.joomla.org/J3.x:Adding_custom_fields",
    "title": "L\u00e0raichean Ioma-ch\u00e0nanach",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Ma tha làrach ioma-chànanach agad, faodaidh tu bileagan agus tuairisgeulan
raointean agus buidhnean raointean a thaisbeanadh ann an cànan an neach-chleachdaidh. Gus seo a dhèanamh:

1.  Mìnich Tiotal agus Tuairisgeul do bhuidheann raoin mar chonstantaichean cànain.
2.  Mìnich Bileag agus Tuairisgeul do raoin mar chonstantaichean cànain.
3.  Stèidhich na constantaichean cànain sin mar ath-sgrìobhadh airson gach cànan agad.

San eisimpleir a leanas, cruthaichear buidheann raoin agus raon Contact airson
roghainnean pearsanta neach-fiosrachaidh. ’S e Favourites ainm na buidhne raoin agus
’s e Car ainm an raoin san eisimpleir. Gu soilleir, faodar barrachd raointean a chur ris
airson rudan eile as fheàrr leotha, leithid biadh no filmichean.

Gus an eisimpleir seo a leantainn, thathar a’ gabhail ris gu bheil thu air làrach
ioma-chànanach a stèidheachadh mar a tha air a mhìneachadh san oideachadh [Làraichean Ioma-chànanach](jdocmanual?article=user/languages/setup-a-multilingual-site).

## Constantaichean Cànain

’S e luchd-àiteachaidh a th’ ann an constantaichean cànain a thèid luachan cànain a chur nan
àite nuair a tha duilleag ga renderadh. Tha na constantaichean agus na luachan aca air an stòradh ann am
faidhlichean cànain leithid JPATH_SITE/languages/en-GB/com_contact.ini agus
JPATH_SITE/administrator/languages/en-GB/com_contact.ini, airson na làraich agus an
deas-bhòrd fa leth. A rèir gnàthachaidh, bidh a’ mhòr-chuid de chonstantaichean cànain a’ tòiseachadh
le ainm an leudachain ann an litrichean mòra, mar eisimpleir COM_CONTACT_...

’S e ath-sgrìobhadh cànain ionadan a tha air a mhìneachadh leis an neach-chleachdaidh airson
constantaichean agus luachan cànain a tha ann mu thràth, no constantaichean agus luachan gu tur ùra,
mar a tha san eisimpleir seo. Tha iad uile air an stòradh ann am faidhlichean singilte, fear airson
duilleagan na Làraich agus fear eile airson duilleagan an Rianaire:
```
SITE_ROOT/language/overrides/en-GB.override.ini
SITE_ROOT/administrator/language/overrides/en-GB.override.ini
```

Tha e cudromach constantaichean cànain ùra a tha air an sònrachadh leis an neach-chleachdaidh a dhèanamh gun samhail gus nach
sgrìobh iad thairis air constantaichean a tha ann mu thràth. Mar eisimpleir:

COM_CONTACT_CUSTOM_FIELDGROUP_FAVOURITES="Favourites"
COM_CONTACT_CUSTOM_FIELDGROUP_FAVOURITES_DESCRIPTION="Favourite car, film, etc."
COM_CONTACT_CUSTOM_FIELD_FAVOURITE_CAR="Favourite Car"
COM_CONTACT_CUSTOM_FIELD_FAVOURITE_CAR_DESCRIPTION="Sometimes used as a security question"

Ma tha dad ceàrr air co-chòrdadh faidhle cànain, cha tèid a luchdadh agus faodaidh na constantaichean uile a tha ann nochdadh
air na duilleagan toraidh. Agus thoir an aire gu bheil faidhle air a sheòrsachadh ann an òrdugh na h-aibideil.

## A’ Mìneachadh nan Ath-sgrìobhadh

Tha e cudromach ath-sgrìobhadh Beurla (GB) a chruthachadh. Bidh Joomla a’ luchdadh nam faidhlichean eadar-theangachaidh en-GB
an toiseach agus an uair sin a’ sgrìobhadh thairis air na luachan leis an fhaidhle cànain a chaidh a thaghadh.
Nì seo cinnteach nach bu chòir do luchd-cleachdaidh teacsa constant fhaicinn a-riamh. Ma tha luach eadar-theangaichte a dhìth,
nochdaidh Beurla san toradh. Tha seo a’ coimhead neònach ach tha e nas fheàrr na constant caran fada fhaicinn,
a bhios mar as trice a’ cur dragh air cruth nan duilleagan.

Bho chlàr-taice an Rianaire:

* Tagh **Siostam / Pannal stiùiridh / Ath-sgrìobhadh Cànain**
* Tagh **Beurla (An Rìoghachd Aonaichte) - Làrach** bhon liosta *Tagh Cànan & Cliant*
* Tagh am putan **Ùr** bhon Bhàr-inneal.
* Anns an raon **Constant Cànain**, cuir a-steach *COM_CONTACT_CUSTOM_FIELDGROUP_FAVOURITES*
* Anns an raon **Teacsa**, cuir a-steach an luach *Favourites*
* Cuir comharra sa bhogsa **Airson an Dà Àite**. Cruthaichidh seo
  ath-sgrìobhadh airson duilleagan na Làraich agus an Rianaire.
* Tagh **Sàbhail & Ùr** bhon liosta tuiteam-sìos *Sàbhail * Dùin*.
* Dèan seo a-rithist airson gach constant riatanach eile.
* Tagh **Dùin** an dèidh an inntrig mu dheireadh a bhith air a shàbhaladh.
* Dèan seo a-rithist airson gach cànan a chaidh a stàladh.

Tha an dealbh-sgrìn a leanas a’ sealltainn eisimpleir de chruthachadh ath-sgrìobhaidh airson
constant cànain Gearmailteach.

![Cruthachadh ath-sgrìobhaidh ann an Gearmailtis](../../../en/images/fields/adding-custom-fields-multilingual-sites/01-fields-overrides-creation-de.png)

## A’ Mìneachadh Buidheann nan Raointean

Bho chlàr-taice an Rianaire:

* Tagh nì a’ chlàir **Com-pàirtean / Contacts / Buidhnean Raointean**.
* Tagh am putan **Ùr** bhon Bhàr-inneal.
* Anns an raon Tiotal, cuir a-steach an constant COM_CONTACT_CUSTOM_FIELDGROUP_FAVOURITES
* Anns an raon Tuairisgeul, cuir a-steach an constant COM_CONTACT_CUSTOM_FIELDGROUP_FAVOURITES_DESCRIPTION
* Tagh **Sàbhail & Dùin** bhon Bhàr-inneal.

## A’ Mìneachadh an Raoin

Gus càr as fheàrr leat a thaghadh, dh’fhaodadh tu liosta tuiteam-sìos de chàraichean a
mhìnicheas tu a thoirt seachad, no liosta tuiteam-sìos de chàraichean a gheibhear bho bhòrd stòr-dàta,
no liosta de phutanan rèidio le bileagan a mhìnicheas tu. Anns a’ chùis seo, leigidh raon inntrigidh teacsa sìmplidh
leat dèanamh agus modail càr sam bith a chur a-steach bho eachdraidh iomlan gnìomhachas nan càraichean.

Bho chlàr-taice an Rianaire:

* Tagh nì a’ chlàir **Com-pàirtean / Contacts / Raointean**.
* Tagh am putan **Ùr** bhon Bhàr-inneal.
* Anns an raon Tiotal, cuir a-steach an constant COM_CONTACT_CUSTOM_FIELD_FAVOURITE_CAR
* Anns an raon Seòrsa, tagh **Teacsa (text)** mura h-eil e air a thaghadh mu thràth.
* Anns an raon Tuairisgeul, cuir a-steach an constant COM_CONTACT_CUSTOM_FIELD_FAVOURITE_CAR_DESCRIPTION
* Anns an raon **Buidheann Raoin** (air an taobh dheas), tagh a’ Bhuidheann Raoin a chruthaich thu.
* Tagh **Sàbhail & Dùin** bhon Bhàr-inneal.

## Deasaich Neach-conaltraidh

Le Beurla air a thaghadh mus tèid an rianaire a-steach, bu chòir taba a bhith
anns an fhoirm inntrigidh dàta Conaltraidh le ainm Beurla na buidhne raoin agad agus
raointean sa bhuidheann sin cuideachd le luachan Beurla.

![Inntrigeadh dàta sa Bheurla](../../../en/images/fields/adding-custom-fields-multilingual-sites/02-fields-overrides-entry.png)

Le Gearmailtis air a thaghadh mus tèid an rianaire a-steach, bu chòir dhut na
h-eadar-theangachaidhean Gearmailteach de na cunbhalaichean cànain agad fhaicinn:

![Inntrigeadh dàta sa Ghearmailtis](../../../en/images/fields/adding-custom-fields-multilingual-sites/03-fields-overrides-entry-de.png)

Rabhadh: eadar-theangachadh le translate.google.co.uk!

## Seall Neach-conaltraidh

Sa Bheurla:

![Taisbeanadh dàta sa Bheurla](../../../en/images/fields/adding-custom-fields-multilingual-sites/04-fields-overrides-display.png)

Agus sa Ghearmailtis:

![Taisbeanadh dàta sa Ghearmailtis](../../../en/images/fields/adding-custom-fields-multilingual-sites/05-fields-overrides-display-de.png)

*Air eadar-theangachadh le openai.com*