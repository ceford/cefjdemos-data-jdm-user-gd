<!--
{
    "source": "https://docs.joomla.org/J6.x:Workflow_Scenarios_Example_1",
    "title": "Eisimpleir Sruth-obrach 1",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Tha sruth-obrach air a dhèanamh suas de *ìrean* agus *ghluasadan* eadar na h-ìrean sin. Airson artaigil sam bith, ’s e an ìre làithreach a tha air a chlàradh san stòr-dàta agus 
air a chleachdadh gus an sruth-obrach agus na gluasadan a chleachdas an sruth-obrach sin aithneachadh.

Faodaidh iomadh sruth-obrach a bhith aig aon làrach. An seo, tha *Sruth-obrach Cuairt-litir* air a chleachdadh mar eisimpleir gus mìneachadh mar a dh’fhaodadh triùir le dreuchdan eadar-dhealaichte a bhith an sàs ann an dèanamh artaigil cuairt-litir. Tha an eisimpleir a’ cleachdadh buidhnean cleachdaiche bunaiteach Joomla, Ùghdar, Deasaiche agus Foillsichear. Tha duilgheadas an lùib sin: chan fhaic Ùghdar ach artaigilean Foillsichte agus mar sin chan urrainn dha artaigilean Neo-fhoillsichte ath-dheasachadh.
Tha dòigh gus an duilgheadas sin a sheachnadh air a mhìneachadh ann an [Eisimpleir 2](jdocmanual?article=user/workflows/workflow-example-2).

![Liosta nan sruth-obrach](../../../gd/images/workflows/workflow-example-1/01-example-1-workflows-list.png)

Thoir fa-near gu bheil an *Sruth-obrach Bunasach* air a shuidheachadh mar an *Bun-roghainn*. Dh’fhaodadh builean trioblaideach a bhith aig seo, a thèid a mhìneachadh nas fhaide air adhart san artaigil seo!

## Na Cleachdaichean

- ’S e cleachdaiche a th’ ann an *Arthur* a tha air a shònrachadh do **Bhuidheann Ùghdaran** Joomla. ’S urrainn dha artaigilean ùra a chruthachadh agus na h-artaigilean aige fhèin a dheasachadh, ach chan urrainn dha artaigilean a sgrìobh cleachdaichean eile a dheasachadh no staid artaigilean atharrachadh. Mar sin chan urrainn dha na h-artaigilean aige fhèin fhoillseachadh. ’S e an obair aige artaigilean ùra a dhreachadh.
- ’S e cleachdaiche a th’ ann an *Eddie* a tha air a shònrachadh do **Bhuidheann Dheasaichean** Joomla. ’S urrainn dha artaigilean a chruthaich cleachdaiche sam bith eile a dheasachadh, Arthur agus e fhèin nam measg. Chan urrainn dha staid artaigil atharrachadh idir. ’S e an obair aige na h-artaigilean a chuireas Eddie a-steach ath-sgrùdadh, agus dèanamh cinnteach à cruinneas, litreachadh agus gràmar, càileachd nan ìomhaighean agus mar sin air adhart.
- ’S e cleachdaiche a th’ ann am *Pru* a tha air a sònrachadh do **Bhuidheann Fhoillsichearan** Joomla. ’S urrainn dhi rud sam bith a dhèanamh as urrainn do Eddie agus Arthur. A bharrachd air sin, ’s urrainn dhi Staid artaigil atharrachadh. ’S e a h-obair co-dhùnadh a bheil artaigil freagarrach airson fhoillseachadh agus fhoillseachadh.

## Na h-Ìrean

Tha ceithir ìrean san t-Sruth-obrach seo:

![Liosta nan sruth-obrach](../../../gd/images/workflows/workflow-example-1/02-example-1-workflow-stages.png)

- Is e **Dreach** an ìre a chruthaicheas Arthur airson artaigil ùr.
- Is e **Ath-sgrùdadh** an ìre far an gabh Eddie os làimh leughadh dearbhaidh an t-susbaint.
- Is e **Aontaich** an ìre far an gabh Pru os làimh co-dhùnadh a bheil an artaigil math gu leòr airson fhoillseachadh.
- Is e **Foillsich** an ìre nuair a chaidh gabhail ris an artaigil agus nuair a chaidh fhoillseachadh.

Chan eil mòran mìneachaidh a dhìth air na foirmean inntrigidh dàta airson ìre, dìreach Ainm agus Tuairisgeul.

## Na Gluasadan

Tha feum air dà ghluasad eadar gach ìre: aon gus an ìre a thilleadh air ais ma tha barrachd obrach a dhìth san ìre roimhe; agus dàrna fear gus gluasad chun ath-ìre. Tha feum air gluasadan a bharrachd gus dèiligeadh ri crìoch artaigil:

![Liosta nan sruth-obrach](../../../gd/images/workflows/workflow-example-1/03-example-1-workflow-transitions.png)

- **Dreach/Ath-sgrùdadh** gus an ìre a ghluasad bho Dreach gu Ath-sgrùdadh.
- **Ath-sgrùdadh/Dreach** gus an ìre a thilleadh bho Ath-sgrùdadh gu Dreach.
- **Ath-sgrùdadh/Aontaich** gus an ìre a ghluasad bho Aonta gu Ath-sgrùdadh.
- **Aontaich/Ath-sgrùdadh** gus an ìre a thilleadh bho Aonta gu Ath-sgrùdadh.
- **Ath-sgrùdadh/Foillsich** gus an ìre a ghluasad gu Foillsichte agus inbhe an artaigil atharrachadh gu *Foillsichte*.
- **Foillsich** Gus staid an artaigil a shuidheachadh gu *Foillsichte* nuair a chuireas Ùghdar no Deasaiche an gluasad an gnìomh.
- **Neo-fhoillsich** gus inbhe an artaigil atharrachadh gu *Neo-fhoillsichte*.
- **Tasglann** gus inbhe an artaigil atharrachadh gu *Tasglannaichte*.
- **Sgudal** gus inbhe an artaigil atharrachadh gu *Air a chur dhan sgudal*.

Leigidh na trì gluasadan mu dheireadh le Pru inbhe artaigil atharrachadh nuair nach eil feum air tuilleadh.

### Deasaich Gluasad

Tha ceithir tabaichean aig an fhoirm inntrigidh cinn-latha, a’ tòiseachadh leis an taba *Gluasad*:

![Liosta nan sruth-obrach](../../../gd/images/workflows/workflow-example-1/04-example-1-edit-transition.png)

- **Ainm** Tha e nas fheàrr na h-ìrean Làithreach agus Targaid a chleachdadh san ainm.
- **Ìre Làithreach** An ìre mus tachair an gluasad.
- **Ìre Targaid** An ìre às dèidh don ghluasad tachairt.
- **Nòta** Nòtaichean mìneachaidh sam bith a chuidicheas gus an gluasad a mhìneachadh.

#### An taba *Gnìomhan Gluasaid*:

![Liosta nan sruth-obrach](../../../gd/images/workflows/workflow-example-1/05-example-1-edit-transition-actions.png)

- **Staid Sònraichte** Mìnich an staid shònraichte a bu chòir a bhith aig nì às dèidh an gluasad seo a chur an gnìomh. Fàg seo aig *-Gun taghadh-* mura h-eil cead aig a’ chleachdaiche a tha dualtach an gluasad seo a chur an gnìomh artaigilean a shònrachadh mar shònraichte.
- **Staid Foillseachaidh** Mìnich an staid fhoillsichte a bu chòir a bhith aig nì às dèidh an gluasad seo a chur an gnìomh. Fàg seo aig *-Gun taghadh-* mura h-eil cead aig a’ chleachdaiche a tha dualtach an gluasad seo a chur an gnìomh staid artaigil atharrachadh.

#### An taba *Brathan*:

![Liosta nan sruthan-obrach](../../../gd/images/workflows/workflow-example-1/06-example-1-edit-transition-notification.png)

- **Cuir Brath** Suidhich seo gu *Tha* far a bheil brathan riatanach, mar
  eisimpleir nuair a dh’fheumas Artair fios a chur gu Eideard gu bheil artaigil
  deiseil airson ath-sgrùdadh.
- **Teacsa Bratha a Bharrachd** Seo teacsa coitcheann a bharrachd gus an
  neach a gheibh e a chuideachadh.
- **Buidhnean-cleachdaidh** Faodaidh tu roghnachadh am brath a chur gu aon
  bhuidheann-cleachdaidh no barrachd, no gun bhuidheann sam bith agus am brath
  a chur gu daoine fa leth na àite.
- **Cleachdaichean** Tagh cleachdaichean fa leth bho liosta nan cleachdaichean.

#### An taba *Ceadan*:

Thoir fa-near gu bheil *Ùghdar* air *Eadar-ghluasad Gnìomhachaidh* a
shuidheachadh gu Ceadaichte (Oighreachd). Na atharraich na roghainnean seo airson
eadar-ghluasadan eile nach bu chòir do Ùghdar a chleachdadh, oir bheir seo buaidh
cuideachd air Luchd-deasachaidh agus Foillsichearan.

## Roinn-seòrsa an Artaigil

Thèid gach artaigil a shònrachadh do shruth-obrach nuair a thèid a shàbhaladh
airson a’ chiad uair. Ma thèid an artaigil a shònrachadh an toiseach do
Roinn-seòrsa aig a bheil Sruth-obrach air a thaghadh, thèid a shònrachadh don
t-sruth-obrach sin. Air neo, thèid a shònrachadh don t-sruth-obrach bhunaiteach.
Dh’fhaodadh sin a bhith na dhuilgheadas oir chan eil am pàirt Sruth-obrach a’
toirt seachad dòigh gus an sruth-obrach atharrachadh aon uair ’s gu bheil e air
a shònrachadh. Faodaidh sàr-chleachdaiche atharrachadh le bhith a’ cleachdadh
na Gnìomh Baidse air duilleag liosta nan Artaigilean.

### Cruthaich Roinn-seòrsa Litir-naidheachd

Tha feum air roinn-seòrsa Litir-naidheachd ùr gus an Litir-naidheachd a
shealltainn mar Bhlog Roinn-seòrsa agus gus dèanamh cinnteach gu bheil na
h-artaigilean Litir-naidheachd air an sònrachadh do Shruth-obrach na
Litir-naidheachd.

![Liosta nan sruthan-obrach](../../../gd/images/workflows/workflow-example-1/07-example-1-newsletter-category.png)

## Nì Clàr-taice na Litreach-naidheachd

Gus am faic luchd-tadhail na làraich an Litir-naidheachd, feumaidh i a bhith na
duilleag-dhachaigh no ceangailte ri nì clàr-taice. Gus an eisimpleir seo a
leantainn, cruthaich nì clàr-taice ùr den t-seòrsa *Blog Roinn-seòrsa* a’ cleachdadh
na roinne-seòrsa *Litir-naidheachd*.

Feuch nì clàr-taice na làraich. Tha e coltach gur e duilleag bhàn a bhios ann leis
a’ bhrath seo:

<div class="alert alert-info">
Chan eil artaigilean san roinn-seòrsa seo. Ma tha fo-roinnean-seòrsa air an sealltainn air an duilleag seo, dh’fhaodadh gu bheil artaigilean annta.
</div>

## Log a-steach mar Artair

Cuimhnich air Artair, an t-Ùghdar? Às dèidh dhut logadh a-steach, bu chòir putan
leis an leubail **Artaigil Ùr** a bhith air duilleag na Litreach-naidheachd.
Tagh e gus artaigil ùr a sgrìobhadh.

### Sgrìobh Artaigil

Lìon a-steach foirm deasachaidh an artaigil mar a dhèanadh tu airson artaigil
sam bith. Ach, mus sàbhail thu e airson a’ chiad uair, thoir sùil air an taba
*Foillseachaidh*.

- Bu chòir **Ìre Sruth-obrach** a shuidheachadh gu **Ruith Eadar-ghluasad**
  *Dreach/Lèirmheas*.
- Bu chòir **Roinn-seòrsa** a shuidheachadh gu *Litir-naidheachd*.

Nuair a bhios tu deiseil a’ deasachadh an artaigil, tagh *Sàbhail* no
*Sàbhail & Dùin*.

<div class="alert alert-danger">Às dèidh an artaigil a dhùnadh, chan urrainn do Artair a dheasachadh a-rithist oir chan urrainn do luchd-cleachdaidh sa bhuidheann Ùghdar artaigilean Neo-fhoillsichte fhaicinn.</div>

## Log a-steach mar Eideard

Tha cead aig Eideard, an Deasaiche, artaigilean Neo-fhoillsichte fhaicinn, agus mar
sin seallaidh duilleag na Litreach-naidheachd nithean Neo-fhoillsichte sam bith
dha airson an deasachadh.

### Dèan Lèirmheas air an Artaigil

Tagh an artaigil a dheasaich Eideard agus dèan atharrachaidhean sam bith a tha
riatanach gus a dhèanamh nas fheàrr. Nuair a bhios tu riaraichte, anns an *Tab
Foillseachaidh*:

- Bu chòir **Ìre Sruth-obrach** a shuidheachadh gu **Ruith Eadar-ghluasad**
  *Lèirmheas/Ceadaich*.

Eu-coltach ri Artair, nach urrainn an artaigil aige fhaicinn às dèidh a
shàbhaladh, faodaidh Eideard an artaigil fhaicinn agus a dheasachadh a-rithist.
Faodaidh e cuideachd an t-eadar-ghluasad airson na h-ath-ìre a shuidheachadh gu
Ceadaich/Foillsich. Obraichidh an t-eadar-ghluasad, ach cha tèid an artaigil
fhoillseachadh oir chan eil cead Foillseachaidh aig Eideard.

## Log a-steach mar Pru

Nuair a chaidh an ìre Ceadaich a shuidheachadh san t-sruth-obrach, bu chòir do Pru
teachdaireachd fhaighinn a’ brosnachadh gnìomh. Mar sin, log a-steach mar Pru gus
an artaigil ath-sgrùdadh agus a *Ìre Sruth-obrach* a shuidheachadh gu **Ruith
Eadar-ghluasad** *Foillsich*. *Sàbhail & Dùin* an artaigil gus an toradh
foillsichte fhaicinn. Log a-mach gus an toradh fhaicinn às aonais a’ cheangail
Deasaich,

Smaoineachadh às dèidh làimh: tha feum air ìre eile gus leigeil le Pru an ìre
atharrachadh bho Foillsich gu Lèirmheas ma tha i airson ’s gun socraich Eideard
rudeigin.

## Sruth-obrach na Cùla-taice

Tha na buidhnean cleachdaichean Ùghdar, Deasaiche agus Foillsichear an dùil airson
cleachdadh air an aghaidh-lìn. ’S e an duilgheadas do Artair nach urrainn dha
na h-artaigilean dhreach aige fhaighinn bhon aghaidh-lìn oir chan eil cothrom
seallaidh aig a’ bhuidheann cleachdaiche aige air artaigilean nach deach
fhoillseachadh fhathast.

Faodaidh tu cothrom air a’ chùla-taic a cheadachadh do gach ball de na buidhnean
seo mar a leanas:

- Rach dhan duilleag **Rèiteachadh Cruinneil**.
- Tagh an taba **Ceadan**.
- Tagh *Ùghdar* agus suidhich **Logadh a-steach rianaire** gu *Ceadaichte*.
- **Sàbhail**
- Rach dhan duilleag **Artaigilean: Roghainnean**.
- Tagh an taba **Ceadan** aige.
- Tagh *Ùghdar* agus suidhich **Cothrom air an eadar-aghaidh rianachd** gu *Ceadaichte*.

Leigidh seo le Artair, Eddie agus Pru logadh a-steach dhan chùla-taic le
cothrom air na nithean Susbaint. Deas-bhòrd Dachaigh mòran nas lugha:

![Deas-bhòrd Dachaigh Artair](../../../gd/images/workflows/workflow-example-1/08-example-1-backend-home.png)

Ach tha cothrom aig Artair a-nis air na h-artaigilean dhreach aige:

![Liosta artaigilean Artair](../../../gd/images/workflows/workflow-example-1/09-example-1-backend-articles.png)

Thoir fa-near nach urrainn do Artair an nì mu dheireadh san liosta a dheasachadh
oir chan e aon de na h-artaigilean aige fhèin a th’ ann. Chan eil tiotal an
artaigil ceangailte. Mar an ceudna, chan urrainn do Artair gin de na
roinnean a th’ ann a dheasachadh oir chan eil cead aige agus chan eil iad
ceangailte nas motha. Faodaidh e Roinn ùr a chruthachadh ach tha i
Neo-fhoillsichte agus chan urrainn dha a foillseachadh!

## Ceartachadh airson Sruth-obrach Mearachdach

Ma shònraicheas tu artaigil don t-sruth-obrach cheàrr, tha dà dhòigh ann airson
an duilgheadas a cheartachadh.

### Dòigh an Sàr-chleachdaiche

- Rach dhan liosta **Artaigilean**.
- Tagh am bogsa-seic airson an artaigil dhuilgheadasaich.
- Tagh am putan **Gnìomhan** sa Bhàr-inneal.
- Tagh am putan **Baidse** bhon liosta.
- Tagh **Atharraich Ìre** bhon chòmhradh *Pròiseas Baidse nan Artaigilean Taghte*.
- Tagh Sruth-obrach agus Ìre targaid iomchaidh.
- Tagh am putan **Pròiseas**.

![Liosta artaigilean Artair](../../../en/images/workflows/workflow-example-1/10-example-1-backend-batch.png)

### Dòigh Thèarmainn

Air neo, faodaidh tu clàr stòr-dàta a dheasachadh le phpMyAdmin no inneal
coltach ris.

Fiosrachadh a tha a dhìth:

- ID an artaigil bhon cholbh mu dheireadh ann an liosta nan Artaigilean.
- ID ìre ann an sruth-obrach a tha a dhìth bhon cholbh mu dheireadh ann an
  liosta nan Ìrean den t-Sruth-obrach a bu toil leat a chleachdadh.

Ann am phpMyAdmin:

- Brabhsaich an clàr #__workflow_associations gus an item_id anns a bheil
  ID an artaigil agad a lorg.
- Atharraich luach stage_id gu ID na h-ìre a lorg thu san t-sruth-obrach a
  tha a dhìth.

Till dhan liosta artaigilean agad agus dèan cinnteach gu bheil an nì
dhuilgheadasaich a-nis a’ cleachdadh an t-sruth-obrach cheart.

*Air eadar-theangachadh le openai.com*