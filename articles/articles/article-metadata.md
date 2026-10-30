<!--
{
    "source": "https://docs.joomla.org/J6.x:_Article_Metadata",
    "title": "Artaigil: Deasaich - Meata-d\u00e0ta",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Is e fiosrachadh mu dhuilleag-lìn a th’ ann am meata-dàta, agus tha e ri
lorg anns a’ chiad phàirt den duilleag eadar na tagaichean `<head>...</head>`.
Chan fhaic luchd-tadhail na làraich a’ mhòr-chuid den fhiosrachadh seo, ach
bidh einnseanan-luirg ga chleachdadh gus toraidhean iomchaidh a thoirt seachad
airson iarrtasan luirg. Mar sin, tha e nad ùidh fhèin meata-dàta fiosrachail a
chleachdadh.

Tha cuid de na nithean meata-dàta air an solarachadh leis an teamplaid a thathar
a’ cleachdadh agus chan fheum thu an suidheachadh thu fhèin. Eisimpleirean
cumanta:

```html
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="generator" content="Joomla! - Open Source Content Management">
```

Tha cruthan eile de mheata-dàta ann, leithid Dàta Open Graph a chleachdas
Facebook agus sgeamachan a thathar a’ cleachdadh gus seòrsachan sònraichte de
dhuilleagan a mhìneachadh, leithid Pearsa, Àite no Bathar. Chan eil iad sin air
an còmhdach an-seo.

Is iad na nithean meata-dàta a thathas gu tric a’ dearmad **Tiotal** na
duilleige, a tha am broinn nan tagaichean `<title>...</title>` ann an
`<head>` na duilleige, agus **Tuairisgeul** na duilleige, a tha am broinn
tagaichean `<meta>` ach a dh’fhaodadh a bhith às-làthair. Tha iad air an
còmhdach an-seo.

## Tiotal na duilleige

Tha feum air tiotal artaigil airson duilleag ùr sam bith. Seo beagan
stiùiridhean is mholaidhean airson tiotalan matha a sgrìobhadh bho Lìonra
Luchd-leasachaidh Mozilla:

>* Seachain tiotalan le aon fhacal no dà fhacal. Cleachd abairt thuairisgeulach, no paidhir teirm-mhìneachaidh airson duilleagan fhaclair no duilleagan ann an stoidhle iomraidh.
>* Mar as trice, seallaidh einnseanan-luirg mu na ciad 55–60 caractaran de thiotal duilleige. Dh’fhaodadh gun tèid teacsa às dèidh sin a chall, mar sin feuch nach bi tiotalan nas fhaide na sin agad. Ma dh’fheumas tu tiotal nas fhaide a chleachdadh, dèan cinnteach gu bheil na pàirtean cudromach nas tràithe agus nach eil dad riatanach sa phàirt den tiotal a tha dualtach a bhith air a leigeil seachad.
>* Na cleachd “cnapan-fhaclan-luirg”. Ma tha an tiotal agad dìreach na liosta fhaclan, bidh algairim gu tric a’ lùghdachadh suidheachadh na duilleige agad ann an toraidhean an luirg.
>* Feuch ri dèanamh cinnteach gu bheil na tiotalan agad cho sònraichte ’s a ghabhas taobh a-staigh na làraich agad fhèin. Faodaidh tiotalan dùblaichte — no cha mhòr dùblaichte — cur ri toraidhean luirg mearachdach.

Molaidhean a bharrachd bho Google:

>- Sònraich tiotal sònraichte airson gach duilleag
>- Dèan an tiotal agad tuairisgeulach air susbaint na duilleige, agus goirid
>- Seachain lìonadh le faclan-luirg (a’ cleachdadh fhaclan coltach ri chèile a-rithist ’s a-rithist, leithid “Foobar,
  foo bar, foobars, foo bars”)
>- Seachain tiotalan coitcheann a chleachdadh — bu chòir tiotal sònraichte a bhith aig gach duilleag,
  agus bu chòir dha ùrachadh gu beothail a rèir an t-susbaint a tha ga shealltainn
>- Dèan branndadh air na tiotalan agad, ach dèan sin gu pongail agus a rèir an t-susbaint
  a thathar a’ frithealadh

Tha diofar Innealan Maighstir-lìn ann a ghabhas cleachdadh gus faighinn a-mach a
bheil duilgheadasan ann leis na liostaichean agad ann an einnsean-luirg
sònraichte — is fhiach daonnan aire a thoirt do dhuilgheadasan sam bith agus
an ceartachadh. Seo aon eisimpleir:

[Artaigil taic Google mu bhith a’ cleachdadh thiotalan airson nan duilleagan-lìn agad](http://support.google.com/webmasters/bin/answer.py?hl=en&amp;answer=35624)

### Prìomhachasan Tiotal na Duilleige

Ann an Joomla, tha Tiotal na Duilleige meata-dàta a thathar a’ cleachdadh anns
a’ cheann agus a tha air a thaisbeanadh ann an taba a’ bhrabhsair a’ tighinn
bho aon de na stòran a leanas, san òrdugh seo:

1. Nì a’ Chlàr-thaice > Taisbeanadh na Duilleige > Tiotal Duilleag a’ Bhrabhsair (ma tha e air a shuidheachadh san fhoirm)
2. Artaigil > Roghainnean > Tiotal Duilleag a’ Bhrabhsair (ma tha e air a shuidheachadh san fhoirm)
3. Tiotal an Artaigil (airson aon artaigil gun nì clàr-taice)
4. Tiotal Nì a’ Chlàr-thaice (airson duilleag cho-dhèanta leithid *Artaigilean Sònraichte*
no *blog Roinn-seòrsa*)

Mar sin, feumaidh tu beagan smaoineachaidh a chur ann an sgrìobhadh
thiotalan agus tiotalan dhuilleagan matha, thuairisgeulach, airson gach cuid
artaigilean agus nithean clàr-taice.

## Tuairisgeul na duilleige

Tha *Tuairisgeul Meta* an artaigil na raon ann an taba *Foillseachaidh* foirm
inntrigidh dàta an artaigil:

![Taba foillseachaidh foirm deasachaidh an artaigil](../../../gd/images/articles/article-metadata/01-articles-edit-publishing-tab.png)

Mura h-eil tuairisgeul meata-dàta aig an artaigil, thèid tuairisgeul
meata-dàta nì clàr-taice aon artaigil a chleachdadh ma tha e air a shuidheachadh.
Mura h-eil tuairisgeul meata-dàta aig nì a’ chlàr-thaice, thèid tuairisgeul
meata na làraich uile-choitcheann a chleachdadh ma tha e air a shuidheachadh.
Air neo, thèid raon tuairisgeul a’ mheata-dàta fhàgail às.

Tha Google a’ moladh na leanas gus dèanamh cinnteach gum faigh thu a’ chuid as
motha às an inn-seòrsachadh le einnsean-luirg:

>- Dèan cinnteach gu bheil tuairisgeulan meta sònraichte, iomchaidh aig gach duilleag
>- Dèan cinnteach gu bheil thu a’ cur meata-dàta an sàs airson duilleagan liostaidh (m.e. cruthan bloga agus liostaichean)
  a bharrachd air artaigilean fa leth — bithear gu tric a’ dearmad seo air
  làraichean-lìn Joomla!
>- Gabh a-steach fiosrachadh fìrinneach ma tha e iomchaidh (m.e. dh’fhaodadh artaigilean bloga
  an t-ùghdar a ghabhail a-steach, agus dh’fhaodadh bathar a’ phrìs no an neach-dèanamh a ghabhail a-steach)
>- Beachdaich air meata-dàta a ghineadh gu fèin-obrachail a chleachdadh — ach dèan cinnteach gu bheil e
  iomchaidh, furasta a leughadh agus ceart.
>- Dèan na tuairisgeulan agad tuairisgeulach!

Iomradh eile:

[Artaigil taic Google mu bhith a’ cleachdadh meata-dàta](http://support.google.com/webmasters/bin/answer.py?hl=en&amp;answer=35624)

## Faclan-luirg

Uair a bha siud, bhiodh Einnseanan-luirg a’ cleachdadh fhaclan-luirg gus
susbaint a sheòrsachadh. Mar sin, bhiodh ùghdaran a’ lìonadh am meata-dàta
fhaclan-luirg le àireamhan mòra de dh’fhaclan-luirg, an dòchas an rangachadh
SEO aca àrdachadh. Mar fhreagairt, sguir Google de bhith a’ cleachdadh
fhaclan-luirg airson adhbharan rangachaidh. Rannsaich an lìon airson comhairle
agus gheibh thu cuid de stòran ag ràdh nach fhiach dragh a ghabhail agus cuid
eile ag ràdh gu bheil luach aca fhathast. 

Cha chleachd cridhe Joomla faclan-luirg. Ma tha teagamh ort, na gabh dragh
mun deidhinn.

## Roboidean

Chan eil luach bunaiteach *Use Global* a’ cur taga meata a-steach do bhann-cinn na duilleige HTML.
Nì luachan eile sin. Tha faidhle `robots.txt` ann am freumh làrach Joomla. 
Ma tha thu airson smachd a chumail air roboidean, bu chòir dhut am faidhle seo a leughadh. Tha mìneachadh ann
air mar a chleachdas tu e

## Ùghdar

Dh’fhaodadh tu ainm foirmeil an Ùghdair a chur a-steach gus nochdadh mar mheata-dàta. 

## Còraichean

Dh’fhaodadh tu brath dlighe-sgrìobhaidh a chur a-steach gus nochdadh mar mheata-dàta.

## Eisimpleir de mheata-dàta

Seo mar a tha am meata-dàta a’ coimhead ann an sealladh tùs an artaigil:
Seo eisimpleir de shusbaint a’ `<head>` às dèidh crìoch a chur air na raointean meata-dàta uile:

```html
    <meta charset="utf-8">
    <meta name="rights" content="Charles Darwin © 1859">
    <meta name="author" content="Charles Darwin">
    <meta name="robots" content="noindex, nofollow">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="Publicity for The Origin of Species.">
    <meta name="generator" content="Joomla! - Open Source Content Management">
    <title>Publicity</title>
```

Thoir fa-near nach eil an raon toraidh airson prìomh-fhaclan ann. 

*Air eadar-theangachadh le openai.com*