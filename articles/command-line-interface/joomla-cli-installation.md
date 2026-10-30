<!--
{
    "source": "https://docs.joomla.org/J4.x:Joomla_CLI_Installation",
    "title": "St\u00e0ladh Joomla CLI",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Mar as trice, thèid an Joomla CMS a stàladh tro eadar-aghaidh brabhsair-lìn. Ach,
is dòcha gum b’ fheàrr le cleachdaichean eòlach Joomla a stàladh a’ cleachdadh
òrdughan ann an eadar-aghaidh crìochnachaidh. Leigidh seo le iomadh eisimpleir
Joomla a chur an sàs gu luath.

## Riatanasan an t-siostaim

Feumaidh Joomla PHP, stòr-dàta agus frithealaiche lìn. Airson an fhiosrachaidh
as ùire mu na bathar-bog a tha a’ faighinn taic agus na tionndaidhean as lugha
agus a thathar a’ moladh, tadhail air duilleag
<a href="https://manual.joomla.org/docs/next/get-started/technical-requirements/"
rel="noreferrer noopener">Riatanasan Teicnigeach</a>.

Faodar an stàladh a dhèanamh ann an dà dhòigh eadar-dhealaichte:

1.  Stàladh làimhe
2.  Stàladh fèin-obrachail air a stiùireadh le sgriobt

## Stàladh làimhe

Bheir stàladh làimhe deagh smachd dhut tron phròiseas stàlaidh. Tha gach
ceum ri fhaicinn sa chrìoch-uidhe agus faodar stad a chur air le `Ctrl+C` ma
thèid inntrigeadh ceàrr a dhèanamh.

### Ceumannan ri choileanadh

1.  Luchdaich suas faidhle zip no tar a’ phacaid stàlaidh dhan fhrithealaiche lìn.
2.  Dì-dhùisg am faidhle zip no tar.
3.  Ath-ainmich am pasgan dì-dhùisgte agus gluais e gu àite iomchaidh ann
    am freumh sgrìobhainnean an fhrithealaiche lìn.
4.  Gluais dhan phasgan anns a bheil còd Joomla agus ruith an àithne a leanas:<br>
    `php installation/joomla.php install`
5.  Thèid iarraidh ort na paramadairean a tha riatanach airson an stàlaidh, mar a chithear
    san eisimpleir a leanas:
```bash
php installation/joomla.php install

Install Joomla
==============

Checking system requirements...OK
Collecting configuration...

 Enter the name of your Joomla site:
 > J51
 Enter the real name of your Super User:
 > John Doe
 Set the username for your Super User account:
 > johndoe
 Set the password for your Super User account:
 >
 Enter the email address of the website Super User:
 > johndoe@example.com
 Database type. Supported: mysql, mysqli, pgsql [mysqli]:
 >
 Database host [localhost]:
 >
 Database username:
 > j4
 Database password:
 >
 Database name [joomla_db]:
 > j51
 Prefix for the database tables [u5dke_]:
 >
 Encryption for the database connection. Values: 0=None, 1=One way, 2=Two way [0]:
 >
 Relative or absolute path to the public folder []:
 >
OK
Validating DB connection...OK
Creating and populating the database...OK
Writing configuration.php and additional setup ...OK
Deleting /installation folder...OK
 [OK] Joomla has been installed
```

Nuair a bhios an sgriobt air a chrìochnachadh gu soirbheachail, gheibhear cothrom
air an làrach-lìn ùr tron bhrabhsair-lìn agad.

### Notaichean

*   Thoir aire mhionaideach do na tha thu a’ cur a-steach. Chan eil e comasach
    dol air ais sa sgriobt. Ma tha an inntrigeadh ceàrr, feumar stad a chur air
    an sgriobt.
*   Nochdaidh ainm na làraich Joomla agad ann am bàr tiotail an Rianaire, mar sin
    cùm goirid agus sònraichte e. Faodar atharrachadh nas fhaide air adhart.
*   Faodar fìor ainm an Àrd-chleachdaiche agad atharrachadh nas fhaide air adhart.
*   Bu chòir don ainm-chleachdaiche airson a’ chunntais Àrd-chleachdaiche agad ainm
    coltach ri *admin* a sheachnadh. Faodaidh e a bhith cunnartach oir ’s urrainn
    do neach-brathaidh tomhas furasta a dhèanamh air.
*   Feumaidh facal-faire a’ chleachdaiche a bhith 12 caractar a dh’fhaid.
*   Is e *mysqli* an seòrsa stòr-dàta bunaiteach. Is iad na seòrsaichean stòr-dàta
    ris a bheil taic MySQL (mysql) agus PostgreSQL (pgsql), a bharrachd air
    seòrsaichean co-fhreagarrach leithid MariaDB.
*   ’S e `localhost` cha mhòr an-còmhnaidh aoigheachd an stòir-dhàta. Cha bu chòir
    seòladh IP no ainm aoigheachd a chur a-steach an seo ach ma tha am frithealaiche
    stòr-dàta iomchaidh air a stàladh air aoigheachd eile. Ach, feumaidh ceadan
    sgrìobhaidh a bhith aig neach-cleachdaidh na crìche-uidhe air an aoigheachd
    a thagh thu. Gheibh thu am fiosrachadh seo bhon t-solaraiche eadar-lìn agad
    (ISP).
*   Mar as trice tha ainm-cleachdaiche an stòir-dhàta eadar-dhealaichte bho ainm
    an Àrd-chleachdaiche.
*   Tha facal-faire an stòir-dhàta airson stòr-dàta Joomla cha mhòr an-còmhnaidh
    eadar-dhealaichte bho fhacal-faire an Àrd-chleachdaiche.
*   Is e `joomla_db` ainm bunaiteach an stòir-dhàta, ach bithear tric a’ cleachdadh
    ainmean eile.
*   Tha ro-leasachan nan clàr stòir-dhàta air a shuidheachadh gu taghadh air thuaiream
    de chòig caractaran. Tha an luach seo air a chleachdadh gus clàran Joomla a
    sgaradh bho chlàran eile san stòr-dàta ma bhios e air a chleachdadh le
    aplacaidean eile cuideachd.
*   Is ann ainneamh a thèid an suidheachadh crioptachaidh airson a’ cheangail
    stòir-dhàta a chleachdadh. Mura faigh thu comhairle eile bhon ISP agad, fàg
    an luach seo aig a’ bhun-roghainn [0].

## Stàladh fèin-obrachail air a stiùireadh le sgriobt

Tha stàladh Joomla fo smachd faidhle *joomla.php* a tha suidhichte sa
fo-phasgan *installation* às dèidh dhut faidhle pacaid Joomla a dhì-phacadh.
Le cànan prògramaidh sam bith a leigeas leat faidhlichean PHP a ghairm agus a
ruith, faodaidh tu sgriobt a chruthachadh a nì fèin-obrachadh air na
h-ullachaidhean riatanach agus an stàladh fhèin a’ cleachdadh caochladairean
gnàthaichte. Gheibhear liosta de pharamadairean leis an àithne a leanas:
```bash
php installation/joomla.php help install
```

Seo eisimpleir de sgriobt shlige ris an canar jinstall.sh, air a chur ann am
pasgan freumh Joomla a chaidh a chruthachadh airson stàladh shìmplidh de Joomla:
```
#!/bin/bash

php installation/joomla.php install \
--site-name=SITE-NAME \
--admin-user=ADMIN-USER \
--admin-username=ADMIN-USERNAME \
--admin-password=ADMIN-PASSWORD \
--admin-email=johndoe@example.com \
--db-type=mysqli \
--db-host=localhost \
--db-user=j51 \
--db-pass=Garbage1n0ut \
--db-name=j51 \
--db-prefix=xyz12_ \
--db-encryption=0 \
--public-folder=j51
```

Le na ceadan aige air an suidheachadh gu 700, tha e furasta an sgriobt a ghairm
bhon loidhne-àithne le `./jinstall.sh`, agus thèid Joomla a stàladh ann an
priobadh na sùla. Dh’fhaodadh an sgriobt a bhith air a dheasachadh gus luachan
luchd-àiteachaidh atharrachadh, no dh’fhaodadh iad a bhith air an atharrachadh
nas fhaide air adhart às dèidh logadh a-steach don Rianaire.

Ma chleachdas tu an dòigh seo, cuimhnich an sgriobt jinstall.sh agad a sguabadh
às no a ghluasad taobh a-muigh do chraoibh lìn airson a chleachdadh ann an àite
eile nas fhaide air adhart. Thèid am pasgan stàlaidh a thoirt air falbh aig
deireadh a’ phròiseis stàlaidh. Mar sin, chan obraich ruith an sgriobt jinstall.sh
an dàrna turas.
*Air eadar-theangachadh le openai.com*