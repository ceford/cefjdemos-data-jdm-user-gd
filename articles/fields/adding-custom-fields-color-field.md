<!--
{
    "source": "https://docs.joomla.org/J3.x:Adding_custom_fields",
    "title": "Raon Dhathan",
    "description": " ",
    "author": ""
}
-->

## Adhbhar

Tha an raon Dhathan a’ toirt seachad roghnaichear airson dath a thaghadh gu lèirsinneach. Tha an raon a’ sealltainn luach hex an toraidh.

## Cruthachadh an Raoin

Roghainnean sònraichte airson an raoin:

- **Clas an Raoin** Suidhich gu *w-auto* e gus an raon a dhèanamh dìreach cho farsaing ’s a tha riatanach airson an t-sampall dhatha agus an luach.

![Cruthachadh an raoin dhathan](../../../gd/images/fields/adding-custom-fields-color-field/01-fields-color-edit.png)

**Nota:** Anns an eisimpleir seo, tha gabhail a-steach seòrsa an raoin san Tiotal airson adhbharan taisbeanaidh a-mhàin. Na cuir a-steach e ann an tiotalan nan raointean agad fhèin.

## Inntrigeadh Dàta

Faodaidh tu luach dath hex a thaipeadh ma tha fios agad gu bheil àireamhan hex a’ ruith bho 0 gu 9 agus an uair sin bho a gu f, agus gu bheil na paidhrichean àireamhan nan dearg, uaine agus gorm. Mar sin, ’s e #00ff00 gun dearg, uaine aig a’ char as motha agus gun ghorm. No faodaidh tu cùrsair a chleachdadh gus dath a thaghadh gu lèirsinneach.

![Inntrigeadh dàta an raoin dhathan](../../../gd/images/fields/adding-custom-fields-color-field/02-fields-color-data-entry.png)

## Taisbeanadh Dàta

Tha an dealbh-sgrìn Làraich a leanas a’ sealltainn an raoin air a thaisbeanadh ann an artaigil. Tha an roghainn *Taisbeanadh fèin-obrachail* cunntachail airson suidheachadh an raoin agus tha an teamplaid agad cunntachail airson dealbhadh an raoin.

’S e luach dath hex an taisbeanadh dàta bunaiteach, rud nach eil gu math feumail. ’S e am fuasgladh furasta tar-sgrìobhadh teamplaide a chruthachadh airson plugan nan raointean / color. Dìreach cuir na loidhnichean seo nan àite:
```
echo htmlentities($value);
```

leis na loidhnichean seo:
```
$value = htmlentities($value);
echo '<span style="background-color: ' . $value . ';"> ' . $value . '</span>';
```

Agus thèid an luach hex a ro-theachdaireachd le sampall dhatha aig a bheil dath cùil an luacha.

Coimhead airson an nì **Dath an Fhlùir**.

![taisbeanadh làraich an raoin dhathan](../../../gd/images/fields/adding-custom-fields-color-field/03-fields-color-site.png)

*Air eadar-theangachadh le openai.com*