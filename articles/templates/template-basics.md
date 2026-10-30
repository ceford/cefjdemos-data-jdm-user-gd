<!--
{
    "source": "https://docs.joomla.org/J4.x:Template_Basics",
    "title": "Bun-bheachdan nan Teamplaidean",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Ann an Joomla! ’s e cruinneachadh de fhaidhlichean a th’ ann an teamplaid
a tha còmhla a’ mìneachadh coltas na làraich-lìn. Tha Joomla 4 a’ toirt
dà theamplaid seachad: ’s e Atum an teamplaid Rianaire a thathar a’
cleachdadh airson rianachd na làraich; agus ’s e Cassiopeia an teamplaid
Làraich a thathar a’ cleachdadh le luchd-tadhail na làraich. Tha mòran
a bharrachd theamplaidean làraich rim faighinn bho sholaraichean
neo-eisimeileach, an-asgaidh no airson cosgais bheag. Gu dearbh, tha
gnìomhachas slàn stèidhichte air solar theamplaidean làraich
shònraichte.

Mar as trice tha faidhlichean PHP ann an teamplaid làraich gus an
t-susbaint a chur an dreach, agus faidhlichean CSS gus stoidhle a chur
air an t-susbaint. Gu tric bidh faidhlichean a bharrachd ann, leithid
dealbhan a thathar a’ cleachdadh san dreach agus faidhlichean
JavaScript a thathar a’ cleachdadh airson eadar-obrachadh le feartan na
làraich leithid ceanglaichean agus putanan. Tha an dealbh-sgrìn a leanas
a’ sealltainn pasganan agus faidhlichean teamplaid Cassiopeia ann an
stàladh ùr de Joomla 4:

![teamplaidean a’ gnàthachadh duilleag cassiopeia](../../../en/images/templates/template-basics/01-templates-customise-cassiopeia.png)

Thoir an aire gu bheil na faidhlichean php ann am pasgan /templates na
làraich agus na faidhlichean mheadhanan ann am pasgan /media na làraich.

## Suidheachaidhean nan Teamplaidean

Tha teamplaid na làraich a’ mìneachadh suidheachaidhean na prìomh
shusbaint, mar eisimpleir artaigil fa leth no dreach bloga de
dh’artaigilean sònraichte, agus modalan sam bith a thèid a thaisbeanadh
os cionn, fon, air an taobh chlì no air an taobh dheas den phrìomh
shusbaint. Tha an dealbh a leanas a’ sealltainn nan suidheachaidhean a
tha rim faighinn ann an Cassiopeia:

![diagram de shuidheachaidhean na teamplaid](../../../en/images/templates/template-basics/02-cassiopeia-template-positions.png)

Cuideachd, chì thu suidheachaidhean na teamplaid ann an teamplaid sam
bith le bhith a’ suidheachadh Ro-shealladh Suidheachaidhean nam
Modalan gu Comasach anns an fhoirm Teamplaid: Roghainnean, agus an uair
sin a’ cur ?tp=1 ris an URL. Ma tha sreang cheist ann mu thràth aig
deireadh an URL, cuir &tp=1 ris na àite.

## Stoidhleadh Cleachdaiche

Tha roghainnean aig Cassiopeia as urrainn dhut atharrachadh gus coltas
na làraich atharrachadh (tha artaigil air leth ann mu Ghnàthachadh
Cassiopeia). Is dòcha nach bi sin gu leòr airson na h-adhbharan agad.
Faodaidh tu na h-atharrachaidhean agad fhèin a dhèanamh air a’ choltas
le duilleag-stoidhle user.css. Feumaidh tu seo a chruthachadh thu fhèin
anns an fhoirm Teamplaidean: Gnàthachadh. Dìreach tagh Faidhle Ùr agus
cuir a-steach Ainm an Fhaidhle: user, tagh Seòrsa an Fhaidhle: .css,
agus tagh css bhon liosta phasganan. An uair sin tagh am faidhle
user.css a chaidh a chruthachadh às ùr anns an fhoirm Deasaich agus cuir
a-steach cuid de stoidhlichean, mar eisimpleir, gus cinn a dhèanamh
uaine dorcha:
```css
    h1, h2, h3, h4, h5, h6 {
      color: darkgreen;
    }
```

## Ath-sgrìobhadh Theamplaidean

A bharrachd air an dreach iomlan a tha air a mhìneachadh le teamplaid na
làraich, tha teamplaid aig gach co-phàirt no modal gus a choltas taobh a
staigh an dreach iomlain a mhìneachadh. Tha na teamplaidean sin ann am
pasgan tmpl taobh a-staigh na co-phàirte no a’ mhodail. Tha teamplaidean
aig cuid de plugain cuideachd. Agus tha dreachan ann a dh’fhaodar a
ghairm bho sheòrsa leudachaidh sam bith.

Uaireannan chan eil aon de na teamplaidean *leudachaidh* sin buileach
a’ còrdadh riut. Anns a’ chùis sin faodaidh tu ath-sgrìobhadh teamplaid
a chruthachadh. ’S e lethbhreac den chòd a thathar a’ cleachdadh gus
dreach an leudachaidh a chruthachadh a tha seo, gus an urrainn dhut
atharrachadh a rèir nan adhbharan agad fhèin. Tha an dealbh-sgrìn a
leanas a’ sealltainn an fhoirm Teamplaid: Gnàthachadh, Cruthaich
Ath-sgrìobhaidhean:

![ath-sgrìobhaidhean teamplaidean](../../../en/images/templates/template-basics/03-cassiopeia-customisation-create-overrides.png)

Tha cuid de dh’ath-sgrìobhaidhean air an stàladh mu thràth ann an
Cassiopeia. Is dòcha gum bi sin coltach ri duilgheadas. Ma dh’atharraicheas
tu gin de na faidhlichean Cassiopeia bunaiteach, thèid na h-atharrachaidhean
agad a sgrìobhadh thairis (agus mar sin caillte) aig an ath-ùrachadh de
Joomla. ’S e teamplaidean cloinne am fuasgladh.

## Dreachan Eile

Tha teamplaid, no ath-sgrìobhadh teamplaid, a’ mìneachadh coltas
leudachaidh ann am faidhle sònraichte, leithid default.php. Ann an cuid
de chùisean is dòcha gum bi thu airson taghadh eadar an dreach bunaiteach
agus dreach eile. Mar eisimpleir, mar as trice feumaidh clàr-taice ann an
suidheachadh àrd dreach eadar-dhealaichte bhon aon chlàr-taice ann an
suidheachadh taobh. Ann am modal clàr-taice tha paramadair Dreach ann
an taba Adhartach de fhoirm deasachaidh a’ mhodail, a leigeas leat taghadh
bho dhreachan eile a tha rim faighinn. Tha oideachadh air leth ann mu
Dhreachan Eile nan Teamplaidean.

## Teamplaidean Cloinne

Bidh teamplaid cloinne a’ cleachdadh nam faidhlichean san teamplaid
phàrant aige, ach a-mhàin faidhlichean sam bith a tha san teamplaid
chloinne. Mar eisimpleir, dh’fhaodadh faidhlichean user.css eadar-
dhealaichte a bhith agad sa phàrant agus sa phàiste gus am biodh sgeamaichean
dhathan eadar-dhealaichte aig diofar dhuilleagan. No dh’fhaodadh tu am
faidhle index.php a chopaigeadh bhon phàrant chun phàiste agus am pàiste
atharrachadh gus dreach eadar-dhealaichte bhon phàrant a chruthachadh.
Tha oideachadh air leth ann mu theamplaidean cloinne.

*Air eadar-theangachadh le openai.com*