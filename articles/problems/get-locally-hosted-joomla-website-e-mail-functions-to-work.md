<!--
{
    "source": "https://docs.joomla.org/Get_locally_hosted_Joomla!_website_e-mail_functions_to_work",
    "title": "Post-d an \u00d2stair Ionadail",
    "description": " ",
    "author": ""
}
-->

## Òstadh Ionadail

Bidh a’ mhòr-chuid de ISPan a’ bacadh port 25, mar sin chan urrainn dhut post-d a chur bhon
t-seirbheisiche SMTP air a’ choimpiutair agad fhèin. Tha seo airson spamaichean a bhacadh. Mura h-eil
thu an dùil spama a chur, faodaidh tu frithealaiche puist-d an ISP agad a chleachdadh.

Gus gnìomh a’ phuist-d bhon t-seirbheisiche SMTP ISP agad a chleachdadh fiù ’s ma tha thu
a’ òstadh an làraich Joomla agad fhèin air a’ choimpiutair agad fhèin, clàraich a-steach don làrach Joomla agad
mar Shàr-chleachdaiche agus rach gu taba **Server** na duilleige **Global
Configuration**. Anns an earrann **Mail** bu chòir don dàta agad a bhith mar a leanas:

    Post-d on: someone@example.com (mar as trice thusa)
    Ainm on: SomeName

    Prògram puist: SMTP
    Òstair SMTP: smtp.charter.net (Ge b’ e dè a dh’innseas an ISP agad dhut a chleachdadh airson na frithealaichean SMTP aca)
    Slighe Sendmail: /usr/sbin/sendmail
    Port SMTP: 25
    Tèarainteachd SMTP: STARTTLS
    Dearbhadh SMTP: Tha (no Chan eil)
    Ainm-cleachdaiche SMTP: johndoe (ainm-cleachdaiche aig tè de na cunntasan puist-d agad leis an ISP agad)
    Facal-faire SMTP: trr33459 (facal-faire aig tè de na cunntasan puist-d agad leis an ISP agad)
Cuir teachdaireachd dheuchainn gus dearbhadh gu bheil e ag obair.

Tha Ainm-cleachdaiche SMTP, Facal-faire agus Òstair nan SMTP nan aon raointean ’s a chuireas tu a-steach nuair a chuireas tu
Cunntas Outlook Express, no Eudora, no teachdaiche puist-d sam bith a chleachdas tu
air a’ choimpiutair agad.

Dh’fhaodadh gum bi duilgheadasan agad le leudachain a dh’atharraicheas an seòladh *From*
anns na puist-d a thathar a’ cur a-mach. Mar eisimpleir, bidh an leudachan ProjectFork
uaireannan a’ cur phuist-d mar gum biodh iad a’ tighinn bhon neach a tha os cionn
a’ phròiseict. Faodaidh seo duilgheadas adhbhrachadh oir cha leig cuid de na frithealaichean SMTP ISP
le seòladh “from” nach eil a’ freagairt ris an ainm-cleachdaiche (m.e.
Rogers ann an Canada). Gheibh thu teachdaireachd mar seo:
“PHPMAILER_FROM_FAILEDname@whatever.com.” ’S e fuasgladh a th’ ann dèanamh cinnteach
gun cleachd thu seòladh puist-d dligheach bhon ISP agad an-còmhnaidh airson do luchd-cleachdaidh.

*Air eadar-theangachadh le openai.com*