<!--
{
    "source": "https://docs.joomla.org/jdocmanual?manual=user&heading=seo&filename=seo-basics.md",
    "title": "Bun-fhiosrachadh SEO",
    "description": " ",
    "author": ""
}
-->

## Mìneachadh

Is e Leasachadh Innealan Rannsachaidh am pròiseas airson raon farsaing de fheartan làraich-lìn a leasachadh leis an amas an suidheachadh anns am bi i air a rangachadh ann an einnseanan rannsachaidh a leasachadh.

Tha pròiseas leasachadh làraich-lìn ioma-thaobhach, oir tha mòran fhactaran ann a bheir buaidh air an àite anns am faodadh duilleag a bhith air a rangachadh ann an einnsean rannsachaidh.

- Dèanamh cinnteach gu bheil structar iomchaidh aig an t-susbaint a’ cleachdadh HTML Semantic
- Leasachadh càileachd susbaint nan duilleagan fa leth.
- Dèanamh cinnteach gun urrainn don làrach-lìn iarrtasan a làimhseachadh gu luath.
- Comasachadh URLan a tha càirdeil do einnseanan rannsachaidh gus seòladh-lìn nan duilleagan a dhèanamh *so-leughaidh do dhaoine*.
- Cur ri Markup Semantic co-theacsail a’ cleachdadh dàta Schema.

Goireas: [Iùl tòiseachaidh airson Search Engine Optimization (SEO)](https://developers.google.com/search/docs/fundamentals/seo-starter-guide)

## Structar Làraich agus URLan Tuairisgeulach

Sna làithean tràtha, bha làraichean-lìn air an structaradh mar fhaidhlichean HTML fa leth ann an rangachd chraoibhe. Tha cuid de làraichean-lìn fhathast air an structaradh mar sin. Tha CMSan eadar-dhealaichte. Tha duilleagan fa leth air an cur ri chèile bho shusbaint a tha air a stòradh ann an clàran stòr-dàta. Tha na URLan airson a’ chiad seòrsa agus an dàrna seòrsa eadar-dhealaichte, ’s dòcha mar seo:

```
https://www.example.com/user/seo/seo-basics.html
https://www.example.com/index.php?option=com_jdocmanual&view=manual&manual=user&heading=seo&filename=seo-basics
```

Tha e follaiseach gu bheil a’ chiad fhear nas fhasa a chuimhneachadh agus a thaipeadh. Is fheàrr le einnseanan rannsachaidh iad.

Anns an CMS Joomla, faodar URL den chiad chruth a chur air dòigh mar a leanas:

1. Cruthaich Roinn Susbaint air a bheil **User**.
2. Cruthaich Roinn Susbaint air a bheil **SEO** agus a tha na pàiste de *User*.
3. Cruthaich artaigil agus sònraich e don roinn *SEO*.
4. Cruthaich nì clàr-taice **User** de sheòrsa **Category List*** a’ cleachdadh na roinne *User*.
5. Cruthaich nì clàr-taice **SEO** de sheòrsa **Category List** a’ cleachdadh na roinne *SEO*.
6. Suidhich comas-gnìomh SEO Joomla ann an *Global Configuration*.

Dèan deuchainn air leis an URL SEO agad: seòl tro na liostaichean User agus SEO chun na duilleige Bun-fhiosrachadh SEO. Bu chòir dha na Breadcrumbs sealltainn: `You are here: Home / User / SEO / SEO Basics`. Ach chan ann ma tha thu air nì clàr-taice de sheòrsa Single Article a chruthachadh airson *SEO Basics*!

## Lùghdaich Dùblachadh

Is e an duilgheadas le CMSan gum faodar an aon susbaint a dhèanamh ri fhaighinn le URLan eadar-dhealaichte. Anns an eisimpleir gu h-àrd obraichidh an dà URL (ach chan ann air an làrach seo), agus obraichidh `https://example.com/index.php?option=com_content&view=category&id=18&ItemID=17` cuideachd. Cha bu chòir ach aon dhiubh sin a bhith air aithneachadh le einnseanan rannsachaidh agus a shuidheachadh mar an URL **canonaigeach**. Ach dè am fear agus ciamar?

Tha am plugan **System - SEF** a’ toirt beagan cuideachaidh. Tha trì roghainnean aige:

- **Site Domain** Ma gheibhear cothrom air an làrach agad tro bharrachd air aon àrainn, cuir a-steach an àrainn as fheàrr leat (ris an canar uaireannan an àrainn chanonaigeach) an-seo. **Nota:** ’S e àrainnean eadar-dhealaichte a th’ ann an `https://example.com` agus `https://www.example.com`.
- **Strict handling of index.php** Tha an roghainn seo a’ comasachadh làimhseachadh nas teinne air `index.php` ann an URLan nuair a tha **Use URL Rewriting** air a chomasachadh ann an Global Configuration. Bheir e air falbh `index.php` ma tha URL fhathast ga chumail ann agus ath-stiùiridh e iarrtasan a thig a-steach le `index.php` chun an tionndaidh gun `index.php`.
- **Trailing slash for URLs** Cuir air Joomla gun cleachd i ach URLan le no às aonais slais dheireannaich. Nuair a thèid seo a shuidheachadh, cuiridh e an URL cheart an gnìomh le ath-stiùiridhean agus cha tèid a chur an sàs ach nuair a tha 'Add suffix to URL' à comas.

Mur eil, faic am mìneachadh air **Canonical Tags** le [Daniel Morell](https://www.danielmorell.com/blog/how-to-create-joomla-canonical-tags).

## Càileachd Susbaint

Dèan na sgrìobhas tu inntinneach agus furasta a leughadh. Tha paragrafan fada gu tric uabhasach agus doirbh an leughadh. Tha paragrafan aon-loidhne a’ coimhead ceàrr! ’S dòcha gum bu chòir dhaibh a bhith nam puingean-liosta dha-rìribh. Feuch ri paragrafan de mu thrì loidhnichean a sgrìobhadh. Leugh na sgrìobhas tu agus deasaich às faclan sam bith nach eil riatanach.

Cùm an t-susbaint agad ùraichte agus seachain fiosrachadh a chopaigeadh bho làraichean eile. Ma ghabhas e dèanamh, dearbhaich an t-susbaint agad.

### HTML Semantic

Bu chòir susbaint a bhith air a dhèanamh suas de rangachd de chinn agus pharagrafan le eileamaidean eile mar a tha riatanach (liostaichean, clàran is mar sin air adhart). Na cuir troimh-chèile air structar agus coltas — mar sin na cleachd ceann airson teacsa a dhèanamh trom no teacsa trom airson ceann a dhèanamh. Seo eisimpleir de markup semantic de artaigil:

```html
  <h2>Using headings</h2>
  <p>This is an article about the importance of headings.</p>

  <h2>Why use headings?</h2>
  <p>It is important to use headings so that search engine bots can tell what
  is an <strong>important</strong> part of your article.</p>

  <h3>Types of headings</h3>
  <p>You can use set types of headings, but they should be ordered, and
  structured, within your page.  H1 will be the page title inserted by Joomla,
  with H2 being used for sub-headings of the page.  Any headings within your
  sub-headings should cascade using H3, H4, and H5 as appropriate.</p>

  <h2>Is it hard to implement headings?</h2>
  <p>It is really easy to implement headings, you just use the appropriate
  HTML code.</p>
```

Thoir fa-near gum bi *Title* artaigil na cheann `<h1>` ma tha sin riatanach, mar sin na cleachd e ann am bodhaig artaigil.

## Dèan Smaoineachadh air Teirmean Rannsachaidh

Tagh tiotalan soilleir airson do dhuilleagan agus cinn taobh a-staigh nan duilleagan. Mar eisimpleir, mura h-eil fios agad dè th’ ann an *Semantic HTML* no ma tha thu ag iarraidh barrachd fiosrachaidh mun chuspair sin, ’s iad sin na faclan a chuireadh tu a-steach do einnsean rannsachaidh. Smaoinich air na daoine a dh’fhaodadh ùidh a bhith aca anns an fhiosrachadh a tha thu a’ toirt seachad. Dè nì iad rannsachadh air? Ach cùm Tiotalan agus Cinn gu math goirid — tha cuid de thobraichean ag ràdh gun a bhith nas fhaide na 60 caractar.

## Bi faiceallach le sanasan

Cha chuir dad stad air luchd-tadhail na làraich nas motha na sanasan a’ nochdadh an seo, an siud agus anns gach àite, agus ag gluasad an fhìor fhiosrachaidh mun cuairt fa chomhair do shùilean. Tha sanasan a dh’atharraicheas gach beagan dhiog cuideachd buaireasach agus a’ caitheamh ghoireasan an neach-cleachdaidh dheireannaich. Cleachdaidh mòran luchd-bacadh shanasan!

## Bi faiceallach le ceanglaichean

Tha ceanglaichean an dà chuid nam beannachd agus nam mallachd! Faodaidh iad buaidh mhath no dhona a thoirt air rangachadh SEO na làraich agad, a rèir a bheil ceanglaichean agad gu stòran earbsach no mì-earbsach. Agus feumar an cumail suas. Dh’fhaodadh ceanglaichean a bhith agad gu h-artaigilean taobh a-staigh no taobh a-muigh a tha air a dhol à bith, a’ taisbeanadh fiosrachadh seann-fhasanta no nach eil buntainneach tuilleadh. A’ chomhairle as fheàrr: dèan ceangal ma chuireas an targaid fìor bhuannachd ri luchd-tadhail na làraich agad, agus cleachd am feart ceangail `nofollow` mura h-eil thu airson gum bi an làrach targaid co-cheangailte ris an làrach agad.

Tha pailteas innealan sgrùdaidh cheanglaichean rim faighinn, cuid dhiubh an-asgaidh no freemium agus cuid eile pàighte, gu tric mar phàirt de sheirbheis sgrùdaidh làraich.

## Tiotal agus Tuairisgeul na Duilleige

Anns an `<head>` de gach duilleag bu chòir taga `<title>` agus taga `<description>` a bhith ann. Tha Joomla ga dhèanamh glè fhurasta tiotal eadar-dhealaichte a shuidheachadh airson gach duilleag. Gu mì-fhortanach, tha e cuideachd ga dhèanamh glè fhurasta dearmad a dhèanamh air Tiotal agus Tuairisgeul freagarrach a shuidheachadh air gach duilleag.

Mar eisimpleir, gabh duilleag liosta nan roinnean **SEO** air an deach iomradh a thoirt gu h-àrd. Tha an `<title>` ann an stòr na duilleige ag ràdh **SEO** agus tha an `<description>` a dhìth. Anns an fhoirm **Menus: Edit Item** airson an nì clàir-thaice seo, tha taba **Page Display** ann le raon **Browser Page Title**. Cuir `SEO - List of Articles` a-steach an sin agus sin a nochdas anns an taga `<title>` agus ann an taba a’ bhrabhsair.

Anns an taba **Metadata**, leis an raon **Meta Description** air a shuidheachadh gu `List of articles on Search Engine Optimisation.`, sin dìreach a nochdas anns an raon `<description>`. Bithear uaireannan a’ cleachdadh an Tuairisgeul còmhla ri Tiotal duilleige ann an toraidhean rannsachaidh, agus mar sin b’ fhiach dèanamh cinnteach gu bheil e buntainneach.

Barrachd fiosrachaidh:
* Artaigil san iris: [Tagaichean tiotail SEO Joomla](https://magazine.joomla.org/all-issues/september/joomla-seo-title-tags)
* [Rannsaich a’ Chridhe: Roghainnean SEO Dùthchasach](https://magazine.joomla.org/all-issues/june/explore-the-core-native-seo-options)

## Leasaich ìomhaighean

Gun teagamh, faodaidh ìomhaighean tarraingeach làrach a neartachadh gu mòr. Ach bidh cus ìomhaighean a tha ro mhòra a’ tàladh peanasan SEO. Seo cuid de mholaidhean:

- Cuir ìomhaighean ri taobh an teacsa a tha iad a’ mìneachadh.
- Cleachd teacsa **alt** tuairisgeulach.
- Cleachd faclan air an sgaradh le soidhne minus airson ainmean nan ìomhaighean, mar eisimpleir cat-on-hot-tin-roof.jpg.
- Cleachd an seòrsa cheart de dh’ìomhaigh airson na h-obrach: png airson postairean, jpg airson dealbhan.
- Cleachd ìomhaighean freagairteach - tha [plugan Joomla](https://responsive-images.dgrammatiko.dev/) ann a chruthaicheas tionndaidhean webp de dh’ìomhaighean png agus jpg gu fiùghantach ann an grunn mheudan.

*Air eadar-theangachadh le openai.com*