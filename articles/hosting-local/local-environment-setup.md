<!--
{
    "source": "https://docs.joomla.org/J4.x:Setting_Up_Your_Local_Environment",
    "title": "Suidheachadh na h-\u00c0rainneachd Ionadail",
    "description": " ",
    "author": ""
}
-->

Bho Joomla! 4 tha sinn air am pròiseas leasachaidh atharrachadh. Chan eil e
comasach tuilleadh an tasg-lann a chlonadh agus stàladh Joomla a bhith agad
a ghabhas cleachdadh.
Bidh sinn a’ leantainn nan cleachdaidhean as fheàrr agus a’ cur pròiseas
togail an gnìomh airson an CMS.

## Iùl Tòiseachaidh Luath

Tha na ceumannan airson an àrainneachd leasachaidh agad a shuidheachadh an
eisimeil an t-siostaim-obrachaidh agad. Chan urrainn dhuinn sgrìobhainnean a
sgrìobhadh airson gach siostam-obrachaidh (OS), mar sin cleachd an t-einnsean
lorg as fheàrr leat gus HowTo a lorg.

### Innealan a dh’fheumas tu

1.  PHP - gu bunaiteach an aon rud ’s a dh’fheumas tu airson làrach Joomla a ruith, ach
    feumaidh tu an tionndadh PHP CLI (eadar-aghaidh na loidhne-àithne).
    (Faic duilleag [A’ rèiteachadh frithealaiche LAMPP airson leasachadh PHP](https://docs.joomla.org/Special:MyLanguage/Configuring_a_LAMPP_server_for_PHP_development "Duilleag Special:MyLanguage/Configuring a LAMPP server for PHP development").)
2.  Composer - airson eisimeileachdan PHP Joomla a stiùireadh. Airson cuideachadh
    le stàladh Composer, leugh na sgrìobhainnean
    aig <a href="https://getcomposer.org/doc/00-intro.md" class="external free"
    target="_blank"
    rel="nofollow noreferrer noopener">https://getcomposer.org/doc/00-intro.md</a>.
3.  Node.js - airson faidhlichean JavaScript agus SASS Joomla a chur ri chèile. Airson cuideachadh
    le stàladh Node.js, lean an stiùireadh a tha ri fhaighinn
    aig <a href="https://nodejs.org/en/" class="external free" target="_blank"
    rel="nofollow noreferrer noopener">https://nodejs.org/en/</a>. Thoir fa-near,
    bidh feum agad air NodeJS 12 no nas àirde gus Joomla a stàladh.
4.  Git - airson tionndaidhean a stiùireadh.

### Ceumannan gus an Àrainneachd Ionadail a Shuidheachadh

1.  Clon an tasg-lann
2.  Dèan checkout air meur na sgaoilidh as ùire.
3.  Ruith `composer install` (composer = manaidsear phacaidean airson PHP) à
    freumh an tasg-lainn git. (Faodaidh tu *--ignore-platform-reqs* a chur ris mura
    h-eil PHP-LDAP agad air a stàladh gu h-ionadail, agus mura bheil feum agad air.)
4.  Ruith `npm ci` (npm = manaidsear phacaidean airson JavaScript, tha am
    paramadair “ci” a’ ciallachadh “stàladh glan”) à freumh an tasg-lainn git.
    (Thoir fa-near, feumaidh tu npm 10.1.0 no nas àirde airson seo.
    Ruith `npm install -g npm@lts` gus an tionndadh npm agad ùrachadh chun
    tionndaidh LTS.)

Faodaidh luchd-cleachdaidh Linux agus OSX an ailias bash a leanas a shuidheachadh
le bhith a’ cur na leanas am broinn an fhaidhle *~/.bashrc*:

```
    alias jclean="rm -rf administrator/templates/atum/css; \
    rm -rf templates/cassiopeia/css; \
    rm -rf administrator/templates/system/css; \
    rm -rf templates/system/css; \
    rm -rf media/; \
    rm -rf node_modules/; \
    rm -rf libraries/vendor/; \
    rm -f administrator/cache/autoload_psr4.php; \
    rm -rf installation/template/css"
    alias jinstall="jclean; composer install; npm ci"
```

Sguabaidh seo às na faidhlichean uile a chaidh an cur ri chèile san t-siostam agad agus
ruithidh e stàladh ùr mar aon àithne le bhith a’ gairm `jinstall` am broinn
an stàlaidh Joomla agad.

## Iùl Tòiseachaidh Beagan Nas Fhaide

Tha Joomla coltach ri mòran innealan-lìn eile an-diugh. Tha pàirt mhòr PHP
aige agus tha barrachd is barrachd còd JavaScript aige. Ged nach eil
uiread de dh’ullachadh a dhìth airson còdadh PHP, tha feum aig JavaScript
air tòrr innealan mun cuairt air. ’S e am prìomh adhbhar nach eil duine a’ sgrìobhadh
còd ann an dòigh a thuigeas gach brabhsair, agus mar sin feumar an còd
atharrachadh bho, mar eisimpleir, ES6 gu tionndadh co-fhreagarrach de
JavaScript. Tha an aon rud fìor airson CSS. Airson Joomla tha sinn a’ cleachdadh
SASS agus thèid seo atharrachadh gu CSS dùthchasach gus am bi brabhsair sam bith
ga thuigsinn. Air an taobh eile, tha suidheachadh àrainneachd leasachaidh
beagan nas toinnte, ach tha na h-innealan a’ dèanamh còdadh nas goireasaiche.
Taing do luchd-faire agus ath-luchdadh fèin-obrachail a’ bhrabhsair, chì thu na
h-atharrachaidhean agad ann an àm fìor.

### PHP

Bu chòir gum biodh e gu leòr `composer install` a ruith, oir stàlaichidh seo
na h-eisimeileachdan PHP a chaidh a shàbhaladh anns an fhaidhle
*composer.lock*. Faodaidh tu seo a dhèanamh cho tric ’s a thogras tu. Cha stàlaich
e ach pacaidean ùra nuair a thèid am faidhle *composer.lock* atharrachadh.
Na ruith `composer update`, oir ùraichidh seo na pacaidean uile gu tionndaidhean
nas ùire agus ùraichidh e am faidhle *composer.lock*.

**Nota:** Dh’fhaoidte gum feum thu `composer install` a ruith leis an roghainn
`--ignore-platform-reqs` gus na riatanasan àrd-ùrlair a tha
sònraichte ann an Composer a leigeil seachad. Is e sin, mura h-eil an
leudachan LDAP aig PHP agad air a stàladh.

### Sgriobtaichean Node/npm

Tha Node.js a’ tighinn le manaidsear phacaidean air a bheil NPM (ann an cuid de
dhòighean coltach ri Composer). Tha àithne `run` aig NPM agus tha sinn air
cuid de sgriobtaichean ullachadh gus do bheatha a dhèanamh nas fhasa. Feumaidh
tu na h-àitheantan a ruith à freumh an tasg-lainn nuair a tha thu air faidhlichean
JS no SASS atharrachadh. Roimhe seo dh’fheumadh tu `npm ci` a ruith aon turas,
gus na h-eisimeileachdan a stàladh.

#### npm run build:css (suas gu Joomla 6.1)

Cuiridh seo faidhlichean SASS ri chèile gu CSS agus cruthaichidh e na faidhlichean
lùghdaichte cuideachd.

#### npm run build:js (suas gu Joomla 6.1)

Cuiridh seo na faidhlichean JavaScript ri chèile agus atharraichidh e iad chun
chruth cheart, agus cruthaichidh e faidhlichean lùghdaichte.

#### Bho Joomla 6.2 cleachd na h-àitheantan a leanas:

- npm run build -- -n <extension> gus leudachan sònraichte ath-thogail 
- ruith npm run builders-list gus ainm an leudachain a lorg
- npm run build -- --all gus gach nì ath-thogail

## Cùisean a dh’fhaodadh èirigh

Nuair a bhios tu a’ ruith composer install, dh’fhaodadh na mearachdan seo nochdadh

```
    Problem 1
        - Installation request for joomla/ldap 2.0.0-beta -> satisfiable by joomla/ldap[2.0.0-beta].
        - joomla/ldap 2.0.0-beta requires ext-ldap * -> the requested PHP extension ldap is missing from your system.
    Problem 2
        - Installation request for symfony/ldap v5.1.5 -> satisfiable by symfony/ldap[v5.1.5].
        - symfony/ldap v5.1.5 requires ext-ldap * -> the requested PHP extension ldap is missing from your system.
```

’S e am fuasgladh composer install a ruith leis an
roghainn `--ignore-platform-reqs` gus na riatanasan àrd-ùrlair
a chaidh sònrachadh ann an Composer a leigeil seachad. ’S e sin, mura
h-eil leudachan LDAP PHP agad air a stàladh.

```
    composer install --ignore-platform-reqs
```

Ma gheibh thu mearachd logaidh a-steach mar a chithear gu h-ìosal, sguab às am faidhle
`administrator/cache/autoload_psr4.php`.

![sgrìn mearachd logaidh a-steach Joomla 4](../../../en/images/hosting-local/local-environment-setup/01-joomla-4-login-error-screen.png)

*Air eadar-theangachadh le openai.com*