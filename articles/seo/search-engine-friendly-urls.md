<!--
{
    "source": "https://docs.joomla.org/Search_Engine_Friendly_URLs",
    "title": "URLan c\u00e0irdeil do dh\u2019innseanan-luirg",
    "description": " ",
    "author": ""
}
-->

## Slighean agus Ròtaichean

Tha URLan SEF a’ dèanamh ciall do dhaoine agus do dh’innseanan-luirg oir tha iad a’ mìneachadh na slighe chun na duilleige shònraichte ris a bheil iad a’ comharrachadh. ’S e **slighe** àite faidhle ann an craobh eòlairean, no a shamhladh ann an còd. Taobh a-staigh, canar **ròta** ris a’ phàirt ionadail de URL SEF (am pàirt às dèidh ainm an àrainn). Mar sin, canar **ròtaigeadh** ri cruthachadh agus giullachd URLan SEF, agus canar **ròtaiche** ris a’ chòd iomchaidh.

Gabhaidh URLan càirdeil do dh’innseanan-luirg a chur an gnìomh leis na ceumannan a leanas:
* Ann an **Rèiteachadh Cruinneil**
    - suidhich an roghainn **URLan Càirdeil do dh’Innnseanan-luirg** gu **Tha**.
    - Suidhich an roghainn **Cleachd Ath-sgrìobhadh URL** gu **Tha**
    - Roghainneil: Suidhich an roghainn **Cuir Iar-leasachan ri URL** gu **Tha**.
* Ann am freumh na làraich, ath-ainmich htaccess.txt gu .htaccess ma tha thu a’ cleachdadh frithealaiche Apache, no coimhead ris na sgrìobhainnean air an taobh a-muigh airson NginX no frithealaichean eile.

Chithear eisimpleir de ròtaigeadh anns a’ bhuaidh mheudachaidh a tha aig na h-atharrachaidhean seo air URL duilleag Bloga Roinn-seòrsa **Articles** anns an dàta shampaill.

- Nuair a tha URLan SEF air an tionndadh dheth ann an Rèiteachadh Cruinneil agus .htaccess ciorramach, tha an URL rudeigin mar `https://www.example.com/index.php?option=com_content&view=category&layout=blog&id=16&Itemid=125` agus tha na slighean-briosgaidh a’ sealltainn:<br>
 *Tha thu an seo: Dachaigh / Cruthan Sampaill / Articles*
- Nuair a tha URLan SEF air an cur air, ach gun ath-sgrìobhadh URL, bidh e:
  `https://www.example.com/index.php/sample-layouts/articles`
- Nuair a tha URLan SEF air, Ath-sgrìobhadh URL air agus .htaccess an comas, bidh e
  `https://www.example.com/sample-layouts/articles.html` (Iar-leasachan a chur ri URL
  suidhichte gu Tha).

## Àireamhan ann an URLan nach eil SEF

Anns a’ phàirt den URL a tha ag ràdh `id=16&Itemid=125`, tha na paramadairean a tha riatanach gus an URL a-staigh a lorg agus an duilleag a tha a dhìth a shealltainn. Anns a’ chùis seo, ’s e a’ chiad àireamh ID de Roinn-seòrsa agus ’s e an dàrna àireamh ID nì clàr-taice Bloga na Roinne-seòrsa airson na Roinne-seòrsa sin.

*Air eadar-theangachadh le openai.com*