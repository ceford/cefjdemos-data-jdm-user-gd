<!--
{
    "source": "https://docs.joomla.org/J6.x:Workflow_Scenarios_Example_2",
    "title": "Eisimpleir Sruth-obrach 2",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Tha an eisimpleir seo a’ gabhail a-steach dithis chleachdaichean, Alice agus Bob, a tha fa leth nan
chathraiche agus nan rùnaire air comataidh. Tha an sruth-obrach a’ gabhail a-steach ullachadh
agus aontachadh chlàran-gnothaich agus gheàrr-chunntasan choinneamhan comataidh. ’S e ball
comataidh a th’ ann an Charlie aig am bi cothrom air pàipearan na comataidh nuair a bhios iad
air am foillseachadh. Chan eil an sruth-obrach a’ cleachdadh ach an aghaidh-shluaigh.

## Buidhnean Chleachdaichean

An toiseach cruthaich Buidhnean Chleachdaichean ùra, uile nan clann de *Registered*.

- **Committee** Clann de *Registered* 
- **Chair** Clann de *Committee*
- **Secretary** Clann de *Committee*

![Buidhnean chleachdaichean gnàthaichte](../../../gd/images/workflows/workflow-example-2/01-example-2-user-groups.png)

## Ìre Cothroim Chleachdaichean

- Cruthaich ìre ùr, **Committee**, agus cuir *Committee* ri Buidhnean Chleachdaichean le Cothrom Seallaidh.
- Anns an Ìre Chothroim *Special*, cuir *Committee* ri Buidhnean Chleachdaichean le Cothrom Seallaidh.

![Ìrean cothroim seallaidh](../../../gd/images/workflows/workflow-example-2/02-example-2-viewing-access-levels.png)

## Cruthaich Cleachdaichean

- **Alice** sa bhuidheann *Chair*.
- **Bob** sa bhuidheann *Secretary*.
- **Charlie** sa bhuidheann *Committee*.

## Cruthaich an Sruth-obrach

- **Ainm** *Committee Workflow*
- **Tuairisgeul** *Sruth-obrach airson pàipearan na Comataidh ullachadh.*
- **Ceadan**
  - **Committee** Suidhich a h-uile càil gu *Inherited* Chan eil cead ann (sealbhaichte).
  - **Chair** Suidhich a h-uile càil gu *Allowed* ach a-mhàin *Delete*. ’S dòcha...
  - **Secretary** Suidhich a h-uile càil gu *Allowed* ach a-mhàin *Delete* agus *Edit State*.

![Liosta nan sruth-obrach](../../../gd/images/workflows/workflow-example-2/03-example-2-workflows-list.png)

### Cruthaich Ìrean an t-Sruth-obrach

- **Dreach** 
  - **Nota** *Pàipearan gan ullachadh.* 
  - **Ceadan** Fàg a h-uile càil aig *Inherited*.
- **Lèirmheas**
  - **Nota** *Pàipearan a’ feitheamh ri aontachadh.* 
  - **Ceadan** Fàg a h-uile càil aig *Inherited*.
- **Foillsich**
  - **Nota** *Pàipearan air am foillseachadh.* 
  - **Ceadan** Fàg a h-uile càil aig *Inherited*.

![Ìrean an t-sruth-obrach](../../../gd/images/workflows/workflow-example-2/04-example-2-stages-committee-workflow.png)

### Cruthaich Eadar-ghluasadan an t-Sruth-obrach

#### Dreach gu Lèirmheas

’S e seo an t-eadar-ghluasad àbhaisteach air adhart ann an sreath nan ìrean.

- **Ainm** *Draft/Review*
- **Tab an Eadar-ghluasaid**
  - **Ìre làithreach** *Draft*
  - **Ìre thargaid** *Review*
  - **Nota** *Eadar-ghluasad chun ath ìre.*
- **Tab Gnìomhan an Eadar-ghluasaid**
  - **Staid nochdaidh** *- None Selected -*
  - **Staid foillseachaidh** *- None Selected -*
- **Tab Fiosrachaidh**
  - **Cuir Fios** *Yes* Feumaidh *Receive System Emails* a bhith air a chur an comas aig luchd-faighinn
    gus fiosan puist-d fhaighinn. 
  - **Teacsa Teachdaireachd a Bharrachd** A bheil dad sònraichte ann airson an t-sruth-obrach seo?
  - **Buidhnean Chleachdaichean** *Chair*
  - **Cleachdaichean** Roghainn eile seach Buidhnean Chleachdaichean a chleachdadh.
- **Tab nan Ceadan** Suidhich a h-uile càil gu **Inherited**.

#### Lèirmheas gu Dreach

’S e seo an tilleadh gu ìre roimhe san t-sreath, air a ghairm nuair a dh’fheumas
an Cathraiche barrachd obrach bhon Rùnaire. Tha na raointean foirme coltach ris na
raointean Dreach/Lèirmheas ach a-mhàin an Nota agus na *Ìre làithreach* agus
*Ìre thargaid* a bhith air an tionndadh mun cuairt.

#### Lèirmheas gu Foillsich

’S e seo an t-eadar-ghluasad a dh’atharraicheas staid nì bho *Unpublished*
gu *Published*. Chan eil cead aig a’ Chathraiche ach an t-atharrachadh sin a dhèanamh.

- **Ainm** *Review/Publish*
- **Tab an Eadar-ghluasaid**
  - **Ìre làithreach** *Review*
  - **Ìre thargaid** *Publish*
  - **Nota** *An t-eadar-ghluasad mu dheireadh gu foillseachadh.*
- **Tab Gnìomhan an Eadar-ghluasaid**
  - **Staid nochdaidh** *- None Selected -*
  - **Staid foillseachaidh** *Published*
- **Tab Fiosrachaidh**
  - **Cuir Fios** *Yes* Feumaidh *Receive System Emails* a bhith air a chur an comas aig luchd-faighinn
    gus fiosan puist-d fhaighinn. 
  - **Teacsa Teachdaireachd a Bharrachd** *Chaidh pàipear comataidh fhoillseachadh agus tha e ri fhaighinn a-nis airson coimhead air.*
  - **Buidhnean Chleachdaichean** *Committee*
  - **Cleachdaichean** Roghainn eile seach Buidhnean Chleachdaichean a chleachdadh.
- **Tab nan Ceadan**
  - **Secretary** Suidhich *Execute Transition* gu *Denied*.

#### Foillsich gu Lèirmheas

’S e seo atharrachadh bho Foillsich air ais gu Lèirmheas. A bheil feum dha-rìribh air?
Faodaidh an Rùnaire no an Cathraiche artaigil foillsichte a dheasachadh fhathast. ’S dòcha gun
deach pàipear comataidh le dàta mothachail fhoillseachadh le mearachd.

Ma tha feum air, cruthaich Eadar-ghluasad coltach ris an eadar-ghluasad *Lèirmheas gu Foillsich*
ach na h-Ìrean air an tionndadh mun cuairt, *Gnìomhan an Eadar-ghluasaid / Staid foillseachaidh*
air a shuidheachadh gu *Unpublished*, agus teachdaireachd choitcheann ann an
*Teacsa Teachdaireachd a Bharrachd*.

#### Tasglann

’S e seo an t-eadar-ghluasad a thèid a chur an gnìomh nuair nach eil feum tuilleadh air pàipear comataidh.
Anns an t-sruth-obrach, bidh e fhathast aig ìre Foillsich ach thèid Staid an artaigil
atharrachadh bho Published gu Archived.

- **Ainm** *Archive*
- **Tab an Eadar-ghluasaid**
  - **Ìre làithreach** *Publish*
  - **Ìre thargaid** *Publish*
  - **Nota** *Atharraich staid an nì bho Published gu Archived.*
- **Tab Gnìomhan an Eadar-ghluasaid**
  - **Staid nochdaidh** *- None Selected -*
  - **Staid foillseachaidh** *Archived*
- **Tab Fiosrachaidh**
  - **Cuir Fios** *No* Chan e eadar-ghluasad a tha seo a dh’fheumas gnìomh. 
- **Tab nan Ceadan**
  - **Secretary** Suidhich *Execute Transition* gu *Denied*.

![Eadar-ghluasadan an t-sruth-obrach](../../../gd/images/workflows/workflow-example-2/05-example-2-transitions-committee-workflow.png)

## Cruthaich Roinn Ùr

<div class="alert alert-warning">Tha an ceum seo glè chudromach! Feumar pàipearan ùra na Comataidh a chruthachadh leis an roinn seo, air neo gabhaidh iad ris an t-sruth-obrach bhunaiteach a dh’fheumas Sàr-chleachdaiche atharrachadh.</div>

- **Tiotal** *Comataidh* 
- **Sruth-obrach** Tagh *Sruth-obrach na Comataidh* bhon liosta Sruthan-obrach.
- **Ceadan** 
  - Ùghdar, Deasaiche agus Foillsichear: Uile suidhichte air *Gun chead* no air am fàgail aig *Gun chead (Oighichte)*.
  - Comataidh: Uile air am fàgail aig *Oighichte*.
  - Cathraiche: Uile ach *Sguab às* suidhichte air *Ceadaichte*.
  - Rùnaire: Uile ach *Sguab às* agus *Deasaich staid* suidhichte air *Ceadaichte*,

## Cruthaich Nì Clàr-taice

- **Tiotal** *Pàipearan na Comataidh*
- **Seòrsa nì clàr-taice** Liosta roinne
- **Tagh roinn** *Comataidh*
- **Cothrom** *Comataidh*

![Nì clàr-taice nam pàipearan na Comataidh](../../../gd/images/workflows/workflow-example-2/06-example-2-menu-item.png)

## Thoir sùil air an Làrach

Clàraich a-steach mar Alice, Bob, Teàrlach agus Sàr-chleachdaiche mu seach gus faicinn na chì iad:

Chì Alice, Bob agus Teàrlach an nì clàr-taice, ach chan fhaic duine sam bith eile e, fiù ’s Sàr-chleachdaiche. Às dèidh dhaibh an nì clàr-taice a thaghadh, chì Alice agus Bob clàr de phàipearan na Comataidh, a’ gabhail a-steach feadhainn nach deach fhoillseachadh fhathast. Chan fhaic Teàrlach ach clàr de phàipearan na Comataidh a chaidh fhoillseachadh, no teachdaireachd mhìneachaidh mura deach gin fhoillseachadh.

Chì Alice agus Bob ceangal Deasaich airson gach artaigil agus putan **Artaigil ùr** cuideachd. Mar as trice cleachdaidh Bob seo gus pàipear Comataidh a chruthachadh, ach faodaidh Alice sin a dhèanamh cuideachd.

![Sealladh Bob air duilleag liosta nan roinnean de phàipearan na Comataidh](../../../gd/images/workflows/workflow-example-2/07-example-2-committee-papers.png)

### Gus Pàipear Comataidh a Chruthachadh agus fhoillseachadh

- Clàraich a-steach mar Rùnaire agus tagh am putan **Artaigil ùr** air an duilleag *Pàipearan na Comataidh*.
- Cuir a-steach an teacsa agus *Sàbhail* e. Gabhaidh seo a dhèanamh thairis air grunn sheiseanan deasachaidh, ’s dòcha thar grunn làithean no sheachdainean. Fuirichidh an t-artaigil Neo-fhoillsichte agus aig ìre an Dreach gus...
- Tagh an taba *Foillseachadh* san fhoirm deasachaidh agus suidhich *Ìre an t-srutha-obrach* gu Ruith an t-eadar-ghluasad **Dreach/Lèirmheas**. 
- Tagh **Sàbhail & Dùin** gus an t-eadar-ghluasad a ruith.
- Tha obair an Rùnaire deiseil aig an àm seo agus chaidh teachdaireachd a chur gu Cathraiche na Comataidh.
- Bidh an Cathraiche a’ clàradh a-steach, a’ dèanamh cinnteach gu bheil am pàipear deiseil airson Lèirmheas agus a’ cleachdadh an eadar-ghluasaid **Lèirmheas/Foillsich** gus am pàipear a dhèanamh *Foillsichte*. Tha obair a’ Chathraiche deiseil aig an àm seo agus thèid teachdaireachd a chur gu buill na Comataidh.
- Faodaidh buill na Comataidh clàradh a-steach agus cothrom fhaighinn air a’ phàipear fhoillsichte.

*Air eadar-theangachadh le openai.com*