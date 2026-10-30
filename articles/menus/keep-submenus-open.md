<!--
{
    "source": "https://docs.joomla.org/https:",
    "title": "Cum Fo-chl\u00e0ran Fosgailte",
    "description": " ",
    "author": ""
}
-->

Faodar modal clàr-taice a chleachdadh gus clàr-taice còmhnard a shealltainn (mar as trice aig mullach na duilleige) no clàr-taice dìreach (mar as trice ann am bàr-taoibh, clì no deas). Ann an clàr-taice còmhnard (mullach), chan eil e ion-mhiannaichte am fo-chlàr-taice a chumail fosgailte. Sin as coireach gur e giùlan bunaiteach modal clàr-taice na fo-chlàran-taice a dhùnadh nuair a luchdaichear an duilleag.

## Giùlan toglaidh na staide *fosgailte*

Ach, ann an clàr-taice dìreach (bàr-taoibh), tha e tric ion-mhiannaichte fo-chlàr-taice fhàgail fosgailte nuair a tha nì clàr-taice gnìomhach na bhroinn. Ann an Joomla 6.0, chaidh clas CSS ùr, `nav-active-open`, a thoirt a-steach gu sònraichte gus smachd a cheadachadh air co-dhiù am bi fo-chlàran-taice air am fosgladh gu fèin-obrachail nuair a luchdaichear an duilleag airson an nì clàr-taice ghnìomhaich. Le bhith a’ suidheachadh a’ chlais seo, tha e comasach seo a choileanadh a-nis. Tha an clas air a shuidheachadh sa mhodal tron cheann-uidhe rianachd.

![suidheachadh clas clàr-taice sa cheann-uidhe rianachd airson nav-active-open gus am fuirich an toglaiche fosgailte air a’ chlàr-taice ghnìomhaich](../../../gd/images/menus/keep-submenus-open/01-menu-class-setting.png)

## Mar a nì thu clàr-taice bàr-taoibh gun toglaiche tuiteam-sìos

Ma tha thu airson a h-uile fo-chlàr-taice a chumail fosgailte, chan eil feum agad air toglaiche tuiteam-sìos. An àite sin, cleachd [tar-sgrìobhadh teamplaid](jdocmanual?article=user/templates/template-overrides).

Seo mar a thèid an tar-sgrìobhadh teamplaid shònraichte seo a chruthachadh:

1. Tòisich le bhith a’ taghadh System → Templates → Site Templates ann an clàr-taice an Rianaire agus an uair sin tagh an nì Cassiopeia Details and Files. Fosglaidh seo am foirm Templates: Customise (Cassiopeia).

2. Gluais chun taba Create Overrides agus tagh mod_menu:

![taghadh tar-sgrìobhadh teamplaid modal clàr-taice](../../../gd/images/menus/keep-submenus-open/02-create-override-select-mod-menu.png)

Nì seo lethbhreac de na faidhlichean cruth uile bhon mhodal clàr-taice dhan tar-sgrìobhadh. Tillidh e an uair sin chun taba Editor.

3. Anns an taba Editor, leudaich na h-inntrigidhean fo HTML → mod_menu.  An seo gheibh thu am faidhle `default.php`. Fosgail am faidhle agus dèan lethbhreac den t-susbaint aige gu àite sàbhailte. Dùin am faidhle.

4. Cruthaich faidhle ùr sa phasgan html → mod_menu. Feumaidh ainm a bhith air nach eil fo-sgrìobhadh ann. San eisimpleir seo, ’s e `treedefault.php` ainm an fhaidhle ùir. Leigidh seo leat cruth a’ chlàr-taice bhunaich no an cruth clàr-taice eile seo a thaghadh ann am modal clàr-taice sam bith agad. Anns an liosta a leanas de fhaidhlichean tar-sgrìobhaidh, tha am fear tùsail air a chomharrachadh ann an dearg agus tha an roghainn ùr air a chomharrachadh ann an uaine.

![taba deasachaidh tar-sgrìobhaidh mod_menu - fosgail default.php](../../../gd/images/menus/keep-submenus-open/03-edit-mod-menu.png)

4. Deasaich am faidhle cruth ùr. Tha na ceumannan a leanas air an liostadh ann an òrdugh cas gus àireamhan nan loidhnichean a ghleidheadh rè a’ phròiseis deasachaidh:

Atharraich loidhne 104 gus am bi na leanas innte:

```
        echo '<ul class="list-unstyled ps-3" aria-hidden="false">';
```

Cumaidh seo an clàr-taice fosgailte agus cuiridh e beàrnan a-steach do na fo-chlàran-taice.

Cuir `break` an àite loidhnichean 98 - 101

```php
                    echo '<button class="mod-menu__toggle-sub" aria-expanded="false">' .
                 break;
                    '<span class="icon-chevron-down" aria-hidden="true"></span>' .
                    '<span class="visually-hidden">' . Text::sprintf('MOD_MENU_TOGGLE_SUBMENU_LABEL', $item->title) . '</span>' .
                    '</button>';
```

Thoir air falbh loidhnichean 93 - 94

```php
                    echo '<span class="icon-chevron-down" aria-hidden="true">' .
                        '</span></button>';
```

Thoir air falbh loidhnichean 66-71

```php
    // The next item is deeper - add toggle only here it is a heading or separator
    if ($item->deeper && (int) $item->level === $startLevel && in_array($item->type, ['separator', 'heading'])) {
        // Add a toggle button.
        echo '<button class="mod-menu__toggle-sub" aria-expanded="false">';
    }
```

Thoir air falbh loidhnichean 15 - 20

```php
/** @var Joomla\CMS\WebAsset\WebAssetManager $wa */
$wa = $app->getDocument()->getWebAssetManager();
$wa->getRegistry()->addExtensionRegistryFile('mod_menu');
$wa->usePreset('mod_menu.menu');
```

Seo am faidhle tar-sgrìobhaidh `treedefault.php` slàn:

```
<?php

/**
 * @package     Joomla.Site
 * @subpackage  mod_menu
 *
 * @copyright   (C) 2009 Open Source Matters, Inc. <https://www.joomla.org>
 * @license     GNU General Public License version 2 or later; see LICENSE.txt
 */

defined('_JEXEC') or die;

use Joomla\CMS\Helper\ModuleHelper;
use Joomla\CMS\Language\Text;

$tagId      = $params->get('tag_id', '') ?: 'mod-menu' . $module->id;
$id         = ' id="' . htmlspecialchars($tagId, ENT_QUOTES, 'UTF-8') . '"';
$startLevel = (int) $params->get('startLevel', 1);

// The menu class is deprecated. Use mod-menu instead
?>
<ul<?php echo $id; ?> class="mod-menu mod-list nav <?php echo $class_sfx; ?>">
<?php foreach ($list as $i => &$item) {
    $itemParams = $item->getParams();
    $class      = 'nav-item item-' . $item->id;

    if ($item->id == $default_id) {
        $class .= ' default';
    }

    if ($item->id == $active_id || ($item->type === 'alias' && $itemParams->get('aliasoptions') == $active_id)) {
        $class .= ' current';
    }

    if (in_array($item->id, $path)) {
        $class .= ' active';
    } elseif ($item->type === 'alias') {
        $aliasToId = $itemParams->get('aliasoptions');

        if (count($path) > 0 && $aliasToId == $path[count($path) - 1]) {
            $class .= ' active';
        } elseif (in_array($aliasToId, $path)) {
            $class .= ' alias-parent-active';
        }
    }

    if ($item->type === 'separator') {
        $class .= ' divider';
    }

    if ($item->deeper) {
        $class .= ' deeper';
    }

    if ($item->parent) {
        $class .= ' parent';
    }

    echo '<li class="' . $class . '">';

    switch ($item->type) :
        case 'separator':
        case 'component':
        case 'heading':
            require ModuleHelper::getLayoutPath('mod_menu', 'default_' . $item->type);
            break;
        default:
            require ModuleHelper::getLayoutPath('mod_menu', 'default_url');
            break;
    endswitch;

    // The next item is deeper.
    if ($item->deeper) {
        // Check type - add only on first level
        // @todo aria-label - set in menu item ???
        if ((int) $item->level === $startLevel) {
            switch ($item->type) {
                case 'heading':
                case 'separator':
                    break;

                default:
                    break;
            }
        }
        echo '<ul class="list-unstyled ps-3" aria-hidden="false">';
    } elseif ($item->shallower) {
        // The next item is shallower.
        echo '</li>';
        echo str_repeat('</ul></li>', $item->level_diff);
    } else {
        // The next item is on the same level.
        echo '</li>';
    }
}
?></ul>
```

## Toradh

’S e liosta shìmplidh a th’ anns an toradh, gun ghnìomhachd toglaiche airson modal clàr-taice na bàr-taoibh, mar a chithear an seo air an taobh chlì:

![toradh le tar-sgrìobhadh teamplaid - liosta shìmplidh gun phutanan toglaiche no gnìomhachd](../../../gd/images/menus/keep-submenus-open/05-site-result.png)

*Air eadar-theangachadh le openai.com*

