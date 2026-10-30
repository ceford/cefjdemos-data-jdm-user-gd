<!--
{
    "source": "https://docs.joomla.org/J5.x:Managing_Mail_Template_Layout",
    "title": "Teamplaidean Puist-d",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Bithear a’ cleachdadh Teamplaidean Puist-d gus teachdaireachdan puist-d an t-siostaim a chur ann an **teacsa lom** no **HTML**, no an dà chuid, mar a thagh thu san fhoirm *Roghainnean: Teamplaidean Puist-d*. Mura tèid ach aon dòigh a thaghadh, cha bhi an dòigh eile an làthair ann am foirm deasachaidh na teachdaireachd. 

Tha an dealbh-sgrìn a leanas a’ sealltainn taghadh de na 26 Teamplaidean Puist-d choitcheann a tha rim faighinn. Gheibhear an liosta le bhith a’ taghadh **Siostam -> Teamplaidean Puist-d** bho chlàr an Rianaire,

![liosta nan teamplaidean puist-d](../../../gd/images/templates/mail-templates/01-mail-templates-list.png)

Faodar na teachdaireachdan puist-d a ghnàthachadh gus cruth, coltas agus briathrachas atharrachadh a rèir feumalachdan na làraich agad. Mar eisimpleir, ’s dòcha gum bu toil leat suaicheantas agus sgeama dhathan na làraich agad a chleachdadh anns na puist-d a chuirear gu luchd-ceannach. Chan eil gnàthachadh nam post-d a chuirear gu rianairean cho cudromach. 

Tha dà dhòigh ghnàthachaidh ann: tro *Roghainnean: Teamplaid Puist-d* airson gach teamplaid puist-d, agus tro *Roghainnean Puist-d a rèir Teamplaid*.

## Roghainnean: Teamplaidean Puist-d

Tagh am putan **Roghainnean** ann am bàr-inneal liosta nan *Teamplaidean Puist-d* gus cothrom fhaighinn air roghainnean iomlan nan teamplaidean puist-d. Tagh am putan *Tog Cuideachadh In-loidhne* gus faicinn a bheil cuideachadh a bharrachd aig gin de na raointean foirm.

![roghainnean nan teamplaidean puist-d](../../../gd/images/templates/mail-templates/02-mail-templates-options.png)

### Cruth a’ Phuist-d

Thoir fa-near gum faod neach-faighinn cleachdaiche puist-d a shuidheachadh gus HTML shìmplidh no Teacsa Lom a chleachdadh, gus luchdachadh sìos dhealbhan a sheachnadh. Mar sin, ’s dòcha gum bi e nas fheàrr an *Cruth Puist-d* a shuidheachadh gu *Teacsa lom* no *An dà chuid*.

### Roghainnean Puist-d a rèir Teamplaid

Ma tha seo air a shuidheachadh gu **Tha**, bidh taba *Roghainnean* a bharrachd aig foirmean deasachaidh fa leth nan teamplaidean puist-d, a leigeas leat roghainnean puist-d na teamplaide sin atharrachadh agus, ma thogras tu, lethbhreac (BCC) a chur gu seòladh puist-d sònraichte, fhad ’s a tha an raon **Cuir Lethbhreac** an seo air a shuidheachadh gu **Comasach** cuideachd.

## Foirm Deasachaidh na Teamplaide

Ann an liosta nan Teamplaidean Puist-d, faodaidh tu teamplaid sam bith a thaghadh airson a dheasachadh. Bheir an ceangal Tiotail thu gu foirm deasachaidh na teamplaide Shasannaich bhunaidh. Tha gach bratach na cheangal ris an aon teamplaid sa chànan sin.

### An taba Post-d

![foirm deasachaidh teamplaid puist-d](../../../gd/images/templates/mail-templates/03-mail-template-edit.png)

Tha susbaint nan raointean Cuspair agus Bodhaig air a stòradh ann an teudan cànain an toiseach. Nì seo e furasta *Ath-shuidhich gu Cuspair Bunaiteach* no *Bodhaig* a thaghadh. Ach, aon uair ’s gu bheil teamplaid puist-d sònraichte air a dheasachadh, thèid na raointean Cuspair agus Bodhaig aige a stòradh sa chlàr `#__mail_templates`. 

’S e tagaichean-àite a th’ anns na nithean eadar cromagan lùbach, agus thèid fìor luachan a chur nan àite nuair a thèid am post-d a chur. San eisimpleir gu h-àrd, bhiodh `{SITENAME}` mar ainm sam bith a thagh thu airson na làraich agad. Bhiodh `{Method}` mar dhòigh còmhdhail a’ phuist a chaidh a thaghadh: `PHP Mail`, `Sendmail` no `SMTP`.

Bidh na tagaichean-àite a tha rim faighinn ag atharrachadh bho phost gu post. Dh’fhaodadh tu na tagaichean-àite gnàthaichte agad fhèin a chur ris, ach feumaidh sin plugan gnàthaichte, air a mhìneachadh ann an [artaigil na h-iris](https://magazine.joomla.org/all-issues/february-2025/joomla-5-email-templates-how-to-add-variables-via-plugin) bhon Ghearran 2025.

### An taba Roghainnean

Chan eil an taba seo an làthair ach ma tha *Roghainnean Puist-d a rèir Teamplaid* air a shuidheachadh gu *Tha* ann an *Roghainnean: Teamplaidean Puist-d*. Tha an dealbh gu h-ìosal a’ sealltainn dealbh-sgrìn le *Roghainnean Puist-d* air an suidheachadh gu *Chan eil*. Ma thèid an suidheachadh gu *Tha*, nochdaidh barrachd raointean foirm a nì ath-sgrìobhadh air na roghainnean puist-d a chaidh a shuidheachadh ann an Rèiteachadh na Cruinne, taba an Fhrithealaiche.

![foirm deasachaidh teamplaid puist-d](../../../en/images/templates/mail-templates/04-mail-template-edit-options.png)

Ma tha thu airson lethbhreac dall (BCC) de phost-d a tha a’ dol a-mach a chur gu seòladh puist-d sònraichte, faodaidh tu a chur a-steach san raon *Cuir Lethbhreac gu Post-d*.

## Ath-sgrìobhaidhean Teamplaidean Puist-d

Gus ath-sgrìobhadh teamplaid puist-d a chruthachadh taobh a-staigh teamplaid gnàthaichte:

1. Rach gu Siostam -> Teamplaidean na Làraich -> Fosgail an teamplaid agad (m.e., Cassiopeia).
2. Anns an taba Cruthaich Ath-sgrìobhaidhean, tagh joomla -> mail.
3. Nì Joomla lethbhreac dhen fhaidhle `mailtemplate.php` dhan eòlaire `/html/layouts/joomla/mail/` den teamplaid agad, far an urrainn dhut atharrachadh mar a tha iomchaidh.

Aon uair ’s gu bheil an ath-sgrìobhadh air a chruthachadh, faodaidh tu cruth agus stoidhlichean nam post-d agad atharrachadh gun buaidh a thoirt air an teamplaid bhunaiteach.

## Liosta de Theamplaidean Puist-d

| Tiotal | Leudachan | Tuairisgeul |
|-------|-----------|-------------|
| Log Gnìomhan Luchd-cleachdaidh: Post Fiosrachaidh | Log Gnìomhan Luchd-cleachdaidh | Post-d air a chur gu rianadairean mu inntrigidhean ùra ann an Log Gnìomhan Luchd-cleachdaidh. |
| Rèiteachadh Cruinneil: Post Deuchainn | Rèiteachadh | Air a chur nuair a bhriogar air a’ phutan “Cuir Post Deuchainn” anns an Rèiteachadh Chruinneil. Thèid a chur chun t-seòlaidh puist-d a tha air a shuidheachadh ann an roghainnean a’ phuist. |
| Luchd-conaltraidh: Post Foirm-conaltraidh | Luchd-conaltraidh | Am post-d “Foirm-conaltraidh”. |
| Luchd-conaltraidh: Lethbhreac de Phost Foirm-conaltraidh | Luchd-conaltraidh | Air a chur chun neach a chuir a-steach am post leis an fhoirm-conaltraidh ma tha an roghainn roghainneil “Cuir Lethbhreac chun Neach a Chuir a-steach e” air a chur an comas agus air a thaghadh. |
| Teachdaireachdan: Teachdaireachd ùr | Teachdaireachdan | Post-d anns a bheil teachdaireachd a chaidh a chruthachadh sa cho-phàirt theachdaireachdan. |
| Prìobhaideachd: Iarr Às-phortadh Dàta (Rianaire) | Prìobhaideachd | Post-d gus innse don chleachdaiche gun deach iarrtas airson an dàta bhon làrach-lìn seo às-phortadh a chruthachadh leis an rianaire |
| Prìobhaideachd: Iarr Toirt air Falbh Dàta (Rianaire) | Prìobhaideachd | Post-d gus innse don chleachdaiche gun deach iarrtas airson an dàta bhon làrach-lìn seo a thoirt air falbh a chruthachadh leis an rianaire |
| Prìobhaideachd: Iarr Às-phortadh Dàta | Prìobhaideachd | Post-d gus dearbhadh gum bu chòir dàta cleachdaiche às-phortadh bhon làrach-lìn |
| Prìobhaideachd: Iarr Toirt air Falbh Dàta | Prìobhaideachd | Post-d gus dearbhadh gum bu chòir dàta cleachdaiche a thoirt air falbh bhon làrach-lìn |
| Prìobhaideachd: Às-phortadh Dàta Cleachdaiche | Prìobhaideachd | Post-d le às-phortadh dàta cleachdaiche |
| Cleachdaichean: Post Mòr-chuid de Chleachdaichean | Cleachdaichean | Am post-d “Post Mòr-chuid de Chleachdaichean”. |
| Cleachdaichean: Ath-shuidheachadh Facail-fhaire | Cleachdaichean | Air a chur gu cleachdaiche leis a’ cheangal “An do dhìochuimhnich thu am facal-faire agad?” m.e. ann am foirm logaidh a-steach. |
| Cleachdaichean: Fios mu Chunntas Ùr don Rianaire | Cleachdaichean | Fios don rianaire gun deach cunntas ùr, gnìomhaichte a chruthachadh. |
| Cleachdaichean: Iarrtas chun Rianaire gus Cunntas Ùr a Dhearbhadh | Cleachdaichean | Fios do rianadairean gus cunntas ùr, dearbhte a dhearbhadh. |
| Cleachdaichean: Cunntas air a Ghnìomhachadh leis an Rianaire | Cleachdaichean | Fios air a chur chun chleachdaiche gun deach an cunntas ùr a ghnìomhachadh le rianaire. |
| Cleachdaichean: Cunntas Ùr le Gnìomhachadh leis an Rianaire | Cleachdaichean | Fios mun chunntas ùr don chleachdaiche, a dh’fheumas a-nis a bhith air a ghnìomhachadh le rianaire. |
| Cleachdaichean: Cunntas Ùr le Gnìomhachadh leis an Rianaire (le Facal-faire) | Cleachdaichean | Fios mun chunntas ùr don chleachdaiche, a dh’fheumas a-nis a bhith air a ghnìomhachadh le rianaire. Tha am facal-faire ann an teacsa shoilleir sa phost-d. |
| Cleachdaichean: Cunntas Ùr gun Ghnìomhachadh | Cleachdaichean | Fios mun chunntas ùr don chleachdaiche. Tha an cunntas air a ghnìomhachadh mu thràth. |
| Cleachdaichean: Cunntas Ùr gun Ghnìomhachadh (le Facal-faire) | Cleachdaichean | Fios mun chunntas ùr don chleachdaiche. Tha an cunntas air a ghnìomhachadh mu thràth. Tha am facal-faire ann an teacsa shoilleir sa phost-d. |
| Cleachdaichean: Cunntas Ùr le Fèin-ghnìomhachadh | Cleachdaichean | Fios mun chunntas ùr don chleachdaiche, a dh’fheumas a-nis an cunntas fhèin a ghnìomhachadh. |
| Cleachdaichean: Cunntas Ùr le Fèin-ghnìomhachadh (le Facal-faire) | Cleachdaichean | Fios mun chunntas ùr don chleachdaiche, a dh’fheumas a-nis an cunntas fhèin a ghnìomhachadh. Tha am facal-faire ann an teacsa shoilleir sa phost-d. |
| Cleachdaichean: Cuimhneachan Ainm-cleachdaiche | Cleachdaichean | Air a chur gu cleachdaiche leis a’ cheangal “An do dhìochuimhnich thu d’ ainm-cleachdaiche?” m.e. ann am foirm logaidh a-steach. |
| Còd air a chur tro phost-d | Dearbhadh Ioma-fhactair - Còd Dearbhaidh tro Phost-d | Air a chur gu cleachdaichean bhon duilleag Dearbhaidh Ioma-fhactair nuair a thathar a’ cleachdadh an roghainn “Còd Dearbhaidh tro Phost-d”. |
| Gnìomh - Aonta Prìobhaideachd: Ath-nuadhaich Aonta | Gnìomhan - Aontaidhean Prìobhaideachd | Cuimhneachan gus an t-aonta prìobhaideachd airson na làraich-lìn seo ath-nuadhachadh. |
| Joomla: Fios mu Ùrachadh | Gnìomh - Fios mu Ùrachadh Joomla! | Air a chur gu rianadairean na làraich nuair a lorgas am plugan gnìomh “Fios mu Ùrachadh Joomla!” ùrachadh. |
| Cleachdaichean: Cleachdaiche Ùr | Cleachdaiche - Joomla! | Air a chur gu cleachdaiche ùr nuair a thèid a chruthachadh san deireadh-sheachdain. |

*Air eadar-theangachadh le openai.com*