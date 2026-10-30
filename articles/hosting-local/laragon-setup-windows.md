<!--
{
    "source": "https://docs.joomla.org/https:",
    "title": "Laragon airson Windows",
    "description": " ",
    "author": ""
}
-->

## A’ stèidheachadh àrainneachd Joomla ionadail a’ cleachdadh Laragon

’S e inneal aotrom airson Windows a th’ ann an Laragon a bhios a’ làimhseachadh Apache, MySQL agus PHP ann an aon stàladh shìmplidh. Chan eil feum air faidhlichean rèiteachaidh no stèidheachadh làimhe - dìreach luchdaich a-nuas e, ruith e agus tòisich air Joomla a thogail/deuchainn. Faic an t-artaigil seo ann an Iris Choimhearsnachd Joomla: [Laragon: Am frithealaiche AMP furasta, àrd-choileanaidh airson Windows](https://magazine.joomla.org/all-issues/october-2025/laragon-the-effortless,-high-performance-amp-server-for-windows).

Bheir an stiùireadh seo thu bho thoiseach tòiseachaidh gu làrach Joomla ionadail a tha ag obair, agus còmhdaichidh e cuideachd cùis bheag san eadar-aghaidh san tionndadh as ùire a tha furasta a chàradh nuair a thuigeas tu dè tha a’ tachairt.

### A’ luchdachadh a-nuas agus a’ stàladh Laragon

Gus tòiseachadh, theirig dhan [duilleag oifigeil luchdachadh a-nuas Laragon](https://laragon.org/download). Luchdaich a-nuas an tionndadh Laragon Full (v8.6.1 aig an àm seo), oir tha a h-uile càil a dh’fheumas tu ann (mar Apache, MySQL agus na tionndaidhean PHP as ùire) dìreach às dèidh a’ stàlaidh.
Air neo, faodaidh tu an [stàlaichear](https://github.com/leokhoa/laragon/releases/download/8.6.1/laragon-wamp.exe) a luchdachadh a-nuas gu dìreach.

Nuair a bhios am faidhle `.exe` air a luchdachadh a-nuas, dèan briogadh dùbailte air gus an stàladh a thòiseachadh.

**Nòta mu Windows Defender:** Leis gur e inneal cumhachdach do luchd-leasachaidh a th’ ann an Laragon, dh’fhaodadh Windows Defender SmartScreen casg a chur air bho bhith a’ tòiseachadh agus sgrìn rabhaidh ghorm a shealltainn. Tha seo àbhaisteach - dìreach briog air **Barrachd fiosrachaidh**, agus an uairsin briog air a’ phutan **Ruith co-dhiù** a nochdas aig a’ bhonn.

![laragon setup windows protected warning](../../../en/images/hosting-local/laragon-setup-windows/01-laragon-setup-windows-protected-warning.png)

Briog troimhe san draoidh stàlaidh. Tha na roghainnean bunaiteach ceart gu leòr, ach cùm sùil air an dà mhion-fhiosrachadh chudromach seo:

1.  **Àite a’ Chinn-uidhe:** Fàg am pasgan stàlaidh mar
    `C:\laragon`. Ma stàlaicheas tu e domhainn am broinn do `Program Files` no `Documents`, dh’fhaodadh sin duilgheadasan ceadachaidh adhbhrachadh nas fhaide air adhart.
2.  **Roghainnean an Stèidheachaidh:** Dèan cinnteach gu bheil am bogsa-seic **Auto virtual hosts** air a thaghadh. ’S e seo am feart a bheir seòladh glan don làrach Joomla ionadail agad (mar `http://myjoomla.test`) an àite seòladh IP lom.

![laragon setup options](../../../en/images/hosting-local/laragon-setup-windows/02-laragon-setup-options.jpg)

Nuair a bhios an stàladh deiseil, ath-thòisich an coimpiutair agad. (brosnaichidh draoidh an stàlaicheir thu gus an aon rud a dhèanamh)

### A’ tòiseachadh an fhrithealaiche agad agus ceadan a’ bhalla-teine

Fosgail Laragon bhon chlàr-taice Start agad agus briog air a’ phutan **Start All**.

Leis gur e seo a’ chiad turas a tha thu a’ ruith frithealaiche ionadail, feumaidh Windows dearbhadh gu bheil e sàbhailte. Chì thu brosnachaidhean bho Windows Defender Firewall a’ nochdadh, ag iarraidh cothrom lìonraidh airson seirbheisean mar **Apache HTTP Server**, **MySQL** agus **Mailpit**.

- Dìreach briog air **Ceadaich cothrom** anns gach aon de na brosnachaidhean seo.

Nuair a bhios iad ceadaichte, tòisichidh Laragon an àrainneachd ionadail agad. Bidh fios agad gu bheil e ag obair nuair a chì thu àireamhan puirt Apache agus MySQL a’ nochdadh ann an uinneag Laragon.

### An duilgheadas “A’ ruith mu thràth” (agus mar a chàraicheas tu i)

Nuair a bhios tu deiseil ag obair, dh’fhaodadh tu briogadh air “Stop All” gus Apache agus MySQL a chur dheth, agus an uairsin briogadh air an “X” san oisean gu h-àrd air an làimh dheis gus uinneag Laragon a dhùnadh.

Seo an duilgheadas: cha chuir briogadh air an “X” Laragon sìos gu tur. Cumaidh e air a’ ruith gu sàmhach sa chùlaibh. Ma dh’fheuchas tu ris an aplacaid Laragon fhosgladh a-rithist bhon chlàr-taice Start no bhon deasg agad, chì thu rabhadh buidhe san oisean gu h-ìosal air an làimh dheis den sgrìn agad a tha ag ràdh:
**“Tha Laragon a’ ruith mu thràth!”**

![laragon setup already running notice](../../../en/images/hosting-local/laragon-setup-windows/03-laragon-setup-already-running-notice.png)

**An Ribe:** Ma bhriogas tu air an “X” air an rabhadh beag buidhe sin gus a dhùnadh, falbhaidh prìomh uinneag Laragon cuideachd, agus cha bhi cothrom agad tuilleadh air a’ phannal smachd. (Nòta: Uaireannan dh’fhaodadh uinneag bheag ceadachais nochdadh cuideachd agus an eadar-aghaidh a reothadh san aon dòigh).

**Am Fuasgladh:** Ma thèid an eadar-aghaidh agad à sealladh no ma reothaicheas e, chan fheum thu ach am pròiseas sa chùlaibh a dhùnadh le forsa agus tòiseachadh às ùr. Tha e glè shìmplidh:

1.  Brùth `Ctrl + Shift + Esc` air a’ mheur-chlàr agad gus **Manaidsear Gnìomhan Windows** fhosgladh.
2.  Coimhead (Lorg) airson **Laragon** anns an liosta de phròiseasan a tha a’ ruith.
3.  Dèan briogadh deas air agus tagh **Cuir crìoch air a’ ghnìomh**.

Sin agad e! Tha thu air am pròiseas sa chùlaibh a bha steigte a mharbhadh gu sàbhailte. Faodaidh tu Laragon fhosgladh bhon chlàr-taice Start agad a-nis, agus luchdaichidh e gu foirfe, a’ toirt cothrom dhut briogadh air “Start All” gun mhearachdan.

### A’ Làimhseachadh nam Pop-upan Ceadachais (Na Sgrionaichean “Nag”)

Tha Laragon saor airson a chleachdadh ann an leasachadh agus deuchainn
neo-mhalairteach gun cheadachas a cheannach. Ach, às dèidh dhut an aplacaid
a chleachdadh greis, tha coltas ann gun nochd iarrtas “License Key” gad
bhrosnachadh gus taic a thoirt don phròiseact.

Leis gu bheil thu a’ cleachdadh an tionndaidh shaor, faodaidh tu na
sgrionaichean seo a dhùnadh gun duilgheadas, ach tha sreath shònraichte
de thachartasan ri shùileachadh:

1.  Nochdaidh prìomh uinneag **License Key** thairis air an
    eadar-aghaidh Laragon agad. Briog air an teacsa **Close** no air an ‘X’.<br>
    ![uinneag iuchair ceadachais rè stèidheachadh laragon](../../../en/images/hosting-local/laragon-setup-windows/04-laragon-setup-license-key-window.png)

2.  Dìreach às dèidh dhut a dùnadh, nochdaidh dàrna pop-up
    **Warning**, a’ cur nad chuimhne gu bheil Laragon a’ ruith gun
    cheadachas. Briog air **OK** no air an ‘X’.<br>
    ![rabhadh gun cheadachas rè stèidheachadh laragon](../../../en/images/hosting-local/laragon-setup-windows/05-laragon-setup-no-license-warning.png)

3.  Nuair a dhùineas tu an dàrna rabhadh sin, dh’fhaodadh Laragon do
    bhrabhsair-lìn fhosgladh gu fèin-obrachail agus do chur air ais gu
    `https://laragon.org/key`. Faodaidh tu an taba sin sa bhrabhsair a
    dhùnadh.
4.  Nuair a thilleas tu dhan eadar-aghaidh Laragon agus a bhriogas tu air
    **Start All** gus an frithealaiche agad a thòiseachadh a-rithist,
    dh’fhaodadh gum feum thu briogadh tro na h-aon dà pop-up sin a-rithist.

Às dèidh dhut an dùnadh an dàrna turas seo, falbhaidh na pop-upan, agus
bidh thu gu tur saor Laragon a chleachdadh!

*(Nota: Ma reòthas an eadar-aghaidh Laragon agad aig àm sam bith rè nan
pop-upan seo agus nach gabh briogadh air, dìreach cuimhnich air cleas
`Ctrl + Shift + Esc` Manaidsear nan Gnìomhan bhon cheum roimhe gus am
pròiseas cùlaibh a chur gu crìch agus tòiseachadh às ùr)*

### A’ Cruthachadh Stòr-dàta airson Joomla

Mus stàlaich thu Joomla, feumaidh tu stòr-dàta bàn gus an dàta aige a
stòradh. Tha manaidsear stòir-dàta togte aig Laragon air a bheil
HeidiSQL, agus mar sin tha a h-uile rud a dh’fheumas tu ann mu thràth.

1.  Dèan cinnteach gu bheil na seirbheisean Laragon agad a’ ruith (briog air **Start All**).
2.  Briog air a’ phutan **Database** air prìomh eadar-aghaidh Laragon.
3.  Fosglaidh uinneag Session Manager. Lìonaidh Laragon na teisteasan
    ionadail bunaiteach dhut gu fèin-obrachail (Cleachdaiche: `root`, Facal-faire:
    *\[fàg bàn\]*).
4.  Briog air a’ phutan **Open** aig a’ bhonn.<br>    
    **Fuasgladh dhuilgheadasan: Mearachd “Access denied for user 'root'@'localhost'”:
    ** Ma bhriogas tu air a’ phutan **Open** agus ma gheibh thu mearachd
    ceangail sa bhad, na gabh dragh! Mar as trice tha seo a’ ciallachadh
    gu bheil prògram MySQL eile (mar XAMPP no MySQL Workbench) a’ ruith
    sa chùlaibh, agus gu bheil e a’ cur bacadh air ruigsinneachd Laragon
    air port an stòir-dhàta (Port 3306).<br>
    ![fuasgladh duilgheadas ruigsinneachd rè stèidheachadh laragon](../../../en/images/hosting-local/laragon-setup-windows/06-laragon-setup-troubleshooting.jpg)

    **Am Fuasgladh:**
    1.  Brùth iuchair Windows, sgrìobh **Services**, agus brùth Enter.
    2.  Sgrolaich sìos an liosta gus **MySQL**, **MySQL80**, no **MariaDB** a lorg.
    3.  Dèan briogadh deas air an t-seirbheis a tha a’ ruith agus tagh **Stop**.
    4.  Till gu Laragon, briog air **Stop All**, an uair sin **Start All**, agus
        feuch ri briogadh air **Open** ann an Session Manager a-rithist. Bu chòir
        dha ceangal gun mhearachd sam bith.
5.  Nuair a bhios tu air ceangal soirbheachail a dhèanamh agus a-staigh ann
    am manaidsear stòir-dàta HeidiSQL, seall air a’ cholbh air an taobh chlì.
    Dèan briogadh deas air ainm an fhrithealaiche (mar as trice air a
    chomharrachadh mar `Laragon.MySQL` no `127.0.0.1`).
6.  Cuir an luchag os cionn **Create new**, agus tagh **Database**.
7.  Nochdaidh iarrtas beag. Sgrìobh ainm sìmplidh airson an stòir-dhàta agad
    san raon “Name” (mar eisimpleir: `joomla_dev`). Faodaidh tu an
    clàr-taice “Collation” fhàgail air an t-suidheachadh bhunaiteach aige.
8.  Briog air **OK**.

Chì thu an stòr-dàta ùr agad a’ nochdadh san liosta air an taobh chlì. Sin
e! Faodaidh tu uinneag manaidsear an stòir-dhàta a dhùnadh gu tur a-nis.

### A’ Faighinn na Faidhlichean Joomla agad

A-nis gu bheil an frithealaiche agus an stòr-dàta agad deiseil, tha an t-àm
ann na faidhlichean Joomla a chur nan àite. Tha mar a nì thu seo an urra gu
tur ri na tha thu airson a choileanadh leis an t-suidheachadh ionadail seo:

**Dòigh 1: Airson Làrach-lìn Inbheach a Thogail** Ma tha thu dìreach airson
làrach-lìn a thogail no leudachain fheuchainn, feumaidh tu an sgaoileadh
seasmhach àbhaisteach.

- Rach gu [duilleag luchdachadh sìos Joomla](https://downloads.joomla.org) 
  oifigeil agus luchdaich sìos am faidhle `.zip` **Pacaid Shlàn** as ùire.

**Dòigh 2: Airson PRan Coimhearsnachd a Dhearbhadh (Deuchainn Phaisdean)** Ma
tha an t-amas agad a’ choimhearsnachd a chuideachadh le bhith a’ dearbhadh
paisean agus Iarrtasan Tarraing, feumaidh tu pasgan ro-thogte anns a bheil an
còd as ùire buileach.

- **An Togail Oidhcheil:** Luchdaich sìos am faidhle `.zip` Togail Oidhcheil
  as ùire bho [Togalaichean Oidhcheil](https://developer.joomla.org/nightly-builds.html).
  Thèid iad sin a chruthachadh gach oidhche agus tha iad air leth freagarrach
  airson an cleachdadh leis a’ cho-phàirt Joomla Patch Tester.
- **Am Pasgan PR Ro-thogte:** Air neo, ma tha thu a’ dèanamh deuchainn air
  PR sònraichte air GitHub, sgrolaich gu bonn duilleag an PR, briog
  **Seall a h-uile sgrùdadh**, agus coimhead airson a’ cheangail
  **Luchdaich sìos pacaidean ro-thogte**.
  ![ceangal pacaid ro-thogte ann an suidheachadh laragon](../../../en/images/hosting-local/laragon-setup-windows/07-laragon-setup-prebuilt-package-link.png)

**Dòigh 3: Airson Còd Bunaiteach a Chur Ris** Ma tha thu an dùil còd a
sgrìobhadh agus na h-Iarrtasan Tarraing agad fhèin a chur a-steach, feumaidh
tu an còd tùsail amh, gun cho-chruinneachadh.

- Clònaich [stòr-dàta GitHub Joomla CMS](https://github.com/joomla/joomla-cms)
  gu dìreach dhan àrainneachd Laragon agad a’ cleachdadh Git.
- *Cudromach:* Cha ruith clòn amh GitHub sa bhad - Feumaidh tu Terminal
  Laragon fhosgladh agus `composer install` agus `npm ci` a ruith am broinn
  a’ phasgain agad gus na h-eisimeileachdan PHP agus na so-mhaoin CSS/JS a
  thogail. (Leis gun do stàlaich thu an tionndadh Làn de Laragon, tha
  Composer agus NPM air an stàladh air an t-siostam agad mu thràth).

### **A’ Cur nam Faidhlichean ann an Laragon:**

Ge bith dè an dòigh a thagh thu, ’s e seo an dearbh phròiseas gus na
faidhlichean a ruith ann an Laragon:

1.  Fosgail eadar-aghaidh Laragon agus briog air a’ phutan **Root**. Fosglaidh
    seo am pasgan `C:\laragon\www` air a’ choimpiutair agad gu fèin-obrachail.
2.  Taobh a-staigh a’ phasgain `www` seo, cruthaich pasgan ùr airson do
    phròiseict. Cùm ainm a’ phasgain sìmplidh, ann an litrichean beaga, agus
    gun bheàrnan (mar eisimpleir: `joomla_dev` no `joomla_pr_test`).
3.  Cuir na faidhlichean Joomla agad am broinn a’ phasgain ùir seo. (Ma
    luchdaich thu sìos `.zip` ann an Dòigh 1 no 2, thoir a-mach a h-uile
    susbaint gu dìreach dhan phasgan seo. Ma tha thu a’ cleachdadh Git ann an
    Dòigh 3, clònaich an stòr-dàta dhan phasgan seo).
4.  Leis gun do chuir thu an comas “Auto virtual hosts” rè an stàlaidh,
    cleachdaidh Laragon ainm a’ phasgain agad gu fèin-obrachail gus seòladh
    lìn ionadail a chruthachadh. Mar sin, bidh pasgan leis an ainm
    `joomla_dev` ruigsinneach sa bhrobhsair agad aig
    `http://joomla_dev.test`.
    <br>
    **Gliocas: Cùm Na h-Àrainneachdan agad Glan:** ’S e deagh bheachd a th’ ann
    pasganan eadar-dhealaichte a chruthachadh airson diofar thionndaidhean
    Joomla no deuchainnean PR sònraichte (m.e., aon phasgan leis an ainm
    `joomla5_stable` agus fear eile leis an ainm `joomla4_dev`). Ruithidh
    Laragon iad uile gu toilichte taobh ri taobh le na URLan `.test` glan aca
    fhèin, a’ cur casg air do chòd agus na stòran-dàta agad a bhith air am
    measgachadh!
    <br>
    ![pasganan pròiseict ann an suidheachadh laragon](../../../en/images/hosting-local/laragon-setup-windows/08-laragon-setup-project-folders.png)

## A’ Ruith Stàlaichear Joomla

Tha an stòr-dàta agad agad, agus tha na faidhlichean Joomla agad nan suidhe
anns a’ phasgan ùr aca (mar eisimpleir, `C:\laragon\www\joomla_dev`). A-nis
tha an t-àm ann Joomla a stàladh dha-rìribh!

**Ceum Deatamach: Ath-luchdaich Apache!** Ma bha Laragon a’ ruith mu thràth
fhad ’s a chruthaich thu am pasgan pròiseict ùr agad, chan eil fios aig
Laragon fhathast gu bheil am pasgan ann.

- Fosgail eadar-aghaidh Laragon.

- Briog air **“Reload”** gu h-àrd air an làimh dheis. *(Bheir seo air Laragon
  am pasgan `www` a sganadh agus an seòladh ùr
  `http://joomla_dev.test` a chruthachadh).*

**A’ Cur Crìoch air an t-Suidheachadh:**

1.  Fosgail am brabhsair-lìn agad agus sgrìobh URL do phròiseict a chaidh a
    chruthachadh gu fèin-obrachail (m.e., `http://joomla_dev.test`).
2.  Bu chòir dhut duilleag Stàlaichear Lìn Joomla fhaicinn sa bhad.
3.  Tagh do chànan agus cuir a-steach ainm airson do làrach Joomla.
4.  Suidhich do chunntas Sàr-chleachdaiche (cuimhnich air na mion-fhiosrachadh
    logaidh a-steach seo, bidh feum agad orra gus faighinn gu deas-bhòrd
    rianaire Joomla!).
5.  Air an sgrìn **Rèiteachadh an Stòir-dhàta**, cuir a-steach teisteanasan
    stòr-dàta Laragon a chruthaich thu na bu tràithe:
    - **Seòrsa an Stòir-dhàta:** `MySQLi` (Bun-bheachdail)
    - **Ainm an Òstair:** `localhost`
    - **Ainm-cleachdaiche:** `root`
    - **Facal-faire:** *\[Fàg seo gu tur bàn\]*
    - **Ainm an Stòir-dhàta:** An dearbh ainm a chuir thu a-steach ann an
      HeidiSQL na bu tràithe (m.e., `joomla_dev`).
    ![roghainnean stòir-dàta stàlaichear joomla ann an suidheachadh laragon](../../../en/images/hosting-local/laragon-setup-windows/09-laragon-setup-joomla-installer-database.png)

6.  Briog air **Stàlaich Joomla.**

Nuair a bhios am bàr adhartais deiseil, chì thu teachdaireachd soirbheachais -
faodaidh tu a-nis briogadh air **Fosgail an Làrach** gus an làrach-lìn
ionadail bheò agad fhaicinn, no air **Fosgail an Rianaire** gus logadh a-steach
do chùlaibh Joomla.

Sin agad e - tha an làrach Joomla ionadail agad beò agus deiseil airson a
chleachdadh.

*Air eadar-theangachadh le openai.com*