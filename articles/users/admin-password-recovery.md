<!--
{
    "source": "https://docs.joomla.org/How_do_you_recover_or_reset_your_admin_password%3F",
    "title": "Ath-bheothachadh Facail-fhaire an Rianaire",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Mar as trice is urrainn do Shàr-chleachdaiche cleachdaichean is faclan-faire a
chur ris, a dheasachadh agus a sguabadh às ann an liosta nan
Cleachdaichean. Ann an cuid de shuidheachaidhean dh’fhaodadh nach bi seo
comasach. Mar eisimpleir, chan eil an neach aig an robh facal-faire
Sàr-chleachdaiche ri fhaighinn tuilleadh. No ’s dòcha gu bheil an
Sàr-chleachdaiche air dìochuimhneachadh dè am facal-faire a chaidh a chleachdadh.

Ann an leithid de chùisean tha dà dhòigh ann a leigeas le Rianaire làraich
logadh a-steach mar Shàr-chleachdaiche.

## Dòigh 1: Deasaich am faidhle configuration.php

Ma tha cothrom agad air an fhaidhle `configuration.php` airson stàladh Joomla
air an fhrithealaiche agad, faodaidh tu facal-faire Sàr-chleachdaiche ath-shuidheachadh no Sàr-chleachdaiche ùr a chruthachadh ma
thèid agad air logadh a-steach mar Mhanaidsear no Rianaire.

Feumaidh tu am faidhle `configuration.php` fhosgladh ann an deasaiche teacsa. An toiseach atharraich
ceadan an fhaidhle gu 644. Mar as trice leigidh na h-innealan rianachd làraich agad, leithid cPanel no
Plesk (tha feadhainn eile ann), leat seo a dhèanamh air loidhne. Mur eil, ’s dòcha gum feum thu FTP a chleachdadh gus am faidhle a luchdachadh a-nuas, atharrachadh gu h-ionadail agus a luchdachadh suas a-rithist.

Cuir an loidhne seo aig bonn an fhaidhle ach ron bhracag lùbach dhùnaidh:
```
    public $root_user='myname';
```

far a bheil **myname** ’na ainm-cleachdaiche le cothrom air a’ bhuidheann
*Manaidsear* no *Rianaire* aig a bheil am facal-faire agad. Cha obraich ainm-cleachdaiche a tha anns na buidhnean *Ùghdar*,
*Deasaiche* no *Foillsichear*, oir chan eil cothrom cùl-fhiosrachaidh aig na buidhnean sin.

Bidh an cleachdaiche seo a-nis na Shàr-chleachdaiche sealach.

Log a-steach don chùl-fhiosrachadh agus atharraich facal-faire an
Sàr-chleachdaiche aig nach eil am facal-faire agad, no cruthaich cunntas
Sàr-chleachdaiche ùr. Ma chruthaicheas tu cleachdaiche ùr, ’s dòcha gum bi thu airson an seann chleachdaiche a bhacadh no a sguabadh às, a rèir do shuidheachaidhean.

Nuair a bhios tu deiseil, dèan cinnteach gun cleachd thu an ceangal *Tagh an-seo gus feuchainn ri seo a dhèanamh gu
fèin-obrachail* a nochdas sa bhogsa rabhaidh gus an loidhne a chaidh a chur ris
an fhaidhle configuration.php a thoirt air falbh. Mura robh cleachdadh a’ cheangail soirbheachail, till air ais agus sguab às an loidhne a bharrachd bhon fhaidhle
configuration.php agad a’ cleachdadh deasaiche teacsa.

Mura h-eil cleachdaiche sam bith agad aig a bheil fios air am facal-faire aca, ’s dòcha gum feum thu atharrachadh a dhèanamh san stòr-dàta agad.

## Dòigh 2: Deasaich an Stòr-dàta

Mura do dh’obraich na dòighean gu h-àrd, tha dà roghainn eile agad, agus feumaidh an dà chuid obrachadh dìreach leis an stòr-dàta MySQL.

### Atharraich Facal-faire san Stòr-dàta

Is e an roghainn as sìmplidhe facal-faire an Sàr-chleachdaiche san stòr-dàta atharrachadh gu luach aithnichte. Feumaidh seo cothrom a bhith agad air stòr-dàta MySQL a’ cleachdadh phpMyAdmin no cliant eile. Tha an stiùireadh seo a’ sealltainn mar a dh’atharraicheas tu facal-faire gu **secret**.

Chan obraich an dòigh seo ach ma tha an cleachdaiche taghte anns na buidhnean *Manaidsear* no *Rianaire*.

**Dèan cinnteach gun atharraich thu facal-faire an Sàr-chleachdaiche aon uair ’s gum faigh thu cothrom air ais!**

1.  Fosgail phpMyAdmin agus tagh an stòr-dàta airson làrach Joomla! Seallaidh seo na clàran-stòr-dàta air taobh clì na sgrìn.
2.  Lorg agus tagh an clàr *#__users* far a bheil *#_* mar ro-leasachan a’ chlàir airson na làraich agad.
3.  Anns an t-sealladh *Brabhsaich*, lorg an cleachdaiche aig a bheil am facal-faire a tha thu airson atharrachadh agus tagh an ìomhaigheag Deasaich airson na sreatha seo.
    - ma tha an liosta fada, tagh am putan SQL aig a’ mhullach agus cleachd a’ cheist seo:<br>
    `SELECT * FROM `xxxxx_users` WHERE `username` = 'username'`<br>
    far an cleachd thu ro-leasachan an stòr-dàta agad an àite `xxxxx` agus an t-ainm-cleachdaiche a dh’fheumas tu a lorg an àite `username`.
4.  Anns an fhoirm dheasachaidh, atharraich am facal-faire gu<br>
    `d2064d358136996bd22421584a7cb33e:trd7TvKHx6dMeoMmBVxYmg0vuXEA4199`<br>
    agus tagh am putan *Rach* aig bonn na foirme. Bu chòir do phpMyAdmin an teachdaireachd *Sreathan air an tugadh buaidh: 1* a shealltainn. Aig an ìre seo, bu chòir am facal-faire a bhith **secret**.
5.  Log a-steach leis a’ chleachdaiche seo agus am facal-faire seo, agus atharraich facal-faire a’ chleachdaiche gu luach tèarainte. Thoir sùil air a h-uile cleachdaiche gus dèanamh cinnteach gu bheil iad dligheach. Ma chaidh do sheacadh, ’s dòcha gum bi thu airson na faclan-faire uile air an làrach atharrachadh.

### Cuir Sàr-chleachdaiche ùr ris

Mura obraich atharrachadh an fhacail-fhaire, no mura bheil thu cinnteach dè an cleachdaiche a tha na bhall de bhuidheann nan Sàr-chleachdaichean, faodaidh tu an dòigh seo a chleachdadh gus Sàr-chleachdaiche ùr a chruthachadh.
1.  Fosgail phpMyAdmin agus tagh an stòr-dàta airson làrach Joomla!.
2.  Tagh am putan *SQL* sa bhàr-inneal gus ceist SQL a ruith air an stòr-dàta a thagh thu. Seallaidh seo raon air a bheil "Ruith ceist/cheistean SQL air stòr-dàta xxxxx".
3.  Sguab às teacsa sam bith san raon seo agus dèan lethbhreac is pasg den cheist a leanas.
    Cuimhnich `xxxxx` a chur an àite le ro-leasachan an stòr-dàta agad fhèin.
    ```
    INSERT INTO `xxxxx_users`
       (`name`, `username`, `password`, `params`, `registerDate`, `lastvisitDate`, `lastResetTime`)
    VALUES ('Administrator2', 'admin2',
        'd2064d358136996bd22421584a7cb33e:trd7TvKHx6dMeoMmBVxYmg0vuXEA4199', '', NOW(), NOW(), NOW());
    INSERT INTO `xxxxx_user_usergroup_map` (`user_id`,`group_id`)
    VALUES (LAST_INSERT_ID(),'8');
    ```

    Tagh am putan *Rach* gus a’ cheist a chur an gnìomh agus an Sàr-chleachdaiche ùr a chur ris a’ chlàr.

Aig an ìre seo, bu chòir dhut a bhith comasach logadh a-steach do chùl-fhiosrachadh Joomla!
leis an ainm-cleachdaiche *admin2* agus am facal-faire *secret*.

An dèidh dhut logadh a-steach, rach gu liosta nan Cleachdaichean agus atharraich am facal-faire gu luach tèarainte ùr, agus cuir seòladh puist-d dealbhach ris a’ chunntas.

Ma tha teans ann gun deach do *sheacadh*, dèan cinnteach gun toir thu sùil a bheil a h-uile cleachdaiche dligheach, gu h-àraidh buill sam bith de bhuidheann nan Sàr-chleachdaichean.

## Faclan-faire Sealach Eile

**Rabhadh:** Tha luachan nam faclan-faire a chithear air an duilleag seo nan eòlas poblach agus
chan eil iad ach airson ath-bheothachaidh. Gus nach tèid do hacadh, dèan cinnteach gun atharraich thu facal-faire sealach
gu luach tèarainte às dèidh dhut logadh a-steach.

    password = "this is the MD5 and salted hashed password"
    ------------------------------------------------------
    admin  = 433903e0a9d6a712e00251e44d29bf87:UJ0b9J5fufL3FKfCc0TLsYJBh2PFULvT
    secret = d2064d358136996bd22421584a7cb33e:trd7TvKHx6dMeoMmBVxYmg0vuXEA4199
    OU812  = 5e3128b27a2c1f8eb53689f511c4ca9e:J584KAEv9d8VKwRGhb8ve7GdKoG7isMm

*Eadar-theangaichte le openai.com*