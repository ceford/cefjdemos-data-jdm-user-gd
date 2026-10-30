<!--
{
    "source": "https://docs.joomla.org/J5.x:Schema_org",
    "title": "Ro-r\u00e0dh do Sgeamaichean",
    "description": " ",
    "author": ""
}
-->

## Criomagan Beairteach

’S e toraidhean rannsachaidh àbhaisteach Google a th’ ann an criomagan beairteach (ris an canar cuideachd *toraidhean beairteach*) le dàta a bharrachd air a thaisbeanadh. Mar as trice, tha an dàta a bharrachd seo air a chur ri chèile bho dhàta structaraichte a gheibhear ann an HTML duilleige. Am measg nan seòrsaichean cumanta de chriomagan beairteach tha lèirmheasan, reasabaidhean agus tachartasan. Faodaidh criomagan beairteach cuideachadh a thoirt do làraichean-lìn seasamh a-mach ann an toraidhean rannsachaidh, barrachd bhriogan a thàladh agus tuigse nas fheàrr a thoirt do luchd-cleachdaidh air an t-susbaint mus briog iad air a’ cheangal.

Bidh Joomla a’ cur an gnìomh Criomagan Beairteach a’ cleachdadh JSON-LD. ’S e seo comharrachadh JavaScript a tha freumhaichte ann an taga `<script>` ann an eileamaid `<head>` de dhuilleag HTML. Chan eil an comharrachadh measgaichte leis an teacsa a chì an neach-cleachdaidh. Tha susbaint nan criomagan air a chur a-steach ann an raointean fhoirmean a tha air an cur an gnìomh le plugain.

## Schema.org

>’S e gnìomh co-obrachail, coimhearsnachd a th’ ann an Schema.org, le rùn sgeamaichean airson dàta structaraichte a chruthachadh, a chumail suas agus adhartachadh air an Eadar-lìon, air duilleagan-lìn, ann am teachdaireachdan puist-d agus nas fhaide air falbh.

’S e cruth cunbhalach a th’ ann an dàta structaraichte airson fiosrachadh air an lìon a chur air dòigh agus a riochdachadh. Tha e a’ toirt seachad dòigh airson cunntas a thoirt air susbaint agus brìgh dàta ann an dòigh structaraichte, ga dhèanamh nas fhasa do dh’einnseanan-rannsachaidh agus do dh’aplacaidean eile am fiosrachadh a thuigsinn agus a phròiseasadh. Tha fiosrachadh nas mionaidiche ri fhaighinn air [làrach-lìn Schema.org](https://schema.org/).

## Buileachadh Joomla

Ann an Joomla, thèid Criomagan Beairteach a chruthachadh a’ cleachdadh comharrachadh dàta structaraichte stèidhichte air sgeamaichean Schema.org. Tha gach seòrsa sgeama air a chur an gnìomh mar plugan fa leth. Leigidh seo le ailtireachd nas modalaiche agus nas fhasa a leudachadh. Tha gach plugan an urra ri comharrachadh an sgeama a chruthachadh airson seòrsa sònraichte de shusbaint, a leigeas le barrachd sùbailteachd agus roghainnean gnàthachaidh. Tha seo ga dhèanamh nas fhasa do luchd-leasachaidh treas-phàrtaidh cur ri leasachadh comasan dàta structaraichte Joomla.

Gus tòiseachadh, rach gu **System -> Plugins** agus cuir an comas am plugan *System - Schema.org*. Mura bheil am plugan seo an comas, cha bhi taba Schema ann am foirm deasachaidh artaigil, fiù ’s ma tha na plugain fa leth uile an comas.

![Liosta de phlugain sgeama](../../../gd/images/schemas/introduction-to-schema-org/01-schema-plugins-list.png)

### Deasaich am plugan System - Schema.org

- **Base Type** Tagh a bheil an làrach-lìn agad a’ riochdachadh buidheann no aon neach.
- **Name** Cuir a-steach ainm na buidhne no an neach a tha an làrach-lìn a’ riochdachadh.
- **Image** Cuir ris an ìomhaigh chompanaidh no phearsanta agad
- **Social Media Accounts** Cuir ris na cunntasan meadhanan sòisealta chompanaidh no pearsanta agad. Tagh soidhne plus a’ phutain uaine gus sreathan a chur ris an fhoirm.
- Tagh **Save & Close**.

![deasaich plugan system schema org](../../../gd/images/schemas/introduction-to-schema-org/02-edit-system-schema-org-plugin.png)

### Deasaich artaigil

Rach gu gin de na h-artaigilean agad agus lìon na raointean fhoirmean Schema. Ma tha an *Schema Type* air a shuidheachadh gu *None*, an roghainn bhunaiteach, chan eil raointean ann ri lìonadh. Tagh Schema sam bith gus liosta de raointean iomchaidh fhaicinn airson an sgeama sin. Tha an dealbh-sgrìn a leanas a’ sealltainn artaigil leis an sgeama Article air a thaghadh:

![deasaich foirm sgeama artaigil](../../../gd/images/schemas/introduction-to-schema-org/03-schema-form-in-an-article.png)

### Toradh

Chan fhaic thu dad co-cheangailte ris an sgeama air an duilleag-lìn. Ach, ma choimheadas tu air tùs na duilleige, chì thu inntrigeadh sgriobt, mar anns an eisimpleir a leanas:

```json
	<script type="application/ld+json">{
    "@context": "https://schema.org",
    "@graph": [
        {
            "@type": "Organization",
            "@id": "http://localhost/jcms-testing/#/schema/Organization/base",
            "name": "Joomla Documentation Team",
            "url": "http://localhost/jcms-testing/"
        },
        {
            "@type": "WebSite",
            "@id": "http://localhost/jcms-testing/#/schema/WebSite/base",
            "url": "http://localhost/jcms-testing/",
            "name": "JCMS Testing",
            "publisher": {
                "@id": "http://localhost/jcms-testing/#/schema/Organization/base"
            }
        },
        {
            "@type": "WebPage",
            "@id": "http://localhost/jcms-testing/#/schema/WebPage/base",
            "url": "http://localhost/jcms-testing/index.php/en/article-en-gb",
            "name": "Article (en-gb)",
            "isPartOf": {
                "@id": "http://localhost/jcms-testing/#/schema/WebSite/base"
            },
            "about": {
                "@id": "http://localhost/jcms-testing/#/schema/Organization/base"
            },
            "inLanguage": "en-GB",
            "breadcrumb": {
                "@id": "http://localhost/jcms-testing/#/schema/BreadcrumbList/139"
            }
        },
        {
            "@type": "Article",
            "headline": "Article Schema Test",
            "description": "Latin text used to simulate layouts.",
            "author": {
                "@type": "person",
                "name": "Superman"
            },
            "@id": "http://localhost/jcms-testing/#/schema/com_content/article/1",
            "isPartOf": {
                "@id": "http://localhost/jcms-testing/#/schema/WebPage/base"
            }
        }
    ]
}</script>
```

Faodaidh tu an dàta structaraichte agad a dhearbhadh tro [dhuilleag Google airson an dàta structaraichte agad a dhearbhadh](https://developers.google.com/search/docs/appearance/structured-data).

## Plugain a tha rim faighinn

| Plugan | Tuairisgeul |
|--------|-------------|
| Plugan Article | An t-àite tòiseachaidh airson schema.org a chleachdadh |
| Plugan Blogposting | Airson susbaint phostaichean bhlogaichean |
| Plugan Book | Airson susbaint leabhraichean |
| Plugan Custom | Airson còd JSON-LD a chur a-steach gu dìreach |
| Plugan Event | Airson susbaint thachartasan |
| Plugan JobPosting | Airson susbaint phostaichean obrach |
| Plugan Organization | Airson susbaint chompanaidhean agus bhuidhnean |
| Plugan Person | Airson susbaint dhaoine |
| Plugan Recipe | Airson susbaint reasabaidhean |

*Air eadar-theangachadh le openai.com*