<!--
{
    "source": "https://docs.joomla.org/J4.x:Template_Overrides",
    "title": "Tar-\u00e0ithean Teamplaid",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Bidh leudachain Joomla a’ mìneachadh coltas an toraidh aca le faidhlichean
teamplaid, anns a bheil HTML agus comharrachadh HTML air a chruthachadh le
PHP, agus faidhlichean CSS a tha a’ mìneachadh cruth, sgeama dhathan,
cruthan-clò agus mar sin air adhart. Dh’fhaodadh sin a bhith freagarrach
gu tur do na feumalachdan agad, gu h-àraidh leis gun urrainn dhut an
coltas atharrachadh leis na stoidhlichean CSS agad fhèin. Uaireannan bidh
thu airson barrachd fiosrachaidh a shealltainn no ’s dòcha nas lugha de
dh’fhiosrachadh. Airson sin, feumaidh tu tar-àithne teamplaid a chruthachadh.

Tha teamplaidean toraidh gu math toinnte aig mòran de leudachain Joomla,
agus tha iad doirbh an leughadh. Feumaidh tu deagh thuigse air HTML, PHP
agus CSS gus dèiligeadh ri cuid dhiubh. Mar sin, tha an t-artaigil seo a’
sealltainn a’ phròiseis le bhith a’ cruthachadh tar-àithne airson an
fhoirm dì-logaidh, a tha dha-rìribh sa mhodal logaidh, mod_login. Bu mhath
le sealbhadair na làraich gun sealladh am foirm dì-logaidh an t-àm aig an
tachair dì-logadh fèin-obrachail an dèidh ùine de neo-ghnìomhachd.

## Eisimpleir: Tar-àithne teamplaid airson mod_login

Tòisich le bhith a’ taghadh **System → Templates → Site Templates** ann an
clàr-taice an Rianaire agus an uair sin tagh an nì Cassiopeia Details and Files.
Fosglaidh sin am foirm Templates: Customise (Cassiopeia):

![template customise cassiopeia site tab](../../../en/images/templates/template-overrides/01-templates-customise-cassiopeia.png)

**Cudromach:** na deasaich gin de na faidhlichean a chaidh a thoirt seachad
mar phàirt de theamplaid Cassiopeia. Aig an ath-ùrachadh Joomla dh’fhaodadh
na faidhlichean sin a bhith air an sgrìobhadh thairis agus thèid na
deasachaidhean agad a chall.

’S ann sa phasgan html a tha na tar-àithean. Ma leudaicheas tu am pasgan
html, chì thu gu bheil tar-àithean ann mu thràth airson layouts,
mod_custom, mod_menu agus tinymce. Leudaich gach fear gus faicinn dè tha
annta. Chan eil mod_login ann aig an ìre seo.

## Cruthaich Tar-àithean

Tagh an taba Create Overrides gus liosta nam Modules, Components,
Plugins agus Layouts fhaicinn airson an urrainn dhut tar-àithean a chruthachadh:

![templates customise cassiopeia overrides tab](../../../en/images/templates/template-overrides/02-cassiopeia-customisation-create-overrides.png)

Tagh an nì mod_login. Thèid na faidhlichean php teamplaid mod_login a
chopachadh dhan phasgan html agus thèid do thilleadh dhan taba Editor.
Leudaich na pasganan html agus mod_login. Chì thu default.php agus
default_logout.php.

Chan eil thu ag iarraidh am faidhle default.php oir ’s e tar-àithne airson
an fhoirm logaidh a th’ ann. Tagh e agus an uair sin am putan **Delete File**
sa bhàr-inneal. Anns a’ chòmhradh rabhaidh, dearbhaich gu bheil thu airson
am faidhle a sguabadh às.

Thoir fa-near cho furasta ’s a tha e faidhlichean a sguabadh às ma
dh’atharraicheas tu d’ inntinn. Agus leis a’ phutan Manage Folders faodaidh
tu pasganan slàn a sguabadh às cuideachd. Bi faiceallach nach sguab thu às
rudeigin nach do chruthaich thu fhèin.

## Deasaich default_logout.php

Anns an taba Editor, tagh am faidhle default_logout.php. Thoir fa-near na
putanan gu h-àrd air an làimh dheis: Show Original File agus Show Differences.
Chaidh an tè mu dheireadh a shuidheachadh gu Yes airson an ath-sgrìn, gus
loidhnichean de chòd a chaidh a chur ris faisg air mullach an fhaidhle a
shealltainn. Bidh na loidhnichean còd seo a’ tomhas cuin a thig seisean an
neach-cleachdaidh gu crìch an dèidh an duilleag anns a bheil am foirm
dì-logaidh a luchdachadh.

![templates customise cassiopeia overrides tab](../../../en/images/templates/template-overrides/03-cassiopeia-customisation-edit-logout-override.png)

Tha an raon Diff a’ sealltainn loidhnichean a chaidh a chur ris le cùl-raon
uaine agus loidhnichean a chaidh a sguabadh às le cùl-raon dearg. Chan eil
loidhnichean a chaidh a sguabadh às sa chùis seo. Tha an còd air a shealltainn
an seo air eagal ’s gum bu toil leat a chopaigeadh gus seo fheuchainn thu fhèin.

```php
    use Joomla\CMS\Factory;

    date_default_timezone_set('Europe/London');
    $config = Factory::getContainer()->get('config');
    $lifetime = $config->get('lifetime', 0);
    $time = time() + $lifetime * 60;
    $endTime = date('H:i:s', $time); // time() returns a time in seconds already
```

Nas fhaide sìos san fhaidhle tar-àithne, loidhne 36, chaidh beagan
loidhnichean eile a chur ris gus an teachdaireachd a bha thu ag iarraidh a
chur a-mach:

```html
<p class="text-center">
Your session will expire at <br><?php echo $endTime; ?>
</p>
```

Sàbhail agus ath-luchdaich duilleag na làraich anns a bheil am foirm
dì-logaidh.

![templates customise cassiopeia overrides tab](../../../en/images/templates/template-overrides/04-cassiopeia-customisation-logout-override-result.png)

Bu chòir dhut an fhoirm dì-logaidh fhaicinn ag atharrachadh gach turas a
thèid an duilleag ath-luchdachadh. Ach dè ma dh’atharraicheas tu d’ inntinn?
No ma tha roghainnean eadar-dhealaichte agad airson diofar bhuidhnean
Luchd-cleachdaidh? Fàilte gu Layouts, cuspair artaigil fa leth.

## Tar-àithean Eile

Tha taba Create Overrides an fhoirm Templates: Customise (Cassiopeia) air
a chleachdadh gus gin de na h-eileamaidean de thoradh Joomla a chruthachadh
airson a bheil e comasach tar-àithean a chruthachadh. Bidh ainmean nam
pasganan tar-àithne mar as trice a’ tòiseachadh le com\_, mod\_ no plg\_.
Thoir fa-near gu bheil an dàrna pàirt de dh’ainm pasgan tar-àithne plugain
a’ comharrachadh buidheann nam plugain. Seo eisimpleir de thaghadh de
phasganan tar-àithne:

![templates customise cassiopeia overrides tab](../../../en/images/templates/template-overrides/05-templates-customise-example-override-folder.png)

## Tar-sgrìobhaidhean Crutha

Bithear a’ cleachdadh fhaidhlichean crutha beaga gu tric airson eileamaidean fa leth de dhuilleagan Joomla! Tha am putan Leugh Tuilleadh, an ìomhaigh tòiseachaidh agus an ìomhaigh shlàn de na h-artaigilean uile nan eisimpleirean de dh’eileamaidean a tha air an gineadh leis na faidhlichean crutha aca fhèin. Gheibhear na meanbh-chruthan seo sa phasgan /layouts. Mar eisimpleir, ann an sealladh Blog na Roinne, tha am faidhle blog_item.php a’ gabhail a-steach a’ chòd gus tiotal an artaigil, ìomhaigh tòiseachaidh, teacsa tòiseachaidh, a bharrachd air diofar phàirtean buntainneach eile den duilleag, a chur an àite. Bidh e a’ dèanamh seo le bhith a’ cleachdadh gairm LayoutHelper, a’ toirt seachad a’ chruth a thèid a chleachdadh mar pharamadair. Seo eisimpleir den ghairm gus Tiotal an Artaigil a chur a-steach ann an cruth a’ bhloga:

```php
<?php echo LayoutHelper::render('joomla.content.blog_style_default_item_title', $this->item); ?>
```

Gheibhear àite an fhaidhle airson an eileamaid shònraichte seo le bhith a’ cur samhlaidhean slais an àite nan samhlaidhean dotag, a’ cur /layouts/ ris an toiseach agus .php ris an deireadh:

```php
    JOOMLAROOT/layouts/joomla/content/blog_style_default_item_title.php
```

Nuair a thèid faidhle tar-sgrìobhaidh a chruthachadh, gheibhear e ann an:

```php
    JOOMLAROOT/templates/cassiopeia/html/layouts/joomla/content/blog_style_default_item_title.php
```

## Barrachd Fiosrachaidh

- Bunaitean nan Teamplaidean
- Pasgain agus Faidhlichean Teamplaid Cassiopeia
- Gnàthachadh Teamplaid Cassiopeia
- Tar-sgrìobhaidhean Teamplaidean
- Cruthan Teamplaidean
- Teamplaid Cassiopeia Shìmplichte - Sgrùdadh Cùise - teamplaid shìmplidh stèidhichte air Cassiopeia

*Air eadar-theangachadh le openai.com*