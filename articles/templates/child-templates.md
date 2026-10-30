<!--
{
    "source": "https://docs.joomla.org/J4.x:Child_Templates",
    "title": "Teamplaidean Chloinne",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Cleachdaidh teamplaidean chloinne na faidhlichean uile de na teamplaidean
phàrant aca ach a-mhàin faidhlichean leis an aon ainm a chuireas tu san
teamplaid chloinne. Chan eil ùrachaidhean Joomla a’ toirt buaidh air
faidhlichean teamplaidean chloinne. Mar sin, dh’fhaodadh tu am faidhle
index.php agad fhèin a chur ann an teamplaid chloinne agus toirt air
rudeigin gu tur eadar-dhealaichte a lìbhrigeadh seach an teamplaid
bhunaiteach, leithid ionadan mhodalan a bharrachd no tar-sgrìobhaidhean
eile airson leudachain.

Smaoinich air an t-suidheachadh a leanas: canaidh sinn gu bheil thu ag
iarraidh gun nochd cuid de na duilleagan agad le cuspair gorm, dathan
bunaiteach Cassiopeia, agus duilleagan eile le cuspair uaine. ’S e dòigh
shìmplidh air sin a dhèanamh teamplaid chloinne a chleachdadh a
chleachdas an duilleag-stoidhle user.css aige fhèin,

## Eisimpleir cheum air cheum

A’ tòiseachadh bho **Siostam → Pannal nan Teamplaidean → Teamplaidean na Làraich**

- Tagh *Mion-fhiosrachadh agus Faidhlichean Cassiopeia*.
- Tagh am putan *Cruthaich Teamplaid Chloinne*.
- Lìon a-steach còmhradh priob-uinneig Teamplaid Chloinne agus tagh am
  putan Cruthaich Teamplaid Chloinne:

![foirm cruthachaidh modal teamplaid chloinne](../../../en/images/templates/child-templates/01-child-templates-create-green.png)

Tha e coltach nach eil taghadh Cassiopeia - Bun-roghainn anns an raon
Stoidhlichean Teamplaid a Bharrachd riatanach (an e mearachd a tha seo?).

- Tagh *Dùin* bhon Chrann-inneal gus foirm na teamplaide pàrant a dhùnadh.
- Tagh an teamplaid ùr, *Mion-fhiosrachadh agus Faidhlichean Cassiopeia_green*,
  bhon liosta Teamplaidean.

Aig an ìre seo tha structar phasganan ann ach dìreach aon fhaidhle:
templateDetails.xml. Faodar am faidhle sin atharrachadh ma thogras tu
taobhan de rèiteachadh na teamplaide atharrachadh, mar eisimpleir ionadan
teamplaide a chur ris no a thoirt air falbh.

### Cruthaich faidhle user.css

- Tagh am putan *Faidhle Ùr* sa Chrann-inneal.
- Anns an fhoirm *Cruthaich no Luchdaich suas faidhle ùr* dèan cinnteach gun
  tagh thu am pasgan `css`
- Lìon a-steach ainm an fhaidhle le `user`. NA cuir iar-leasachan ris!
- Tagh an Seòrsa Faidhle `.css`.
- Tagh am putan *Cruthaich*.

![foirm cruthachaidh user css na teamplaide chloinne](../../../en/images/templates/child-templates/02-child-templates-create-green-user-css.png)

Tha am faidhle user.css falamh, deiseil dhut airson stoidhlichean gnàthaichte
a chur a-steach. Cuir a-steach na leanas gus tòiseachadh air a’ chuspair
uaine:
```css
    .container-header {
      background-color: darkgreen;
      background-image: none;
    }
    h1, h2, h3, h4, h5, h6 {
      color: darkgreen;
    }
    .h1, .h2, .h3, .h4, .h5, .h6 {
      color: darkgreen;
    }
    a, a:hover, a:focus {
      color: darkgreen;
    }
    .btn-info {
        background-color: darkgreen;
        border-color: #30638d;
        color: #fff;
    }
    .btn-primary, .btn-primary:focus, .btn-primary:hover {
        background-color: darkgreen;
        border-color: var(--cassiopeia-color-hover);
    }

    .btn-check:focus + .btn-info, .btn-info:focus, .btn-info:hover {
        background-color: darkgreen;
        border-color: #264f71;
        color: #fff;
    }
```

Dh’fhaodadh gum feum thu tilleadh chun fhaidhle user.css seo gus barrachd
stoidhlichean a chur ris nas fhaide air adhart.

- Tagh *Sàbhail agus Dùin no, fa leth, *Sàbhail* agus an uair sin *Dùin am
  Faidhle*.
- Tagh *Dùin* gus am foirm Gnàthaich a dhùnadh.

### Nì Clàr-taice

Aig an ìre seo tha feum air nì clàr-taice gus feum a dhèanamh den teamplaid
chloinne. Tha an Prìomh Chlàr-taice ann an stàladh ùr de Joomla 4 ann an
ionad bàr-taoibh na làimhe deise le aon nì ann. Tha sin coltach ri àite
math airson nì clàr-taice ùr.

- Tagh **Clàran-taice → Prìomh Chlàr-taice** bho chlàr-taice an Rianaire.
- Tagh am putan *Ùr* bhon Chrann-inneal.
- Cuir a-steach tiotal iomchaidh; tha *Artaigilean Sònraichte Uaine* iomchaidh
  sa chùis seo.
- Tagh am putan **Seòrsa Nì Clàr-taice → Tagh**.
- Tagh seòrsa nì clàr-taice bho chòmhradh priob-uinneig Seòrsa Nì Clàr-taice -
  Artaigilean Sònraichte san eisimpleir seo.
- Tagh *cassiopeia_manual - Bun-roghainn* bhon raon foirm *Stoidhle na
  Teamplaide*.

![foirm deasachaidh nì clàr-taice na teamplaide chloinne](../../../en/images/templates/child-templates/03-child-templates-create-green-menu-item.png)

- Airson adhbharan na glac-sgrìn a leanas, chaidh Cruth Bloga a shuidheachadh
  gu Artaigilean Bheò: 0, Artaigilean Ro-ràdh: 3 agus Stiùir Ioma-cholbh:
  Tarsainn.

### Sealladh na Làraich

- air duilleag-dhachaigh na làraich agad, tagh an nì clàr-taice a chaidh
  a chruthachadh às ùr.

![làrach a’ sealltainn teamplaid cuspair uaine gnàthaichte](../../../en/images/templates/child-templates/04-child-templates-green-site-result.png)

### Deasaich an Stoidhle

- Tagh **Siostam → Pannal nan Teamplaidean → Stoidhlichean Teamplaidean na
  Làraich** bho chlàr-taice an Rianaire.
- Tagh *Cassiopeia_green - Bun-roghainn* bhon liosta Stoidhlichean.
- Atharraich Ainm na Stoidhle gu *Cassiopeia Uaine*. Bidh sin dìreach a’
  sgioblachadh an ainm mar a nochdas e ann an liostaichean.
- Tagh *Sàbhail agus Dùin*.

*Air eadar-theangachadh le openai.com*