<!--
{
    "source": "https://docs.joomla.org/J3.x:Adding_custom_fields",
    "title": "Tar-sgr\u00ecobhadh Teamplaid Eisimpleir",
    "description": " ",
    "author": ""
}
-->

## Taisbeanadh Fèin-obrachail an Raoin

Tha roghainn air a bheil *Taisbeanadh Fèin-obrachail* aig gach raon a tha ri
làimh, agus faodar a shuidheachadh gu aon de na leanas:

* Às dèidh an Tiotail
* Ro Shusbaint an Taisbeanaidh
* Às dèidh Susbaint an Taisbeanaidh
* Na seall gu fèin-obrachail

Ma thèid an roghainn mu dheireadh dhiubh sin a thaghadh, cha tèid an raon a
thaisbeanadh mura cruthaich thu tar-sgrìobhadh teamplaid gus an taisbeanadh
fhèin a làimhseachadh. No dh’fhaodadh tu `{field ID}` a chur ann an artaigil
gus an raon a chur far a bheil thu ag iarraidh. Ach feumaidh tu cuimhneachadh
air seo a dhèanamh anns gach artaigil.

Tha an eisimpleir seo a’ sealltainn mar a chruthaicheas tu tar-sgrìobhadh
teamplaid airson Neach-conaltraidh. Tha na dòighean seo iomchaidh cuideachd
airson nan co-phàirtean Susbaint agus Cleachdaiche.

## Cruthaich Tar-sgrìobhadh Teamplaid

Bhon chlàr Rianaire:

* Tagh **System / Site Templates / Cassiopeia Details and Files**
* Tagh an taba **Create Overrides**.
* Tagh **com_contact** o phannal nan *Components*
* Tagh **Contact** bhon liosta de sheallaidhean a tha ri làimh. Seo cruth
  aon neach-conaltraidh.

Sa phannal **Editor**:
* Tagh **html / com_contact / contact / default.php**, ’s e seo am faidhle
  a shuidhicheas cruth iomlan duilleag an aon neach-conaltraidh.
* Sgrolaich sìos am faidhle seo agus mothaich sreath de bhlocaichean
  `<php if (...) : ?>`. Seallaidh no falaichidh gach fear earrann de theacsa a
  rèir roghainnean an neach-conaltraidh.
* Mothaich na loidhnichean anns a bheil
```
    <?php echo $this->item->event->afterDisplayTitle; ?> (line 73)
    <?php echo $this->item->event->beforeDisplayContent; ?> (line 98)
    <?php echo $this->item->event->afterDisplayContent; ?> (line 189)
```

Thèid aon de na caochladairean sin, no gin dhiubh, a lìonadh a rèir luach an
raoin Taisbeanaidh Fèin-obrachail.

## A’ cleachdadh raointean nad thar-sgrìobhadh

Tha cothrom agad air na raointean uile a bhuineas don nì làithreach tro
sheilbh `$this->item->jcfields`, a tha na shreath anns a bheil an dàta a leanas
airson gach raoin (tha an eisimpleir seo airson raon Deasaiche):

```php
    Array
    (
        [4] => stdClass Object
            (
                [id] => 4
                [title] => article-editor
                [name] => article-editor
                [checked_out] => 0
                [checked_out_time] => 0000-00-00 00:00:00
                [note] =>
                [state] => 1
                [access] => 1
                [created_time] => 2017-04-07 12:08:59
                [created_user_id] => 856
                [ordering] => 0
                [language] => *
                [fieldparams] => Joomla\Registry\Registry Object
                    (
                        [data:protected] => stdClass Object
                            (
                                [buttons] =>
                                [width] =>
                                [height] =>
                                [filter] =>
                            )

                        [initialized:protected] => 1
                        [separator] => .
                    )

                [params] => Joomla\Registry\Registry Object
                    (
                        [data:protected] => stdClass Object
                            (
                                [hint] =>
                                [render_class] =>
                                [class] =>
                                [showlabel] => 1
                                [disabled] => 0
                                [readonly] => 0
                                [show_on] =>
                                [display] => 2
                            )

                        [initialized:protected] => 1
                        [separator] => .
                    )

                [type] => editor
                [default_value] =>
                [context] => com_content.article
                [group_id] => 0
                [label] => article-editor
                [description] =>
                [required] => 0
                [language_title] =>
                [language_image] =>
                [editor] =>
                [access_level] => Public
                [author_name] => Super User
                [group_title] =>
                [group_access] =>
                [group_state] =>
                [value] => Bar
                [rawvalue] => Bar
            )
    )
```

## Taisbean an raoin

Thèid an gnìomh `FieldsHelper::render()` a chleachdadh gus gach raon a
thaisbeanadh. An toiseach, cuir aithris
`use Joomla\Component\Fields\Administrator\Helper\FieldsHelper;` ris an
liosta de na h-aithrisean `use` aig mullach faidhle an tar-sgrìobhaidh:

```php
defined('_JEXEC') or die;

use Joomla\CMS\Helper\ContentHelper;
use Joomla\CMS\HTML\HTMLHelper;
use Joomla\CMS\Language\Text;
use Joomla\CMS\Layout\FileLayout;
use Joomla\CMS\Layout\LayoutHelper;
use Joomla\CMS\Plugin\PluginHelper;
use Joomla\CMS\Router\Route;
use Joomla\Component\Contact\Site\Helper\RouteHelper;
use Joomla\Component\Fields\Administrator\Helper\FieldsHelper;
```

An uairsin, ge bith càite a bheil thu airson na raointean a chur san teamplaid
agad, cleachd an còd a leanas:
```php
<?php foreach ($this->item->jcfields as $field) : ?>
    <?php echo FieldsHelper::render($field->context, 'field.render', array('field' => $field)); ?><br>
<?php endforeach ?>
```

No airson tar-sgrìobhadh amh, nach eil ag eadar-theangachadh an leubail:

```php
<?php foreach ($this->item->jcfields as $field) : ?>
    <?php echo $field->label . ':' . $field->value; ?><br>
<?php endforeach ?>
```

## A’ luchdadh raointean fa leth

Gus raointean fa leth a chur ris an t-susbaint agad, tòisich le bhith a’
taghadh ainmean sònraichte airson nan raointean gnàthaichte agad, a’ cleachdadh
an raoin **Name**, a thèid a chleachdadh gus iomradh dìreach a thoirt air an
raon agad ann an còd an tar-sgrìobhaidh. Anns an taba `Options`, tagh **No**
anns an raon `Automatic Display` gus nach tèid a thaisbeanadh gu fèin-obrachail
ann an gin de na h-àiteachan àbhaisteach.

An uairsin, gus cothrom dìreach a chomasachadh air raointean gnàthaichte a rèir
ainm ann an tar-sgrìobhadh, cuir an còd gu h-ìosal aig toiseach an fhaidhle
agad. Bu chòir dhut seo a dhèanamh airson gach faidhle PHP tar-sgrìobhaidh
far a bheil thu airson raointean gnàthaichte fa leth a chur.

```php
<?php foreach($this->item->jcfields as $jcfield) {
    $this->item->jcFields[$jcfield->name] = $jcfield;
} ?>
```

Agus mu dheireadh, bu chòir dhut an còd airson suidheachadh an raoin a chur
anns an àite far a bheil thu airson leubail no luach an raoin a shealltainn.

Gus **leubail** an raoin a chur ris an tar-sgrìobhadh agad, cuir a-steach an
còd gu h-ìosal, agus cuir ainm an raoin an àite `name-of-field`.

```php
<?php echo $this->item->jcFields['name-of-field']->label; ?>:&nbsp;
```

Gus **luach** an raoin a chur ris an tar-sgrìobhadh agad, cuir a-steach an còd
gu h-ìosal, agus cuir ainm an raoin an àite `name-of-field`.

```php
<?php echo $this->item->jcFields['name-of-field']->rawvalue; ?>
```

Faodaidh tu an còd seo a chur ri pàirt sam bith den tar-sgrìobhadh agad.
Eisimpleirean: susbaint `div`, an `src` ann an taga `img`, taobh a-staigh
buadh clas CSS, agus mar sin air adhart.

*Air eadar-theangachadh le openai.com*