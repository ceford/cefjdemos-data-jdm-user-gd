<!--
{
    "source": "https://docs.joomla.org/J4.x:Multi-factor_Authentication",
    "title": "Dearbhadh Ioma-fhactar",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Tha siostam Dearbhaidh Ioma-fhactar Joomla! stèidhichte air Akeeba
Loginguard agus chaidh mòran den sgrìobhainn seo a chruthachadh le
cead bho Akeeba.

## Dè nì e?

Cuiridh e iomadh dòigh roghainneil airson Dearbhadh Dà Cheum ri logadh
a-steach Joomla!. Às dèidh dhut logadh a-steach le d’ ainm-cleachdaiche
agus facal-faire a-mhàin, thèid iarraidh ort an dàrna ceum de dhearbhadh
a thoirt seachad, mar eisimpleir còd a chruthaich Google Authenticator.
Gus an toir thu seachad dearbhadh ceart airson an dàrna cheum, cha bhith
e comasach dhut duilleag sam bith air an làrach fhaighinn. Thèid do
stiùireadh an-còmhnaidh air ais chun na duilleige “logaidh a-steach
glacaidh”. Tha seo coltach ris na nì Google nuair a dh’fheuchas tu ri
logadh a-steach do Gmail.

Tha seo eadar-dhealaichte bhon dòigh thùsail aig Joomla! airson
dearbhadh dà-fhactar, far am feumadh an dàrna factar dearbhaidh (m.e. an
còd a chruthaich Google Authenticator) a bhith air a chur a-steach còmhla
ris an ainm-cleachdaiche agus am facal-faire.

Is iad na buannachdan aig Dearbhadh Dà Cheum:

- Tha e nas lugha de mhì-mhisneachd don neach-cleachdaidh. Chan eil feum
  tuilleadh air an raon “Iuchair Dhìomhair”, a tha a’ cur luchd-cleachdaidh
  troimhe-chèile.
- Faodaidh e obrachadh le dòighean logaidh a-steach nach eil stèidhichte
  air facal-faire, leithid logadh a-steach sòisealta (m.e. Facebook),
  tòcan bathair-chruaidh tèarainte, SSO (logadh a-steach singilte) is eile.
  Soilleireachadh: Faodar Dearbhadh Dà Cheum a rèiteachadh gus an tèid
  iarraidh às dèidh do neach-cleachdaidh logadh a-steach le dòigh logaidh
  a-steach nach eil stèidhichte air facal-faire. Chan eil e a’ cur an
  gnìomh dhòighean logaidh a-steach nach eil stèidhichte air facal-faire.
- Tha smachd inntrigidh nas fheàrr aige. Faodaidh tu Roghainnean
  Cleachdaiche a shuidheachadh gus Dearbhadh Ioma-fhactar iarraidh no a
  chur à comas a rèir buidheann an neach-cleachdaidh.
- Leigidh e le dòighean dearbhaidh eile taobh a-staigh aon chunntais.
  Faodaidh grunn dhòighean dearbhaidh a bhith agad air a’ chunntas agad.
  Mar eisimpleir, faodaidh tu aplacaid Google Authenticator agus YubiKey
  a chur air dòigh.
- Tha e a’ cur taic ri dòighean far nach eil feum air còd a chur a-steach.
  Mar eisimpleir, dongalan FIDO2, dearbhadh bith-mheatrach is eile. Feumaidh
  iad sin conaltradh a dhèanamh leis a’ bhrabhsair agus/no leis an
  t-siostam-obrachaidh tro APIan dùthchasach HTML5.
- Tha e a’ cur taic ri dòighean a dh’fheumas eadar-obrachadh bhon
  neach-cleachdaidh. Mar eisimpleir, còd a chur tro theachdaireachd putaidh,
  SMS no post-d. Feumaidh na dòighean seo fios a bhith aca cò an
  neach-cleachdaidh a tha ga dhearbhadh mus tèid an còd dearbhaidh a chur
  thuige.
- Tha e saor an-asgaidh. Eu-coltach ri seirbheisean treas-phàrtaidh a
  bheir seachad dearbhadh ioma-fhactar, chan fheum thu cìs stèidheachaidh
  ro-làimh no cìs cumail suas mhìosail/bhliadhnail a phàigheadh airson gach
  làrach no neach-cleachdaidh a bhios a’ cleachdadh Dearbhadh Dà Cheum.
  Tha am bathar-bog saor an-asgaidh.

## Ciamar a tha e ag obair?

Logaidh tu a-steach don làrach agad mar as àbhaist, mar eisimpleir le
d’ ainm-cleachdaiche agus facal-faire a thoirt seachad. Tha e cudromach
a thoirt fa-near nach fheum thu teisteanasan dearbhaidh an dàrna cheum
a chur a-steach aig an ìre seo.

Mothaichidh an siostam gu bheil thu a-nis air logadh a-steach ach nach
eil thu air dearbhadh an dàrna cheum a dhèanamh. Sàbhalaidh e an URL a
bu chòir dhut fhaicinn agus stiùiridh e thu sa bhad chun na duilleige
logaidh a-steach glacaidh. Ma dh’fheuchas tu ri seòladh gu duilleag eile,
nochdaidh an duilleag ghlacaidh.

Faodaidh fiosrachadh sochairichte a bhith ann am modalan air an làrach
agad. Gus dèanamh cinnteach à dìomhaireachd, thèid na modalan a chur à
comas gu h-èiginneach aig àm an renderachaidh. Tha seo a’ ciallachadh
nach tèid suidheachadh mhodalan sam bith a renderadh air an duilleag.
Cuimhnich air seo ma mhothaicheas tu gu bheil am bann-cinn no raointean
dealbhaidh cudromach eile den làrach agad a dhìth air an duilleag
logaidh a-steach glacaidh.

Thoir fa-near, ge-tà, nach eil plugain à comas. Tha seo an dà chuid air
sgàth ’s gu bheil Joomla ga dhèanamh uabhasach doirbh plugain sònraichte
a thoirt air falbh às dèidh dhaibh a bhith air an luchdadh, agus air sgàth
’s gu bheil a’ mhòr-chuid de phlugain a’ coileanadh ghnìomhan deatamach
air an làrach agad.

Às dèidh dhut dearbhadh an dàrna cheum a thoirt seachad, thèid bratach a
shuidheachadh ann an seisean an neach-cleachdaidh, a’ sealltainn gu bheil
làn-ùghdarras agad an làrach a chleachdadh. A bharrachd air sin, thèid
do stiùireadh chun an URL a shàbhail e dìreach às dèidh dhut logadh a-steach
an toiseach.

## Dearbhadh dà-fhactar an aghaidh logaichean WebAuthn

'S e logadh a-steach le WebAuthn an roghainn as tèarainte. Cha toir thu
seachad ach ainm-cleachdaiche a bu chòir a bhith air a mheas mar
fhiosrachadh poblach gun shochairean. Cruthaichidh an làrach dùbhlan
crioptografach a thèid a shoidhnigeadh leis a' bhrabhsair a' cleachdadh
bathar-cruaidh tèarainte — tòcan bathar-cruaidh tèarainte air an taobh a-muigh
no am Trusted Platform Module / Secure Enclave aig an uidheam agad — agus
thèid a thilleadh dhan fhrithealaiche. Dearbhaidh am frithealaiche an
soidhne. Cleachdaidh an dearbhadh seo crioptografaidheachd iuchrach
phoblach, leis an làrach a' stòradh na h-iuchrach poblach a-mhàin. Nì seo an
logadh a-steach cha mhòr do-dhèanta a mhealladh le phishing agus air leth
tèarainte. Ma chleachdas tu sin, chan eil feum agad air dàrna factar
dearbhaidh — ach ma tha thu dha-rìribh ga iarraidh, faodaidh tu WebAuthn a
chleachdadh air a shon cuideachd.

Mura cleachdar dòighean logaidh a-steach co-aonaichte sam bith (leithid
logadh a-steach leis a' chunntas mheadhanan sòisealta agad, seirbheis
Single Sign-On, frithealaiche LDAP is eile), chan eil logadh a-steach
àbhaisteach le ainm-cleachdaiche + facal-faire faisg air cho tèarainte ri
logadh a-steach WebAuthn. Faodar ainm-cleachdaiche agus facal-faire a
ghlacadh, a ghoid no a thomhas. Nì seo earbsa ann an ainm-cleachdaiche agus
facal-faire a-mhàin gu math trioblaideach.

Airson dearbhadh ioma-fhactar, cha toir thu seachad ach d' ainm-cleachdaiche
agus d' fhacal-faire. Gheibheadh ionnsaigh phishing shoirbheachail am
fìor chiad fhactar dearbhaidh seo a-mhàin, ach chan fhaigheadh i an dàrna
factar dearbhaidh agad. Às dèidh logadh a-steach soirbheachail, thèid
duilleag bacaidh a shealltainn dhut. Chan urrainn dhut dad sam bith eile a
dhèanamh air an làrach gus an toir thu seachad an dàrna factar agad. Leis gu
bheil cur a-steach an dàrna factair air a shealltainn air a dhuilleag fhèin,
faodaidh e a bhith eadar-ghnìomhach (m.e. WebAuthn), asioncronach (m.e.
OTP fhaighinn tro phost-d, teachdaireachd teacsa no brath putaidh) no air a
thòiseachadh leis an neach-cleachdaidh (m.e. TOTP no OTP Yubikey). Nas
fheàrr buileach, faodaidh iomadh dòigh dàrna factair a bhith aig neach-
cleachdaidh air an comasachadh sa chunntas aige gus casg a chur air glasadh
a-mach gun fhiosta bhon làrach. Mar eisimpleir, dh'fhaodadh tu WebAuthn a
chleachdadh le dongle bathar-cruaidh tèarainte air an taobh a-muigh mar an
dàrna factar agad, am fear as tèarainte. Dh'fhaodadh TOTP àbhaisteach a
bhith agad cuideachd air a chur air dòigh gun fhios nach caill thu an dongle
no gun dìochuimhnich thu a thoirt leat. Tha cuid de dhòighean dàrna
factair a' ceadachadh iomadh eisimpleir; mar eisimpleir, faodaidh grunn
luchd-dearbhaidh WebAuthn a bhith agad gus an urrainn dhut an neach-dearbhaidh
a th' air a thogail a-steach don choimpiutair Windows agad, don iPhone agad
agus don chlàr Android agad a chleachdadh gun fheum a bhith agad cuimhneachadh
air dongle bathar-cruaidh agus innealan-atharrachaidh a phacadh gach turas a
dh'fhàgas tu an deasg agad.

Nach dèan sinn ath-sgrùdadh. Bhon roghainn as tèarainte chun an roghainn as
lugha tèarainte, is iad na roghainnean agad:

- WebAuthn mar phrìomh dhòigh logaidh a-steach agad le dearbhadh ioma-fhactar
  àrd-sgoile.
- WebAuthn mar an aon dòigh logaidh a-steach agad.
- Ainm-cleachdaiche agus facal-faire mar phrìomh dhòigh logaidh a-steach agad
  le dearbhadh ioma-fhactar àrd-sgoile.
- Dìreach ainm-cleachdaiche agus facal-faire mar an aon dòigh logaidh a-steach
  agad.

## Pluganain

Tha gach factar ann an dearbhadh ioma-fhactar air a chur an gnìomh tro
phlugain. Faodar an comasachadh no an cur à comas mar a tha riatanach. Agus
faodar feadhainn ùra a chur ris nuair a thig dòighean ùra am bàrr. Tha na
pluganain a thig le cridhe Joomla a' gabhail a-steach:

- **Còd dearbhaidh**: còdan dearbhaidh sia-dhigitich a ghineas aplacaid
  dearbhaidh (Google Authenticator, Authy, LastPass
  Authenticator, msaa), manaidsear fhaclan-faire (1Password, BitWarden, Keeper,
  KeePassXC, Strongbox, msaa) no, ann an cuid de chùisean, am brabhsair aca.
- **YubiKey**: A' leigeil le luchd-cleachdaidh air an làrach agad dearbhadh
  ioma-fhactar a chleachdadh a' cleachdadh tòcan bathar-cruaidh tèarainte
  YubiKey. Feumaidh YubiKey fhèin a bhith aig luchd-cleachdaidh, ri fhaighinn
  bho www.yubico.com.
- **Dearbhadh lìn**: a' faighinn taic bho gach brabhsair ùr-nodha. Tha a'
  mhòr-chuid de bhrabhsairean a' tabhann dearbhadh sònraichte don uidheam,
  air a dhìon le facal-faire agus/no biometrigs (mothachadair lorgan-meòir,
  sganadh aodainn, ...).
- **Còd dearbhaidh tro phost-d**: Cleachd còdan tèarainteachd sia-dhigitich,
  le ùine chuingealaichte, a thèid a chur thugad tro phost-d. 'S e 2 mhionaid
  an suidheachadh bunaiteach.
- **Còd stèidhichte**: tha seo an dùil airson deuchainn agus mìneachadh, agus
  tha e à comas a ghnàth. Cha bu chòir a chur an comas air làrach
  riochdachaidh.

Thoir fa-near gu bheil plugan air leth ann, **System - WebAuthn Passwordless
Login**, airson logadh a-steach a làimhseachadh bhon phutan Dearbhadh lìn san
fhoirm logaidh a-steach.

## Roghainnean luchd-cleachdaidh

Tha foirm Dearbhadh ioma-fhactar aig an fhoirm Luchd-cleachdaidh:
Roghainnean gus rèiteachadh mar a tha dearbhadh ioma-fhactar ag obair ann an
Joomla. Tagh am putan Tog cuideachadh in-loidhne airson fiosrachadh mu gach
roghainn.

![foirm dearbhaidh ioma-fhactar roghainnean luchd-cleachdaidh](../../../gd/images/users/multi-factor-authentication/01-users-configuration-mfa.png)

## Pròifil an Neach-cleachdaidh

Tha tabaichean fa leth aig an fhoirm Rianaire / Cleachdaichean: Deasaich
Pròifil airson Logadh a-steach WebAuthn agus Dearbhadh Ioma-fhactar, ach
chan eil am fear mu dheireadh ri fhaicinn ach do shealbhadair a’ chunntais.
Chan fhaic eadhon Sàr-chleachdaichean an taba seo airson luchd-cleachdaidh
eile.

Tha tabaichean foirm backend na foirme Làrach / Deasaich do Phròifil air
an cur aon os cionn an fhir eile, rud a dh’fhaodadh a bhith troimh-chèileach
oir nochdaidh Dearbhadh Lìn dà thuras: an toiseach airson logadh a-steach
gun fhacal-faire agus an uair sin airson Dearbhadh Ioma-fhactar. Tha an
dealbh a leanas a’ sealltainn pàirt Dearbhadh Ioma-fhactar na foirme às
dèidh modh a chruthachadh. Suidhichidh sin am feart gu Comasach gu
fèin-obrachail agus seallaidh e an roghainn Còdan Cùl-taice a chruthachadh.

![sealladh làraich de fhoirm dearbhaidh ioma-fhactar an neach-cleachdaidh](../../../gd/images/users/multi-factor-authentication/02-multi-factor-authentication-site-profile.png)

Mar a chaidh ainmeachadh gu h-àrd, faodaidh tu gach fear fheuchainn le bhith
a’ taghadh a’ phutan + Cuir ris ..., ach tagh Sguir dheth san fhoirm
a leanas ma cho-dhùnas tu gun a dhol air adhart.

*Air eadar-theangachadh le openai.com*