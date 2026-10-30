<!--
{
    "source": "https://docs.joomla.org/Joomla_3.x_to_4.x_Step_by_Step_Migration",
    "title": "Joomla 3 gu 4 Ceum air Cheum",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

**Rabhadh:** Tha an stiùireadh seo a’ gabhail ris gu bheil thu a’ tòiseachadh air Joomla 3.10.x. Ma tha thu
air dreach nas tràithe, dèan cinnteach gun ùraich thu gu Joomla 3.10 an toiseach mus gluais thu
gu Joomla 4. Chan eil cabhag ann. Dèan cinnteach gu bheil na leudachain agad uile deiseil
airson Joomla 4.x. Tha Joomla 3.10.x a’ faighinn taic gu 16 Lùnastal 2023.

Seo stiùireadh ceum air cheum airson làrach 3.10.x a ghluasad
gu Joomla! 4.x. Ged a tha ceudan de shuidheachaidhean eadar-dhealaichte ann, bheir
seo dhut am modh-obrach bunaiteach ri leantainn. Tha coltas ann gum bi imrich
glè thoinnte mar thoradh air leudachain treas-phàrtaidh a chaidh a stàladh. Thathar
a’ moladh dhut fios a chur gu luchd-leasachaidh nan leudachan treas-phàrtaidh a chaidh a stàladh
air an làrach Joomla agad airson an t-slighe a mholas iad gus na
leudachain aca a ghluasad.

## Ceum air Cheum

### Suidhich Àite Leasachaidh

1.  Dèan cinnteach gu bheil thu a’ ruith an tionndadh Joomla 3.10.x as ùire mus
    lean thu air adhart.
2.  Dèan lethbhreac-glèidhidh den làrach bheò 3.10.x agad. Faodaidh tu inneal a thathar a’ moladh a chleachdadh
    (faic na *h-innealan a thathar a’ moladh* aig bonn na duilleige) no faodaidh tu seo a dhèanamh
    le làimh.
    -  [Bunaitean lethbhreac-glèidhidh airson làrach-lìn Joomla!](https://docs.joomla.org/Special:MyLanguage/Backup_Basics_for_a_Joomla!_Web_Site)
    -  [Dè na cleachdaidhean as fheàrr airson lethbhreacan-glèidhidh làraich?](https://docs.joomla.org/Special:MyLanguage/What_are_the_best_practices_for_site_backups%3F)
3.  Dèan cinnteach gu bheil an àrainneachd agad a’ coileanadh nan
    [riatanasan theicnigeach airson Joomla 4](https://downloads.joomla.org/technical-requirements)
    mus lean thu air adhart.
4.  Cruthaich stòr-dàta ùr agus cleachdaiche ùr gus an làrach 3.10.x agad aiseag thuige.
5.  Cruthaich làrach deuchainn no raon togail airson obrachadh ann agus aiseag
    lethbhreac-glèidhidh na làraich 3.10.x agad ann an aon de na h-àiteachan a leanas:
    - Fo-àrainn.
    - Fo-eòlaire.
    - Inneal ionadail. Tha oideachadh mionaideach aig Joomla mu stàladh
      XAMPP. Ach tha [WAMP](https://www.wampserver.com/en/),
      [MAMP](https://www.mamp.info/en/windows/) agus
      [LAMP](https://sourceforge.net/projects/lampas/)
      uile nan roghainnean eile freagarrach.
    - Cunntas aoigheachd ùr air àrainn shealach ann am bun-eòlaire. (Ma
      bu mhath leat aoigheachd atharrachadh rè pròiseas na h-imrich.)
      - Aiseag làraich air inneal ionadail.
        Faic [A’ stàladh Joomla gu h-ionadail](https://docs.joomla.org/Special:MyLanguage/Installing_Joomla_locally)
        agus  [A’ suidheachadh an stèisein-obrach agad airson leasachadh Joomla](https://docs.joomla.org/Special:MyLanguage/Setting_up_your_workstation_for_Joomla_development).
      - Aiseag làraich le inneal air a liostadh aig bonn na duilleige.
        (Leugh sgrìobhainnean an leasaiche.)
6.  Anns an àite deuchainn agad, ùraich an t-eisimpleir Joomla! 3.10.x agad chun
    fhoillseachaidh gleidhidh as ùire.
7.  Dèan cinnteach gu bheil an sgeama stòr-dàta as ùire agad air ùrachadh chun
    tionndadh 3.10.x as ùire le bhith a’ dol gu taba **Manaidsear nan Leudachan → Stòr-dàta**. Mura h-eil an sgeama agad ùraichte mar a chithear san
    dealbh a leanas, briog air a’ phutan **Ceartaich**:
![stòr-dàta nan leudachan Joomla 3](../../../en/images/migration/joomla-3-x-to-4-x-step-by-step-migration/01-admin-extension-database-fix.png)

8.  Falamhaich an sgudal: A bheil artaigilean sam bith agad san sgudal? Ma tha, sguab
    às iad (agus meadhanan iomchaidh sam bith a dh’fhaodadh a bhith co-cheangailte riutha mura
    bheil iad gan cleachdadh ann an àite eile air an làrach). Faodaidh artaigilean (roinnean agus nithean
    clàir-taice cuideachd) a tha air am fàgail san sgudal duilgheadasan adhbhrachadh gus nach tèid imrich
    a chrìochnachadh gun mhearachdan.
9.  Dèan deuchainn.
10. Dèan lethbhreac-glèidhidh a-rithist.

### Meas Gach Leudachan

Rè do phlanaidh, cho-dhùin thu dè na leudachain treas-phàrtaidh a bhiodh
air fhàgail no air an toirt air falbh agus mar a dhèanadh iad imrich. Airson a’
phàirt seo den Stiùireadh Ceum air Cheum, bidh thu a’ cleachdadh dà earrann
eadar-dhealaichte den làrach gu farsaing: an *Sgrùdadh Ro-ùrachaidh* ann an
**Co-phàirtean → Ùrachadh Joomla!** agus **Leudachain → Stiùirich → Stiùirich**.
Bidh thu a’ coimhead air gach leudachan a tha air a stàladh air an làrach agad.
Co-dhùnaidh tu am feum iad a bhith air an ùrachadh dhan tionndadh as ùire no
air an dì-stàladh. Barrachd fiosrachaidh ann an [Sgrùdadh Ro-ùrachaidh](https://docs.joomla.org/Special:MyLanguage/:Pre-Update_Check).

1.  A’ cleachdadh an **Sgrùdaidh Ro-ùrachaidh**, gus an Sgrùdadh Ro-ùrachaidh
    a chleachdadh, feumaidh tu co-phàirt Ùrachadh Joomla! a shuidheachadh gu
    Joomla 4. Gus seo a dhèanamh, lean na ceumannan seo:
2.  Rach gu **Co-phàirtean → Ùrachadh Joomla**. Bu chòir dha ràdh nach deach
    ùrachaidhean sam bith a lorg. Mura h-eil, ùraich Joomla dhan tionndadh as
    ùire (feumaidh gur e 3.10.x a th’ ann) agus dèan deuchainn. An uair sin
    dèan lethbhreac-glèidhidh eile. Briog air a’ phutan Roghainnean aig a’
    mhullach air an làimh dheis.
3.  Tagh *Joomla Next* bhon liosta-thuiteamach airson Sianal Ùrachaidh.
![taghadh sianal roghainnean ùrachaidh](../../../en/images/migration/joomla-3-x-to-4-x-step-by-step-migration/02-update-options-channel.png)

4.  Briog air **Sàbhail & Dùin**
5.  Chì thu an uair sin an Tionndadh Joomla a tha air a stàladh, an tionndadh
    Joomla! as ùire agus an URL airson a’ phacaid ùrachaidh. Seallaidh Joomla
    dhut na riatanasan airson Joomla 4 a-rithist. Ma chomharraicheas e gu bheil
    siostam no leudachain neo-fhreagarrach agad, innsidh e dhut an seo. Gabh
    mionaid airson an duilleag seo ath-sgrùdadh.
![ùrachadh gu 4 — sgrùdadh ro-ùrachaidh](../../../en/images/migration/joomla-3-x-to-4-x-step-by-step-migration/03-update-to-4-pre-update-check.png)

    <div class="alert alert-warning"><strong>Sanas:</strong> NA ùraich gu Joomla! 4
    an-dràsta. Chan eil seo ach airson na leudachain treas-phàrtaidh agad ullachadh
    agus an làrach a dhèanamh co-chòrdail ri Joomla! 4.</div>
6.  Coimhead air an Sgrùdadh Ro-ùrachaidh agus Sgrùdadh Ro-ùrachaidh nan
    Leudachan anns an taba Sgrùdadh Ro-ùrachaidh de cho-phàirt Ùrachadh Joomla.
    Ma tha leudachan sam bith nach eil nad phlana air a liostadh an seo, cuir ris
    an liosta agad de leudachain ri sgrùdadh.
7.  Ma rinn thu imrich bho Joomla! 2.5 gu 3.x roimhe, dh’fhaodadh gum bi
    leudachain air fhàgail ann a dh’fheumas a bhith air an glanadh. Seo na
    leudachain as sine de 2.5 no 3.x a dh’fheumas a bhith air an dì-stàladh
    mus ùraich thu gu Joomla 4:
    - plg_content_geshi
    - Teamplaid Rianaire Bluestork
    - Beez_20
    - Beez5
    - Atomic
    1.  A thaobh theamplaidean, dì-stàlaich a h-uile teamplaid bunaiteach
        aghaidh no cùil ach Protostar agus Beez3 (teamplaidean aghaidh) agus
        Isis no Hathor (teamplaidean rianaire). **NOTA:
        Chan eil Protostar co-chòrdail ri Joomla 4**. Às dèidh na h-imrich
        falbhaidh e. Feumaidh aon teamplaid a bhith agad air a thaghadh mar
        *bunaiteach* agus faodaidh tu Protostar no Beez3 a chleachdadh. Falbhaidh
        Protostar nuair a nì thu imrich gu Joomla 4.x.
    2.  Ma thig thu tarsainn air faidhlichean eile a dh’fheumas a bhith air an
        dì-stàladh, cuir iad ris an duilleag seo. ’S e uici a tha seo, agus mar
        sin faodaidh duine sam bith cur ris an duilleag. Mòran taing ro-làimh
        airson do sheirbheis.
8.  Mothaichidh tu na tagaichean a tha ag innse a bheil leudachan co-chòrdail
    no nach eil. Mar as trice bidh na tagaichean seo ag innse na fìrinn ma
    chanas iad Chan eil no Tha. Ma chanas iad *Tag Co-chòrdalachd a dhìth*,
    tha sin a’ ciallachadh nach do chleachd leasaiche an leudachain taga san
    leudachan aige, agus mar sin chan eil fios againn a bheil e co-chòrdail ri
    Joomla 4 no nach eil. Bruidhinn ris an leasaiche gus dearbhadh fhaighinn.
9.  **Ùraich Leudachain:** ùraich leudachain sam bith a chumas tu air an
    làrach-lìn agad. Ann an Joomla! 3.10.x faodaidh tu a dhol gu
    **Manaidsear Leudachan → taba Ùrachaidh** agus briogadh air **Lorg
    Ùrachaidhean**, a chuireas fiosrachadh co-chòrdalachd ann an tooltip sa
    cholbh Tionndaidh, fon taba Stiùirich, a’ toirt seachad beagan
    fiosrachaidh co-chòrdalachd bhon deireadh-chùil. Chan eil an goireas seo
    a’ cur taic ach ri leudachain a bhios gan ùrachadh tron taba Ùrachaidh ann
    am Manaidsear Leudachan. Ma tha leudachain agad air an stàladh nach
    cleachd ùrachadh leudachan Joomla, feumar am measadh le làimh mar a tha
    mìnichte gu h-ìosal. Tha an aon rud fìor airson nan leudachan sin aig a
    bheil tooltip. Feumaidh tu fhathast seòrsa a’ phacaid agus slighe na
    h-imrich a dhearbhadh leis an leasaiche leudachain gus dearbhadh fhaighinn
    air mar a nì thu ùrachadh/imrich.
10. Dèan sgrùdadh air agus dì-stàlaich Leudachain: rach gu
    **Manaidsear Leudachan → Stiùirich**
11. Briog air a’ phutan *Innealan Rannsachaidh* gus na roghainnean criathraidh
    a shealltainn
12. Tagh Pasgan bhon liosta-thuiteamach *Tagh Seòrsa*.
![duilleag stiùiridh nan leudachan](../../../en/images/migration/joomla-3-x-to-4-x-step-by-step-migration/04-extensions-manage.png)

    <div class="alert alert-info">Thathar a’ moladh Pasgan a thaghadh
    an toiseach oir ma tha rudeigin ann am pasgan a dh’fheumas tu a dhì-stàladh,
    dì-stàlaichidh e gu fèin-obrachail na Modailean, na Plugain no rud sam bith
    eile co-cheangailte ris sa phasgan aig an aon àm.</div>
13. Dì-stàlaich Pasganan sam bith nach eil feum orra tuilleadh no nach tèid
    imrich gu Joomla 4.
14. Dèan a-rithist am pròiseas seo le bhith a’ dol tron taba Stiùirich airson
    gach Seòrsa san liosta-thuiteamach: Co-phàirt, Faidhle, Cànan, Leabharlann,
    Modal, Plugan
    agus Teamplaid. Ma tha an t-Ùghdar ag ràdh Pròiseact Joomla!, fàg na
    leudachain sin mar a tha. Airson càch uile, dèan cinnteach gun
    dì-stàlaich thu an fheadhainn nach eil gan cleachdadh no nach eil
    co-chòrdail ri Joomla! 4.x.
    <div class="alert alert-danger"><strong>NOTA!</strong> Cha bhith e
    comasach dhut teamplaid sam bith a chaidh a shuidheachadh mar an
    àbhaist a dhì-stàladh. Feumaidh tu teamplaid le taic bhon Chridhe
    leithid Beez3 no Protostar a thaghadh agus an uair sin an teamplaid
    a dhì-stàladh ma tha feum agad air sin.
    <em>Cuimhneachan eile:</em> <strong>Chan eil Protostar co-chòrdail ri
    Joomla 4</strong>. Nuair a nì thu imrich, falbhaidh e. Le bhith ga
    thaghadh mar an àbhaist, gheibh thu dìreach gu Joomla 4.x.</div>
15. Dèan nota de na tionndaidhean de Phacaidean agus Cho-phàirtean a tha
    a’ ruith an-dràsta agus a chumas tu air an làrach agad. Faodaidh tu
    lethbhreac/cur ann an sgrìobhainn a dhèanamh dhiubh mar iomradh.
16. Airson leudachain sam bith a tha thu a’ cumail ach nach ùraich thu le
    aon bhriogadh leis a’ Mhanaidsear Leudachain (**Leudachain → Stiùirich → Ùraich**),
    ùraich na leudachain uile chun nan tionndaidhean as ùire.
17. Mus ùraich thu agus fhad ’s a tha thu gan ùrachadh, thoir fa-near a
    bheil tionndaidhean 3.10.x agus 4.x aig na leudachain anns an aon
    phacaid. Ma tha, bidh iad ceart gu leòr airson
    *ùrachadh le aon bhriogadh*. Mur eil, agus ma tha pacaidean eadar-
    dhealaichte aig 3.10 agus 4.x, feumaidh tu coimhead orra cùis air
    chùis. Mar as trice, tuitidh iad ann an aon de na suidheachaidhean
    a leanas:
    - Tha pacaidean fa leth aig an leudachan ach, nuair a nì thu ùrachadh
      gu 4.x, lorgaidh iad seo gu fèin-obrachail agus obraichidh iad fhathast.
      Dèan cinnteach gu bheil an leasaiche a’ dearbhadh seo.
    - Tha pacaidean fa leth aig an leudachan a dh’fheumas a bhith air an
      dì-stàladh ann an 3.10.x agus an uair sin air an stàladh leis an
      tionndadh Joomla 4.x aon uair ’s gu bheil an làrach air imrich.
      Dh’fhaodadh plugan susbaint a bhith na eisimpleir de seo. Tha e
      glè shìmplidh a dhì-stàladh ann an 3.10.x agus an uair sin a stàladh
      a-rithist ann an 4.x.
    - Faic [Beachdachaidhean mu Theamplaidean](https://docs.joomla.org/Special:MyLanguage/Template_Considerations_During_Migration)
      airson fiosrachadh nas mionaidiche mu theamplaidean agus
      [Ag Iompachadh teamplaid de Thionndadh Joomla! roimhe](https://docs.joomla.org/J3.x:Converting_A_Previous_Joomla!_Version_Template)

#### Notaichean mu Lorg (com_search)

Thèid Lorg (com_search) a sgaradh bho phrìomh shiostam Joomla 4.x. Nì
Lorg (com_search) imrich gu Joomla 4. Às dèidh na h-imrich, feumaidh tu
ùrachadh gu tionndadh Joomla 4.x tro com_installer. Leanaidh e air a
cumail suas, ach nas coltaiche ris an dòigh sa bheil leudachan treas-
phàrtaidh air a chumail suas, le bhith a’ faighinn ùrachaidhean tro
com_installer. Thathar a’ moladh Smart Search (com_finder) a chleachdadh
san àm ri teachd. Tha Lorg fhathast ri fhaighinn bhon
[Directory Leudachain Joomla](https://extensions.joomla.org/category/official-extensions/).

#### Notaichean mu Weblinks

Chaidh Weblinks a sgaradh bho phrìomh shiostam Joomla 3.4. Ma bha e ga
chleachdadh air làrach 2.5, bhiodh pròiseas na h-imrich a’ toirt fa-near
dha seo agus a’ dèanamh imrich air co-phàirt agus dàta Weblinks. Airson
na h-imrich bho 3.10.x gu 4.x, bidh e mar an ceudna. Tha e fhathast ri
fhaighinn agus ga chumail suas air an JED aig
[Leudachain Oifigeil](https://extensions.joomla.org/category/official-extensions).

#### Notaichean mu Shligheachadh Dìleabach

Cha bhi sligheachadh dìleabach ri fhaighinn ann an Joomla 4.x. Cha bhi
ach sligheachadh Ùr-nodha ri fhaighinn. Nuair a nì thu an imrich, ma tha
thu a’ cleachdadh sligheachadh dìleabach, atharraichidh an siostam iad
gu sligheachadh Ùr-nodha gu fèin-obrachail. Bidh thu airson dearbhaiche
cheanglaichean briste a ruith air an làrach agad às dèidh na h-imrich gu
Joomla 4.x agus *mus tèid an làrach beò*.

### Ag gluasad gu Joomla! 4.x

Nuair a bhios tu air na leudachain treas-phàrtaidh agad ùrachadh no
dì-stàladh gus nach bi ach an fheadhainn a tha co-chòrdail ri Joomla! 4
air fhàgail san stàladh agad, lean air adhart leis na ceumannan a leanas:

1. Rach gu **Siostam → Rèiteachadh cruinneil → taba an Fhrithealaiche** agus
    atharraich Aithris mhearachdan bho Bhuna-bheachd an t-Siostaim gu As motha. Dèan cinnteach gun
    tagh thu Sàbhail & Dùin.
![taba frithealaiche rèiteachadh cruinneil an t-siostaim](../../../en/images/migration/joomla-3-x-to-4-x-step-by-step-migration/05-system-global-configuration-server-tab.png)

2. Dèan lethbhreac-glèidhidh eile.
3. Rach gu **Co-phàirtean → Ùrachadh Joomla**. (Bu chòir dha ràdh nach deach ùrachaidhean
    a lorg. Mura h-eil, ùraich Joomla chun an tionndaidh as ùire agus dèan deuchainn.
    An uair sin dèan lethbhreac-glèidhidh eile.) Briog air a’ phutan Roghainnean aig an oisean
    gu h-àrd air an làimh dheis.
4. Tagh *Joomla Next* bhon chlàr-taice airson Seanail ùrachaidh.
![co-phàirt Joomla ùrachadh tagh seanal ùrachaidh](../../../en/images/migration/joomla-3-x-to-4-x-step-by-step-migration/06-update-select-channel.png)

5.  **Sàbhail & Dùin**.
6.  Chì thu an uair sin an Tionndadh Joomla a tha air a stàladh, an tionndadh Joomla!
    as ùire agus an URL airson a’ phacaid ùrachaidh. Seallaidh Joomla dhut na
    riatanasan airson Joomla 4 a-rithist. Ma chomharraicheas e gu bheil siostam no
    leudachain neo-chòrdail agad, innsidh e dhut an seo. Gabh mionaid gus an duilleag seo
    ath-sgrùdadh.
![sgrùdadh ùrachaidh e airson Joomla 4](../../../en/images/migration/joomla-3-x-to-4-x-step-by-step-migration/07-update-check.png)

7.  Mura nochd an t-ùrachadh, rach gu **Manaidsear nan leudachan → Ùrachadh** agus
    brùth air Glan tasgadan bhon bhàr-inneal. Bu chòir an t-ùrachadh gu Joomla! 4 nochdadh a-nis.
8.  Cuir do chorragan tarsainn, agus dèan cinnteach gu bheil an lethbhreac-glèidhidh sin agad
    ri làimh gun fhios nach bi feum air.
9.  Briog air a’ phutan Stàlaich an t-ùrachadh.
10. Dèan tì fhad ’s a bhios am bàr inbhe a’ luchdachadh gus am bi e làn uaine. Tha an ùine
    a bheir seo an urra ris an làrach agad, ris a’ cheangal Eadar-lìn agus ri astar an
    fhrithealaiche. Bheir am pròiseas mu dhà mhionaid. Nuair a bhios an t-ùrachadh
    deiseil, is dòcha gun tèid do logadh a-mach à Rianaire. Clàraich a-steach a-rithist.
    Dà thuras.
11. Ma thèid a h-uile càil gu math, gheibh thu sealladh gu tur ùr air pannal
    rianachd a’ chùlaibh.
![deas-bhòrd dachaigh Joomla 4 no 5](../../../en/images/migration/joomla-3-x-to-4-x-step-by-step-migration/08-j4-home-dashboard.png)

12. Rach gu **Siostam → Cumail suas → Stòr-dàta** agus briog air *Ceartaich* ma
    nochdas mearachdan sam bith.
13. Ann an **Siostam → Stàlaich → Lorg**, faic a bheil leudachain sam bith
    ri stàladh. (Cha bu chòir gin a bhith ann!)
14. Rach gu aghaidh na làraich agad agus faic a bheil i a’ nochdadh, fiù ’s mura h-e
    an teamplaid cheart a th’ ann. Ma tha, lean air adhart. Mura h-eil, faic mearachdan
    cumanta rè imrich.
15. Dèan lethbhreac-glèidhidh.
16. Stàlaich an teamplaid ùr agad no leudachain eile ma tha gin agad ri stàladh.
    Dèan lethbhreac-glèidhidh gu tric.
17. Rèitich iad. Dèan lethbhreac-glèidhidh gu tric.
18. Ruith dearbhadair cheanglaichean briste agus ceartaich ceanglaichean briste sam bith.
19. Dèan deuchainn air a h-uile càil. Dèan lethbhreac-glèidhidh gu tric.
20. Ma tha a h-uile càil ag obair mar a bha dùil, atharraich Aithris mhearachdan air ais gu
    Bun-bheachd an t-Siostaim (**Siostam → Rèiteachadh cruinneil → taba an Fhrithealaiche**).
    Dèan cinnteach gun tagh thu **Sàbhail & Dùin**.

### A’ cur do làrach Joomla! 4.x beò

1.  Nuair a bhios tu deiseil airson a dhol beò, dèan lethbhreac-glèidhidh den làrach 3.10
    agad airson na h-ùine mu dheireadh. Thoir air ais i ann am fo-eòlaire no
    fo-àrainn ma thogras tu.
2.  Dèan lethbhreac-glèidhidh den làrach Joomla! 4.x agad agus gluais no thoir air ais an làrach Joomla! 4.x
    agad dhan fhreumh (no atharraich na frithealaichean ainmean ma bha thu a’ togail air
    àrainn shealach aig freumh cunntais aoigheachd ùr).
3.  Dèan deuchainn a-rithist.
4.  MA tha thu air atharrachaidhean tèarainteachd a dhèanamh air an fhaidhle .htaccess san àm a dh’ fhalbh,
    is dòcha gum feum thu loidhne (no loidhnichean) atharrachadh ann gus ùrachadh chun an
    ath-thionndaidh de Joomla 4. Tadhail air
    [Atharrachaidhean Htaccess às dèidh Joomla 4](https://docs.joomla.org/Htaccess_changes_after_joomla4.0.4)
    gus faighinn a-mach am feum thu am faidhle agad atharrachadh no nach fheum.
5.  Thoir air falbh an làrach Joomla! 3.10 bhon fhrithealaiche taobh a-staigh latha no dhà
    mura h-eil thu air am faidhle *robots.txt* agad a dheasachadh gus casg a chur air damhain-allaidh
    nan einnseanan-rannsachaidh.
6.  Thoir air falbh a h-uile làrach leasachaidh leis an robh thu ag obair, no cùm iad
    ùraichte ma tha iad a’ ruith tionndadh làithreach, gus oidhirpean hacaidh air an
    fhrithealaiche agad a chumail air falbh.

Ma dh’atharraich dàta air an làrach 3.10 fhad ’s a bha thu ag imrich gu 4.x,
bidh thu airson an dàta sin a ghluasad dhan làrach 4.x mus tèid thu
beò. ’S urrainn dhut seo a dhèanamh le làimh (dèan cinnteach gun cùm thu na h-aon IDan
cleachdaiche - obraich ann an òrdugh) no le bhith a’ cleachdadh [leudachan treas-phàrtaidh](https://extensions.joomla.org/category/migration-a-conversion/data-import-a-export%20transfer%20tool/third-party%20extension/).

## Innealan a thathar a’ moladh

- Tha [Akeeba Backup](http://extensions.joomla.org/extensions/access-a-security/site-security/backup/1606)
  glè chumanta airson lethbhreac-glèidhidh agus ath-nuadhachadh.
- Barrachd [innealan lethbhreac-glèidhidh](https://extensions.joomla.org/tags/backup/).

*Air eadar-theangachadh le openai.com*