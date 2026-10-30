<!--
{
    "source": "https://docs.joomla.org/J3.x:Adding_custom_fields",
    "title": "Raon SQL",
    "description": " ",
    "author": ""
}
-->

## Adhbhar

Tha an raon SQL a’ solarachadh liosta a-nuas de dh’inntrigidhean a gheibhear bho
cheist stòr-dàta. Gus an raon seo a chleachdadh, feumaidh fios a bhith agad
ciamar a thogas tu ceist, agus bu chòir dhut a dhearbhadh ann am phpMyAdmin.

## Cruthachadh an Raoin

Is iad na roghainnean sònraichte taobh a-staigh an raoin seo:

- **Ioma-luachan** Leig le iomadh luach a bhith air a thaghadh. Ma tha e air a shuidheachadh gu *Tha*, seallaidh an liosta 4 nithean. Mur eil, seallaidh e 1 nì. Anns gach cùis, tha liosta fhada ann airson gluasad troimhe gus taghaidhean a dhèanamh - ma tha e air a chur an gnìomh.
- **Ceist** A’ cheist SQL a bheir seachad an dàta airson na liosta a-nuas.
Feumaidh a’ cheist dà cholbh a thilleadh; aon dhiubh air a bheil ‘value’ a chumas
luachan nithean na liosta; agus am fear eile air a bheil ‘text’ anns am bi an teacsa
san liosta a-nuas.

San eisimpleir seo, tha clàr anns a bheil liosta de dh’ainmean dhùthchannan ga chleachdadh. Seo
a’ cheist:
[[[PROTEACTED```
SELECT `id` AS value, `title` AS text
FROM `#__countrybase_countries`
WHERE `state` = 1
ORDER BY `title` ASC
```

![Cruthachadh raon SQL](../../../gd/images/fields/adding-custom-fields-sql-field/01-fields-sql-edit.png)

**Nòta:** San eisimpleir seo, tha toirt a-steach seòrsa an raoin san Tiotal airson
adhbharan taisbeanaidh a-mhàin. Fàg a-mach e sna tiotalan raoin agad fhèin.

## Inntrigeadh Dàta

Sìmplidh - tagh on liosta.

![Inntrigeadh dàta raoin SQL](../../../gd/images/fields/adding-custom-fields-sql-field/02-fields-sql-data-entry.png)

## Taisbeanadh Dàta

Tha an glacadh-sgrìn Làraich a leanas a’ sealltainn an raoin mar a nochdas e ann an artaigil. ’S e an roghainn *Taisbeanadh fèin-obrachail* a tha cunntachail airson suidheachadh an raoin, agus ’s e an teamplaid agad fhèin a tha cunntachail airson dealbhadh an raoin.

![Taisbeanadh raoin SQL air an làraich](../../../gd/images/fields/adding-custom-fields-sql-field/03-fields-sql-site.png)

’S e aon nì no liosta de nithean air an sgaradh le cromagan (ainmean dhùthchannan)
a th’ anns an toradh, a’ leantainn leubail an Raoin (Dùthaich Thùsail).

*Air eadar-theangachadh le openai.com*