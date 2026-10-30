<!--
{
    "source": "https://docs.joomla.org/Multiple_Domains_and_Web_Sites_in_a_single_Joomla!_installation",
    "title": "Ioma-raointean agus L\u00e0raichean-l\u00ecn ann an aon st\u00e0ladh Joomla!",
    "description": " ",
    "author": ""
}
-->

**Nòta:** Chaidh an t-artaigil seo ùrachadh mu dheireadh ann an 2012!

Ged a tha e na dheagh chleachdadh an raon-lìn, an stàladh Joomla! agus an stòr-dàta fhèin a thoirt do gach Làrach-lìn,
faodaidh suidheachaidhean sònraichte a bhith ann far a bheil fuasgladh ioma-làraich fo aon stàladh Joomla! iomchaidh.

## Eisimpleir de Thagradh

Tha dà bhrand eadar-dhealaichte ach co-cheangailte aig gnìomhachas beag, ‘Johnson Candies’: *Red Candy* agus *Yellow Candy*. Tha feum aca air aon Làrach-lìn stèidhichte air Joomla! far a bheil an dà sheòrsa siùcair ri fhaicinn, le duilleag-dhachaigh fa leth aig gach fear air làrach Joomla! a tha a’ freagairt ris na raointean `www.redjohnsoncandy.com` agus `www.yellowjohnsoncandy.com`.

A bharrachd air sin, **tha feum aig gach brand agus làrach air a dhealbhadh fhèin**: teamplaid bhuidhe airson aon dhiubh; teamplaid dhearg airson an tè eile.

## Buannachdan

Le bhith a’ gabhail a-steach an dà bhrand ann an aon stàladh lìn Joomla!, faodaidh Johnson Candies ùine deasachaidh a shàbhaladh (dìreach aon logadh a-steach), artaigilean agus dàta a cho-roinn eadar an dà bhrand (no làrach), agus aon fheart, leithid foirm “Cuir fios thugainn”, a chleachdadh airson an dà bhrand.

## Modh-obrach an Gnìomhachaidh

### Ullaich na Raointean agad

Cleachd aon raon airson a’ chunntais aoigheachd agad, mar as àbhaist. Cruthaich na raointean cur-ris a tha riatanach ann am pannal-smachd a’ chunntais aoigheachd agad. Airson adhbharan an oideachaidh seo, cleachdaidh sinn `www.redjohnsoncandy.com` a bharrachd air ainm an raoin bhunaiteach `www.yellowjohnsoncandy.com`.

### Stàlaich agus Suidhich Joomla!

Stàlaich agus suidhich Joomla! mar as àbhaist. An uair sin leasaich artaigilean, clàir-thaice agus mòilean airson gach làraich.

### Cruthaich Teamplaidean

An ath rud, leasaich agus stàlaich na teamplaidean riatanach — aon airson gach làraich a tha thu airson a bhith agad. Anns an eisimpleir gu h-àrd, chruthaicheadh tu teamplaid airson *red candy* leis an ainm *Red Template*, agus teamplaid airson *yellow candy* leis an ainm *Yellow Template*. Nuair a bhios na teamplaidean air an stàladh, sònraich iad do na nithean clàir-thaice iomchaidh, a’ cleachdadh manaidsear theamplaidean Joomla! ann an raon Rianaire Joomla!.

### Cuir Ath-stiùireadh ris

#### Roghainn #1: Cruthaich ath-stiùireadh .htaccess (Apache)

**Nòta** *Cuir URLan SEF an comas ann an Joomla! an toiseach*

Is e aon roghainn .htaccess (Apache) a chleachdadh gus iarrtasan gu raon sònraichte ath-stiùireadh gu duilleag shònraichte Joomla!.

Is e ar n-amas iarrtasan sam bith gu ainm raoin Red Candy ath-stiùireadh gu duilleag shònraichte air làrach Joomla!. San eisimpleir seo, bidh sinn ag ath-stiùireadh iarrtasan sam bith gu `www.redjohnsoncandy.com` gu duilleag blog-roinn. Bhiodh tu air an teamplaid ‘red cand  y’ a shònrachadh don nì clàir-thaice seo roimhe, gus coltas làraich fa leth a chruthachadh.
```
#The following rule works, but it changes which domain name displays.
RewriteCond %{HTTP_HOST} ^(www\.)?redjohnsoncandy\.com$
RewriteRule (.*) http://www.yellowjohnsoncandy.com/index.php?option=com_content&view=category&layout=blog&id=3&Itemid=12 [R=301,L]
```

Uill, tha sin ag obair — ach chì thu an ana-cothrom sa bhad. Ged a tha an cleachdaiche a’ coimhead air làrach Red Candy gu soirbheachail, chì iad fhathast ainm raoin Yellow Candy. Gu mì-fhortanach, ma tha thu a’ cleachdadh an dà chuid .htaccess agus pàirceadh raoin (ath-stiùireadh gu teicnigeach), tha seo riatanach gus nach cruthaichear LÙB.

#### Roghainn #2: Cruthaich Ath-stiùireadh Bann-cinn PHP

Tha buannachd aig an fhuasgladh seo leis gu bheil e a’ cumail suas coltas raointean/làraichean-lìn fa leth don neach-tadhail. An àite .htaccess (Apache) a chleachdadh airson an ath-stiùiridh againn, cleachdaidh sinn aon de na teamplaidean air an làraich.

San eisimpleir seo, ’s e `www.redjohnsoncandy.com` an raon bunaiteach. Tha thu air teamplaid a chruthachadh airson na sgìre sin leis an ainm *Red Template*. ’S e an cleas faidhle index.php *Red Template* fhosgladh agus na leanas a chur ris **mar na ciad loidhnichean fhèin** de phrìomh index.php an stàlaidh.

```php
<?php
$domain = $_SERVER["HTTP_HOST"];
$uri = $_SERVER["REQUEST_URI"];
$url = $domain . $uri;

if (($url == "redjohnsoncandy.com/") ||
   ($url == "www.redjohnsoncandy.com/")) {
   header("Status: 301 Moved Permanently");
   header("Location: http://www.redjohnsoncandy.com/index.php?option=com_content&view=category&layout=blog&id=3&Itemid=12");
}
?>
```

Seo a’ bhuannachd: Thèid an neach-tadhail ath-stiùireadh a-nis gu duilleag iomchaidh *Red Site*, aig a bheil an *Red Template* air a shònrachadh dha **a-mhàin** ma tha iad air ruighinn aig ainm raoin na ‘làraich dheirge’. Air neo, thèid riaghailt chumhachdach PHP a leigeil seachad, agus luchdaichear an Làrach Bhuidhe.

Tha e cudromach cuimhneachadh cuideachd an URI (an URL a tha a’ leantainn an raoin fhìor) iarraidh gus an urrainn dhut ath-stiùiridhean a dhèanamh chun an aon raoin. Nuair a tha an URI do-fhaicsinneach san URL, bidh an caochladair na chomharra “/”. Sin as coireach gum feum thu an URL fhìor agad a choimeas ri comharra “/” aig an deireadh. Mar seo, bidh e comasach dhut ath-stiùiridhean 301 a dhèanamh san aon raon. Air neo, cruthaichidh tu lùb neo-chrìochnach sa phròiseas ath-stiùiridh.

#### Roghainn #3: Cruthaich Ath-stiùireadh Bann-cinn PHP, airson iomadh raon le ath-stiùiridhean raoin sònraichte airson teamplaidean gnàthaichte

Fuasgladh airson aon àite-lìn, le diofar raointean, aon stàladh Joomla!, agus a rèir an raoin far an tig an cleachdaiche air tìr, ath-stiùireadh gu duilleag bhunaiteach eadar-dhealaichte. Cuir an còd PHP a leanas **mar a’ chiad rud fhèin** ann am prìomh fhaidhle index.php an stàlaidh. Gus raon eile a shònrachadh, dìreach dèan lethbhreac/gluadh den ghnìomh “if” agus deasaich e leis na luachan aig an raoin eile san aon dòigh. A bharrachd air sin, gus na seallaidhean teamplaid a shuidheachadh, feumaidh tu ailiasan eadar-dhealaichte airson nithean/ceanglaichean nam mòilean a shònrachadh agus seallaidhean nan teamplaidean a shuidheachadh taobh a-staigh manaidsear theamplaidean Joomla!. Tha feum air suidheachadh an ailiais nuair a chleachdas tu roghainnean SEF.
```php
<?php
$domain = $_SERVER["SERVER_NAME"];
$requri = $_SERVER['REQUEST_URI'];
if (($domain == "www.example.de" && $requri == "/" ||
   $domain == "example.de"))  {
   header("Status: 301 Moved Permanently");
   header("Location: http://www.example.de/index.php?option=com_content&view=article&id=6");
}
?>
```

*Air eadar-theangachadh le openai.com*