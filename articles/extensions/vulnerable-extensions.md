<!--
{
    "source": "https://docs.joomla.org/jdocmanual?manual=user&heading=extensions&filename=vulnerable-extensions.md",
    "title": "Leudachain So-le\u00f2nte",
    "description": " ",
    "author": ""
}
-->

## Tùsan Leudachan

Faodaidh duine sam bith leudachan Joomla! a sgrìobhadh agus a sgaoileadh mar sheirbheis don choimhearsnachd chruinneil. Gheibhear leudachain **treas-phàrtaidh** mar seo air làraichean-lìn luchd-leasachaidh leudachan proifeiseanta, làraichean-lìn bhlogaichean pearsanta, GitHub agus ionadan-tasgaidh coltach ris, agus air làrach-lìn Directory nan Leudachan Joomla.

## Leudachain So-leònte

Is e glè bheag de thùsan a tha a’ tabhann leudachain a tha droch-rùnach a dh’aona ghnothaich. Mar as trice, ’s e **leudachan so-leònte** fear a chaidh a lorg a’ gabhail a-steach (no a’ cur ri) so-leòntachd tèarainteachd às dèidh a chiad fhoillseachaidh.

Chan eil leudachain so-leònte riatanach air an còdadh gu dona. Mar a bhios an Lìon a’ fàs, bidh riatanasan theicnigeach agus cleachdaidhean còdaidh ris an gabhar gu cumanta ag atharrachadh. Bidh pròiseactan gnìomhach a’ foillseachadh tionndaidhean ùra de na leudachain aca mar a bhios riatanasan ag atharrachadh agus a’ càradh gu luath so-leòntachdan sam bith a thèid aithris.

Ma tha dragh ort mu aon sam bith de na leudachain agad, bu chòir dhut coimhead ri liosta Leudachain So-leònte Joomla (VEL), anns a bheil fiosrachadh mu chòrr is 240 leudachan, a’ mhòr-chuid dhiubh sean.

## An Dearbhadair JED

Ma tha dragh ort mu leudachan nach eil a’ nochdadh anns an VEL, faodaidh tu an leudachan JED Checker a chleachdadh. ’S e leudachan a tha seo a thathar a’ cleachdadh gus sùil a chumail air leudachain a chuirear a-steach airson nochdadh ann an liosta Directory nan Leudachan Joomla. Tha e air a stàladh mar leudachan sam bith eile. Nuair a thèid a chleachdadh, gabhaidh e faidhle zip leudachain agus nì e sgrùdadh air na tha na bhroinn gus dèanamh cinnteach gu bheil e a’ gèilleadh ri inbhean JED. Tha e air leth feumail eadhon airson leudachain nach eil a’ nochdadh ann an liosta JED. Seo dealbh-sgrìn eisimpleir:

![toradh an dearbhadair JED](../../../en/images/extensions/vulnerable-extensions/01-extensions-jed-checker.png)

Tha na 400 faidhlichean PHP aig nach eil Sanas Ceadachais GPL ann an leabharlannan treas-phàrtaidh aig a bheil Ceadachas eadar-dhealaichte. Tha na 30 faidhlichean a chaidh an comharrachadh le Sgriobt Sganadh an-aghaidh Malware Joomla cuideachd anns na leabharlannan treas-phàrtaidh sin. Tha obair ri dhèanamh air na faidhlichean aig nach eil tèarainteachd JEXEC!

## A’ Toirt air Falbh Leudachan So-leònte

### Dèan Liosta de na Faidhlichean a Thèid a thoirt air Falbh

Mas urrainn dhut a lorg, leugh faidhle XML an leudachain gus faighinn a-mach dè na seòlaidhean, faidhlichean agus bùird stòr-dàta a chaidh a chur ris an t-siostam agad. Tha am faidhle XML anns an tasg-lann zip thùsail a chaidh a chleachdadh rè pròiseas stàlaidh an leudachain. Mar eisimpleir, bhiodh tasg-lann zip airson leudachan air a bheil mod_vulnerable a’ gabhail a-steach faidhle XML air a bheil mod_vulnerable.xml, agus ’s dòcha gum biodh liosta de fhaidhlichean ann mar a leanas:

```
    mod_vulnerable.php
    mod_vulnerable/vulnerable_file.txt
    mod_vulnerable/another_vulnerable_file.txt
    mod_vulnerable/yet_another_vulnerable_file.txt
    mod_vulnerable/index.html
```

### Dì-stàlaich tro Shuidhichear Joomla

A’ cleachdadh an t-Suidhicheir ann an deireadh-rianachd Joomla!, dì-stàlaich an leudachan so-leònte. Is dòcha gum feum thu cuideachd modalan, co-phàirtean no plugain co-cheangailte a dhì-stàladh.

### Dearbhaich gun deach am Pròiseas Dì-stàlaidh a Chrìochnachadh

Na bi an urra ris an leudachan gus na faidhlichean aige uile a thoirt air falbh gu sàbhailte. Dèan coimeas eadar na seòlaidhean agus na faidhlichean air an t-siostam agad agus liosta XML an leudachain gus dèanamh cinnteach gun deach na faidhlichean co-cheangailte uile a thoirt air falbh dha-rìribh.

### Roghainneil, Thoir air falbh na Bùird Stòr-dàta Co-cheangailte

Thoir sùil air an stòr-dàta agad agus thoir air falbh bùird sam bith a chaidh a chruthachadh leis an leudachan. Gus am pròiseas ùrachaidh gu tionndaidhean ùra a dhèanamh nas fhasa, cha bhith mòran sgriobtaichean dì-stàlaidh a’ toirt air falbh bùird stòr-dàta co-cheangailte. Gheibh thu liosta nam bòrd ann am faidhle XML gach leudachain.

Ma tha thu an dùil tionndadh nas sàbhailte, co-fhreagarrach den aon leudachan a stàladh agus gu bheil thu airson an dàta a th’ ann ath-chleachdadh, mar as trice faodaidh tu na bùird stòr-dàta fhàgail mar a tha iad.

### Thoir air falbh Ceanglaichean a’ Chlàir-thaice

Chan eil dìreach toirt air falbh nan ceanglaichean clàr-taice gu leudachan, no foillseachadh modal, **gu leòr** gus an làrach agad a dhìon! Cho fad ’s a tha faidhlichean an leudachain ann air an fhrithealaiche agad, tha thu so-leònte. Thoir fa-near mar a chì neach-ionnsaigh anns na h-eisimpleirean a leanas faighinn seachad air faidhle clàr-amais Joomla! gus cuimseachadh dìreach air faidhle sam bith, de leudachan sam bith.

```
    www.your_site.org/components/com_bad_component/vulnerable_file.php
    www.your_site.org/modules/mod_bad_module/vulnerable_file.php
```

*Air eadar-theangachadh le openai.com*