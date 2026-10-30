<!--
{
    "source": "https://docs.joomla.org/Visual_Studio_Code_Primer",
    "title": "Ro-r\u00e0dh do Visual Studio Code",
    "description": " ",
    "author": ""
}
-->

## VS Code - IDE Saor mòr-chòrdte

Bho Wikipedia:

> ’S e deasaiche còd-stòrais a th’ ann an Visual Studio Code, ris an canar
> VS Code gu cumanta cuideachd, a rinn Microsoft airson Windows, Linux agus macOS.
> Am measg nam feartan tha taic airson dì-bhugadaidh, soilleireachadh co-chòrdadh,
> crìochnachadh còd tuigseach, criomagan, ath-eagrachadh còd, agus
> Git freumhaichte. Faodaidh luchd-cleachdaidh an cuspair, ath-ghoiridean meur-chlàir,
> roghainnean atharrachadh, agus leudachain a stàladh a chuireas comas-gnìomh a bharrachd ris.

## Stàladh

Tha liosta tuiteam-sìos airson gach àrd-ùrlar le taic air duilleag
bhunaiteach làrach VS Code. Is dòcha gu bheil an àrd-ùrlar agad air a thaghadh
ro-làimh. Mar sin luchdaich sìos e agus stàlaich e, agus bidh thu deiseil airson tòiseachadh.

### A’ Tòiseachadh

Tha cuid de nithean *Start*, liosta de nithean *Recent*, agus liosta ghoirid
de *Walkthroughs* air duilleag *Get Started* VS Code. Ma tha thu
gu tur ùr do VS Code, thathar a’ moladh gun coimhead thu orra. Cha toir iad
ach beagan mhionaidean.

Tha Sgrìobhainnean VS Code rim faighinn bhon chlàr *Help / Documentation*
. ’S fhiach coimhead air na [Bideothan Ro-ràdh](https://code.visualstudio.com/docs/getstarted/introvideos)
. Bheir gach fear 2 gu 6 mionaidean agus bheir iad ro-ràdh sàr-mhath
do fheartan VS Code.

’S e na sgrìobhainnean oifigeil an t-àite dhan tèid thu ma tha thu airson
fiosrachadh sònraichte a lorg.

### Leudachain VS Code

Faodar VS Code a chleachdadh airson seòrsa sam bith de theacsa, a’ gabhail a-steach raon farsaing de
chànanan prògramachaidh. Bidh e ag obair le JavaScript gun leudachain a chur ris.
Thèid cànanan eile a lorg a rèir co-theacsa, mar sin ma thòisicheas tu air
còd PHP a chruthachadh agus a shàbhaladh, tha e coltach gun tèid iarraidh ort pasgan
PHP Support a stàladh.

Briog air an ìomhaigheag *Extensions* anns an *Activity Bar* chlì gus faicinn dè
a tha thu air a stàladh agus dè tha air a mholadh. Bidh feum agad air an leudachan PHP Debug!

### Cruth Sgrìn VS Code

Seo cuid de na briathran a thèid a chleachdadh anns an stiùireadh a leanas:

- **Activity Bar** am bàr caol air taobh clì na sgrìn. Tagh ìomhaigheag sam bith
  gus am Prìomh Bhàr-taoibh fhosgladh no a dhùnadh.
- **Primary Side Bar** nuair a tha e fosgailte, seallaidh e mion-fhiosrachadh mun ghnìomhachd a thagh thu.
- **Status Bar** aig bonn na sgrìn. Seallaidh e dè tha a’ tachairt.
- **Panel** raon fo na deasaichean teacsa airson fiosrachadh eile a thaisbeanadh.

Tagh ìomhaigheag crutha aig a’ mhullach dheis gus gin de na nithean seo fhosgladh no a dhùnadh.

## A’ Còdadh Leudachan Joomla

Gus leudachan a chruthachadh, ’s e an t-amas agad faidhle zip a chruthachadh as urrainn
dhut a stàladh air làrach Joomla a tha ag obair. Mar sin feumaidh tu pasgan airson
do chòd a chumail. Bu chòir seo a bhith taobh a-staigh an àite fhaidhlichean pearsanta
agad air an laptop no air a’ choimpiutair deasg agad a tha air a chleachdadh airson leasachadh
ionadail. Cha bu chòir dha a bhith ann an craobh na làraich-lìn agad. Mar eisimpleir,
dh’fhaodadh tu *~/jextensions* a chleachdadh gus fo-phasganan a chumail airson diofar leudachan.
Bidh mise a’ cleachdadh *~/git* oir tha e goirid agus furasta a litreachadh, ged a dh’fhaodadh
e troimh-chèile adhbhrachadh leis gu bheil gach fo-phasgan a’ cleachdadh stòras git fa leth.

### Còd Eisimpleir

Ma bu toil leat còd eisimpleir airson obrachadh air, tha leudachan ri fhaighinn
air GitHub leis an ainm *mod_debugme*. Mar a tha an t-ainm a’ ciallachadh, ’s e modal a th’ ann
anns a bheil cuid de bhugaichean. A bharrachd air còd a’ mhodail, tha faidhle
*build.xml* ann gus aon dòigh air togail a dhèanamh fèin-obrachail airson deuchainn
agus faidhle zip a chruthachadh a shealltainn.

Tha am modal air a dhealbhadh gus na beagan thachartasan (3 gu bunaiteach) a tha romhainn
(co-làithean breith) a shealltainn bho liosta a tha air a stòradh ann an clàr stòr-dàta.
Dh’fhaodadh tu smaoineachadh air seo ga chleachdadh ann an oifis no air làrach teaghlaich
le dùil ri cèic.

Is dòcha gur fheàrr tòiseachadh le bhith a’ cleachdadh àitheantan git bhon loidhne-àithne.
Cruthaich pasgan airson do chòd an toiseach agus an uair sin clon an
stòras iomallach:
```sh
    mkdir ~/git
    cd ~/git
    git clone https://github.com/ceford/j4xdemos-mod-debugme
```

Cha bu chòir don fhreagairt ach beagan dhiog a thoirt:
```sh
    Cloning into 'j4xdemos-mod-debugme'...
    remote: Enumerating objects: 23, done.
    remote: Counting objects: 100% (23/23), done.
    remote: Compressing objects: 100% (16/16), done.
    remote: Total 23 (delta 3), reused 23 (delta 3), pack-reused 0
    Unpacking objects: 100% (23/23), done.
```

Bu chòir dhut mionaid a ghabhail airson coimhead air susbaint a’ phasgain:
```sh
    cd j4xdemos-mod-debugme
    ls -al
    total 16
    drwxr-xr-x   6 ceford  staff   192  2 Sep 17:48 .
    drwxr-xr-x   3 ceford  staff    96  2 Sep 17:48 ..
    drwxr-xr-x  12 ceford  staff   384  2 Sep 17:48 .git
    -rw-r--r--   1 ceford  staff  1402  2 Sep 17:48 README.md
    -rw-r--r--   1 ceford  staff   927  2 Sep 17:48 build.xml
    drwxr-xr-x   8 ceford  staff   256  2 Sep 17:48 mod_debugme
```

Tha fiosrachadh mun stòras anns a’ phasgan *.git*. ’S e sgrìobhainn markdown a th’ anns an fhaidhle *README.md*
a tha a’ mìneachadh an stòrais seo. ’S e faidhle a th’ anns an fhaidhle *build.xml* a thathar a’ cleachdadh
gus an leudachan a thogail le inneal air an taobh a-muigh, Phing - air a mhìneachadh nas fhaide air adhart.
Tha còd an leudachain anns a’ phasgan *mod_debugme*.

### Stàlaich ann an Joomla

Dèan teannachadh air pasgan an leudachain gus faidhle zip a chruthachadh a ghabhas a stàladh:
```sh
    zip -r mod_debugme.zip mod_debugme
```

Faodaidh tu a-nis am faidhle zip a stàladh air an làrach Joomla a chleachdas tu airson deuchainn.
Às dèidh na stàlaidh, feumaidh tu modal Làraich a chruthachadh agus a shònrachadh do
shuidheachadh modal. Leis gur e modal briste a th’ ann, dh’fhaodadh tu a shònrachadh do
shuidheachadh air *All pages* fhad ’s a tha thu ag obair air; no dh’fhaodadh tu a shònrachadh
do shuidheachadh air aon duilleag; no dh’fhaodadh tu a chur ann an artaigil aig a bheil
nì clàr-taice aige fhèin.

Às dèidh na stàlaidh, sguab às am faidhle zip.

### Cuir Modh Deasbaid air

Ann an Rèiteachadh Cruinneil Joomla, suidhich *Debug System* gu *Yes* agus
*Error Reporting* gu *Maximum*.

Nuair a dh’fhosglas tu duilleag anns a bheil am modal lochtach, chì thu lorg
staca a dh’innseas dhut càit an deach mearachd a bhrosnachadh.

![lorg staca vscode](../../../en/images/test-installations/visual-studio-code-primer/01-vscode-primer-stack-trace.png)

Uaireannan tha am mearachd còdaidh air a’ chiad loidhne den lorg staca.
Air neo, ma thèid a’ mhearachd a bhrosnachadh ann an còd leabharlainn, mar
eisimpleir le bhith a’ cur dàta mì-dhligheach gu gnìomh stòr-dàta, dh’fhaodadh
gum bi am mearachd còdaidh nas fhaide sìos liosta nan gairmean gnìomh.

## Fosgail Pasgan an Leudachain ann an VS Code

Ann an VS Code, cleachd an nì clàr-taice File / Open Folder gus am pasgan anns a
bheil do lethbhreac ionadail de chòd an leudachain *mod_debugme* a lorg agus
fhosgladh. Bu chòir dhut rudeigin coltach ris na leanas fhaicinn:

![sealladh pasgain vscode](../../../en/images/test-installations/visual-studio-code-primer/02-vscode-primer-screen.png)

Dh’fhaodadh gum bi e comasach dhut an duilgheadas a dhearbhadh dìreach le bhith
a’ leughadh a’ chòd. A thaobh na mearachd *Class "DebugHelper" not found* chì thu
gun deach aithris *use* a chur ann am beachd beagan loidhnichean roimhe.
Is e mearachd chumanta rè leasachadh tùsail a th’ ann a bhith a’ dìochuimhneachadh
aithris *use* a chur a-steach!

Ceartaich an duilgheadas sin agus an uair sin dèan teannachadh air a’ mhodal agus
stàlaich a-rithist e. Bidh an ceum sin caran sgìtheil nuair a tha iomadh
duilgheadas agad. Seo far a bheil innealan togail feumail.

## Phing

’S e inneal loidhne-àithne a th’ ann am Phing, ri fhaighinn airson gach àrd-ùrlar,
a thathar a’ cleachdadh gus pasganan bathar-bhog a thogail a’ cleachdadh
stiùiridhean a tha air an stòradh ann am faidhle xml, leis an ainm
build.xml mar as àbhaist. Nuair a bhios tu ag obair le còd leudachain, faodar a
chleachdadh airson dà rud:

- faidhlichean atharraichte a chopaigeadh bhon phasgan stòr leudachain agad gu na
  h-àiteachan cheart ann am pasgan na làraich-lìn agad.
- faidhle zip ùr a chruthachadh airson stàlaidhean ùra.

Luchdaich sìos agus stàlaich Phing. Tha innealan togail eile
ri fhaighinn! Dh’fhaodadh tu Phing a stàladh sa phasgan bin agad fhèin no ann am
pasgan bin an t-siostaim. Feumaidh tu slighe a’ chòd Phing agad a thoirt fa-near.
San eisimpleir seo ’s e *~/bin/phing-latest.phar* a th’ ann. Faodaidh tu fheuchainn
bhon loidhne-àithne às dèidh dhut gluasad dhan phasgan anns a bheil còd an
leudachain agad:
```sh
    cd ~/git/j4xdemos-mod-debugme
    php ~/bin/phing-latest.phar
```

Freagairt:
```sh
    Buildfile: /Users/ceford/git/j4xdemos-mod-debugme/build.xml

    mod_debugme > main:
          ... Any copied files will be mentioned here
          [zip] Building zip: /Users/ceford/zips/mod_debugme.zip

    BUILD FINISHED

    Total time: 0.0863 seconds
```

## Gnìomhan VS Code

Gus Phing a ruith taobh a-staigh VS Code, feumaidh tu faidhle *tasks.json* a
chruthachadh sa phasgan *.vscode* aig freumh a’ phasgain
*j4xdemos-mod-debugme*. Mura h-eil am fear mu dheireadh ann, cruthaich e an
toiseach. An uair sin cruthaich am faidhle *tasks.json* agus cuir a-steach an
còd a leanas:
```json
    {
        // See https://go.microsoft.com/fwlink/?LinkId=733558
        // for the documentation about the tasks.json format
        "version": "2.0.0",
        "tasks": [
          {
            "label": "Build mod_debugme",
            "type": "shell",
            "command": "php ~/bin/phing-latest.phar",
            "windows": {
              "command": "php ~/bin/phing-latest.phar"
            },
            "group": "build",
            "presentation": {
              "reveal": "always",
              "panel": "shared"
            }
          }
        ]
    }
```

Feumaidh luchd-cleachdaidh Windows an àithne shònraichte do Windows a cheartachadh.
Faodaidh tu an leudachan a thogail a-nis le bhith a’ cleachdadh a’ chlàr-taice
*Terminal / Run Build Task*. Bu chòir toradh na h-àithne nochdadh ann am Pannal
an Terminal fon raon Deasaich.
```sh
      *  Executing task: php ~/bin/phing-latest.phar

    Buildfile: /Users/ceford/git/gitdemo/j4xdemos-mod-debugme/build.xml

    mod_debugme > main:

          [zip] Nothing to do: /Users/ceford/zips/mod_debugme.zip is up to date.

    BUILD FINISHED

    Total time: 0.1031 seconds

     *  Terminal will be reused by tasks, press any key to close it.
```

Dh’fhaodadh gum bi teachdaireachdan mearachd do-thuigsinn ann. Is e an adhbhar as
coltaiche gu bheil slighean mì-dhligheach gu pasganan anns an fhaidhle
*build.xml*, no nach deach pasgan a chruthachadh. Dìreach seòrsa eile de
dhuilgheadas ri dheasbad!

## Deasbad

Bu chòir dhut a bhith comasach air a’ chiad bhuga a cheartachadh le sgrùdadh a’
chòd. Feumaidh duilgheadasan nas toinnte dhut gluasad tron chòd ceum air cheum
leis an deas-bhugadair. Leigidh sin leat caochladairean a sgrùdadh gus faicinn a
bheil na luachan annta ris a bheil dùil agad, mar eisimpleir nuair a tha thu a’
cur argamaidean gu gnìomhan leabharlainn.

### Roghainnean *php.ini*

Gus deasbad a stèidheachadh le Xdebug, feumaidh tu cuid de dh’inntrigidhean a
chur aig mullach an fhaidhle *php.ini* agad.
```ini
    zend_extension="xdebug.so"
    xdebug.mode="debug"
    xdebug.client_port=9003
    xdebug.start_with_request = yes
```

An dèidh dhut atharrachaidhean sam bith a shàbhaladh, ath-thòisich am frithealaiche
Apache agad.

### Cuir Uinneag na Làraich-lìn ris

Chan eil anns a’ phasgan leudachain agad ach beagan fhaidhlichean, is iad sin
***stòran*** nam faidhlichean a chaidh a stàladh air an làrach-lìn agad. Tha
deasbad rè-ruith a’ gabhail a-steach puingean-briseadh a shuidheachadh ann am
faidhlichean na ***làraich*** agad, agus mar sin feumaidh cothrom a bhith agad air
na faidhlichean sin. Dh’fhaodadh tu an clàr-taice *File / Add Folder to
Workspace...* a chleachdadh gus pasgan na làraich a chur ris an Àite-obrach agad.
Ach tha deagh chothrom ann gun dèan thu atharrachaidhean air faidhlichean na
làraich an àite nam faidhlichean stòr. Mar sin, ’s dòcha gur fheàrr uinneag
VS Code fa leth fhosgladh airson deasbad.

- **Fosgail uinneag ùr:** Bhon chlàr-taice VS Code, tagh *File / New Window*
  agus tagh am pasgan anns a bheil làrach-lìn Joomla agad.
- **Fosgail pasgan:** Anns an uinneag a chaidh fhosgladh às ùr, tagh *File / Open
  Folder...* bhon chlàr-taice VS Code. Lorg pasgan na làraich-lìn agad agus tagh
  e. Bu chòir dhut liosta de na faidhlichean uile air làrach-lìn Joomla agad
  fhaicinn sa bhàr-taoibh Bhun-sgoile.

### Rèiteachadh Tòiseachaidh

Gus am bi deasbad ag obair dha-rìribh ann an VS Code, feumaidh tu rèiteachadh
tòiseachaidh. Aig freumh na làraich-lìn agad, cruthaich pasgan leis an ainm
*.vscode* (thoir fa-near a’ phuing aig an toiseach) anns a bheil faidhle leis an
ainm *launch.json* agus an t-susbaint a leanas:
```json
    {
        "configurations": [
            {
                "name": "Listen for XDebug",
                "type": "php",
                "request": "launch",
                "hostname": "0.0.0.0",
                "port": 9003,
                "stopOnEntry": true,
                "pathMappings": {
                    "/Users/ceford/Sites/j421rc2": "${workspaceFolder}"
                }
            }
        ]
    }
```

Cuimhnich an nì pathMappings san eisimpleir seo a chur an àite leis na
pathMappings fhèin air an làrach agad. Cuiridh an nì stopOnEntry stad air cur an
gnìomh aig a’ chiad loidhne de chòd PHP a thèid a chur an gnìomh.

### Dì-bhugachadh *mod_debugme*

A-nis tha thu deiseil airson na bugaichean sa mhodal stàlaichte a lorg agus a chàradh.

- **Lorg còd a’ mhòidil:** Lorg a’ chiad bhug air loidhne 16 de
  JROOT/modules/mod_debugme/mod_debugme.php.
- **Suidhich puing-bhrisidh:** Briog anns an àite air taobh clì an àireimh 16. Nochdaidh
  blàb dearg bàn nuair a thèid thu thairis air, agus tionndaidhidh e làn dhearg às dèidh
  dhut briogadh, a’ sealltainn gun deach puing-bhrisidh a shuidheachadh.
- **Tòisich dì-bhugachadh:** Bho chlàr-taice VS Code tagh *Run / Start Debugging*.
  Ath-luchdaich an làrach agad sa bhrobhsair. Bu chòir dhan uinneag VS Code agad nochdadh a-rithist
  leis a’ chòd air stad aig a’ chiad loidhne den fhaidhle *index.php* aig an làrach.
  Aig mullach na sgrìn tha ìomhaighean airson smachd a chumail air pròiseas an dì-bhugachaidh.
  Bu chòir dhaibh a bhith furasta an tuigsinn. Mura h-eil, coimhead suas iad ann an
  Help / Documentation VS Code.
- **Lean air adhart:** Tagh am putan leantainneachd - ruithidh an còd air adhart chun
  chiad phuing-bhrisidh agad. Dèan sgrùdadh air a’ chòd gus faicinn dè an duilgheadas a th’ ann.
- **Thoir an luchag thairis:** Ma thèid thu thairis air caochladair dhan deach luach a shònrachadh,
  nochdaidh Mola-sgrìn beag a’ toirt geàrr-chunntas air buadhan a’ chaochladair sin.
  Chan eil Mola-sgrìn ann airson caochladairean nach deach luachan a shònrachadh dhaibh.
- **Caochladairean:** Tha barrachd fiosrachaidh sa cholbh chlì mu staid a’ chòd aig a’ phuing-bhrisidh.
  Tha cus dhiubh ann airson an còmhdach an-seo. Rannsaich iad mar a bhios feum agad!
- **Cuir stad air dì-bhugachadh:** ’S dòcha gur fheàrr an ìomhaigh Lean air adhart a thaghadh;
  air neo thèid an duilleag-lìn a lìbhrigeadh bàn. Air neo eile, dh’fhaodadh tu am putan Stad
  no an clàr-taice Run / Stop Debugging a chleachdadh.

### Càraich Bug

**Cuimhnich:** Na càraich am bug ann an còd na làraich-lìn! Càraich e sa
chòd thùsail!

Càraich an còd tùsail agus an uair sin cleachd *Terminal / Run Build Task...*.

Tòisich dì-bhugachadh a-rithist.

### Molaidhean

Beagan dhuilgheadasan nach eil cho follaiseach:

- Càraichidh tu a’ chiad bug ach tuitidh e fhathast air an loidhne sin. Coimhead ann an
  mod_debugme.xml gus faicinn càit a bheil src nan clasaichean le namespace air a mhìneachadh.
  Nuair a bhios e air a chàradh san chòd thùsail, feumaidh tu am faidhle zip ath-stàladh no
  *administrator/cache/autoload_psr4.php* a sguabadh às. Nuair nach eil e ann, togaidh Joomla am
  faidhle sin a-rithist bho fhaidhlichean manifesto. Ach ma tha inntrigeadh ceàrr no a dhìth ann,
  cha tèid a chàradh gus an tèid an leudachan ath-stàladh.
- Uaireannan feumaidh tu puing-bhrisidh a shuidheachadh beagan loidhnichean ron loidhne
  far a bheil am mearachd a’ tachairt, gu h-àraidh ma tha thu airson sùil a thoirt air luachan a thèid
  a chur gu gairmean ghnìomhan.
- Chan eil an clàr *xxx.yyy\\debugme* ann. Ah seadh, cha deach an còd airson
  clàr a chruthachadh nuair a thèid a stàladh agus a thoirt air falbh nuair a thèid a dhì-stàladh
  a chruthachadh riamh. Feumaidh tu ceist SQL a ruith ann am phpMyAdmin a’ cleachdadh susbaint
  an fhaidhle *mod\\debugme.sql*. Cuimhnich *\#\\* atharrachadh ann an ainmean nan clàr
  airson ro-leasachan an stòr-dàta agad. Agus ma dh’fhàillig e fhathast, thoir sùil air ainm a’ chlàir
  sa chòd.

## Glacadh-sgrìn

Nuair a bhios a h-uile càil air a chàradh, seo na dh’fhaodadh tu fhaicinn:

![sealladh làraich a’ mhòidil air a dhì-bhugachadh ann an vscode](../../../en/images/test-installations/visual-studio-code-primer/03-vscode-primer-debugme-fixed.png)

Làithean cèic?

## Iomraidhean

Bho Sgrìobhainnean Joomla!: tha [Visual Studio Code](https://docs.joomla.org/Visual_Studio_Code) cuideachd a’ còmhdach rèiteachadh innealan eile, mar eisimpleir CodeSniffer agus PHPUnit.

*Air eadar-theangachadh le openai.com*

