<!--
{
    "source": "https://docs.joomla.org/J4.x:Module_and_Menu_Styles",
    "title": "Stoidhlichean Mh\u00f2idealan agus Cl\u00e0ran-b\u00ecdh",
    "description": " ",
    "author": ""
}
-->

## Mu Dheidhinn Duilleagan-stoidhle CSS

Tha duilleagan làraich-lìn a chuireas Joomla! a-mach air an dèanamh suas de thagaichean HTML le buadhan stoidhle
ann an riochd aithrisean clas. Mar eisimpleir, dh’fhaodadh ceann-sgrìobhadh
taobh a-staigh artaigil a bhith `<h3 class="special-warning">Watch Out!</h3>`. 
Dh’fhaodadh an ceann-sgrìobhadh seo nochdadh ann an cruth-clò nas motha, le
dathan eadar-dhealaichte airson an teacsa agus a’ chùlaibh, agus ’s dòcha
iomall agus ìomhaigheag rabhaidh. Bhiodh na stoidhlichean clas air am mìneachadh
san fhaidhle user.css san teamplaid, mar seo:
```css
    h3.special-warning {
      color: #900;
      background-color: #fee;
      border: 1px solid #900;
      padding: 1rem;
      font-size: 2rem;
    }
```

Tha seo ag obair oir thèid an duilleag-stoidhle user.css a luchdadh mu dheireadh agus bidh
prìomhachas aig stoidhlichean sam bith a tha na bhroinn thairis air na h-aon
stoidhlichean ann am faidhlichean css a chaidh a luchdadh roimhe. Chan eil an stoidhle
`special-warning` a’ buntainn ri tagaichean `<h3>` eile, ach ris an fheadhainn aig a bheil an clas
shònraichte seo. Bidh e ag obair taobh a-staigh artaigil oir ’s ann an sin a chuireas tu ainm a’ chlas
a-steach thu fhèin.

Ach dè ma tha thu airson stoidhle a chur air modal no air duilleag slàn? Mar eisimpleir, dh’fhaodadh tu
dathan cùil eadar-dhealaichte a chur air diofar mhodalan no dhuilleagan.
No dh’fhaodadh tu stoidhle eadar-dhealaichte a chur air ceann-sgrìobhadh na duilleige aghaidh agad seach air na cinn-sgrìobhaidh
air duilleagan eile. Faodar seo uile a choileanadh le bhith a’ cur ainmean clas ris
an fhoirm deasachaidh modal no ris an fhoirm deasachaidh nì clàr-bìdh. Thèid na clasaichean stoidhle a
chur a-steach don fhaidhle user.css an uairsin.

## Stoidhlichean Mhòidealan

Tha an eisimpleir shìmplidh seo a’ cur stoidhlichean ghnàthaichte an sàs sa mhodal Log a-steach agus san
tiotal aige. Tha an dealbh-sgrìn a leanas a’ sealltainn ainmean nan stoidhlichean a chaidh a chur a-steach don
taba Adhartach den fhoirm deasachaidh Modules: Login. Chaidh Clas a’ Mhodail a shuidheachadh gu
`make-me-light-green` agus chaidh Clas a’ Chinn-sgrìobhaidh a shuidheachadh gu
`make-me-dark-green`. Thoir fa-near gun urrainn dhut soidhnichean minus no
fo-loidhnichean a chur ann an ainmean chlasaichean, ach bidh beàrnan a’ sgaradh ainmean chlasaichean eadar-dhealaichte.

![foirm deasachaidh a’ mhodail logaidh a-steach, taba adhartach a’ sealltainn clas gnàthaichte](../../../en/images/template-tips/module-and-menu-styles/01-templates-edit-module-style.png)

Tha na h-aithrisean stoidhle a leanas gan cleachdadh san fhaidhle user.css:
```css
    .make-me-light-green {
      background-color: #efe;
      border-color: darkgreen;
    }
    .make-me-dark-green {
      color: darkgreen;
      border-color: #264f71;
    }
```

Thoir fa-near don phuing (.) a thathar a’ cleachdadh ann an css gus clas leis an ainm sin a mhìneachadh.
Chan fhaodar a’ phuing a chleachdadh ann am foirm cuir a-steach dàta a’ mhodail.
Tha an toradh san eisimpleir seo mar a leanas:

![coltas na làraich leis a’ mhodal ghnàthaichte agus na h-innealan leasachaidh](../../../en/images/template-tips/module-and-menu-styles/02-templates-edit-module-style-result.png)

Tha bonn na h-ìomhaigh a’ sealltainn pannal Innealan Leasachaidh a’ bhrabhsair, leis an taga
`<div>` a tha a’ cuairteachadh modal Login air a thaghadh. Chì thu gun deach stoidhle gnàthaichte
Clas a’ Mhodail a chur ri deireadh nan stoidhlichean a bha air am mìneachadh mu thràth ann an teamplaid a’ mhodail.
Tha an ath loidhne a’ sealltainn an taga `<h3>` cuideachd, le Clas a’ Chinn-sgrìobhaidh ghnàthaichte
air a chur ri deireadh nan stoidhlichean a bha air am mìneachadh mu thràth.

’S dòcha gun còrd an stoidhle mhodail seo riut no nach còrd! Ach chan eil seo ach na leasan air
mar a nì thu e, chan ann air dè nì sgeama dathan math!

## Stoidhlichean Dhuilleagan

Tha grunn dhòighean ann gus coltas iomlan duilleige a ghnàthachadh.
Bidh iad uile ag obair tron fhoirm Clàran-bìdh: Deasaich Nì:

- Tha roghainn Stoidhle Teamplaide air an taba Mion-fhiosrachadh, às am faod thu
  teamplaid shònraichte a thaghadh airson a chleachdadh.
- Tha raointean Clas Prìomh-Artaigil agus Clas Artaigil air an taba Cruth Blog
  far an urrainn dhut ainm clas a chur a-steach.
- Tha raon Tagh Cruth air an taba Roghainnean, às am faod thu taghadh
  a dhèanamh à cruthan a tha rim faighinn airson gach nì.
- Tha raointean airson Clas Ceangail, Clas Ìomhaigheag Ceangail agus
  Clas Ìomhaigh air an taba Seòrsa Ceangail.
- Tha raointean airson Clas Duilleige air an taba Taisbeanadh Duilleige.

’S e an tè mu dheireadh san liosta seo a tha air a chòmhdach san artaigil seo. Dè
thachras le `make-me-aliceblue` air a chur a-steach san raon seo? Agus na
leanas air a chur a-steach ann an user.css:
```css
    .make-me-aliceblue {
      background-color: aliceblue;
    }
```

Thèid an clas a chur ri taga body na duilleige:

![coltas na làraich leis an duilleag ghnàthaichte agus na h-innealan leasachaidh](../../../en/images/template-tips/module-and-menu-styles/03-templates-edit-page-class-result.png)

*Air eadar-theangachadh le openai.com*

