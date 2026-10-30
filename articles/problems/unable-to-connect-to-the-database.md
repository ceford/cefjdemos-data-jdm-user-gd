<!--
{
    "source": "https://docs.joomla.org/Unable_to_connect_to_the_database",
    "title": "Ceangal ris an St\u00f2r-d\u00e0ta",
    "description": " ",
    "author": ""
}
-->

## Mearachd “Cha ghabh ceangal a dhèanamh”

Ma gheibh thu mearachd "**Cha ghabh ceangal a dhèanamh ris an stòr-dàta**" rè an
stàlaidh, dearbhaich gu bheil thu air mion-fhiosrachadh an stòir-dhàta MySQL/MariaDB
a chur a-steach gu ceart. Cha leig an sgriobt **stàlaidh** leat leantainn air adhart
mura h-eil am mion-fhiosrachadh ceart.

Thoir fa-near nach eil dùil gun cruthaich thu cleachdaiche stòir-dàta agus facal-faire rè
an stàlaidh. Feumaidh iad a bhith air an cruthachadh an toiseach.

Ma thachras an fhàilligeadh às dèidh dhut an làrach agad a ghluasad gu aoigheachd eile,
sgrùd na nithean a leanas san fhaidhle *configuration.php*. Seo na roghainnean àbhaisteach
airson an stòir-dàta:

    public $dbtype = 'mysqli';
    public $host = 'localhost';
    public $user = 'yourdbuser';
    public $password = 'yourdbpassword';
    public $db = 'yourdbname';
    public $dbprefix = 't6q6i_';

Ma thachras an fhàilligeadh air làrach a bha ag obair, tha grunn adhbharan
comasach ann, cuid dhiubh sealach agus cuid eile gun fhiosta.

## Na Mearachdan as Cumanta

1.  Uaireannan chì thu an teachdaireachd seo ma tha MySQL/MariaDB air sgur
    a bhith a’ ruith air an fhrithealaiche agad. Dh’fhaodadh rianaire an
    fhrithealaiche agad MySQL/MariaDB a dhùnadh sìos rè ùine gus obair
    cumail suas a dhèanamh. Ann an suidheachaidhean mar seo, tha coltas ann
    gun till an làrach agad a dh’aithghearr.
2.  Chaidh cleachdaiche an stòir-dhàta agad a sguabadh às. Ma tha seo fìor,
    feumaidh tu do chleachdaiche stòir-dàta ath-chruthachadh leis an aon ainm-cleachdaiche agus
    facal-faire a bha ann nuair a stàlaich thu Joomla an toiseach. Cleachd pannal-smachd
    an àrainn agad gus seo a rianachd no cuir fios chun rianaire frithealaiche agad.
3.  Tha ainm-cleachdaiche no facal-faire an stòir-dhàta agad air atharrachadh.

*Air eadar-theangachadh le openai.com*