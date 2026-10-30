<!--
{
    "source": "https://docs.joomla.org/Installing_Joomla!_using_BitNami_Joomla!_stack",
    "title": "St\u00e0ladh Bitnami",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

**NOTA:** Chan eil stac BitNami Joomla! ri fhaighinn tuilleadh mar stàlaichear fa leth.
An àite sin, tha e ri fhaighinn mar: 1) Eisimpleir stèidhichte air sgòth, 2) Ann an soitheach, an dara cuid
Kubernetes no Docker, no 3) Inneal mas-fhìor. Ruithidh an t-inneal mas-fhìor air
an t-siostam-obrachaidh agad ann an hypervisor leithid Virtual Box no VMware Player.
Tha e fhathast a’ tighinn leis na h-eisimeileachdan riatanach uile, mar a bha san stàlaichear fa leth.

Chan eil Roghainn 1 gu h-àrd iomchaidh tuilleadh. Cuideachd, ann an Roghainn 2, tha BitNami Lamp Stack nas fhaide
sìos ri fhaighinn san sgòth no mar inneal mas-fhìor. Co-dhiù, tha Bitnami a’ dèanamh
stàladh ionadail de Joomla! a tha ag obrachadh gu math furasta agus coileanta.

Faodaidh tu an tionndadh as ùire den phasgan Bitnami airson Joomla! airson
Windows, Linux agus Mac a luchdachadh a-nuas aig <a href="http://bitnami.org/stack/joomla"
rel="nofollow noreferrer noopener">http://bitnami.org/stack/joomla</a>.

**Feumar ath-sgrùdadh!**

Tha BitNami Joomla! Stack na stàlaichear uile-ann-aon a tha ga dhèanamh furasta
Joomla a stàladh air a’ choimpiutair agad. Tha e saor, furasta a chleachdadh agus
fèin-sheasmhach. Tha sin a’ ciallachadh gu bheil e a’ cruinneachadh agus a’ rèiteachadh
gu fèin-obrachail gach pìos bathair-bhog (eisimeileachd) a tha riatanach gus Joomla a ruith
airson adhbharan leasachaidh no riochdachaidh, a’ gabhail a-steach Apache HTTP Server, MySQL
agus PHP.

## Roghainn 1: Stac Joomla! (Air a mholadh)

Tha an dòigh seo a’ gabhail ris gu bheil
àrainneachd (**W**indows/**L**inux/**M**ac)...**AMP**(Apache HTTP Server, MySQL, &
PHP) agad air a stàladh mu thràth.

### A’ stàladh Joomla! Stack

Ge bith dè an siostam-obrachaidh a tha thu a’ ruith (Windows / Linux /
Mac), tha am pròiseas stàlaidh mar an ceudna.

Luchdaich a-nuas an tionndadh as ùire de Joomla! Stack bhon
<a href="http://bitnami.org/stack/joomla"
rel="nofollow noreferrer noopener">làrach-lìn BitNami</a>.

Lorg an stàlaichear a luchdaich thu a-nuas (bidh ainm an fhaidhle coltach ri
bitnami-joomla-VERSION-linux-installer.run. Briog dùbailte air an ìomhaigheag gus
an stàlaichear a chur air bhog.

Ma tha Linux agad, feumaidh tu ceadan so-ghnìomhaichte a thoirt don
fhaidhle an toiseach, a’ cleachdadh na h-àithne seo:

chmod +x /path/to/bitnami-joomla-VERSION-linux-installer.run

<img src="https://docs.joomla.org/images/a/a0/Joomla_welcome2.png"
decoding="async" data-file-width="614" data-file-height="538"
width="614" height="538" alt="Suidheachadh Joomla Bitnami lampstack" />

Briog air "Air adhart".

<img src="https://docs.joomla.org/images/5/5f/Joomla_components2.png"
decoding="async" data-file-width="614" data-file-height="538"
width="614" height="538" alt="Co-phàirtean Joomla Bitnami lampstack" />

Tagh na co-phàirtean a tha thu airson an stàladh. Mura h-eil thu cinnteach,
fàg na co-phàirtean bunaiteach air an taghadh. Briog air "Air adhart" nuair a
bhios tu deiseil.

<img src="https://docs.joomla.org/images/0/0a/Joomla_directory2.png"
decoding="async" data-file-width="614" data-file-height="538"
width="614" height="538" alt="Eòlaire stàlaidh Joomla Bitnami lampstack" />

A-nis faighnichidh e càit a bheil thu airson am prògram a stàladh. Thoir seachad
an t-àite far a bheil thu airson stac BitNami Joomla! a stàladh agus briog air
"Air adhart" nuair a bhios tu deiseil.

<img src="https://docs.joomla.org/images/3/3c/Joomla_userdata2.png"
decoding="async" data-file-width="614" data-file-height="538"
width="614" height="538" alt="Cunntas rianaire Joomla Bitnami lampstack" />

Thèid an t-ainm-cleachdaiche agus am facal-faire a bheir thu seachad an-seo a
chleachdadh gus cunntas rianaire a chruthachadh ann an Joomla! Briog air
"Air adhart" nuair a bhios tu deiseil.

<img src="https://docs.joomla.org/images/8/8b/Joomla_sitename2.png"
decoding="async" data-file-width="614" data-file-height="538"
width="614" height="538" alt="Ainm làraich Joomla Bitnami lampstack" />

Sgrìobh a-steach an t-ainm a tha thu airson a chleachdadh airson do làrach
Joomla, agus briog air "Air adhart".

<img src="https://docs.joomla.org/images/d/dd/JoomlaReadytoinstall2.png"
decoding="async" data-file-width="614" data-file-height="538"
width="614" height="538" alt="Joomla Bitnami lampstack Deiseil airson a stàladh2" />

Leigidh an stàlaichear leat cunntas puist-d a rèiteachadh gus an urrainn do
Joomla! brathan a chur tro phost-d. Briog air "Air adhart".

<img src="https://docs.joomla.org/images/9/9d/JoomlaCopyingfiles2.png"
decoding="async" data-file-width="614" data-file-height="538"
width="614" height="538" alt="Joomla Bitnami lampstack A’ dèanamh lethbhreac de na faidhlichean" />

Fuirich mionaid fhad ’s a tha an stàlaichear a’ dèanamh lethbhreac de na
faidhlichean agus a’ rèiteachadh an stàlaidh Joomla! agad.

<img src="https://docs.joomla.org/images/e/ea/Joomlafinalscreen2.png"
decoding="async" data-file-width="614" data-file-height="538"
width="614" height="538" alt="Sgrìn dheireannach Joomla Bitnami lampstack" />

Tha Joomla! a-nis air a rèiteachadh agus deiseil airson a chleachdadh. Briog air
"Crìochnaich" gus an aplacaid a chur air bhog.

<img src="https://docs.joomla.org/images/8/8d/JoomlaManager.png"
decoding="async" data-file-width="784" data-file-height="586"
width="784" height="586" alt="Joomla Bitnami lampstack A’ stiùireadh frithealaichean" />

Tha e furasta inneal a’ mhanaidseir a chleachdadh gus na frithealaichean Apache
agus MySQL a thòiseachadh/a stad.

<img
src="https://docs.joomla.org/images/7/73/Joomlaapplicationscreen2.png"
decoding="async" data-file-width="982" data-file-height="729"
width="982" height="729" alt="Sgrìn aplacaid Joomla" />

’S urrainn dhut stòr-dàta Joomla! a stiùireadh gu furasta le phpMyAdmin.

<img src="https://docs.joomla.org/images/f/f3/JoomlaphpMyAdmin.png"
decoding="async" data-file-width="982" data-file-height="751"
width="982" height="751" alt="Sgrìn phpMyAdmin" />

## Roghainn 2: BitNami LAMPStack agus Joomla!

### Dè th’ ann am BitNami LAMPStack?

’S e pasgan an-asgaidh, furasta a stàladh, a th’ ann am BitNami LAMPStack a
chuireas ri chèile gach pìos bathair-bhog (eisimeileachd) a tha riatanach gus
àrainneachd LAMP (Apache, MySQL agus PHP airson Linux) a chur air chois agus a
ruith airson adhbharan leasachaidh no riochdachaidh. Tha e fèin-sheasmhach, chan
eil e a’ dèanamh atharrachaidhean sam bith air an t-siostam agad agus faodar a
dhì-stàladh gu furasta. ’S urrainn dhut an tionndadh as ùire de BitNami
LAMPStack airson Linux a luchdachadh a-nuas aig
<a href="http://bitnami.org/stack/lampstack"
rel="nofollow noreferrer noopener">http://bitnami.org/stack/lampstack</a>.
Tha <a href="http://bitnami.org/stack/wampstack"
rel="nofollow noreferrer noopener">tionndadh Windows</a>
agus <a href="http://bitnami.org/stack/mampstack"
rel="nofollow noreferrer noopener">tionndadh OS X</a> rim faighinn cuideachd.

Ge bith dè an siostam-obrachaidh a tha thu a’ ruith (Windows / Linux /
Mac), tha am pròiseas stàlaidh mar an ceudna.

### A’ stàladh BitNami LAMPStack

Lorg an stàlaichear a luchdaich thu a-nuas bhon làrach-lìn BitNami (bidh
ainm an fhaidhle coltach ri
bitnami-lampstack-VERSION-linux-installer.run). Dèan briogadh dùbailte air an ìomhaigheag gus an stàlaichear a chur air bhog.

<img src="https://docs.joomla.org/images/1/14/Lampstack_welcome.png"
decoding="async" data-file-width="516" data-file-height="391"
width="516" height="391" alt="Fàilte Bitnami lampstack" />

Briog air "Air adhart".

<img src="https://docs.joomla.org/images/7/78/Lampstack_directory.png"
decoding="async" data-file-width="516" data-file-height="391"
width="516" height="391" alt="Pasgan Bitnami lampstack" />

A-nis faighnichidh e dhut càit a bheil thu airson am prògram a stàladh. Tagh an
t-àite air an inneal agad agus briog air "Air adhart" nuair a bhios tu deiseil.

<img src="https://docs.joomla.org/images/2/22/Lampstack_passwd.png"
decoding="async" data-file-width="516" data-file-height="391"
width="516" height="391" alt="Facal-faire Bitnami lampstack" />

Cuir a-steach am facal-faire root MySQL agad. Is e seo am facal-faire airson an
cleachdaiche "root" airson an stòr-dàta.

<img
src="https://docs.joomla.org/images/7/72/LampstackReadytoinstall.png"
decoding="async" data-file-width="516" data-file-height="391"
width="516" height="391" alt="Bitnami lampstack deiseil airson a stàladh" />

Tha an stàlaichear a-nis deiseil airson tòiseachadh air a’ phròiseas stàlaidh. Briog
air "Air adhart".

<img src="https://docs.joomla.org/images/1/19/LampstackCopyingfiles.png"
decoding="async" data-file-width="516" data-file-height="391"
width="516" height="391" alt="Bitnami lampstack a’ dèanamh lethbhreac de na faidhlichean" />

Fuirich mionaid fhad ’s a nì an stàlaichear lethbhreac de na faidhlichean agus a
rèiticheas e an stàladh LAMPStack agad.

<img src="https://docs.joomla.org/images/b/bc/Lampstackfinalscreen.png"
decoding="async" data-file-width="516" data-file-height="391"
width="516" height="391" alt="Sgrìn dheireannach Bitnami lampstack" />

Tha BitNami LAMPStack a-nis air a stèidheachadh agus deiseil airson a chleachdadh. Briog air "Crìochnaich" gus an aplacaid a chur air bhog.

### A’ stàladh Joomla! le làimh

Lean an stiùireadh a tha air a mhìneachadh san artaigil  A’ stàladh
Joomla.

*Air eadar-theangachadh le openai.com*