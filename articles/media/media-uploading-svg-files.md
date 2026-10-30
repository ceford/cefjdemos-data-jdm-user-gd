<!--
{
    "source": "https://docs.joomla.org/J4.x:Media:_Uploading_SVG_files",
    "title": "Luchdachadh suas faidhlichean SVG",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Chan eil faidhlichean SVG (Scalable Vector Graphics) a’ faighinn taic ann an Joomla
gu bunaiteach. Tha feum air beagan cheumannan gus leigeil leis a’ cho-phàirt Meadhanan
taic a thoirt dhaibh.

## Roghainnean nam Meadhanan

Bhon chlàr Rianaire:

* Tagh **Meadhanan** bhon *Deas-bhòrd Dachaigh* no bhon chlàr *Susbaint*.
* Tagh am putan **Roghainnean** on *Bàr-innealan* Meadhanan.

Tha 3 raointean ann a dh’fheumas ùrachadh; ’s e liostaichean air an sgaradh le cromagan a th’ annta uile, mar sin chan eil agad ach cromag agus an luach iomchaidh a chur ris:

- Ann an *Leudachain Ceadaichte*, cuir ris aig deireadh na liosta a tha ri fhaighinn mar-thà:
  `,svg`.
- Ann an *Leudachain Ìomhaighean Laghail*, cuir ris aig deireadh na liosta a tha ri fhaighinn mar-thà:
  `,svg`.
- Ann an *Seòrsachan MIME Lagha*, cuir ris aig deireadh na liosta a tha ri fhaighinn mar-thà:
  `,image/svg+xml`.
- **Sàbhail & Dùin**

Bho seo a-mach, bu chòir dhut a bhith comasach air faidhlichean SVG a luchdachadh suas gu
Mhanaidsear nam Meadhanan. Mura h-eil...

## A bheil Joomla fhathast a’ cur casg air luchdachadh suas faidhlichean SVG?

Chan e cruth ìomhaigh raster a th’ ann an SVG (mar fhaidhlichean PNG, anns a bheil piogsail);
tha e sgrìobhte ann an XML (Extensible Markup Language). Tha e stèidhichte air teacsa,
faodar a chleachdadh gu dìreach taobh a-staigh an DOM (Document Object Model), faodaidh CSS
na feartan atharrachadh agus faodaidh JavaScript eadar-ghnìomhachd a chur ris.

Mar sin, tha faidhlichean SVG buailteach do gach pàtran ionnsaighe co-cheangailte ri XML:

- Sgriobtadh thar làraichean – no XSS (tro a thag `<script>` agus tachartasan).
- In-stealladh HTML (tro an eileamaid `<foreignObject>` – leigidh foreignObject
  leat eileamaidean bho raon-ainm XML eadar-dhealaichte a ghabhail a-steach).
- Diùltadh seirbheis (ma thèid an eileamaid `<xlink:href>` a mhì-chleachdadh).

A’ tòiseachadh le Joomla 4.1, thathar a’ cleachdadh inneal glanaidh gus susbaint faidhle SVG sam bith
a thèid a luchdachadh suas tro Mhanaidsear nam Meadhanan a sgrùdadh. Tha na riaghailtean teann agus
bidh iad a’ dèanamh cinnteach nach urrainn dha na faidhlichean cron a dhèanamh air an làrach. Mar sin,
dh’fhaodadh gum feum cuid de na faidhlichean a bhith air an **glanadh**
le làimh (cuimhnich gur e faidhlichean teacsa a th’ ann am faidhlichean SVG agus gun gabh an deasachadh
ann an deasaiche teacsa) no tro inneal air an taobh a-muigh mus gabh an luchdachadh suas gu soirbheachail.

**Gliocas:** glanaidh na làraichean seo faidhlichean svg a chaidh a chruthachadh ann an *Inkscape*:

* [Deuchainn Glanaidh SVG](https://svg.enshrined.co.uk/)
* [Glanadair & Optimiser SVG](https://iconly.io/tools/svg-cleaner)
* [SVGminify.com](https://www.svgminify.com/)

*Air eadar-theangachadh le openai.com*