<!--
{
    "source": "https://docs.joomla.org/J4.x:Article_Check-out_and_Check-in",
    "title": "Artaigil: Sgr\u00f9dadh a-steach",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Tha iomadh neach-cleachdaidh aig mòran de làraichean-lìn Joomla aig a bheil cead
artaigilean a dheasachadh. Gus casg a chur air dithis neach-cleachdaidh bho bhith a’
feuchainn ris an aon artaigil a dheasachadh aig an aon àm, tha raon stòr-dàta
**checked_out** aig gach artaigil gus sealltainn a bheil e ga chleachdadh no nach eil.
Tha e air a shuidheachadh nuair a thèid artaigil fhosgladh airson deasachadh agus air
a dhì-shuidheachadh nuair a dhùinear am foirm deasachaidh le bhith a’ cleachdadh an
phutan *Sàbhail & Dùin* no *Dùin*.

Uaireannan chan eil foirm deasachaidh artaigil air a dhùnadh mar bu chòir, mar eisimpleir
le bhith a’ cleachdadh putan air ais a’ bhrabhsair no nuair a thig seisean an neach-cleachdaidh
gu crìch. Anns a’ chùis seo, tha an raon checked_out fhathast air a shuidheachadh. Tha seo
air a chomharrachadh ann an liostaichean nan artaigilean le ìomhaigheag bheag de ghlas-uisge.
Chithear an ìomhaigheag ghlas-uisge cuideachd far am bu chòir ceangal deasachaidh a bhith ann
nuair a tha thu air logadh a-steach air aghaidh na làraich.

Gus obrachadh àbhaisteach ath-stèidheachadh, feumar nithean a chaidh a sgrùdadh a-mach a
sgrùdadh a-steach.

## Sgrùdadh a-steach artaigil

Tha grunn dhòighean rim faighinn gus artaigil a sgrùdadh a-steach.

- Mas e thusa an neach mu dheireadh a dheasaich an artaigil, bidh e comasach dhut
  an artaigil a dheasachadh bhon chùlaibh no bhon aghaidh gun fheum air
  sgrùdadh a-steach.
- Cuir fios chun neach mu dheireadh a dheasaich an artaigil gus faighinn a-mach
  a bheil iad deiseil leis. Faodaidh tu an cursair a chur thairis air a’ ghlas-uisge
  agus seallaidh an uinneag-iùil pop-up ainm an neach-cleachdaidh a rinn sgrùdadh
  a-mach air an artaigil.
- Mas e Super User no Rianaire a th’ annad, faodaidh tu ìomhaigheag a’ ghlas-uisge
  a thaghadh gus an nì seo a sgrùdadh a-steach.
- Faodaidh tu cuideachd grunn artaigilean a thaghadh agus an nì *Sgrùdadh a-steach* a
  chleachdadh bhon phutan *Gnìomhan* sa Bhàr-inneal.
- Mura h-urrainn dhut an nì a sgrùdadh a-steach thu fhèin, iarr air Super User no
  Rianaire a dhèanamh.

## Sgrùdadh a-steach cruinneil

Mas e Super User no Rianaire a th’ annad, faodaidh tu an goireas Sgrùdadh a-steach
Cruinneil a chleachdadh gus nithean a thaghadh a thèid a sgrùdadh a-steach.

Bu chòir an goireas seo a chleachdadh le fìor chùram, gu h-àraidh ann an àrainneachdan
ioma-neach-cleachdaidh. Bidh e a’ sgrùdadh a-steach gach nì a chaidh a sgrùdadh a-mach
roimhe, ge b’ e an tusa no nach tusa a rinn an sgrùdadh a-mach. Dh’fhaodadh gum bi
iomadh neach-deasachaidh ag obair air an aon sgrìobhainn aig an aon àm mar thoradh
air seo. Anns a’ chùis seo, thèid an dreach aig an neach a bhriogas air a’ phutan
sàbhalaidh mu dheireadh a shàbhaladh mar an lethbhreac dheireannach.

Bu chòir dhut cuideachd a bhith mothachail gu bheil raointean **checked_out** aig mòran
leudachain eile. Mar eisimpleir, faodar modalan agus roinnean a sgrùdadh a-mach airson
deasachadh agus am fàgail gun fhiosta san staid sin.

Bho chlàr an Rianaire:

- Tagh **Deas-bhòrd na Dachaigh → Sgrùdadh a-steach cruinneil** no
  **Siostam → Pannal cumail suas → Sgrùdadh a-steach cruinneil**.
- Tha an liosta a’ sealltainn àireamh nan nithean a chaidh a sgrùdadh a-mach.

![Duilleag sgrùdaidh a-steach cruinneil](../../../gd/images/articles/article-check-in/01-global-checkin.png)

- Bho liosta nan clàran stòr-dàta, tagh am bogsa-sgrùdaidh airson an t-seòrsa
  nithe a thèid a sgrùdadh a-steach.
- Tagh *Sgrùdadh a-steach* bhon Bhàr-inneal.

Thèid gach nì a chaidh a sgrùdadh a-mach sa chlàr sin a sgrùdadh a-steach.

## Clàran le raon checked_out

Gheibh thu a-mach dè na clàran aig a bheil colbh checked out leis a’ cheist seo
a thathar a’ cleachdadh ann am phpMyAdmin:

    SELECT DISTINCT TABLE_NAME FROM INFORMATION_SCHEMA.COLUMNS WHERE COLUMN_NAME IN ('checked_out') AND TABLE_SCHEMA='j423sd';

Agus bu chòir don toradh a bhith mar seo:

    TABLE_NAME
    bi2hb_banner_clients
    bi2hb_banners
    bi2hb_categories
    bi2hb_contact_details
    bi2hb_content
    bi2hb_extensions
    bi2hb_fields
    bi2hb_fields_groups
    bi2hb_finder_filters
    bi2hb_menu
    bi2hb_modules
    bi2hb_newsfeeds
    bi2hb_scheduler_tasks
    bi2hb_tags
    bi2hb_update_sites
    bi2hb_user_notes
    bi2hb_workflow_stages
    bi2hb_workflow_transitions
    bi2hb_workflows

*Air eadar-theangachadh le openai.com*

