<!--
{
    "source": "https://docs.joomla.org/J4.x:Joomla_Standard_Font_Awesome_Fonts",
    "title": "Cruthan-cl\u00f2 nan \u00ecomhaigheagan Font Awesome",
    "description": " ",
    "author": ""
}
-->

## Ìomhaigheagan ann an teamplaidean àbhaisteach

Tha na teamplaidean àbhaisteach, Cassiopeia (làrach) agus Atum (cùlaibh), a’ tabhann seata de dh’ìomhaigheagan an-asgaidh bho Font Awesome.
Air sgàth adhbharan eachdraidheil, tha dà chlas CSS eadar-dhealaichte againn gus na h-ìomhaigheagan inntrigeadh. A bharrachd air sin, tha an clas *ro-leasachan* Font Awesome eadar-dhealaichte airson ìomhaigheagan àbhaisteach ***Joomla*** agus na h-ìomhaigheagan ***Brand***.

## Mar a chleachdas tu na h-ìomhaigheagan

### Ìomhaigheagan àbhaisteach Font Awesome

Faodar ìomhaigheagan Font Awesome a chleachdadh ann an HTML ann an gin de na riochdan a leanas:

```html
    <i class="fa fa-!name!"></i>
    <i class="fa fa-!name! large-icon"></i>
    <i class="fa fa-!name!" style="font-size: 48px;"></i>

    <span class="fa fa-!name! large-icon"></span>
```

Is fheàrr an eileamaid `<i>` leis na clasaichean na an eileamaid `<span>`!

Cuir aon de na h-ainmean ìomhaigheagan bhon liosta **FA Icons - Joomla** an àite `!name!`. Mura h-eil clas no stoidhle meud crutha-clò air a shònrachadh, bidh cruth-clò na h-ìomhaigheige aig an aon mheud ris a’ ghobhad anns a bheil e (paragraf, liosta, ceann, ...)

Tha an dearbh chlas `fa-!name!` an cois clas ro-leasachan. Tha an clas ro-leasachan `fa` goirid airson `fas`, a tha goirid airson `fa-solid`, agus faodar an tè mu dheireadh a chleachdadh na àite.

### Ìomhaigheagan Brand Font Awesome

Tha ìomhaigheagan brand Font Awesome eadar-dhealaichte bho ìomhaigheagan àbhaisteach anns a’ chiad phàirt de ainm a’ chlas, is e `fab` a th’ ann seach `fa`. 

```html
    <i style="font-size: 48px;" class="fab fa-!name!"></i>

    <span class="fab fa-!name! large-icon"></span>
```

Cuir aon de na h-ainmean ìomhaigheagan bhon liosta **FA Icons - Brands** an àite `!name!`.

’S e "fab" a th’ anns a’ phàirt ro-leasachan, goirid airson "fa-brands", agus faodar an tè mu dheireadh a chleachdadh na àite

### Ath-àiteachadh Font Awesome airson ìomhaigheagan IcoMoon

Chaidh ìomhaigheagan bho J3! (IcoMoon) a chur nan àite le fo-sheata nas lugha de dh’ìomhaigheagan Font Awesome. Faodar an cleachdadh anns na riochdan a leanas:

```html
    <i style="font-size: 48px;" class="icon-!name!"></i>

    <span class="icon-!name! large-icon"></span>
```

Cuir aon de na h-ainmean ìomhaigheagan bhon liosta **FA Icons - IcoMoon** an àite `!name!`.

’S e `icon-` a th’ anns a’ phàirt ro-leasachan (eisimpleirean `icon-calendar`, `icon-file`). Seallaidh gin de na riochdan a leanas ìomhaigheag Joomla!:

```html
    <span class="icon-joomla large-icon"></span>

    <span class="icon-joomla" style="font-size:24px;"> </span>
```

## Meud a’ chruth-chlò

Leis gur e cruthan-clò a th’ anns na h-ìomhaigheagan, faodaidh tu am meud aca a riaghladh le aithris `class` no `style` a bharrachd. Feumaidh tu an clas a mhìneachadh san fhaidhle stoidhle .css no .less agad.

## Tùsan CSS

Ann an Joomla, gheibhear na faidhlichean css anns na slighean a leanas:

Teamplaid Atum:

```
    media\templates\administrator\atum\css\vendor\fontawesome-free\fontawesome.css
```

Teamplaid Cassiopeia:

```
    media/system/css/joomla-fontawesome.css

    media/system/scss/joomla-fontawesome.scss 
```

## Ìomhaigheagan rim faighinn ann an Joomla!

Font Awesome Free 6.7.2

Faic na liostaichean fa leth airson:

- Ìomhaigheagan àbhaisteach Font Awesome Jooomla
- Ìomhaigheagan Brand Font Awesome
- Ìomhaigheagan ùra Icomoon Font Awesome
*Air eadar-theangachadh le openai.com*