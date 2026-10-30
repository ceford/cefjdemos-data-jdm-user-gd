<!--
{
    "source": "https://docs.joomla.org/J4.x:FatalError",
    "title": "Mearachd Marbhtach",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Bho àm gu àm faodaidh Joomla duilleag mearachd a shealltainn an àite na duilleige
a bha thu an dùil fhaicinn. Tha dà sheòrsa de dhuilleag mhearachd ann:

- Tha cùl-raon dearg air duilleag mearachd an t-siostaim. Thèid a gairm ma thachras
  mearachd chudromach mus tèid teamplaid na làraich no an rianaire a renderadh.
- Tha coltas duilleag mearachd na teamplaide coltach ris an teamplaid àbhaisteach
  den làrach no an rianaire, ach thèid teachdaireachd mearachd a chur an àite na
  raoin susbaint. Thèid seo a gairm nuair a thachras a’ mhearachd sa chòd susbaint.

### Duilleag Mearachd an t-Siostaim

![Duilleag mearachd marbhtach an t-siostaim](../../../gd/images/problems/fatal-error/01-fatal-error.png)

### Duilleag Mearachd na Teamplaide

![Duilleag mearachd na teamplaide](../../../gd/images/problems/fatal-error/02-template-error.png)

## Mar a Rèiticheas Tu E

Tha grunn adhbharan comasach ann airson mearachdan marbhtach. Seo
beagan dhiubh:

- Atharrachadh san aoigheachd agad, mar eisimpleir tionndadh PHP ùraichte nach eil
  co-chòrdail ri Joomla no ri fear dhe na Leudachain agad.
- Duilgheadas le àite diosga, cleachdadh cuimhne no ùine-crìochnachaidh sgriobt.
- Leudachan a chaidh a stàladh no a chomasachadh o chionn ghoirid nach eil co-chòrdail
  ri Joomla. Dh’fhaodadh plugan dona casg a chur air logadh a-steach an Rianaire!

### Cuir an Dì-bhugachadh an comas

Ma tha an eadar-aghaidh Rianaire agad **fhathast** ag obair:
- Rach gu **Deas-bhòrd Dachaigh → Pannal an t-Siostaim → Rèiteachadh Cruinneil**. 
- Anns an taba Siostaim, suidhich *Dì-bhugachadh an t-Siostaim* gu *Tha*. 
- Anns an taba Frithealaiche, suidhich *Aithris Mhearachdan* gu *As motha*. 
- An uair sin *Sàbhail & Dùin*.

Mura h-eil an eadar-aghaidh Rianaire agad ag obair, deasaich am faidhle
*configuration.php* sa phasgan freumhaich de làrach-lìn Joomla agad.

1.  Atharraich na ceadan bho *444* no *-r--r--r--* (chan eil cead aig duine
    sgrìobhadh dhan fhaidhle) gu *644* no *-rw-r--r--* (chan eil cead sgrìobhaidh
    ach aig an t-Sealbhadair).
2.  Deasaich am faidhle le deasaiche teacsa agus suidhich `$debug` gu `true` agus 
    `$error_reporting` gu `'maximum'`.
3.  *Sàbhail* am faidhle.

Às dèidh dhut na h-atharrachaidhean a dhèanamh, ath-luchdaich an duilleag a bha
ag adhbhrachadh na mearachd. Bu chòir dhut lorg-staca fhaicinn a-nis. Eisimpleir:

![Duilleag mearachd na teamplaide](../../../en/images/problems/fatal-error/03-template-error-stack-trace.png)

Tha a’ chiad nì san lorg-staca a’ sealltainn càit an deach a’ mhearachd a
bhrosnachadh. Uaireannan tha sin gu leòr gus an Leudachan lochtach aithneachadh.
Uaireannan tha an Leudachan lochtach nas fhaide sìos san lorg-staca. Is dòcha nach
dèan e mòran ciall dhut, ach tha an lorg-staca air leth luachmhor dha na
h-eòlaichean a fhreagras ceistean ann am Fòraman Joomla.

Mas urrainn dhut an Leudachan lochtach aithneachadh, cuir à comas e. Faodaidh tu
seo a dhèanamh leis an eadar-aghaidh Rianaire ma tha e ag obair. Mur eil, cleachd
phpMyAdmin gus an Leudachan a lorg ann an clàr-dàta `#__extensions` agus suidhich
a luach `enabled` gu `0`. Cha bu chòir gum feumadh tu Leudachain bunaiteach
Joomla sam bith a chur à comas.

## Neach-cuideachaidh Phuist an Fhòraim

Gus cuideachadh le fuasgladh dhuilgheadasan, bu chòir dhut an
[Neach-cuideachaidh Phuist an Fhòraim (FPA)](https://forumpostassistant.github.io/docs/) a luchdachadh a-nuas agus
a chur ann am freumh làrach-lìn Joomla agad. Tha an ceangal airson a lorg cuideachd
faisg air mullach gach duilleig Fòram Joomla. ’S e sgriobt PHP fa leth a th’ anns
an FPA a nì mion-sgrùdadh air stàladh Joomla agad agus a dh’innseas dhut dè
dh’fhaodadh a bhith ceàrr. A-rithist, is dòcha nach dèan e mòran ciall dhut, ach
dh’fhaodadh na h-eòlaichean a fhreagras ceistean sna Fòraman iarraidh ort sealltainn
dhaibh e.

## Glanadh

Nuair a bhios an duilgheadas agad air a rèiteachadh:

1.  Rach gu **Deas-bhòrd Dachaigh → Pannal an t-Siostaim → Rèiteachadh Cruinneil**
2.  Tagh an taba Siostaim agus suidhich *Dì-bhugachadh an t-Siostaim* gu *Chan eil*.
3.  Tagh an taba Frithealaiche agus suidhich *Aithris Mhearachdan* gu *Bun-roghainn an t-Siostaim*.
4.  *Sàbhail & Dùin*.
5.  Thoir air falbh an Neach-cuideachaidh Phuist an Fhòraim.

Thèid ceadan *configuration.php* a shuidheachadh gu leughadh a-mhàin (444 no *r--r--r--*) 
nuair a thèid am foirm Rèiteachaidh Chruinneil a shàbhaladh. Chan eil feum air seo
a dhèanamh le làimh.

*Air eadar-theangachadh le openai.com*