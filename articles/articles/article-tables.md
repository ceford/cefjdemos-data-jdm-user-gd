<!--
{
    "source": "https://docs.joomla.org/J4.x:Article_Tables",
    "title": "Artaigil: Deasaich - Cl\u00e0ran",
    "description": " ",
    "author": ""
}
-->

## Mu Chlàran

Ann an HTML, tha clàran air an dèanamh suas de shreathan agus cholbhan de
cheallan. Mar eisimpleir, faodaidh 4 sreathan agus 4 colbhan a bhith ann an
clàr sìmplidh, a’ toirt 16 ceallan gu h-iomlan. Ach, faodar ceallan a
chothlamadh gu còmhnard no gu dìreach gus structaran clàir caran toinnte a
chruthachadh. Tha feartan aig clàran cuideachd nach eil cho follaiseach,
leithid bann-cinn, corp, bann-coise agus fo-thiotalan. Faodar clàran a
neadachadh!

Gu bunaiteach, leudaichidh ceallan clàir gus an t-susbaint aca a ghabhail
a-steach. Tha an aon stoidhleachadh a’ tighinn bho chomharrachadh a’ chlàir:
gu bunaiteach, tha teacsa trom, meadhanaichte ann an ceallan bann-cinn
(`<th>`), agus tha teacsa àbhaisteach, co-thaobhach ris an taobh chlì, ann an
ceallan dàta (`<td>`).

Bu chòir cleachdadh chlàran a bhith glèidhte airson dàta a tha dha-rìribh
tabular, leithid Clàr-ama no Mìosachan, far a bheil e cudromach structar nan
sreathan is nan colbhan a chumail suas. Cha bu chòir clàran a chleachdadh
airson cruth na duilleige, leithid ìomhaighean no teacsa a chur taobh ri
taobh.

Tha barrachd fiosrachaidh anns na h-artaigilean a leanas:

- [Bunaitean nan Clàr](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics)
- [Feartan Adhartach agus So-ruigsinneachd](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Advanced)
- [Stoidhleachadh Chlàran](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Styling_tables)

Tha clàran nan dileab! Ma chuireas tu clàr a-steach a’ cleachdadh innealan
chlàran TinyMCE, bidh an clàr a’ coimhead math air an sgrìn deasachaidh agus
air an làraich, ach tha an cruth air a choileanadh le stoidhlichean CSS
in-loidhne a dh’fhaodas a bhith lìonmhor agus doirbh a dheasachadh. Ma
chuireas tu an clàr a-steach mar HTML fìor-ghlan, chan eil an toradh a’
coimhead math ann an deasaiche teacsa TinyMCE, ach faodaidh e buannachd a
ghabhail à clasaichean Bootstrap agus coimhead fada nas fheàrr air an làraich.
Tha an dà dhòigh air an còmhdach gu h-ìosal.

## Cuir Clàr a-steach le h-Innealan TinyMCE

Gus tòiseachadh le clàr:

- Fosgail an t-artaigil a tha thu airson a dheasachadh.
- Cuir an cùrsair air loidhne bhàn far a bheil an clàr gu bhith.
- Tagh am putan *Clàr* anns a’ chiad shreath de dh’innealan TinyMCE.
- Anns a’ chlàr a tha a’ nochdadh, tagh Clàr agus gluais an cùrsair gus an
  àireamh de shreathan is cholbhan a mhìneachadh. Obraichidh na saighdean
  meur-chlàir airson seo cuideachd.
- Tagh an cealla mu dheireadh anns a’ mhaitris 4x4.
- Lìon ceallan a’ chlàir.

Roghainnean deasachaidh:

- Faodaidh tu sreath a chur a-steach os cionn no fo chealla a chaidh a thaghadh.
- Faodaidh tu colbh a chur a-steach ro no às dèidh cealla a chaidh a thaghadh.
- Faodaidh tu sreath no colbh a sguabadh às.
- Faodaidh tu crìochan nan colbhan a shlaodadh gus leud no àirde nan colbhan atharrachadh.
- Faodaidh tu ceallan a cho-aonadh - slaod thairis air na ceallan gus an taghadh agus
  an uair sin cleachd Clàr -> Cealla - > Co-aonaich ceallan.
- Faodaidh tu Feartan a’ Chlàir a thaghadh, a’ gabhail a-steach leud, stoidhle
  agus dath na crìche, agus dath a’ chùlaibh.

Ma chleachdas tu am putan Tog an Deasaiche, chì thu gu bheil an cruth air a
choileanadh le aithrisean stoidhle in-loidhne air gach sreath agus gach cealla.
Seo sampall goirid"

```html
<table style="border-collapse: collapse; width: 100%; height: 96px;" border="1"><colgroup><col style="width: 24.9735%;"><col style="width: 24.9735%;"><col style="width: 24.9735%;"><col style="width: 24.9735%;"></colgroup>
<tbody>
<tr style="height: 24px;">
<td style="height: 24px;">Day</td>
<td style="height: 24px;">Morning</td>
<td style="height: 24px;">Afternoon</td>
<td style="height: 24px;">Evening</td>
</tr>
<tr style="height: 24px;">
<td style="height: 24px;">Tuesday</td>
<td style="height: 24px;">Welcome</td>
<td style="height: 24px;">Presentations</td>
<td style="height: 24px;">BBQ</td>
</tr>
...
</tbody>
</table>
```

## Cuir Clàr a-steach mar HTML

Mas fheàrr leat, dh’fhaodadh tu cur às do stoidhlichean in-loidhne agus clasaichean
Bootstrap a chleachdadh. Dh’fheumadh tu an clàr a chruthaich innealan Clàr
TinyMCE atharrachadh, no a sgrìobhadh thu fhèin. Bhiodh e mar seo:

```html
<div class="table-responsive">
<table class="table table-striped table-bordered table-group-divider">
<thead>
<tr>
<th>Day</th>
<th>Morning</th>
<th>Afternoon</th>
<th>Evening</th>
</tr>
</thead>
<tbody class="table-group-divider">
<tr>
<th>Tuesday</th>
<td>Welcome</td>
<td>Presentations</td>
<td>BBQ</td>
</tr>
...
</tbody>
</table>
</div>
```

An seo, tha na buaidhean a leanas aig clasaichean Bootstrap:

- `table` - a’ cur grunn stoidhlichean an sàs gus cruth clàir àbhaisteach snog a thoirt seachad.
- `table-striped` - tha sreathan mu seach dorcha is aotrom.
- `table-bordered` - a’ cur crìochan an sàs air ceallan.
- `table-group-divider` - a’ cur loidhne thiugh os cionn eileamaid.
- `table-responsive` - a’ leigeil le clàr farsaing sgroladh deas is clì.

Tha an glacadh-sgrìn a leanas den Làraich a’ sealltainn clàr airson prògram
co-labhairt leis na stoidhlichean in-loidhne bunaiteach de TinyMCE, agus clàr
coltach ris le stoidhlichean Bootstrap:

![Eisimpleirean de chlàran](../../../gd/images/articles/article-tables/01-articles-site-tables.png)

Faic na sgrìobhainnean Bootstrap mu [Chlàran](https://getbootstrap.com/docs/5.3/content/tables/)
airson barrachd roghainnean.

## Smaoineachadh às dèidh làimhe

Dh’fhaodadh tu an HTML airson clàr a chur ann am modal Gnàthaichte agus am modal
sin a ghabhail a-steach san artaigil. Anns an artaigil, nochdaidh e mar
`{loadmoduleid xx}`, far a bheil xx mar ID a’ mhodail.

*Air eadar-theangachadh le openai.com*

