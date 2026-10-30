<!--
{
    "source": "https://docs.joomla.org/J5.x:Add_a_class_selector_to_the_create_link_dialog",
    "title": "Artaigil: Deasaich - Stoidhlichean Cheanglaichean",
    "description": " ",
    "author": ""
}
-->

## Tuairisgeul

Leigidh clasaichean cheanglaichean gnàthaichte a chuirear ri roghainnean deasaiche TinyMCE leat ceangal artaigil atharrachadh gu luath gu putan no buaidhean lèirsinneach eile a chur ris gun fheum air còd HTML atharrachadh gu dìreach.

### Ceumannan gus an Taghadh Chlasan a Chleachdadh

1. Bhon Deas-bhòrd Dachaigh, rach gu liosta nam Plugan agus lorg am plugan TinyMCE.
2. Fosgail am plugan TinyMCE agus, leis an taba Plugain air a thaghadh, sgrolaich sìos gu bonn na duilleige.
3. Cuir clasaichean ris an *Liosta Chlasan Cheanglaichean*. Mar eisimpleir, clasaichean Bootstrap gus putanan eireachdail a chruthachadh. Is dòcha gum feum thu an liosta a sgroladh bho chlì gu deas no meudachadh sgrion atharrachadh gus na putanan cuir ris, thoir air falbh agus òrduich fhaicinn aig an deireadh.
4. Sàbhail & Dùin.

![Suidhich clasaichean cheanglaichean ann an tinymce](../../../gd/images/articles/article-link-styles/01-article-edit-link-style-tinymce.png)

Gheibh thu eisimpleirean de theamplaidean a chleachdas Bootstrap gu dùthchasach ann an [Sgrìobhainnean Oifigeil Bootstrap](https://getbootstrap.com/docs/5.3/components/buttons/)

Seo cuid de chlasaichean as urrainn dhut a chleachdadh airson caochlaidhean phutanan Bootstrap:

- `btn btn-primary` airson putan bun-sgoile
- `btn btn-secondary` airson putan àrd-sgoile
- `btn btn-success` airson putan soirbheachais
- `btn btn-danger` airson putan cunnartach
- `btn btn-warning` airson putan rabhaidh
- `btn btn-info` airson putan fiosrachaidh
- `btn btn-light` airson putan aotrom
- `btn btn-dark` airson putan dorcha
- `btn btn-link` airson putan ceangail

#### Roghainnean Eile airson Putanan le Oirean

Faodaidh tu cuideachd na caochlaidhean de phutanan le oirean a chleachdadh:

- `btn btn-outline-primary` airson putan bun-sgoile le oir
- `btn btn-outline-secondary` airson putan àrd-sgoile le oir
- … (msaa.)

#### Airson meudan phutanan, cuir na clasaichean seo ris

- `btn-lg` airson putan mòr
- `btn-sm` airson putan beag

**Eisimpleir:** `btn btn-dark btn-lg` (putan dorcha mòr)

## Cruthaich ceangal ann an artaigil

1. Fosgail artaigil agus tagh teacsa, facal no abairt, airson ceangal a chruthachadh.
2. Tagh an ìomhaigheag Ceangail a nochdas nuair a thaghas tu teacsa.
3. Cuir a-steach URL a’ cheangail.
4. Aig bonn a’ chòmhraidh airson ceangal a chruthachadh, tagh aon de na clasaichean rèitichte.
5. Sàbhail an Ceangal.
6. Sàbhail an Artaigil.
7. Ro-sheall an Artaigil

![Cuir stoidhle cheangail an sàs ann an artaigil](../../../gd/images/articles/article-link-styles/02-article-edit-link-style-apply.png)

Agus seo eisimpleir far an deach clas a’ Phutain Cheangail a shuidheachadh gu `btn btn-sm btn-outline-info` agus ’s e *Bootstrap* an teacsa ceangailte:

![Ro-shealladh de Phutan Ceangail gnàthaichte](../../../gd/images/articles/article-link-styles/03-article-edit-link-style-preview.png)

## Cleachdadh Adhartach: A’ Cur Clasaichean Gnàthaichte an Sàs

Chan eil am feart seo cuingealaichte ri clasaichean Bootstrap. Faodaidh tu cuideachd na clasaichean CSS gnàthaichte agad fhèin a chur an sàs airson feumalachdan sònraichte. Mar eisimpleir, faodaidh tu ìomhaigheag a chur ron cheangal le buaidh nuair a thèid an luchag thairis air. Nì seo e furasta stoidhle a chur air ceanglaichean gun fheum air còd tùsail an artaigil atharrachadh.
*Air eadar-theangachadh le openai.com*