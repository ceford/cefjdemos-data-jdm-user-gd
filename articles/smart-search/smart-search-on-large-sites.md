<!--
{
    "source": "https://docs.joomla.org/Smart_Search_on_large_sites",
    "title": "Lorg Glic air L\u00e0raichean M\u00f2ra",
    "description": " ",
    "author": ""
}
-->

## Clàr-innse na Làraich

Bidh Lorg Glic ag obair le bhith a’ cruthachadh agus a’ cumail suas clàr-innse neo-eisimeileach de theirmean luirg ann an grunn chlàran stòr-dàta. Is e an duilgheadas le làraichean mòra gum faod am pròiseas clàraidh-innse a bhith gu math trom a thaobh cleachdadh CPU, cuimhne agus diosg. Eadhon às dèidh a’ chiad chruthachadh den chlàir-innse, faodaidh ùrachaidhean mean air mhean a bhith trom cuideachd. ’S e an naidheachd mhath gu bheil ceasnachadh a’ chlàir-innse na obrachadh caran luath agus aotrom.

Tha Lorg Glic freagarrach airson a’ mhòr-chuid de làraichean Joomla. Ach, tha dùbhlain shònraichte an lùib lorg airson làraichean mòra. Bu chòir cuimhneachadh gur e buileachadh PHP fìor-ghlan de einnsean luirg a th’ ann an Lorg Glic, agus dh’fhaodadh gum biodh làraichean air leth mòr nas fheàrr dheth le einnsean luirg neo-eisimeileach leithid Solr.

Gus Lorg Glic a chleachdadh air làrach mhòr, ’s dòcha gum feum thu cuid de na roghainnean rèiteachaidh atharrachadh. Seo cuid de chomhairle choitcheann mu na rudan air am bu chòir sùil a chumail agus na rudan a dh’fhaodadh tu feuchainn ri gleusadh.

## Cleachd an Clàraiche-innse CLI an-còmhnaidh

Leis gum faod am pròiseas clàraidh-innse tùsail ùine mhòr a thoirt, tha e nas fheàrr an clàraiche-innse a ruith bhon loidhne-àithne gus duilgheadasan sam bith le seiseanan a’ bhrabhsair a’ tighinn gu crìch a sheachnadh. Cha tig ùine-ama gu crìch air a’ chlàraiche-innse CLI ge bith dè cho fada ’s a bheir e gus crìochnachadh, agus faodar a chur dheth gu furasta ma nochdas duilgheadasan. A bharrachd air sin, chithear teachdaireachdan mearachd leis a’ chlàraiche-innse CLI, ach dh’fhaodadh iad a bhith falaichte nuair a bhios e ga ruith bhon Rianaire.

Gus an CLI a chleachdadh, fosgail ceann-uidhe, gluais dhan phasgan cli ann am bun-eòlaire na làraich agad agus cuir a-steach an àithne a leanas:

```
php joomla.php finder:index
```

## Bacaidseadh

Bidh an clàraiche-innse a’ briseadh na h-obrach clàraidh-innse ann am buidseanan de nithean susbaint. Gu bunaiteach, tha meud a’ bhaidse suidhichte aig 50, a’ ciallachadh gun tèid suas ri 50 nì susbaint a chlàradh anns gach baidse. Dh’fhaodadh àrdachadh meud a’ bhaidse am pròiseas clàraidh-innse a dhèanamh nas luaithe, ach cleachdaidh e barrachd cuimhne agus ’s dòcha barrachd àite diosga sealach.

## Duilgheadasan le Dìth Cuimhne

Ma tha an clàraiche-innse a’ ruith a-mach à cuimhne, feuch na h-atharrachaidhean a leanas aon aig aon àm gus am bi an duilgheadas air fhuasgladh.

1.  Lùghdaich meud a’ bhaidse. Ma tha nithean susbaint air leth mòr agad, faodaidh an clàraiche-innse ruith a-mach à cuimhne eadhon air aon nì susbaint, mar sin feuch ri a leigeil sìos gu 5 an toiseach agus, ma tha thu fhathast a’ ruith a-mach à cuimhne, leig sìos gu 1 e.
2.  Mas urrainn dhut barrachd cuimhne a riarachadh don chlàraiche-innse, dèan sin. Faodaidh tu a’ chuimhne a tha air a riarachadh don chlàraiche-innse loidhne-àithne àrdachadh le paramadair a bharrachd air an loidhne-àithne. Mar eisimpleir, gus crìoch na cuimhne àrdachadh gu 256Mb, cleachd an àithne a leanas, a’ cur na h-uimhir de chuimhne ’s as urrainn dhut a riarachadh gu sàbhailte do phròiseas air an t-siostam agad an àite *256M*.
```php
    php -d memory_limit=256M joomla.php finder:index
```

3.  Feuch ri aithneachadh dè na nithean susbaint a tha ag adhbhrachadh don chlàraiche-innse ruith a-mach à cuimhne. Mura h-eil e follaiseach, dh’fhaodadh tu feuchainn ris na plugain Lorg Glic uile a chur à comas ach aon dhiubh. Bu chòir ruith a’ chlàraiche-innse le dìreach aon phlugain an comas aig aon àm innse dhut dè an seòrsa no na seòrsaichean susbaint a tha ag adhbhrachadh na cùise. Mar roghainn mu dheireadh, smaoinich air beagan de na nithean susbaint air leth mòr a bhriseadh nan nithean fa leth. Ma tha an duilgheadas co-cheangailte ri seòrsa susbaint ghnàthaichte, thoir sùil air còd a’ phlugain agus smaoinich air nas lugha den t-susbaint a tha ri fhaighinn a chlàradh airson gach nì.

## Duilgheadasan le Dìth Àite Diosga

Faodaidh clàran clàr-innse Lorg Glic fàs gu luath! Tha an clàr
*#__finder_links_termsX* a’ cumail aon ràgh airson gach teirm/abairt airson gach nì susbaint, agus mar as trice bidh aon artaigil Joomla anns a bheil 1000 facal a’ leantainn gu mu 3000 ràgh a bharrachd anns na clàran seo. Cuiridh dàrna artaigil den aon mheud mu àireamh cho-ionann de ràghan ris, fiù ’s ma tha na h-aon fhaclan anns an dà artaigil. Tha coltas ann gum bi milleanan de ràghan anns a’ chlàr mhapachaidh seo air làrach anns a bheil deichean mhìltean de dh’artaigilean, cuid dhiubh le mìltean de fhaclan. Chan eil e neo-àbhaisteach gum bi na clàran clàr-innse a’ gabhail grunn gigabytes de dh’àite diosga ann an suidheachaidhean mar seo.

Tha roghainn aig a’ chlàr-innse airson co-dhùnadh eadar mionaideachd an luirg agus meud a’ chlàir-innse. Nuair a bhios “Lorg abairtean” an comas anns na roghainnean coitcheann aig a’ cho-phàirt, bidh an clàr-innse agad nas motha, ach leigidh e cuideachd le toraidhean luirg nas mionaidiche. Ma bhios e à comas, bidh an clàr-innse tòrr nas lugha, ach cha bhi e comasach abairtean slàn a lorg.

## Notaichean

1.  Chan eil glasadh co-aontachais ann an-dràsta gus casg a chur air barrachd air aon phròiseas an clàraiche-innse a ruith aig an aon àm. Cha mhòr cinnteach gun adhbharaich seo clàr-innse truaillte. Dh’fhaodadh eadhon cuideigin a’ sàbhaladh atharrachaidhean do nì susbaint fhad ’s a thathar a’ dèanamh clàr-innse slàn cron a dhèanamh air a’ chlàr-innse.

*Air eadar-theangachadh le openai.com*