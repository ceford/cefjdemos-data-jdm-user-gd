<!--
{
    "source": "https://docs.joomla.org/category-list-override.md",
    "title": "Seach-chur Liosta Roinne",
    "description": "Ionnsaich mar a chruthaicheas tu seach-chur teamplaide gus cruth liosta de luchd-aithne ann an roinn a leasachadh ",
    "author": ""
}
-->

## Liosta Luchd-aithne ann an Roinn

Tha cruth bunaiteach an luchd-aithne ann an roinn fo smachd teamplaide ann an còd a’ cho-phàirt 
com_contacts. Tha an cruth bunaiteach a’ coimhead mar seo:

![comataidh chultarail a’ cleachdadh a’ chruth agus an stoidhle bhunaiteach](../../../en/images/contacts/category-list-override/01-contacts-culture-committee.png)

’S dòcha gur e beachd pearsanta a tha seo, ach dhòmhsa chan eil cruth bunaiteach an neach-aithne buileach 
riarachail. Seo na duilgheadasan agam:

* Bha na dealbhan thùsail de na daoine 500 piogsail a leud agus fada ro làidir.
* Chan eil ainm an neach-aithne air a shoilleireachadh gu leòr.
* Chan eil ceann-sgrìobhadh air liosta nam puingean le fiosrachadh pearsanta agus tha coltas gun cheangal air.
* Chan eil ceann-sgrìobhadh air dreuchd an neach.
* Tha na raointean airson seòladh agus còd-puist a dhìth.
* Tha an dàta mun àite neo-choileanta.
* Tha dàta gach neach-aithne air a chur ann an clàr agus tha e caran teann air scrionaichean cumhang.

Mar sin, ciamar a shocraicheas mi e mar a thogras mi? ’S e am fuasgladh agam seach-chur 
teamplaide a chruthachadh agus stoidhlichean gnàthaichte a chur ris. Seo an toradh:

![comataidh gnìomhachais a’ cleachdadh seach-chur teamplaide agus stoidhlichean gnàthaichte](../../../en/images/contacts/category-list-override/02-contacts-business-committee.png)

## Seach-chur Cruth na Teamplaide

Tha trì faidhlichean PHP sa phasgan com_contact/tmpl/category: default.php,
default_children.php agus default_items.php. Tha cruth a’ chlàir airson na liosta anns an fhear mu dheireadh dhiubh.

Tha na faidhlichean seach-chuir air an cruthachadh tro System / Site Templates / Cassiopeia
Details and Files / Create Overrides. Tagh com_contact agus an uairsin category.
Bidh am pasgan html an uair sin a’ gabhail a-steach com_contact/category leis na trì faidhlichean
teamplaide air an deach iomradh a thoirt gu h-àrd. 

### Atharraich am faidhle default.php gu mydefault.php

Tha loidhne anns an fhaidhle `default.php` a shònraicheas dè an cruth a thèid a chleachdadh airson 
gach clàr fa leth. Tagh am faidhle seo airson a dheasachadh agus **ath-ainmich** e gu 
`mydefault.php` (no cleachd ro-leasachan sam bith a thogras tu an àite `my`). Na cleachd fo-loidhne ann an ainm an fhaidhle!

Nuair a thèid thu nas fhaide air adhart chun fhoirm Contacts / Category / Edit, leigidh an raon 
Layout air taba Options leat taghadh eadar cruth a’ cho-phàirt agus cruth do sheach-chuir.
Tha e a’ coimhead mar seo:

```
---From Global Options---
  Use Global
---From Component---
  Default
---From cassiopeia Template---
  mydefault

```

### Deasaich am faidhle mydefault.php

Tha `$this->subtemplatename = 'items';` ann an loidhne 20 de `mydefault.php`.
Atharraich `items` gu `myitems` gus am bi loidhnichean 18 gu 23 mar a leanas:

```html
<div class="com-contact-category">
    <?php
        $this->subtemplatename = 'myitems';
        echo LayoutHelper::render('joomla.content.category_default', $this);
    ?>
</div>
```

### Atharraich am faidhle default_items.php gu mydefault_myitems.php

Tha cruth gach neach-aithne anns an fhaidhle `default_items.php`. Feumar ath-ainm a thoirt air 
gus an roghainn an cruth tùsail a chleachdadh a ghlèidheadh. Chan eil a’ chiad phàirt den 
ainm cudromach. ’S e am pàirt `myitems`, air a bheil iomradh san fhaidhle
`mydefault.php`, a thèid a chleachdadh airson a’ chruth.

### Deasaich am faidhle mydefault_myitems.php

Tha an earrann `<table>...</table>` den fhaidhle seo a’ gabhail a-steach loidhnichean 85 gu 204. Airson an
seach-chur crutha, chuir mi an comharrachadh clàir an àite leis a’ chomharrachadh clèithe Bootstrap a leanas. Air scrionaichean cumhang tha na trì colbhan air an càrnadh. Air scrionaichean nas fharsainge na
768 piogsail tha na colbhan taobh ri taobh. Tha an comharrachadh ath-leasaichte air na raointean 
gnàthaichte a ghluasad fo ainm an neach-aithne.

```
<div class="container-fluid text-center border border-2">
<?php $nrows = 0; foreach ($this->items as $i => $item) : ?>
    <?php if ($item->published !== 1 ||
        (!empty($item->publish_up) && strtotime($item->publish_up) > strtotime(Factory::getDate())) ||
        (!empty($item->publish_down) && strtotime($item->publish_down) < strtotime(Factory::getDate()))) { continue; } ?>
        <div class="row cat-list-row<?php echo $nrows % 2; $nrows += 1; ?> align-items-center">
            <div class="col-12 col-md-3">
                <?php if ($this->params->get('show_image_heading')) : ?>
                    <?php if ($item->image) : ?>
                        <?php echo LayoutHelper::render(
                            'joomla.html.image',
                            [
                                'src'   => $item->image,
                                'alt'   => 'official image of ' . $item->name,
                                'class' => 'contact-thumbnail img-thumbnail',
                            ]
                        ); ?>
                    <?php endif; ?>
                <?php endif; ?>
            </div>
            <div class="col-12 col-md-3">
                <div class="parliament-committee-fields">
                <a href="<?php echo Route::_(RouteHelper::getContactRoute($item->slug, $item->catid, $item->language)); ?>">
                    <span class="fs-2"><?php echo $this->escape($item->name); ?></span>
                </a>
                    <?php echo $item->event->beforeDisplayContent; ?>
                </div>
            </div>
            <div class="col-12 col-md-6 text-start">
                <?php if ($this->params->get('show_position_headings') && !empty($item->con_position)) : ?>
                    <strong><?php echo Text::_('COM_CONTACT_FIELD_INFORMATION_POSITION_LABEL'); ?></strong><br>
                    <?php echo $item->con_position; ?><br>
                <?php endif; ?>
                <?php if ($this->params->get('show_suburb_headings')) : ?>
                    <?php $location = []; ?>
                    <?php if (!empty($item->address)) : ?>
                        <?php $location[] = $item->address; ?>
                    <?php endif; ?>
                    <?php if (!empty($item->suburb)) : ?>
                        <?php $location[] = $item->suburb; ?>
                    <?php endif; ?>
                    <?php if (!empty($item->state)) : ?>
                        <?php $location[] = $item->state; ?>
                    <?php endif; ?>
                    <?php if (!empty($item->postcode)) : ?>
                        <?php $location[] = $item->postcode; ?>
                    <?php endif; ?>
                        <strong><?php echo Text::_('COM_CONTACT_FIELD_INFORMATION_ADDRESS_LABEL'); ?></strong><br>
                    <?php echo implode("<br>\n", $location); ?><br>
                <?php endif; ?>
                <?php if (!empty($item->misc)) : ?>
                    <?php echo $item->misc; ?>
                <?php endif; ?>
            </div>
        </div>
    <?php endforeach; ?>
</div>
```

## Stoidhleadh

Faodar clasaichean stoidhle Bootstrap a mhìneachadh anns an fhaidhle `mydefault_myitems.php`.
Mar eisimpleir, thathar a’ cleachdadh `<span class="fs-2">...</span>` gus meud cruth-clò
ainm an neach-aithne àrdachadh. Faodar stoidhlichean eile a chur ris anns an fhaidhle `user.css`, mar eisimpleir,
gnàthachadh liostaichean puingean a nochdas a-mhàin taobh a-staigh taga aig a bheil clas
`contactList`.

Seo na stoidhlichean a chaidh a chur a-steach don fhaidhle user.css gus an cruth
den Chomataidh Ghnìomhachais a chithear gu h-àrd fhaighinn.

```
.contact-thumbnail {
  max-width: 200px;
  margin-right: 1rem;
}
a:has(.contact-thumbnail) {
  font-weight: 700;
  font-size: larger;
}
#contactList ul {
  list-style-type: none;
  padding-left: 0;
}
.cat-list-row0 {
  background-color: #efefef;
}
.cat-list-row0:hover, .cat-list-row1:hover  {
  background-color: #ddd;
}
div.parliament-committee-fields {
  text-align: left;
  margin-top: 1rem;
}
div.parliament-committee-fields ul.fields-container {
  list-style-type: none;
  padding-left: 0;
}
div.parliament-committee-fields ul.fields-container span.field-label {
  font-weight: 700;
}
```

*Air eadar-theangachadh le openai.com*