<!--
{
    "source": "https://docs.joomla.org/jdocmanual?manual=user&heading=help&filename=administrator-help.md",
    "title": "Cobhair an Rianaire",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Tha bàr-inneal anns cha mhòr a h-uile duilleag Rianaire Joomla anns a bheil
putan **Cobhair** faisg air bàrr deas na duilleige. Chan eil bàr-inneal, agus mar
sin chan eil putan Cobhair, aig na Deas-bhùird a-mhàin.

Tha putan aig iomadh duilleag cuideachd air a bheil **Tog Cobhair Amalaichte**
. Bidh seo dìreach a’ sealltainn no a’ falach tuairisgeul raoin ma tha fear
ri fhaighinn. ’S e an t-adhbhar aige loma-làn na duilleige a lùghdachadh ach
uidheam cuimhneachaidh a thoirt seachad far am biodh sin feumail. Cha tèid
dèiligeadh ris a-rithist an-seo.

Bidh am putan **Cobhair** a’ fosgladh uinneag ùr a’ cleachdadh URL a tha
freumhaichte sa phutan. Eisimpleir:
```
data-url="https://help.joomla.org/proxy/index.php?keyref=Help51:Articles&lang=en"
```

Anns a’ chùis seo, tha susbaint na duilleige Cobhair a’ tighinn bho thùs
bhon taobh a-muigh.

## Stòr na Cobhair - làrach MediaWiki

’S e MediaWiki am bathar-bog a chleachdas WikiPedia. ’S e pasgan Bathar-bog
Saor is Stòr Fosgailte (FOSS) a th’ ann a chleachdas PHP agus MySQL, dìreach mar
Joomla. ’S urrainn dhut a luchdachadh a-nuas agus a stàladh thu fhèin. Ann an
teòiridh, dh’fhaodadh tu an t-seirbheisiche Cobhair agad fhèin a chruthachadh
agus sin a chleachdadh an àite an t-Seirbheisiche Cobhair choitcheann Joomla.
Ann an cleachdadh, feumaidh fios a bhith agad gu bheil feum aig duilleagan
MediaWiki air beagan giullachd gus am bi iad freagarrach airson an taisbeanadh
mar dhuilleagan Cobhair.

Seo far a bheil an **proksi** a’ tighinn a-steach. Bidh e a’ faighinn na
duilleige a tha a dhìth bho stàladh MediaWiki agus ga ullachadh airson a
taisbeanadh mar dhuilleag Cobhair. Chì thu duilleag MediaWiki thùsail san
eisimpleir seo aig https://docs.joomla.org/Help5.x:Articles agus ’s urrainn dhut
a dheasachadh ma chì thu rudeigin ceàrr.

## URL na Cobhair Choitcheann

Tha caochladair `$helpurl` anns an fhaidhle **configuration.php** ann am freumh
stàlaidh Joomla:

```
$helpurl = 'https://help.joomla.org/proxy/index.php?keyref=Help{major}{minor}:{keyref}&lang={langcode}';
```

Nuair a thèid putan Cobhair a thaghadh, thèid gach nì sna camagan lùbach a
chur na àite. Is iad na luachan {major} agus {minor} na roghainnean tionndaidh
airson do stàlaidh. ’S e {langcode} còd a’ chànain Rianaire a thagh thu an-dràsta,
a dh’fhaodadh a bhith en, de no fr.

’S e an caochladair {keyref} ainm-faidhle duilleige air an t-seirbheisiche
Cobhair, às aonais an raoin-ainm aige. Mar sin, airson na duilleige Articles ’s e
*Articles* an t-ainm-faidhle iomchaidh.

**Nota:** ’S e `https://docs.joomla.org/` an làrach airson duilleagan Cobhair a
dheasachadh. Ach ’s e `https://help.joomla.org/proxy` an làrach airson duilleagan
Cobhair fhaighinn air ais.

Chan eil dòigh ann URL bunaiteach an t-seirbheiseir Cobhair atharrachadh o
fhoirmean Rèiteachadh Coitcheann an Rianaire, ach ’s urrainn dhut atharrachadh
le deasaiche teacsa.

Seo an liosta iomlan de na còdan ionaid a tha rim faighinn:

| Còd          | Thèid seo a chur na àite                                                         |
|---------------|--------------------------------------------------------------------------------|
| {app}         | Ainm an aplacaid (m.e. “Rianaire” ann an ceann-cùil Joomla CMS)             |
| {component}   | Ainm na co-phàirt (m.e. “com_content” ann am Manaidsear nan Artaigilean)                     |
| {keyref}      | Iomradh iuchrach sgrìn na Cobhair (às dèidh a dhol tron t-siostam eadar-theangachaidh)       |
| {major}       | Àireamh prìomh ath-sgrùdaidh Joomla (m.e. “5” ann an Joomla 5.6).                         |
| {minor}       | Àireamh bheag ath-sgrùdaidh Joomla (m.e. “1” ann an Joomla 5.1)                          |
| {maintenance} | Àireamh ath-sgrùdaidh cumail suas Joomla (m.e. “3” ann an Joomla 5.1.1).                 |
| {language}    | Còd slàn a’ chànain (m.e. “en-GB”)                                              |
| {langcode}    | Pàirt taga cànain a’ chòd chànain (m.e. “en” mas e “en-GB” an còd slàn) |
| {langregion}  | Pàirt taga roinne na còd chànain (m.e. “GB” mas e “en-GB” an còd slàn)   |

## Cobhair Choitcheann san Àm ri Teachd

Tha cleachdadh làraich MediaWiki airson duilleagan Cobhair a lìbhrigeadh na
eallach caran mòr dhaibhsan a tha a’ cumail suas na sgrìobhainnean, agus
dh’fhaodadh an dòigh-obrach atharrachadh san àm ri teachd. Ma thachras
atharrachadh, tha e coltach gum bi an stòr air a dhèanamh suas de fhaidhlichean
HTML ro-thogte a gheibhear thuige le atharrachadh sìmplidh air àrainn stòir
$helpurl.

## Cobhair Ionadail do Cho-phàirtean Gnàthaichte

Ma tha co-phàirt ghnàthaichte agad agus ma tha thu comhfhurtail le deasachadh
còd tùsail php agus cruthachadh susbaint, ’s urrainn dhut na duilleagan Cobhair
fa leth agad fhèin a chruthachadh. Gabh co-phàirt Jdocmanual mar eisimpleir.
Mar cho-phàirt ghnàthaichte, chan eil duilleagan Cobhair air làrach MediaWiki
docs.joomla.org. Chan eil cead aig co-phàirtean treas-phàrtaidh duilleagan
Cobhair a fhrithealadh às an sin.

Thoir sùil air a’ chriomag chòd seo bho administrator/components/com_jdocmanual/src/View/Manual/ViewHtml.php:
```
        $tmpl = $app->input->getCmd('tmpl');
        if ($tmpl !== 'component') {
            ToolbarHelper::help('jdocmanual', true);
        }
```

Tha sònrachadh na gairm ToolbarHelper::help mar a leanas:
```
@param $ref: The name of the target file (excluding the file extension).
@param $useComponent: Use the help file in the component directory.
@param $url: Use this URL instead of any other.
@param $component: Name of component to get Help (null for current component)
function Toolbar::help(
    string $ref,
    bool $useComponent = false,
    string $url = null,
    string $component = null
): HelpButton
Writes a help button for a given option (opens a popup window).
```

San eisimpleir seo, ’s e ainm-faidhle a th’ ann an **$ref** airson a chleachdadh,
sa chùis seo `'jdocmanual'` (feumaidh e a bhith a’ freagairt ri litrichean mòra
is beaga an fhaidhle thargaid) agus tha **$useComponent** na `true`, a’ ciallachadh
gum bi an duilleag Cobhair a thèid a chleachdadh suidhichte taobh a-staigh
faidhlichean na co-phàirte aig
administrator/component/com_jdocmanual/help/en-GB/jdocmanual.html

Bu chòir cleachdadh faidhle Cobhair taobh a-staigh na co-phàirte a bhith a’
ciallachadh nach bi Cobhair a-riamh a dhìth agus gur dòcha gum bi i an-còmhnaidh
suas chun latha.

## Cuideachadh Iomallach airson Co-phàirt Ghnàthaichte

Nuair a chruthaicheas tu am putan Cuideachaidh, dh’fhaodadh tu $useComponent = false a shuidheachadh agus an URL a shuidheachadh gus comharrachadh gu àite sònraichte air an làrach agad fhèin no air làrach iomallach.

```
    ToolbarHelper::help('jdocmanual', false, 'http://example.com/help/en-GB/jdocmanual.html');
```

Mar sin, chan eil a dhìth ach duilleag HTML leis an ainm cheart san àite cheart.

*Air eadar-theangachadh le openai.com*