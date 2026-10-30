<!--
{
    "source": "https://docs.joomla.org/J4.x:Fix_%22Database_Table_Structure_NOT_Up_to_Date%22_before_Update",
    "title": "Structar Cl\u00e0ir an St\u00f2r-d\u00e0ta",
    "description": " ",
    "author": ""
}
-->

## Mearachdan a chaidh aithris

Nuair a bhios tu ag ùrachadh Joomla!, feumaidh structar clàir an stòir-dhàta
a bhith ùraichte mus tòisich am pròiseas. Bidh an *Sgrùdadh ro-ùrachaidh airson
Joomla* a’ gearain mura h-eil seo fìor.

Ach nuair a thèid thu gu **Siostam → Cumail suas → Stòr-dàta**, chan eil
inntrigeadh ri fhaighinn. Chaidh seo aithris ann an grunn dhreachan de Joomla! 4.x.

## Dè an t-Adhbhar

Tha an duilgheadas air adhbhrachadh le clàr `#__schemas` falamh san stòr-dàta. As
coltaiche, bidh seo a’ tachairt nuair nach eil an t-eisimpleir de Joomla! air a
stàladh leis an stàlaichear oifigeil Joomla!, ach tro sgriobt gnàthaichte nach do
lìon a-steach an dàta riatanach gu lèir.

## Mar a shocraicheas tu

Faodaidh tu seo a chàradh le bhith a’ cur an luach a tha a dhìth ris a’ chlàr. A’ cleachdadh phpMyAdmin
(no cliant stòir-dhàta eile), rach don chlàr `#__extensions`. Rannsaich airson
name='files_joomla' agus sgrìobh sìos an extension_id (anns a’ chùis againn *211*).

An ath rud, feumaidh fios a bhith agad dè an sgriobt SQL as ùire a chaidh a stàladh. Rach gu
`administrator/components/com_admin/sql/updates/mysql` agus faigh ainm an fhaidhle leis an
tionndadh as àirde. San eisimpleir seo, gabh ris gur e
*4.0.3-2021-09-05.sql* ainm an fhaidhle leis an tionndadh as àirde. A-nis feumaidh tu
seo a chur ris a’ cheist insert agad mar an dàrna luach:

    INSERT INTO `#__schemas` (`extension_id`, `version_id`) VALUES
    (211, '4.0.3-2021-09-05');

no airson PostgreSQL:

    INSERT INTO "#__schemas" ("extension_id", "version_id") VALUES
    (211, '4.0.3-2021-09-05');

Cuir ro-leasachan an stòir-dhàta agad an àite `#__` mus ruith thu na h-aithrisean.

An uairsin, bhon chlàr-taice Rianaire, rach gu
**Siostam → Cumail suas → Stòr-dàta** agus càraich na clàir.

Bu chòir don ùrachadh obrachadh mar a bha dùil a-nis.

*Air eadar-theangachadh le openai.com*