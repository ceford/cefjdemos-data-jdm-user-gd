<!--
{
    "source": "https://docs.joomla.org/How_do_UNIX_file_permissions_work%3F",
    "title": "Ceadan fhaidhlichean UNIX",
    "description": " ",
    "author": ""
}
-->

Faodaidh ceadan fhaidhlichean Unix/Linux a bhith troimh-chèile. Tha na ceadan
bunaiteach UNIX a’ tighinn ann an trì seòrsaichean;

    Ceadan an t-Sealbhadair : Smachd air do chothrom fhèin air faidhlichean.
    Ceadan na Buidhne : Smachd air cothrom dhut fhèin agus do dhuine sam bith sa bhuidheann agad.
    Ceadan Eile : Smachd air cothrom airson a h-uile duine eile.

Ann an Unix, nuair a thèid ceadan a rèiteachadh, leigidh am frithealaiche leat
ceadan eadar-dhealaichte a mhìneachadh airson gach aon de na trì roinnean
seo de luchd-cleachdaidh. Ann an àrainneachd frithealaiche-lìn, thathar a’ cleachdadh
ceadan gus smachd a chumail air cò de shealbhadairean nan làraichean-lìn aig a bheil
cothrom air na h-eòlairean agus na faidhlichean.

## Cò ris a tha ceadan Unix coltach?

Nuair a choimheadas tu air na faidhlichean agad tron loidhne-àithne a’ cleachdadh
àithne Unix `ls -l`, chì thu loidhnichean mar na leanas, aon airson gach faidhle agus eòlaire:
```
drwxr-xr-x@  7 username  usergroup    224 13 Feb 10:48 includes
-rw-r--r--@  1 username  usergroup   1060 13 Apr 21:00 index.php
```

Mìneachadh:
* ’S e d a’ chiad charactar san loidhne airson eòlaire, no - airson faidhle, no ...
* ’S e na 9 caractaran a leanas 3 buidhnean de 3 a tha a’ seasamh airson leughadh (r), sgrìobhadh (w) agus cur an gnìomh (x), no samhla minus (-) a’ ciallachadh gun chothrom airson gach aon de na Sealbhadairean, a’ Bhuidheann agus Daoine Eile.
* Tha an samhla @ am measg grunn bhuadhan leudaichte a dh’fhaodadh a bhith ann,
* ’S e an àireamh ron ainm-chleachdaiche doimhneachd an eòlaire.
* ’S e an dà ainm ainm-cleachdaiche an t-sealbhadair agus buidheann-cleachdaiche,
* ’S e an t-slànaighear a leanas meud an fhaidhle ann am bytes.
* Tha an ceann-latha a leanas a’ sealltainn na h-ùine airson nithean o chionn ghoirid, no na bliadhna airson nithean nas sine.
* Mu dheireadh tha ainm an fhaidhle no an eòlaire ann.

Ann an goireas FTP, dh’fhaodadh an t-òrdugh a bhith eadar-dhealaichte agus dh’fhaodadh
barrachd no nas lugha de dh’fhiosrachadh a bhith ann.

### Tha Sealbhadair (Cleachdaiche) co-cheangailte ri ainm-cleachdaiche

Mar as trice ’s tusa an Sealbhadair (Cleachdaiche), agus thèid na ceadan seo a chur an gnìomh
air ainm a’ chunntais aoigheachd agad.

### Tha Buidheann co-cheangailte ri buidheann-cleachdaiche

Thèid ceadan na Buidhne a chur an gnìomh air daoine eile a tha sa
bhuidheann cheudna riut; ann an àrainneachd aoigheachd, is glè ainneamh a bhios
daoine eile sa bhuidheann cheudna riut. Bidh seo a’ dìon nam faidhlichean agus
nan eòlairean agad bho bhith rim faighinn do dhuine sam bith eile aig a bheil
cunntas aoigheachd air an aon fhrithealaiche riut.

### Tha “Eile” a’ buntainn ris a h-uile duine eile

Tha na ceadan “Eile” seo gan cur an gnìomh air duine sam bith eile
air an fhrithealaiche nach eil thusa no nach eil sa bhuidheann agad. Mar sin,
ann an àrainneachd frithealaiche-lìn, a’ cuimhneachadh nach eil duine sam bith
eile mar as trice sa bhuidheann agad, ’s e seo a h-uile duine eile a tha a’
faighinn cothrom air an fhrithealaiche ach thusa. Tha gach aon de na trì
seataichean de cheadan air an sònrachadh mar a leanas;

    r = Ceadan Leughaidh
    w = Ceadan Sgrìobhaidh
    x = Ceadan Ruith

    Sealbhadair Buidheann Eile
    r w x r w x r w x

Mar a tha mòran agaibh eòlach mu thràth, bithear mar as trice a’ cur an
cèill ceadan mar luach àireamhach, rudeigin mar 755 no 644. Mar sin, ciamar
a tha seo a’ buntainn ris na bhruidhinn sinn gu h-àrd? Tha luach àireamhach
air a shònrachadh do gach caractar de na ceadan, agus thèid seo a shònrachadh
anns gach seata de thrì, agus mar sin chan fheum sinn ach trì luachan a
chleachdadh agus an ath-chleachdadh airson gach seata.

    Sealbhadair Buidheann Eile
    r w x r w x r w x
    4 2 1 4 2 1 4 2 1

A-nis gu bheil luach againn a tha a’ riochdachadh gach cead, is urrainn dhuinn
an cur an cèill ann an teirmean àireamhach. Chan eil anns na luachan ach an
cur ri chèile anns na seataichean fa leth de 3, agus bheir seo dhuinn trì
àireamhan a dh’innseas dhuinn dè na ceadan a tha gan suidheachadh. Ma thèid
innse dhuinn gu bheil ceadan faidhle 777, bhiodh seo a’ ciallachadh gu robh
na leanas fìor.

    Sealbhadair Buidheann Eile
    r w x r w x r w x
    4 2 1 4 2 1 4 2 1

Mar sin...

      4+2+1 4+2+1 4+2+1
    =   7     7     7

Bhiodh làn cheadan Leughaidh, Sgrìobhaidh agus Ruith aig sealbhadair an
fhaidhle, bhiodh làn cheadan Leughaidh, Sgrìobhaidh agus Ruith aig a’
bhuidhinn cuideachd, agus bhiodh an còrr den t-saoghal comasach air am faidhle
a Leughadh, a Sgrìobhadh agus a Ruith cuideachd. Mar as trice, ’s iad na
ceadan àbhaisteach, bunaiteach a bhios am frithealaiche a’ sònrachadh do
fhaidhlichean agus eòlairean;

    Faidhlichean = 644
    Eòlairean = 755

Bheireadh na ceadan seo cothrom, airson faidhlichean;

    644 = rw- r-- r--
    Tha Leughadh agus Sgrìobhadh aig an t-Sealbhadair
    Chan eil ach Leughadh aig a’ Bhuidhinn
    Chan eil ach Leughadh aig Eile

agus airson eòlairean;

    755 = rwx r-x r-x
    Tha Leughadh, Sgrìobhadh agus Ruith aig an t-Sealbhadair
    Chan eil ach Leughadh agus Ruith aig a’ Bhuidhinn
    Chan eil ach Leughadh agus Ruith aig Eile

A-nis, faodaidh cùisean fàs car toinnte nuair a thòisicheas sinn a’ bruidhinn
mu fhrithealaichean-lìn cho-roinnte. Bidh bathar-bog an fhrithealaiche-lìn a’
ruith leis an ainm-cleachdaiche agus ainm-buidhne aige fhèin. Tha a’ mhòr-chuid
de na frithealaichean air an rèiteachadh gus “apache” agus “apache” no
“nobody” agus “nobody” a chleachdadh mar ainm-cleachdaiche agus ainm-buidhne.
Seo an duilgheadas. Bidh am frithealaiche-lìn agad a’ ruith mar a
chleachdaiche fhèin, agus chan eil an cleachdaiche seo thusa no sa bhuidheann
agad, agus mar sin chan eil a’ chiad dà sheata de cheadan a’ buntainn ris.
Chan eil ach ceadan an t-saoghail (eile) a’ buntainn. Mar sin, ma rèiticheas tu
seata cheadan coltach ri 640 air faidhlichean na làraich-lìn agad, cha bhi am
frithealaiche-lìn agad comasach air faidhlichean na làraich-lìn agad a ruith.

    640 = rw- r-- ---
    Tha Leughadh agus Sgrìobhadh aig an t-Sealbhadair
    Chan eil ach Leughadh aig a’ Bhuidhinn
    Chan eil còraichean aig Eile

Chan eil ceadan sam bith air an sònrachadh don fhrithealaiche-lìn agus chan
urrainn dha Ruith, Sgrìobhadh no, nas cudromaiche buileach, am faidhle a
Leughadh gus a shusbaint a lìbhrigeadh gu brabhsair neach-tadhail na
làraich-lìn. Nam biodh ceadan 750 air an sònrachadh do dh’eòlaire, bhiodh an
aon bhuaidh aig seo, leis nach eil ceadan aig an fhrithealaiche-lìn eadhon
faidhlichean san eòlaire a leughadh, ged a bhiodh ceadan fàbharach aig na
faidhlichean am broinn an eòlaire sin.

    750 = rw- r-x ---
    Tha Leughadh agus Sgrìobhadh aig an t-Sealbhadair
    Tha Leughadh agus Ruith aig a’ Bhuidhinn
    Chan eil còraichean aig Eile

Tha cleas a bharrachd aig eòlairean: mura h-eil an cead Ruith air a
shuidheachadh ann an seata an t-Saoghail, an uair sin, fiù ’s ma tha Leughadh
agus Sgrìobhadh air an suidheachadh, mura h-eil am prògram ga ruith mar an
cleachdaiche no mar bhall den bhuidhinn, cha bhi e fhathast comasach air
faighinn gu na faidhlichean taobh a-staigh an eòlaire. Leigidh an suidheachadh
Ruith leis a’ phrògram òrdughan a “Ruith” san eòlaire, agus mar sin, às aonais
seo cha bhi am prògram (frithealaiche-lìn sa chùis againn) comasach air an
òrdugh “Leughadh” a ruith, agus mar sin cha bhi e comasach dha am faidhle agad
a lìbhrigeadh gu brabhsair-lìn nan cleachdaichean.

## Ciamar a tha seo co-cheangailte ri Joomla?

Deagh cheist; uill, sa chiad dol a-mach bhiodh seo cudromach rè
pròiseas an Stàlaichear-lìn. Ma chuimhnicheas tu air ais chun àm a ruith
thu Stàlaichear-lìn Joomla!, bha sinn a’ coimhead airson eòlairean sònraichte
a bhith air an sònrachadh mar eòlairean a ghabhas sgrìobhadh annta. Chì sinn
grunn phuist a tha ag ràdh gun robh duilgheadasan ann rè an stàlaidh le
ceadan, no a tha a’ faighneachd dè na ceadan a thathar a’ moladh. Tha cuid
eadhon den bheachd gu bheil an teachdaireachd, a tha ag iarraidh ceadan
“Writable”, ro neo-shònraichte.

Gu mì-fhortanach, leis nach eil fios aig Stàlaichear-lìn ciamar a tha an
frithealaiche agad air a rèiteachadh, chan urrainn dha a bhith nas
sònraichte; ge-tà, nuair a thuigeas tu na roghainnean cheadan agus nuair a
bhios beagan eòlais agad air àrainneachdan frithealaidh-lìn, gheibh thu a-mach
gu bheil am briathar *writable* dha-rìribh gu math sònraichte agus na
thuairisgeul nas motha na iomchaidh air na tha a dhìth air Joomla!. A’ toirt
sùil air an fhiosrachadh gu h-àrd, ’s dòcha gu bheil cuimhne agad gu bheil
trì àiteachan ann far am faodar ceadan *write* a shuidheachadh;

    Owner Writable
    Group Writable
    Other Writable

Cuideachd, cuimhnich nach bi am frithealaiche-lìn mar as trice a’ ruith mar
an cleachdaiche agad fhèin no sa bhuidheann agad fhèin. Nuair a ruitheas tu
Stàlaichear-lìn bho bhrobhsair, is e am frithealaiche-lìn a tha a’ feuchainn
ri cothrom fhaighinn air na faidhlichean; mar sin, ’s e na ceadan “Other” a
bheidh iomchaidh dha. Mura leig na ceadan “Other” leis a’ fhrithealaiche-lìn
na h-eòlairean Joomla! a leughadh, a sgrìobhadh no òrdughan a chur an gnìomh
annta, gheibh thu an teachdaireachd ag ràdh nach gabh sgrìobhadh sna
h-eòlairean.

Anns a’ chùis seo, feumaidh tu na ceadan Other a rèiteachadh gu “7” air na
h-eòlairean a tha air an liostadh ann an Stàlaichear-lìn. Mar sin, dh’fhaodadh
na ceadan iomlan agad a bhith rudeigin mar 757; anns a’ chùis as miosa
dh’fhaodadh gum feum thu 777 a shuidheachadh. Faodar na ceadan glè fhosgailte
seo ath-shuidheachadh gu 755 às dèidh dhan stàlaichear ruith, gus cuideachadh
le tèarainteachd nan eòlairean agus nam faidhlichean agad.

    757 = rwx r-x rwx
    Tha cead Leugh, Sgrìobh agus Cuir an gnìomh aig an t-Sealbhadair
    Tha cead Leugh agus Cuir an gnìomh aig a’ Bhuidhinn
    Tha cead Leugh, Sgrìobh agus Cuir an gnìomh aig Eile

Gus cùisean a dhèanamh eadhon nas troimh-chèile, bidh mòran chompanaidhean
aoigheachd a’ cleachdadh bathar-bog air a bheil phpsuExec no suExec; bidh na
h-innealan seo ag atharrachadh mar a bhios am frithealaiche-lìn a’ ruith.
Mar as trice cha bhiodh am frithealaiche-lìn a’ ruith mar an t-ainm
cleachdaiche agad; anns a’ chùis seo, ge-tà, bidh. Is dòcha nach bi feum air
na ceadan *other* a chleachdadh; ’s dòcha nach fheum thu a-nis ach na
h-eòlairean a rèiteachadh gus am bi iad *writable* don ainm-cleachdaiche agus
ainm-buidhne agad fhèin. Leigidh seo le ceadan nan eòlairean a bhith air an
suidheachadh mar 755 no 775 an àite 757 no 777.

    755 = rwx r-x r-x
    Tha cead Leugh, Sgrìobh agus Cuir an gnìomh aig an t-Sealbhadair
    Tha cead Leugh agus Cuir an gnìomh aig a’ Bhuidhinn
    Tha cead Leugh agus Cuir an gnìomh aig Eile

    775 = rwx rwx r-x
    Tha cead Leugh, Sgrìobh agus Cuir an gnìomh aig an t-Sealbhadair
    Tha cead Leugh, Sgrìobh agus Cuir an gnìomh aig a’ Bhuidhinn
    Tha cead Leugh agus Cuir an gnìomh aig Eile

Bidh feum fhathast aig a’ fhrithealaiche-lìn air cead Cuir an gnìomh a bhith
air a shuidheachadh airson an ainm-cleachdaiche, agus air ceadan Leugh agus
Cuir an gnìomh airson ainm na buidhne, gus an urrainn dha an àithne Leugh a
chur an gnìomh air faidhlichean taobh a-staigh an eòlaire. A-rithist, faodar
na ceadan seo ìsleachadh air ais gu 755 às dèidh do Stàlaichear-lìn
crìochnachadh. Sin na bunaitean mu eòlairean; dè mu na faidhlichean? Seo far
a bheil cùisean beagan nas sìmplidhe. Bidh a’ mhòr-chuid de na faidhlichean
a bhios Joomla! a’ cleachdadh gu math toilichte leis na ceadan bunaiteach
644.

    644 = rw- r-- r--
    Tha cead Leugh agus Sgrìobh aig an t-Sealbhadair
    Tha cead Leugh aig a’ Bhuidhinn
    Tha cead Leugh aig Eile

Tha seo dligheach mura bheil feum agad air sgrìobhadh dha na faidhlichean
bhon fhrithealaiche-lìn; tha na h-aon riaghailtean a’ buntainn ri
h-eòlairean ma tha an fheum seo agad. ’S e am faidhle configuration.php agad
aon fhaidhle a dh’fhaodadh tu a bhith airson a dhèanamh “Writable” don
fhrithealaiche-lìn. ’S e seo faidhle rèiteachaidh Joomla!; ma tha thu an
 dùil an rèiteachadh atharrachadh tron eadar-aghaidh Rianachd-lìn, feumaidh
am faidhle seo a bhith Writable don fhrithealaiche-lìn.

Nam biodh feum aig an fhrithealaiche agad air ceadan nan eòlairean a bhith air
an suidheachadh mar “Other” Writable airson an stàlaidh, is dòcha gum feum am
faidhle seo a bhith 757 no 777 cuideachd. Tha e cunnartach am faidhle seo
fhàgail mar 757 no 777 ge-tà, oir tha thu a’ leigeil le gach neach cothrom
“Write” fhaighinn. Bidh mòran de dh’ionnsaighean air làraichean-lìn a’ gabhail
brath air an fhìrinn seo; mar sin, san fharsaingeachd chan eilear a’ moladh am
faidhle seo fhàgail leis na ceadan sin.

Ma tha aon de na h-innealan SU air a stàladh air an fhrithealaiche-lìn agad
agus nach robh agad ach 755 a rèiteachadh air na h-eòlairean airson an
stàlaidh, is dòcha nach fheum thu ach 755 no 775 a shuidheachadh air an
fhaidhle seo cuideachd, gus deasachadh a cheadachadh tron eadar-aghaidh
Rianachd. Sa chumantas, thathar a’ gabhail ris gu bheil na ceadan seo nas
tèarainte na 757 no 777.

Mar cho-dhùnadh, dè na ceadan a bu chòir a shuidheachadh airson stàladh
Joomla!? Uill, mar a chì thu, tha e an urra ris an t-suidheachadh!

Tha fios agam nach eil seo cho cuideachail ’s a bhiodh tu air iarraidh agus
gu cinnteach chan e freagairt dheimhinnte a tha ann, ach san fharsaingeachd,
às dèidh an stàlaidh, faodar roghainnean “7” neo-thèarainte sam bith
ath-shuidheachadh gu rudeigin nas tèarainte. Mar eisimpleir:

    Faidhlichean = 644
    Eòlairean = 755

Leigeadh na ceadan seo leis na faidhlichean;

    644 = rw- r-- r--
    Tha cead Leugh agus Sgrìobh aig an t-Sealbhadair
    Chan eil aig a’ Bhuidhinn ach cead Leugh
    Chan eil aig Eile ach cead Leugh

agus airson nan eòlairean,

    755 = rwx r-x r-x
    Tha cead Leugh, Sgrìobh agus Cuir an gnìomh aig an t-Sealbhadair
    Chan eil aig a’ bhuidheann ach cead Leughaidh is Cur an Gnìomh
    Chan eil aig Eile ach cead Leughaidh is Cur an Gnìomh

Ma tha cothrom slige SSH agad, faodar na h-òrdughan a leanas a ruith bhon
loidhne-àithne gus na faidhlichean is na pasganan uile ath-shuidheachadh gu
roghainnean bunaiteach an fhrithealaiche, 755 agus 644. Atharraich gu
prìomh phasgan (“ / ”) an stàlaidh Joomla! agad, agus ruith:

    find . -type f -exec chmod 644 {} \;
    find . -type d -exec chmod 755 {} \;

Mura h-eil agad ach cothrom FTP, faodaidh seo a bhith na obair a bheir
glè fhada, ge-tà, mura do dh’atharraich thu barrachd phasganan rè an
stàlaidh a chaidh iarraidh, cha bu chòir dhut ach mu 10 pasganan agus am
faidhle *configuration.php* ath-shuidheachadh.

Cuimhnich, gus leudachain no teamplaidean sam bith a stàladh às dèidh
stàladh fhèin Joomla!, is dòcha gum feum thu na ceadan bunaiteach àrdachadh
a-rithist air na pasganan iomchaidh dìreach rè ùine an stàlaidh; faodaidh
tu an uair sin an lùghdachadh a-rithist às dèidh dhan tuilleadan a bhith
air a stàladh.

Ma cho-dhùnas tu *tasgadh* a chleachdadh, feumaidh am pasgan tasgaidh a bhith
*sgrìobhaidh* don chleachdaiche frithealaiche-lìn gus leigeil leis na
faidhlichean sealach aige a sgrìobhadh.

## Càradh ath-chùrsach air ceadan

Ann an uinneag crìche, a’ tòiseachadh bho fhreumh làrach Joomla, cleachd na
h-òrdughan a leanas gus ceadan nam faidhlichean is nam pasganan a shuidheachadh
gu roghainnean bunaiteach Joomla.

find . -type f -exec chmod 644 {} \;
find . -type d -exec chmod 755 {} \;

Nota: Tha an t-òrdugh find a’ gabhail ris gum bu chòir dha tòiseachadh bhon
phasgan làithreach. Gus a bhith sàbhailte, rach don phasgan public_html agad
agus sònraich slighe mar a’ chiad argamaid. Feumaidh cuid de shligean, leithid
bash air Apple OS X, slighe a bhith air a sònrachadh san òrdugh find.

Dèan deuchainn air gach leudachan treas-phàrtaidh às dèidh dhut na ceadan atharrachadh.

*Air eadar-theangachadh le openai.com*