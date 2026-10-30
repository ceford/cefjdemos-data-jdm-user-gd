<!--
{
    "source": "https://docs.joomla.org/Setting_up_automatic_Smart_Search_indexing",
    "title": "Indeacsadh Rannsachadh Glic",
    "description": " ",
    "author": ""
}
-->

## Indeacsadh Fèin-obrachail

Ged a thèid clàr-amais Rannsachadh Glic ùrachadh gu fèin-obrachail
nuair a thèid nithean susbaint atharrachadh, tha suidheachaidhean ann far a bheil
feum agad air an Innealaiche-indeacsachaidh a ruith a-rithist. Faodaidh tu seo a dhèanamh le làimh
a’ cleachdadh a’ phutan *Index* air a’ bhàr-inneal air an duilleag *Smart Search: Indexed Content*. Ach ma tha feum agad
air susbaint ath-indeacsadh gu fèin-obrachail, tha e comasach cuideachd an Innealaiche-indeacsachaidh a ruith
bhon eadar-aghaidh loidhne-àithne. Tha seo gu sònraichte goireasach airson an
Innealaiche-indeacsachaidh a ruith bho obair *cron*.

Bhon phasgan cli, ’s e seo an loidhne-àithne:

```
php joomla.php finder:index
```

Tha toradh àbhaisteach bhon Innealaiche-indeacsachaidh loidhne-àithne a’ coimhead mar seo:

```sh
    Smart Search INDEXER
    ============================

    Starting Indexer
    Setting up Finder plugins
    Setup 154 items in 0.094 seconds.
     * Processed batch 1 in 0.213 seconds.
     * Processed batch 2 in 0.182 seconds.
     * Processed batch 3 in 0.177 seconds.
     * Processed batch 4 in 0.009 seconds.
    Total Processing Time: 0.676 seconds.
```

## A’ Glanadh Mus tèid Indeacsadh

Mar as trice, nì ruith an Innealaiche-indeacsachaidh ùrachadh mean air mhean air
a’ chlàr-amais. ’S e sin, chan ùraich e ach an clàr-amais airson nan nithean susbaint
sin a tha air atharrachadh bhon uair mu dheireadh a chaidh an clàr-amais ùrachadh. Cha
toir e air falbh nithean sam bith bho indeacsadh roimhe a thàinig bho plugain a chaidh an dì-stàladh.
Mar sin, ma tha feum agad air na h-inntrigidhean clàr-amais a th’ ann mu thràth a ghlanadh gu tur mus tèid an
clàr-amais ath-thogail gu tur, feumaidh tu obrachadh “glanadh agus an uair sin indeacsadh”
a dhèanamh. Gus sin a dhèanamh, faodaidh tu an argamaid `-- purge` a chur ris an
loidhne-àithne, mar seo

    php joomla.php finder:index -- purge

Thoir fa-near gun fheuch seo ri sìoltachain statach sam bith a chuir thu air dòigh a ghlèidheadh, ach cha ghlèidh taghadh **Cumail suas→Glan an clàr-amais** air bàr-inneal an Rianaire na sìoltachain statach agad.

## A’ Stèidheachadh Obair *cron*

Ged a tha na mion-fhiosrachadh taobh a-muigh raon an artaigil seo, sa chumantas
cha leig thu leas ach an àithne gu h-àrd a chur a-steach do mhanaidsear na h-obrach *cron*
agus an t-àm no na h-amannan aig am bi an obair ri ruith a shònrachadh. Is dòcha
gum feum thu an t-slighe iomlan chun an inneil indeacsachaidh a chur a-steach. Mar eisimpleir,
mar seo

    php /var/www/myjoomla/cli/joomla.php finder:index -- purge

Dh’fhaodadh gum bi e riatanach cuideachd an t-slighe iomlan chun na h-àithne php a shònrachadh, mar `/usr/local/opt/php@8.2/bin/php`.

## Duilgheadasan Cuimhne a’ Ruith A-mach

Ma tha riatanasan indeacsachaidh gu sònraichte toinnte aig an làrach agad, tha
e comasach nach bi an riarachadh cuimhne àbhaisteach gu leòr gus an
Innealaiche-indeacsachaidh a ruith gu deireadh. Faodaidh tu an cuimhne a tha air a riarachadh
don inneal indeacsachaidh loidhne-àithne àrdachadh le paramadair a bharrachd air an
loidhne-àithne, mar seo:

    php -d memory_limit=256M joomla.php finder:index

Cuir na tha iomchaidh airson do shuidheachaidhean an àite `256M`.

Bidh Innealaiche-indeacsachaidh na loidhne-àithne a’ cleachdadh nan aon pharamadairean ris an Innealaiche-indeacsachaidh air an duilleag **Smart
Search: Indexed Content**. Faodaidh tu na paramadairean atharrachadh le bhith a’ cleachdadh
a’ phutan *Options* air bàr-inneal na duilleige sin. Thoir fa-near gu bheil an dà raon
**Indexer Batch Size** agus **Memory Table Limit** a’ toirt buaidh air na tha de chuimhne a bhios an Innealaiche-indeacsachaidh a’ cleachdadh.

*Air eadar-theangachadh le openai.com*