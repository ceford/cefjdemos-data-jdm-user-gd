<!--
{
    "source": "https://docs.joomla.org/https:",
    "title": "Suidheachadh Docker",
    "description": " ",
    "author": ""
}
-->

## A’ Stèidheachadh Àrainneachd Joomla Ionadail a’ Cleachdadh Docker

Gus Joomla a ruith air a’ choimpiutair agad, tha feum air ceithir rudan: 
- frithealaiche-lìn a luchdachadh sìos agus a rèiteachadh, **Apache** no **nginx**, 
- seirbheis stòr-dàta mar **MySQL** no **MariaDB**, 
- agus, gu dearbh, tha feum againn air **PHP** 
- agus **Joomla.** 

Gus am bi na diofar phàirtean seo uile a’ conaltradh ri chèile, bidh a’ mhòr-chuid againn an urra ri bathar-bog pacaichte leithid **XAMPP**, **Laragon**, no **FlyEnv**.

Ach faodaidh suidheachaidhean thraidiseanta leantainn gu còmhstri puirt no frithealaichean stòr-dàta a dhiùltas tòiseachadh gu dìomhair. Nuair a thuiteas frithealaiche ionadail, is dòcha gum feum thu làraichean Joomla slàn a luchdachadh sìos agus ath-stàladh le làimh a-rithist ’s a-rithist dìreach airson aon PR a dhearbhadh, agus dh’fhaodadh tu do chuid obrach a chall fhad ’s a tha thu a’ càradh buga. Bidh seo a’ caitheamh ùine luachmhor, agus mar as trice chan eil anns na fuasglaidhean ach leigheasan sealach.

**An gluasad gu Docker ([Ionnsaich mu Docker](https://docs.docker.com/get-started/))** 
Le Docker, faodaidh tu an rèiteachadh làimhe a sheachnadh gu tur. An àite frithealaichean-lìn a stàladh gu dìreach air a’ choimpiutair agad, cha dèan thu ach aon fhaidhle “reasabaidh” a sgrìobhadh. Bidh Docker a’ luchdachadh sìos, a’ dealachadh agus a’ ceangal a h-uile càil sa chùlaibh gu fèin-obrachail. Ma bhriseas rudeigin, cha leig thu leas an suidheachadh slàn agad ath-stàladh; dìreach ath-thòisich an soitheach.

San stiùireadh seo, ionnsaichidh tu an dòigh as sìmplidhe air àrainneachd Joomla ionadail a ruith a’ cleachdadh Docker, gus an urrainn dhut nas lugha de ùine a chaitheamh a’ càradh frithealaichean agus barrachd ùine a chur ri tabhartasan.

### Riatanasan

Chan fheum thu ach aon rud a bhith air a stàladh mus tòisich sinn: **Docker Desktop**.

- Luchdaich sìos e bho [**docker.com**](https://www.docker.com/) agus ruith an stàlaichear
- Air Windows, fàg an roghainn “Use WSL 2 instead of Hyper-V” air a thaghadh - nì seo cùisean nas luaithe
- Fosgail Docker Desktop agus feitheamh gus am bi an oisean gu h-ìosal air an taobh chlì a’ sealltainn inbhe uaine **Engine running**.

![Docker Desktop](../../../en/images/hosting-local/docker-setup/01-docker-setup-desktop.png)

Sin agad e.

### Am faidhle docker-compose.yml

Nuair a tha feum agad air iomadh seirbheis a bhith a’ conaltradh ri chèile - leithid frithealaiche-lìn
(Apache/Nginx), PHP, agus stòr-dàta (MySQL/MariaDB) - bidh thu a’ cleachdadh faidhle orcastraidh sònraichte air a bheil `docker-compose.yml`. Bidh am faidhle seo na phlana airson a’ phròiseict agad, a’ mìneachadh nan seirbheisean uile a tha riatanach agus mar a bhios iad ag obair còmhla. (Tha ìomhaigh oifigeil Docker Joomla air a togail os cionn ìomhaigh PHP agus Apache. Tha seo a’ ciallachadh, le bhith a’ cleachdadh dìreach an aon ìomhaigh Joomla seo, gum faigh thu PHP, Apache agus Joomla uile air am pasgadh còmhla).

An toiseach, cruthaich pasgan ùr air a’ choimpiutair agad airson a’ phròiseict agad (mar eisimpleir, air an Deasg agad, cruthaich pasgan air a bheil `joomla-docker`).

Taobh a-staigh a’ phasgain sin, cruthaich faidhle teacsa ùr agus thoir an dearbh ainm seo air:

    docker-compose.yml

Fosgail am faidhle sin ann an deasaiche teacsa sam bith (leithid VS Code no Notepad), cuir a-steach an còd a leanas dìreach mar a tha e, agus sàbhail e:

```
    services:
      joomla:
        image: joomla:latest
        ports:
          - "8080:80"
        environment:
          - JOOMLA_DB_HOST=db
          - JOOMLA_DB_USER=joomla
          - JOOMLA_DB_PASSWORD=joomlapass
          - JOOMLA_DB_NAME=joomladb
        depends_on:
          - db
      db:
        image: mariadb:10.11
        environment:
          - MYSQL_ROOT_PASSWORD=rootpass
          - MYSQL_DATABASE=joomladb
          - MYSQL_USER=joomla
          - MYSQL_PASSWORD=joomlapass
        volumes:
          - db_data:/var/lib/mysql
    volumes:
      db_data:
```

### A’ Tòiseachadh na h-Àrainneachd

Fosgail an ceann-uidhe agad (no PowerShell air Windows), gluais dhan phasgan `joomla-docker` agad agus ruith:

```
    docker compose up -d
```

A’ chiad uair a ruitheas tu seo, luchdaichidh Docker sìos na h-ìomhaighean Joomla agus MariaDB, agus dh’fhaodadh gun toir seo mionaid no dhà a rèir astar an eadar-lìn agad. Às dèidh sin, bidh gach tòiseachadh às dèidh làimh cha mhòr sa bhad, mar a chì thu gu h-ìosal.

![Toradh tòiseachaidh docker sa cheann-uidhe](../../../en/images/hosting-local/docker-setup/02-docker-setup-terminal-transcript.png)

### Stàlaichear Joomla

Fosgail am brabhsair agad agus rach gu `http://localhost:8080`. Bu chòir dhut sgrìn stàlaidh Joomla fhaicinn.

![Ainm na làraich ann an suidheachadh stàlaichear Joomla](../../../en/images/hosting-local/docker-setup/03-docker-setup-joomla-installer-sitename.png)

Lìon a-steach ainm na làraich agad agus fiosrachadh an rianaire air a’ chiad sgrìn.

![Dàta logaidh a-steach stàlaichear Joomla](../../../en/images/hosting-local/docker-setup/04-docker-setup-joomla-installer-login-data.png)

Nuair a ruigeas tu an sgrìn **Rèiteachadh an Stòr-dàta**, seo far am faigh a’ mhòr-chuid de dhaoine greim:

**Na sgrìobh `localhost` mar ainm an òstair.**

Leis gu bheil an stòr-dàta a’ ruith na shoitheach fhèin, tha feum aig Joomla air ainm seirbheis an t-soithich — chan e localhost. Cleachd na luachan seo dìreach:

- **Seòrsa an Stòr-dàta:** MySQLi
- **Ainm an Òstair:** `db`
- **Ainm-cleachdaiche:** `joomla`
- **Facal-faire:** `joomlapass`
- **Ainm an Stòr-dàta:** `joomladb`

![Suidheachadh stòr-dàta stàlaichear Joomla](../../../en/images/hosting-local/docker-setup/05-docker-setup-joomla-installer-database-config.png)

Briog tro na ceumannan, cuir crìoch air an stàladh, agus sin agad e.

Nuair a bhios tu deiseil ag obair airson an latha, ruith `docker compose stop` gus na soithichean a chur nan stad agus cuimhne a shaoradh. Bidh an làrach agad dìreach far an do dh’fhàg thu i an ath thuras.

------------------------------------------------------------------------

### Cùisean Cumanta

- **Cha luchdaich an duilleag aig localhost:8080 dìreach às dèidh tòiseachaidh:** Bheir an soitheach stòr-dàta beagan dhiog gus crìoch a chur air a’ chiad shuidheachadh. Fuirich 30 diog agus ùraich an duilleag.
- **Tha port 8080 ga chleachdadh mu thràth:** Atharraich `"8080:80"` gu `"8081:80"` anns an fhaidhle compose agus faigh cothrom air aig `localhost:8081` na àite.
- **Thòisich na soithichean ach tha Joomla a’ sealltainn mearachd stòr-dàta:** Dèan sgrùdadh dùbailte gur e `db` an t-Ainm Òstair agad anns an stàlaichear agus nach e `localhost`.

### Pro-Tip: A’ faighinn cothrom air faidhlichean Joomla airson leasachaidh

An-dràsta, tha an làrach Joomla agad a’ ruith, ach tha na faidhlichean PHP fhèin
falaichte am broinn a’ chontaeinair Docker. Ma tha thu airson cur ri Joomla,
PRan a dhearbhadh, no na plugain agad fhèin a sgrìobhadh, feumaidh na faidhlichean
sin a bhith agad air a’ choimpiutair agad gus am fosgail thu iad ann an VS Code
no anns an deasaiche as fheàrr leat.

Gus na faidhlichean a shioncronachadh bhon chontaeinair dhan draibh chruaidh ionadail agad, chan eil agad ach
dà loidhne(`volumes: `) agus (`- ./site_joomla:/var/www/html`)
a chur ris an earrann `joomla` den fhaidhle `docker-compose.yml` agad mar a chithear gu h-ìosal:

```yml
services:
  joomla:
    image: joomla:latest
    ports:
      - "8080:80"
    volumes:
      - ./site_joomla:/var/www/html
    # ... (rest of your settings)
```

**Na nì seo:** 

An ath thuras a ruitheas tu `docker compose up -d`, cruthaichidh Docker gu fèin-obrachail
pasgan air a bheil `site_joomla` dìreach ri taobh an fhaidhle compose agad.
Dèan lethbhreac dhe phrìomh-chòd Joomla gu lèir (a’ gabhail a-steach deas-bhòrd an rianaire,
co-phàirtean agus teamplaidean) dhan phasgan sin.

![Rannsaichear IDE de stàladh Joomla ann an Docker](../../../en/images/hosting-local/docker-setup/06-docker-setup-ide-explorer.png)

Ùraichidh atharrachaidhean còd sam bith a nì thu sa phasgan sin air a’ choimpiutair agad sa bhad
am broinn a’ chontaeinair a tha a’ ruith! Tha thu a-nis làn-uidheamaichte airson leasachadh ionadail.

### Gliocas a Bharrachd 1: A’ dèanamh deuchainn air dreachan sònraichte de Joomla agus PHP

Nuair a bhios tu a’ dèanamh deuchainn air PRan, bidh luchd-gleidhidh gu tric ag iarraidh ort deuchainn a dhèanamh an aghaidh
dhreachan sònraichte de PHP. Le XAMPP, tha ìsleachadh no ùrachadh PHP na throm-laighe. Le Docker, cha toir e ach dà dhiog.

An àite `image: `**`joomla:latest`** a chleachdadh anns an
**`docker-compose.yml`** agad, faodaidh tu dreachan mionaideach a shònrachadh a’ cleachdadh tagaichean. Mar eisimpleir, ma dh’fheumas tu
deuchainn a dhèanamh air **Joomla 5.2** air **PHP 8.3**, dìreach atharraich
an aon loidhne sin gu: **`image: joomla:5.2-php8.3-apache`**

Ruith **`docker compose up -d`** a-rithist, agus atharraichidh Docker àrainneachd an fhrithealaiche agad sa bhad. Gheibh thu na tagaichean dreacha uile a tha rim faighinn air duilleag
<a href="https://hub.docker.com/_/joomla" class="ng-star-inserted"
target="_blank" rel="noopener" data-hveid="0"
data-ved="0CAAQ_4QMahgKEwjl8vi347CTAxUAAAAAHQAAAAAQkgI">oifigeil Joomla
Docker Hub</a>.

### Gliocas a Bharrachd 2: A’ cur phpMyAdmin ris

Ma tha thu a’ tighinn bho **XAMPP**, is dòcha gum bi thu ag ionndrainn eadar-aghaidh lèirsinneach
gus coimhead air an stòr-dàta agad. Faodaidh tu **phpMyAdmin** a chur ris an
rèiteachadh agad gu furasta le bhith a’ cur **bloc seirbheis** ùr ri bonn an
fhaidhle **`docker-compose.yml`** agad:

```yml
    phpmyadmin:
        image: phpmyadmin/phpmyadmin:latest
        ports:
          - "8081:80"
        environment:
          - PMA_HOST=db
        depends_on:
          - db
```

Ath-thòisich na soithichean agad, agus faodaidh tu a-nis faighinn gu phpMyAdmin le bhith a’ dol gu
**http://localhost:8081** sa bhrobhsair agad. Dìreach log a-steach le **`joomla`**
mar an t-ainm-cleachdaiche agus **`joomlapass`** mar am facal-faire.

*Air eadar-theangachadh le openai.com*

