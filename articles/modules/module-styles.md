<!--
{
    "source": "https://docs.joomla.org/jdocmanual?manual=user&heading=modules&filename=module-styles.md",
    "title": "Stoidhlichean Mh\u00f2idilean",
    "description": " ",
    "author": ""
}
-->

## Bun-bheachdan Stoidhle

Tha taba **Adhartach** aig foirm inntrigidh dàta mòidil. Bidh na raointean aige ag atharrachadh a rèir seòrsa a’ mhòidil agus chì thu seo dhut fhèin le bhith a’ taghadh mòideal Clàir-thaice agus ga choimeas ri mòideal Logaidh a-steach no mòideal Breadcrumbs. Chì thu na trì raointean fhoirm a leanas co-cheangailte ri stoidhle:

* Tha **Clas a’ Mhòidil** na raon teacsa a leigeas leat do chlas CSS fhèin a chur ri taga gleidhidh a’ mhòidil, mar as trice `<div>`.
* Tha **Clas a’ Bhann-cinn** na raon teacsa a leigeas leat do chlas CSS fhèin a chur ri taga a’ Bhann-chinn, taga `<h3>` a ghnàth.
* Tha **Stoidhle a’ Mhòidil** na liosta a leigeas leat aon de ghrunn stoidhlichean àbhaisteach a thaghadh. Tha an liosta a’ gabhail a-steach none, html5, outline, table, card agus noCard. ’S e card an roghainn bhunaiteach ann an stoidhlichean teamplaid Cassiopeia.

Faodaidh tu na roghainnean *Stoidhle a’ Mhòidil* fheuchainn le bhith a’ deasachadh mòidil agus ag atharrachadh an luach gus faicinn dè nì e ri taisbeanadh na làraich.

* Bheir **html5** `<div class="moduletable ">`
* Bheir **none** air an `<div>` a-muigh a thoirt air falbh gu tur agus bheir e air falbh taga `<h3>` a’ mhòidil cuideachd.
* Bheir **outline** `<div class="mod_preview_info">`, le fiosrachadh mun t-suidheachadh agus mun stoidhle a’ dol an àite taga `<h3>` a’ mhòidil.
* Bheir **table** cruth clàir a’ tòiseachadh le `<table class="moduletable ">`, agus taga `<th>` an àite an taga h3 a bh’ ann roimhe.
* Bheir **card** `<div class="sidebar-right card ">`, an roghainn bhunaiteach.
* Bheir **noCard** `<div class="sidebar-right no-card ">`

## Clas a’ Mhòidil

Aig an ìre seo feumaidh eòlas beag a bhith agad air Duilleagan Stoidhle Casgach, no CSS.
Ma chuireas tu aon fhacal ann an raon Clas a’ Mhòidil, can **green**, leis gu bheil clasaichean CSS a rèir gnàthach uile ann an litrichean beaga, agus le Stoidhle a’ Mhòidil air a shuidheachadh gu **inherited**, bidh an toradh a’ gabhail a-steach `<div class="sidebar-right card green">`.

Chan eil atharrachadh follaiseach ann an coltas na Làraich oir chan eil an clas green air a mhìneachadh. Gus a mhìneachadh, dèan inntrigeadh ann am faidhle user.css an teamplaide.

Bhon chlàr-taice Rianadair:
* Tagh **Siostam / Teamplaidean na Làraich / Teamplaidean is Faidhlichean Cassiopeia**.
* Tagh **Faidhle Ùr** on *Chrann-inneal*
* Tagh **css** sa cholbh chlì, ceann-uidhe an fhaidhle ùir.
* Sgrìobh **user** ann an raon Ainm an Fhaidhle.
* Tagh **css** o liosta Seòrsa an Fhaidhle.
* Tagh am putan **Cruthaich**.

Faodaidh tu a-nis am pasgan css fhosgladh gus am faidhle user.css a lorg agus fhosgladh airson deasachadh.
Cuir a-steach na h-aithrisean stoidhle seo agus mothaich litreachadh na SA de *color*:
```
.sidebar-right.card.green {
    background-color: #ddffdd;
}
.sidebar-right.card.green .card-body {
    background-color: #eeffee;
}
```

Dh’fhaodadh an stoidhle `.green` a-mhàin a chleachdadh, ach dh’fhaodadh sin buaidh a thoirt air tagaichean eile
leis an stoidhle sin air duilleagan eile.

## Clas a’ Bhann-chinn

Till don fhoirm deasachaidh mhòidil agus cuir **blue** ann an raon Clas a’ Bhann-chinn. Chan eil atharrachadh follaiseach air a’ mhòideal air an làrach, ach tha an ceann a-nis a’ nochdadh mar
`<h3 class="card-header blue">`. Till gus am faidhle user.css a dheasachadh agus cuir inntrigeadh ris airson stoidhle a’ chinn:
```
.card-header.blue {
    color: navy;
}
```

Tha ceann a’ mhòidil a-nis dorcha gorm. Tha grunn dhòighean ann dath a shònrachadh ann an CSS. ’S iad hexadecimal agus ainmean datha àbhaisteach na dòighean as cumanta.
Leugh a h-uile càil mu dheidhinn ann an àite eile!

## Dùbhlan CSS

* Atharraich dath crìoch a’ mhòidil gu gorm nèibhi!
* Atharraich crìoch ìosal a’ chinn cuideachd.
* Cuir an stoidhle seo an sàs ann an grunn mhodalan an àite aon aig aon àm

![Eisimpleir de Mhòideal Artaigilean Tasgaidh](../../../gd/images/modules/module-styles/01-modules-site-message.png)

*Air eadar-theangachadh le openai.com*