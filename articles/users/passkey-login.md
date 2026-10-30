<!--
{
    "source": "https://docs.joomla.org/WebAuthn_Passwordless_Login",
    "title": "Logadh a-steach le iuchair inntrigidh",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Tha logadh a-steach le iuchair inntrigidh, air an robh Dearbhadh Lìn no WebAuthn 
air ainmeachadh roimhe, a’ leigeil le cleachdaiche logadh a-steach gu làrach gu 
tèarainte gun fhacal-faire a chleachdadh, ged a tha ainm-cleachdaiche fhathast 
a dhìth. Bidh e a’ cleachdadh crioptagrafaidheachd làidir ann an dòigh a tha 
air leth dìonach an aghaidh nan duilgheadasan as cumanta le faclan-faire:

* rinn cuideigin tomhas air (ionnsaigh feachd amh)
* ghabh cuideigin ris (ionnsaigh duine sa mheadhan)
* mheall cuideigin thu gus a nochdadh (ionnsaigh fiasgaich)
* bhris cuideigin e às dèidh dhaibh lethbhreac den dàta bhon stòr-dàta agad fhaighinn
  (ionnsaighean stealladh SQL)
* ghoid cuideigin e.

Chan eil logadh a-steach le iuchair inntrigidh dìreach glè thèarainte; tha e 
cuideachd glè fhurasta do luchd-cleachdaidh! Chan fheum thu tuilleadh faclan-faire 
fada a chuimhneachadh no manaidsear fhaclan-faire a chleachdadh. Chan eil agad 
ach *dearbhadair*, ris an canar uaireannan cuideachd *iuchair inntrigidh*.

Faodaidh dearbhadair iomadh cruth a bhith air, corporra no mas-fhìor. Faodaidh 
e a bhith na iuchair bhathar-chruaidh air leth a cheanglas ris an inneal agad 
tro USB, Bluetooth no NFC. Faodaidh e a bhith mar an inneal agad fhèin, a’ 
fuasgladh an dearbhadair thogte aige le PIN, leughadair lorgan-meòir, sganadh 
aodainn no sgrùdadh bith-mheatrach coltach ris.

Tha am feart seo ag obair mu thràth air uidheaman Android agus iOS/iPadOS agus 
tha sinn ag obair gus a chur an comas air Windows cuideachd. Faodaidh e fiù ’s 
a bhith mar am fòn agad — aig an àm seo tha seo comasach le fònaichean Android, 
ach tha am feart seo cuideachd a’ tighinn gu uidheaman iOS / iPadOS.

Chan obraich logadh a-steach le iuchair inntrigidh ach thairis air HTTPS agus 
dìreach nuair a tha an làrach agad a’ cleachdadh teisteanas dligheach, earbsach 
air a shon. Na gabh dragh, chan fheum thu airgead a bharrachd a chosg; mar as 
trice tha seirbheisean an-asgaidh leithid Let’s Encrypt amalaichte ann am 
pannalan-smachd aoigheachd-lìn agus tha iad ag obair gu math le logadh a-steach 
le iuchair inntrigidh.

Bidh logadh a-steach le iuchair inntrigidh a’ cleachdadh crioptagrafaidheachd 
iuchrach phoblach, an aon theicneòlas dhearbhte a chumas na làraichean agad 
sàbhailte le HTTPS, a chumas fiosrachadh do bhanca tèarainte agus mar sin air 
adhart. Cha bhi an iuchair phrìobhaideach a-riamh a’ fàgail an dearbhadair. Chan 
eil an làrach agad a’ stòradh ach iuchair phoblach. Fiù ’s ma dh’fhuilingeas tu 
briseadh-dàta, chan eil aig an neach-ionnsaigh ach iuchair phoblach a tha cha mhòr 
gun fheum; bheireadh e mìltean gu milleanan de bhliadhnaichean CPU gus a bhriseadh, 
an coimeas ris na beagan mhionaidean no uairean a dh’fheumar gus hash facal-faire 
stèidhichte a chuimhneachadh a bhriseadh.

Is e logadh a-steach le iuchair inntrigidh àm ri teachd an dearbhaidh. Furasta, 
tèarainte agus gun dragh. A h-uile rud nach eil faclan-faire stèidhichte.

Tha an dealbh a leanas a’ sealltainn inneal bathar-chruaidh air a chur ann am 
port USB coimpiutair-glùine. Chosg e £15 sa Ghearran 2022.

![dealbh de dh’Inneal bathar-chruaidh](../../../en/images/users/passkey-login/01-hardware-device.jpg)

Bidh logadh a-steach le iuchair inntrigidh a’ cleachdadh plugan siostaim a tha 
air a chomasachadh gu bunaiteach. Bidh putan **Log a-steach le iuchair inntrigidh** 
ann an scrionaichean logadh a-steach bunaiteach Joomla 4 agus nas fhaide air adhart, 
mar a chithear ann an scrion logadh a-steach an Rianaire:

![foirm logadh a-steach tèarainte an rianaire](../../../gd/images/users/passkey-login/02-login-form.png)

## Rèiteachadh a’ Chleachdaiche

Feumaidh an cleachdaiche clàradh an toiseach le Ainm-cleachdaiche agus Facal-faire 
àbhaisteach. Às dèidh logadh a-steach, rach gu foirm Pròifil a’ Chleachdaiche. 
Airson Rianaire:

- Tagh **Clàr-taice a’ Chleachdaiche → Deasaich Cunntas → Logadh a-steach le iuchair inntrigidh** gus am foirm fhaicinn, 
  gun dearbhadairean clàraichte an toiseach.
- Tagh **Cuir Iuchair Inntrigidh Ùr ris**

Tha an dearbh shealladh den ath cheum an urra ris a’ bhrabhsair agad. Mar as 
trice, chì thu rabhadh, teachdaireachd no uinneag ag iarraidh ort seòrsa 
dearbhadair a thaghadh no, ma tha thu a’ cleachdadh dearbhadair bathar-chruaidh 
ceangailte ris an inneal agad, a’ cur nad chuimhne am putan air an dearbhadair 
bathar-chruaidh a bhrùthadh. Airson adhbharan tèarainteachd agus practaigeach, 
chan eil ach ùine car goirid ri fhaighinn airson an dearbhadair a chur an gnìomh: 
60 diog.

![brosnachadh bathar-chruaidh airson logadh a-steach tèarainte an rianaire](../../../en/images/users/passkey-login/03-hardware-prompt.png)

Aon uair ’s a dh’fhuasglas tu an dearbhadair agad — le bhith a’ cnagadh air putan, 
a’ sganadh do lorgan-meòir / d’ aodann, a’ cur a-steach PIN no measgachadh dhiubh 
sin a rèir an dearbhadair agad — falbhaidh an teachdaireachd, clàraichear an 
dearbhadair agus nochdaidh an sgrion mar a leanas:

![dearbhadair clàraichte ann an logadh a-steach tèarainte an rianaire](../../../gd/images/users/passkey-login/04-registered-authenticator.png)

Tha e glè chudromach toirt fa-near nach urrainn dhut dearbhadairean a chlàradh 
no a thoirt air falbh ach air a’ chunntas cleachdaiche agad fhèin. Airson adhbharan 
tèarainteachd, chan eil cead aig eadhon Sàr-chleachdaiche dearbhadairean a chlàradh, 
a dheasachadh no a chur ri cunntasan chleachdaichean eile.

### Dearbhadairean

Faodaidh tu dearbhadair FIDO U2F no FIDO2 sam bith a chleachdadh. ’S e
inbhe nas sine a th’ ann am FIDO U2F a tha a’ cur taic ri taghadh nas
cuingealaichte agus nach eil cho tèarainte de dhòighean crioptografach. ’S e
FIDO2 an inbhe as ùire, a tha a’ cur taic ri dòighean crioptografach mòran
nas tèarainte, a’ gabhail a-steach Crioptografaidheachd Churrachan
Elliptigeach, dòigh crioptografach a thathar a’ creidsinn a bhios seasmhach
eadhon an aghaidh coimpiutaireachd cuantamaich (ma bhios agus nuair a
bhios sin na fhìrinn phractaigeach). A bharrachd air sin, faodar
dearbhadairean FIDO2 a shuidheachadh le dìonan a bharrachd leithid
PIN no smachd bith-mheatrach (m.e. sgan lorgan-meòir), agus tha sin a’
ciallachadh ged a chailleas tu seilbh chorporra air an dearbhadair fhèin,
nach urrainn don neach a lorgas e logadh a-steach do na làraichean agad.

Ma tha thu airson dearbhadair bathair-chruaidh a cheannach, faodaidh tu
"FIDO2" a lorg anns a’ mhargaidh as fheàrr leat, leithid Amazon. Tha taghadh
farsaing ann.

Faodaidh tu iuchair FIDO bathar-bhog leithid Krypton a chleachdadh mar
dhearbhadair agad cuideachd.

Tha dearbhadh a tha a’ gèilleadh ri FIDO2 air a thogail a-steach do dh’
iomadh inneal:

- Tha Windows 10 agus 11 a’ gabhail a-steach Windows Hello le PIN, sganadair lorgan-meòir,
  camara aithneachaidh aghaidh no measgachadh de iuchair bathair-chruaidh agus PIN.
- Tha TouchID aig macOS air a h-uile coimpiutair-uchd leis a’ chip T2 no air an fheadhainn a tha stèidhichte air
  Apple Silicon a’ cleachdadh an t-seinsir TouchID a tha air a thogail a-steach, a bharrachd air a h-uile
  coimpiutair deasg stèidhichte air Apple Silicon a’ cleachdadh meur-chlàr ùr Apple Aluminium le sganadair lorgan-meòir.
- Tha TouchID aig iOS / iPadOS air a h-uile inneal le sganadair lorgan-meòir agus
  FaceID air a h-uile inneal nas ùire le camara ro-mheasaidh dotagan infridhearg FaceID.
- Tha sganadair lorgan-meòir no camara aithneachaidh aghaidh aig cuid de dh’innealan Android. Faodaidh iad sin
  obrachadh cuideachd mar dhearbhadairean FIDO2, air Android 9 no nas ùire a’ cleachdadh Google Chrome co-dhiù.
- Dh’fhaodadh innealan eile a bhith rim faighinn cuideachd. Mar eisimpleir, fònaichean Android a’ cleachdadh
  [caBLE](https://groups.google.com/a/fidoalliance.org/g/fido-dev/c/go6GoFW27Dw/m/9flCLR5pBQAJ?pli=1)

### Brabhsairean a tha co-chòrdail ri logadh a-steach le Passkey

Gu practaigeach, ma chaidh an siostam-obrachaidh agus am brabhsair agad fhoillseachadh
às dèidh meadhan 2020, cha bu chòir duilgheadas sam bith a bhith agad. Chan eil ach
beagan bhrobhsaran glè neo-àbhaisteach fhathast gun taic do logadh a-steach le Passkey.

## Dearbhadh

Gus logadh a-steach, feumaidh tu d’ ainm-cleachdaiche a chur a-steach ann an raon
Ainm-cleachdaiche na foirme logaidh a-steach. Chan fheum thu am facal-faire agad a
chur a-steach, ach ma chuireas am brabhsair agad a-steach dhut e, fàg mar a tha e.
CHAN EIL am facal-faire air a chur chun an fhrithealaiche nuair a chuirear an fhoirm
a-steach tron phutan Dearbhadh Lìn.

Mar sin, faodaidh tu logadh a-steach an dàrna cuid leis an Ainm-cleachdaiche agus
am Facal-faire agad no le logadh a-steach leis an Ainm-cleachdaiche agus Passkey.

## Mar a chuireas tu am plugan à comas

Mura h-eil thu airson logadh a-steach le Passkey a cheadachadh, rach dìreach chun
liosta nam pluganan agus lorg am plugan **System - Passkey (Passwordless) Login**
sa bhuidheann System, agus cuir à comas e. Chan eil paramadairean ri shuidheachadh.

## Riatanasan an fhrithealaiche

Gus am bi logadh a-steach le Passkey ag obair, feumar na ro-chumhachan a leanas a choileanadh:

- HTTPS le teisteanas dligheach, soidhnichte. Leigidh a’ mhòr-chuid de luchd-aoigheachd leat teisteanasan an-asgaidh
  a chleachdadh a chuireas Let's Encrypt a-mach. Bidh iad sin ag obair gu foirfe
  le logadh a-steach le Passkey.
- Feumaidh an leudachan OpenSSL airson PHP a bhith air a stàladh agus air a chomasachadh.
- Feumaidh an leudachan PHP GMP no an leudachan PHP BCmath a bhith air a stàladh
  agus air a chomasachadh (nì aon seach aon dhiubh an gnothach).
- Bu chòir an leabharlann Sodium a bhith air a chomasachadh mas urrainn; tha e a’ comasachadh
  Crioptografaidheachd Churrachan Elliptigeach a chleachdadh air dearbhadairean FIDO2 co-chòrdail, rud a tha,
  mar a thuirt sinn, na dhòigh crioptografach as tèarainte.

## Ceistean Bitheanta agus Fuasgladh Dhuilgheadasan

### Chan fhaic mi am putan *Sign in with passkey*

Chan eil thu a’ faighinn cothrom air an làrach agad tro HTTPS. Chan eil logadh a-steach le Passkey ri fhaighinn ach
airson làraichean HTTPS le teisteanas dligheach. ’S e rabhadh tèarainteachd a tha seo a chaidh
a thoirt a-steach do inbhe logadh a-steach le Passkey. Bidh am plugan a’ sgrùdadh gu dearbh
a bheil cothrom ga fhaighinn air an làrach tro HTTPS a’ cleachdadh clas Uri Joomla. Ann an corra chùis ainneamh
far a bheil am frithealaiche ag innse breug mun phròtacal, ’s dòcha nach fhaic thu am putan ged a tha an làrach agad
ag ràdh (no a’ leigeil oirre) gur e HTTPS a th’ ann. Tha an aon rud fìor ma tha thu air am faidhle
configuration.php agad a dheasachadh agus air am paramadair rèiteachaidh roghainneil \$live_site a shuidheachadh
le ro-leasachan pròtacail http:// an àite https://.

Cuimhnich cuideachd gur dòcha nach seall modalan agus co-phàirtean logaidh a-steach treas-phàrtaidh a tha a’ cur an gnìomh
an fhoirm logaidh a-steach aca fhèin na putanan seo fhathast. Chuir sinn bun-structar ùr ris gus taic a thoirt dhaibh,
coltach ris na dh’fheumadh sinn a dhèanamh ann an Joomla! 3.2 gus taic a thoirt do Dhearbhadh Dà-Fhactar.

### Feumaidh mi fhathast ainm-cleachdaiche a thoirt seachad. Nach eil còir aig logadh a-steach le Passkey cur às do dh’ainmean-cleachdaiche?

Chan eil buileach, chan eil. Chan eil sònrachadh làithreach logadh a-steach le Passkey a’ toirt seachad stiùireadh dearbh-aithne. Feumaidh brobhsairean-lìn gun cuir sinn liosta de dh’iuchraichean poblach iomchaidh airson logadh a-steach le Passkey thuca rè ìre an logaidh a-steach. Tha seo a’ ciallachadh gu bheil feum againn air d’ ainm-cleachdaiche gus an lorg.

A dh’aindeoin sin, tha cleachdadh logadh a-steach le Passkey mu dheireadh a’ dèanamh soilleir nach eil ainmean-cleachdaiche *ri am meas mar dhìomhaireachdan*. Thathar gam meas mar fhiosrachadh poblach a ghabhas a chur gu saor gu nàmhaid, dìreach mar na h-iuchraichean poblach a tha air an stòradh ann an stòr-dàta na làraich. Is e an aon dìomhaireachd a tha air a stòradh anns an dearbhadair fhèin agus nach fhàg an dearbhadair idir!

### Tha mi air dearbhadair a chlàradh ach nuair a dh’fheuchas mi ri logadh a-steach tha e ag innse dhomh nach eil. An e buga a tha seo?

’S e buga a th’ ann, ach chan ann leis a’ plugan logadh a-steach le Passkey fhèin.

Bidh aon phlugain no barrachd air an làrach agad a’ tilgeil PHP Notices, Warnings no Errors, agus mar sin a’ truailleadh na freagairt a chuireas am frithealaiche agad air ais. Mar thoradh air an sin, chan urrainn don JavaScript air an duilleag freagairt an fhrithealaiche a pharsadh agus chan eil e cinnteach a bheil dearbhadairean sam bith clàraichte leis an neach-chleachdaidh.

Rach gu backend na làraich agad, System, Global Configuration agus suidhich Error Reporting gu None. Anns a’ mhòr-chuid de chùisean le plugainean bunaiteach agus 3PD nach eil gan giùlan fhèin ceart, tha seo gu leòr. Air neo, dèan sgrùdadh air toradh na h-iarrtais a’ cleachdadh innealan leasaiche a’ bhrobhsair agad gus faicinn dè tha a’ truailleadh na h-iarrtais.

### Chan eil sgiobalta ann an Safari airson an dearbhadair agam a chleachdadh

Cha bu chòir seo a bhith a’ tachairt tuilleadh le iOS 13, iPadOS 13 agus macOS
Catalina no tionndadh sam bith nas ùire.

’S e buga Safari a tha seo ann an tionndaidhean nas sine de Safari. Cha robh ann an tionndaidhean nas sine de Safari ach taic do logadh a-steach le Passkey mar fheart deuchainneach agus cha robh e deiseil buileach.

### Chan urrainn dhomh sensor bith-mheatrach a chleachdadh (TouchID, lorgan-meòir, Windows Hello)

Cha robh làn thaic aig cuid de bhrobhsairean nas sine stèidhichte air Chromium (ach a-mhàin Google Chrome fhèin) do dhearbhadairean togte. Bhiodh iad a’ tuiteam às a chèile no a’ crochadh nuair a dh’fheuchadh tu ri fear a chleachdadh. Chaidh na cùisean seo a chàradh anns na brobhsairean seo mu mheadhan 2020.

Ma tha Windows ga chleachdadh agad, cuimhnich FEUMAIDH sliseag Trusted Platform Module (TPM) a bhith san inneal agad agus feumaidh i a bhith an comas sa BIOS. Cha dèan sensor bith-mheatrach a tha co-chòrdail ri Windows Hello an gnothach leis fhèin. ’S e rabhadh tèarainteachd a tha seo ann an inbhe logadh a-steach le Passkey fhèin: feumar fiosrachadh an dearbhadair a phròiseasadh a’ cleachdadh bathar-cruaidh tèarainte, a tha an aghaidh bacadh, gus casg a chur air fo-thionndadh na h-iuchrach (m.e. chan urrainn do malware a tha a’ ruith air a’ choimpiutair an iuchair a thathar a’ cleachdadh airson dearbhadh a ghoid).

Mu dheireadh, cumaibh nad inntinn gu bheil taic do Windows Hello fhathast ga leasachadh agus gun tèid a leigeil ma sgaoil le Joomla 4.2.

### Ma ’s urrainn dhomh dearbhadair bathar-bhog a chleachdadh, carson a bu chòir dhomh dragh a ghabhail mu thòcan bathar-cruaidh?

Is e dìomhaireachd iomlan na h-iuchrach phrìobhaideach prìomh phuing logadh a-steach le Passkey. Chan eil fios aice ach aig an dearbhadair agus bu chòir gum biodh e do-dhèanta conaltradh a dhèanamh rithe leis an t-saoghal a-muigh.

A thaobh dearbhadair bathar-cruaidh, ge b’ e inneal bathar-cruaidh fa leth no TPM / Secure Enclave a tha air a thogail a-steach don inneal agad, tha seo cinnteach le nàdar an uidheim sin fhèin.

Bidh dearbhadair bathar-bhog a’ gineadh iuchair dhìomhair agus ga stòradh san t-siostam fhaidhlichean. Ach, ’s e aplacaid bathar-bhog àbhaisteach a th’ ann fhathast a tha a’ ruith taobh a-staigh an t-siostaim-obrachaidh àbhaistich agad, ge b’ e siostam an fhòn agad no a’ choimpiutair agad. Mar thoradh air sin, tha e buailteach do ghrunn sheòrsaichean ionnsaigheis a ghabhas cleachdadh gus fiosrachadh a ghoid gu dìomhair (cùisean tèarainteachd sa bhathar-bhog fhèin, malware a’ cleachdadh so-leòntachdan den t-seòrsa Spectre ann an CPUan an latha an-diugh is msaa).

Mar sin, tha dearbhadair bathar-bhog fada nas goireasaiche agus nas tèarainte na facal-faire àbhaisteach, ach tha dearbhadair bathar-cruaidh a’ tabhann na tèarainteachd as fheàrr. Tagh an dearbhadair agad a rèir do bhuidseit agus na feumalachdan tèarainteachd agad.

Leis gu bheil prìs iuchair FIDO (a tha co-chòrdail ri logadh a-steach le Passkey) nas lugha na €20 air Amazon, faodaidh tu dearbhadair bathar-cruaidh a chleachdadh anns a’ mhòr-chuid de chùisean cleachdaidh phractaigeach.

### Carson a tha na teisteanasan air an crioptachadh san stòr-dàta? Nach eil seo cus?

Is e an aon rud a tha air a stòradh san stòr-dàta an iuchair phoblach a
thill an dearbhadair nuair a tha sinn a’ dèanamh an deas-ghnàth dearbhaidh
(is e sin an t-ainm foirmeil airson dearbhadair a chlàradh a rèir
sònrachadh logaidh a-steach Passkey). Leis gur e iuchair phoblach a th’ ann,
chan fheum i dìon an aghaidh leughaidh. Fiù ’s ged a b’ urrainn do chleachdaiche
gun chead am fiosrachadh seo a leughadh, cha bhiodh e comasach dhaibh an
dearbhadair atharrais, mar eisimpleir le bhith ga chlònadh.

Ach, nam biodh cothrom sgrìobhaidh aig cleachdaiche droch-rùnach air dìreach
an clàr-stòr-dàta `#__webauthn_credentials`, gun chothrom leughaidh air an
t-siostam fhaidhlichean agus gun chothrom sgrìobhaidh air clàr sam bith eile,
dh’fhaodadh iad, gu teòiridheach, an dearbhadair aca fhèin a **chur ris**, agus
mar sin a bhith comasach air atharrais a dhèanamh air a’ chleachdaiche air a
bheil iad ag amas san t-siostam. ’S e ionnsaigh gu math teòiridheach a tha
seo, oir bhiodh aca cuideachd ri làmh a’ chleachdaiche air a bheil iad a’
toirt ionnsaigh a bhith aca, rud a tha nas duilghe fhaighinn gun eòlas
a-staigh air an làrach fhèin. A bharrachd air an sin, tha e air leth eu-coltach
gum biodh cothrom sgrìobhaidh aca air a’ chlàr seo a-mhàin, seach air an
stòr-dàta air fad (agus anns a’ chùis sin dh’fhaodadh iad Super User ùr a
chruthachadh). A dh’aindeoin sin, tha sinn a’ crioptachadh nan teisteanasan
gus nach bi e comasach eadhon don ionnsaigh seo, a tha gu tur teòiridheach,
soirbheachadh.

Tha làn fhios againn ma tha cothrom leughaidh aig cleachdaiche air siostam
fhaidhlichean an fhrithealaiche, gu bheil cothrom aca air an iuchair
crioptachaidh agus air fiosrachadh ceangail an stòir-dhàta, agus tha seo uile
air a stòradh ann an configuration.php. Ach, anns a’ chùis seo, tha thu
air do sheacadh mu thràth: faodaidh an neach-ionnsaigh configuration.php a
leughadh agus mar sin tha fios aca ciamar a cheanglas iad ris an stòr-dàta
agad. Anns a’ chùis seo faodaidh iad rud sam bith a thogras iad a dhèanamh
ris an làrach agad, a’ gabhail a-steach gach Super User a th’ ann mar-thà a
sguabadh às agus an cunntas Super User aca fhèin a chruthachadh. Mar sin chan
eil adhbhar ann feuchainn ris an t-suidheachadh seo fhuasgladh; bhiodh tu air
do chur an cunnart gu tur (air do sheacadh). Is e an aon rud a dh’fhaodadh do
shàbhaladh cùl-taic cunbhalach, dheuchainneach agus far an làraich.

### Tha mi air Dearbhadh Dà-Fhactar a stèidheachadh ach tha mi air logadh a-steach gun an Iuchair Dhìomhair agam a thoirt seachad. Nach eil seo mì-shàbhailte?

Chan eil, tha seo a dh’aona ghnothaich agus mar phàirt den dealbhadh.

Nuair a chuir sinn Dearbhadh Dà-Fhactar (TFA) ri Joomla! 3.2 cha robh thu
comasach air logadh a-steach don làrach agad ach a’ cleachdadh ainm-cleachdaiche
agus facal-faire. Faodar faclan-faire a ghoid no a thomhas. Mar sin b’ e TFA
an aon dòigh air ìre bheag de thèarainteachd a thoirt seachad air targaidean
le cunnart àrd agus luach àrd. Bha sin air ais ann an 2013.

’S e fuasgladh dearbhaidh gu tur eadar-dhealaichte a th’ ann an logadh a-steach
Passkey, aig nach eil gin de na duilgheadasan a tha co-cheangailte ri faclan-faire
stèidhichte. Bidh e a’ cleachdadh crioptagrafaidheachd làidir agus bathar-cruaidh
tèarainte gus a dhèanamh cha mhòr do-dhèanta na h-iuchraichean crioptagrafach
dearbhaidh a chur fo smachd. Chan fhaodar a mhealladh leis an dàrna cuid, is
e sin, chan urrainn dhut a bhith air do mhealladh gus a chleachdadh air làrach
a tha a’ dèanamh atharrais, leis gu bheil teisteanas logaidh a-steach Passkey
ceangailte ris an dearbh ainm àrainneis airson an deach a chur a-mach
(tha, ma chleachdas tu iomadh àrainn airson na làraich agad no ma ghluaiseas
tu an làrach agad gu àrainn eile, feumaidh tu na dearbhadairean logaidh a
-steach Passkey agad uile ath-chlàradh – thuig thu sin ceart!). Mar thoradh
air an sin, tha dearbhadh le logadh a-steach Passkey air leth tèarainte agus
a’ dol nas fhaide na na h-adhbharan a dh’fheumadh TFA. Tha seo a’ ciallachadh
ma dhearbhas tu d’ aithne gu soirbheachail le logadh a-steach Passkey, nach
feumar an iuchair dhìomhair TFA a sgrùdadh – agus mar sin chan eil i air a
sgrùdadh idir.

Ann an saoghal air leth freagarrach, cha bhiodh e comasach dhut logadh a
-steach don làrach agad ach a’ cleachdadh logadh a-steach Passkey. ’S e feart
a tha seo air a bheil sinn ag obair agus ’s dòcha nach bi thu airson a
chomasachadh; às dèidh na h-uile, ma dh’atharraicheas d’ ainm àrainneis no ma
chailleas tu cothrom air na dearbhadairean logaidh a-steach Passkey agad uile,
no ma nì thu ath-shuidheachadh orra, bhiodh tu glaiste a-mach às an làrach
agad. Mar sin bu chòir dhut TFA a chomasachadh fhathast air a’ chunntas
cleachdaiche agad, leis gum faodar logadh a-steach le facal-faire a chleachdadh
fhathast mar dhòigh eile air logadh a-steach don làrach agad agus feumar a
dhìon an aghaidh ionnsaighean aithnichte air faclan-faire stèidhichte.

### Nach eil TFA math gu leòr? Carson a tha feum againn air logadh a-steach le Passkey?

Tha TFA leis fhèin math gu leòr sa mhòr-chuid de chùisean, ach tha dà
dhuilgheadas aige.

An toiseach, tha e a’ toirt seachad eòlas cleachdaiche caran mì-ghoireasach.
Feumaidh tu an iuchair dhìomhair agad, a bhios ag atharrachadh an-còmhnaidh,
a thoirt seachad còmhla ri d’ ainm-cleachdaiche agus d’ fhacal-faire. Bidh a’ mhòr-chuid
a’ cleachdadh TOTP (an PIN sia-dhigitach a bhios ag atharrachadh gach 30 diog),
a chuireas maill air logadh a-steach agus a tha buailteach do luchd-cleachdaidh
a shàrachadh. Tha cleachdadh YubiKey fada nas luaithe, ach tha e cuideachd nas
daoire agus nas toinnte a sholarachadh nuair a tha barrachd air dithis no triùir
de luchd-cleachdaidh agad air an làrach. Tha beatha ris a bheil dùil aig YubiKey
de mu 2 bhliadhna de chleachdadh làitheil nuair a thathar a’ gineadh Faclan-faire
Aon-chleachdaidh (ruithidh e a-mach às a’ chuimhne sgrìobhaidh-aon-uair a chleachdas
e gus sùil a chumail air na h-ainmean-sgrìobhte a chuir e a-mach).

San dara àite, ma tha thu a’ cleachdadh TOTP, tha thu fhathast fosgailte do
chùisean tèarainteachd leithid luchd-glacaidh iuchraichean, phishing agus an
comas gun tèid an iuchair dhìomhair a chleachdar gus an TOTP a ghineadh a ghoid.
A bharrachd air sin, le millean comas agus trithead diog airson feuchainn orra,
tha e comasach gum faigh neach-ionnsaigh fortan, leis nach eil Joomla a’ glasadh
do chunntais no a’ cleachdadh cuingealachadh reata ann an dòigh eile airson
oidhirpean logadh a-steach a dh’fhàillig. Ged a ghabhadh na dìonan seo a chur an
gnìomh, dh’fhaodadh an cur an gnìomh fhèin a bhith air a mhì-chleachdadh gus
suidheachadh diùltadh seirbheis a chruthachadh a ghlasas cleachdaiche dligheach
a-mach às an làrach aige fhad ’s a tha an neach-ionnsaigh trang ga shàthadh.
’S e cùis a tha seo far a bheil an leigheas nas miosa na an galar.

Bidh logadh a-steach le Passkey a’ leasachadh eòlas a’ chleachdaiche gu mòr.
Ghabh prìomh bhrobhsairean ri logadh a-steach le Passkey agus tha iad a’ tabhann
eòlas cleachdaiche tarraingeach, a’ stiùireadh luchd-cleachdaidh gu bhith a’
cleachdadh dearbhadairean gu soirbheachail. Tha logadh a-steach le Passkey nas
goireasaiche eadhon an coimeas ri bhith a’ cleachdadh feart lìonadh
fèin-obrachail manaidsear fhaclan-faire. Le dreachan ùra de shiostaman-obrachaidh
gluasadach, tha an t-eòlas sin, a bha beagan troimh-chèile uaireigin, a’
fàs gu luath nas fhasa na bha faclan-faire agus TFA a-riamh.

Far a bheil logadh a-steach le Passkey dha-rìribh air leth math, ’s ann aig
aghaidh na tèarainteachd a tha e. Leis gu bheil e a’ cleachdadh bathar-cruaidh
tèarainte agus dearbhadh làidir air ainm àrainn na làraich, tha e cha mhòr
neo-bhuaileach do luchd-glacaidh iuchraichean, phishing agus fo-thionndadh
iuchraichean. Tha dìon togte aige eadhon an aghaidh clonadh iuchraichean. Seadh,
faodaidh tu fhathast do bhathar-cruaidh a chall — ach faodar dearbhadairean
FIDO2, ge bith an e innealan taobh a-muigh no innealan togte a th’ annta, a
ghlasadh a-mach le PIN no biometrics. San fharsaingeachd, tha cleachdadh
logadh a-steach le Passkey le dearbhadairean FIDO2 nas seasmhaiche an aghaidh
goid agus call na iuchraichean an taighe no a’ chàir agad.

## Notaichean don Leasaiche

### Putanan logaidh a-steach a bharrachd

Tha am modal plugain agus com_users a-nis a’ cleachdadh an tachartais
onUserLoginButtons, a tha air a mhìneachadh agus air a ghairm ann an
`Joomla\CMS\Helper\AuthenticationHelper::getLoginButtons`, gus mìneachaidhean
putanan a bharrachd sam bith a dh’fheumar a chur às dèidh a’ phutain logaidh
a-steach àbhaistich fhaighinn air ais.

Bu chòir do gach leasaiche a tha a’ cur modal logaidh a-steach an gnìomh no, san
fharsaingeachd, foirm logaidh a-steach a chleachdadh cuideachd an dòigh phoblach
stataigeach
`Joomla\CMS\Helper\AuthenticationHelper::getLoginButtons` gus na mìneachaidhean
sin fhaighinn air ais agus na putanan sin a thaisbeanadh, gus am bi am bathar-bog
aca làn-fhreagarrach ri Joomla 4.

Bu chòir do luchd-leasachaidh a tha airson putanan gnàthaichte a chur an gnìomh
sùil a thoirt air mar a tha am plugan siostaim logaidh a-steach Passkey a’
cur na gnìomhachd seo an gnìomh. Faodar na putanan sin a chleachdadh gus
seirbheisean soidhnidh singilte treas-phàrtaidh a chur an gnìomh no eadhon gus
logadh a-steach a’ cleachdadh seirbheisean dearbh-aithne treas-phàrtaidh leithid
an fheadhainn a tha air an tabhann leis na meadhanan sòisealta cumanta
(Facebook, Google, Twitter, GitHub msaa).

Chan eil an t-atharrachadh seo a’ toirt droch bhuaidh air co-fhreagarrachd
air ais. Leanaidh modalan logaidh a-steach agus foirmean logaidh a-steach
treas-phàrtaidh orra ag obair gu h-àbhaisteach eadhon mura cuir iad feart nam
putanan logaidh a-steach a bharrachd an gnìomh, ach bidh amalachaidhean a tha
air an comasachadh leis an fheart sin, leithid Dearbhadh Lìn fhèin, a dhìth.
’S e sin ri ràdh, cha sguir iad de bhith ag obair (rud a bhiodh na bhriseadh
b/c), ach cha bhi iad coileanta a thaobh fheartan.

### A’ ceadachadh com_ajax air duilleag logaidh a-steach an deireadh-sheachdain

Tha duilleag logaidh a-steach an Rianaire a’ cur com_ajax air liosta gheal ann an
AdministratorApplication gus an gabh a chleachdadh gus iarrtasan bho
luchd-cleachdaidh aoigheachd a làimhseachadh.

Chan eil an t-atharrachadh seo ag adhbhrachadh cùisean co-fhreagarrachd air ais
fhad ’s a chleachdas luchd-leasachaidh cleachdaidhean ciallach agus nach gabh iad
ris gu bheil a bhith air an gairm le com_ajax san deireadh-sheachdain na dhearbhadh
gu bheil an cleachdaiche air logadh a-steach don deireadh-sheachdain. Bhiodh sin
na dhroch chleachdadh tèarainteachd. ’S e an cleachdadh ciallach an nì User aig
Joomla a chleachdadh gus faighinn a-mach an e cleachdaiche aoigheachd a th’ ann
agus, mura h-e, a bheil cead aig a’ chleachdaiche a tha riatanach gus an gnìomh
a chaidh iarraidh tro com_ajax a choileanadh. ’S e sin ri ràdh, ma bhris an
t-atharrachadh seo an còd agad, bha an còd agad briste mu thràth agus bha feum
air ath-obrachadh co-dhiù.

## Barrachd Fiosrachaidh

Tha a’ chiad sgrìobhainnean mun fheart seo san iarrtas tarraing aig
[PR #28094](https://github.com/joomla/joomla-cms/pull/28094)

*Air eadar-theangachadh le openai.com*