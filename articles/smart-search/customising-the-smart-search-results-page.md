<!--
{
    "source": "https://docs.joomla.org/Customising_the_Smart_Search_results_page",
    "title": "S\u00e0r-sgr\u00ecobhaidhean Cruth Rannsachaidh Glica",
    "description": " ",
    "author": ""
}
-->

## Duilleagan nan Toraidhean

Tha còig faidhlichean crutha aig a’ cho-phàirt Rannsachadh Glic as urrainn dhut
ath-sgrìobhadh gus cruth a chruthachadh a fhreagras air do roghainn fhèin. Gus am
pròiseas a thòiseachadh bhon chlàr-taice Rianaire:

* Tagh **Siostam / Teamplaidean Làraich / Mion-fhiosrachadh agus Faidhlichean Cassiopeia**.
* Tagh an taba **Cruthaich Sàr-sgrìobhaidhean**.
* Bhon phannal Co-phàirtean, tagh **com_finder**.
* Tagh an nì **Rannsachadh**
* Bhon phannal Deasaiche, tagh **html / com_finder / search** gus an liosta
  de na faidhlichean sàr-sgrìobhaidh a chaidh a chruthachadh fhaicinn.

Cha bhi buaidh aig ùrachaidhean Joomla air na faidhlichean seo, ach dh’fhaodadh
gun tèid do chuimhneachadh sùil a thoirt orra ma thèid na tùsan tùsail ùrachadh.

## Sealladh an Rannsachaidh (Cruth Bunaiteach)

Tha sealladh rannsachaidh a’ chruth bhunaiteach air a roinn ann an grunn phàirtean: 

- cruth bunaiteach
- cruth an fhoirm
- cruth nan toraidhean
- cruth an t-seòrsachaidh.

### An cruth bunaiteach (default.php)

Tha an cruth seo glè shìmplidh. Chan eil e a’ mìneachadh ach an structar anns a
bheil am foirm rannsachaidh agus toraidhean an rannsachaidh air an taisbeanadh.
Tha an cruth seo cuideachd an urra ri luchdachadh na duilleige-stoidhle CSS
bhunaiteach airson Rannsachadh Glic, a tha suidhichte ann an
`media/com_finder/css/finder.css`, agus mar sin dh’fhaodadh gum bi thu airson
sin atharrachadh gus na riaghailtean CSS agad fhèin airson Rannsachadh Glic a
luchdachadh.

### Cruth an fhoirm (default_form.php)

Tha an cruth seo a’ mìneachadh a’ chòd a tha riatanach gus am bi am foirm
rannsachaidh ag obrachadh mar bu chòir. Bidh an cruth a’ cleachdadh còd
JavaScript, mar sin feumaidh tu a bhith faiceallach na taghadairean a ghleidheadh
nach bu chòir atharrachadh mura h-eil fios agad dè tha thu a’ dèanamh.

Tha grunn raointean falaichte anns an dòigh-seallaidh `getFields` a tha riatanach
airson rannsachadh earbsach. Tha teirm an rannsachaidh air a mhìneachadh leis an
raon ion-chuir leis an ainm "q".

### Cruth nan toraidhean (default_results.php)

Bidh an cruth seo a’ cruthachadh liosta de na toraidhean a tha a’ freagairt ris an
teirm rannsachaidh. Bidh e cuideachd a’ làimhseachadh duilleagachadh agus a’
luchdachadh cruth airson gach toradh rannsachaidh fa leth.

### Cruth an toraidh (default_result.php)

Seo an cruth a thathar a’ cleachdadh gus aon toradh a thaisbeanadh.

### Cruth an t-seòrsachaidh (default_sorting.php)

Chan eil an nì seo an làthair ach ma tha *Seall Raointean Seòrsachaidh* air a
shuidheachadh gu *Tha* agus ma tha aon raon seòrsachaidh a bharrachd no barrachd
air an taghadh ann an taba Adhartach Nì a’ Chlàir-thaice.

*Air eadar-theangachadh le openai.com*