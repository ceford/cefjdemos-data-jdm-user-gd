<!--
{
    "source": "https://docs.joomla.org/How_to_debug_SMTP_mail_in_Joomla_4",
    "title": "Post-d SMTP agus Gmail",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Air duilleag an Rèiteachaidh Choitcheann, sa phannal Fhrithealaiche, tha roghainn ann àidseant lìbhrigidh puist a thaghadh. Is e *PHP Mail* an roghainn bhunaiteach. Mura obraich seo, dh’fhaoidte gun tèid comhairle a thoirt dhut SMTP a chleachdadh. Bidh e a’ cleachdadh an aon uidheamachd ris an aplacaid puist agad. Tha grunn shuidheachaidhean ann a dh’fheumas tu a rèiteachadh gu ceart. Ann an geàrr-chunntas:

Rach gu **Rèiteachadh Coitcheann** agus tagh an taba **Frithealaiche**. Coimhead airson a’ phannail *Post* faisg air bonn na foirm.

- **Mailer** suidhichte gu SMTP. Nochdaidh grunn raointean eile
- **Òstair SMTP** Is e localhost an roghainn bhunaiteach, ach chan eil e coltach gun obraich sin. Feumar a shuidheachadh dhan òstair a làimhsicheas am post a-mach agad, mar eisimpleir cunntas Gmail.
- **Port SMTP** Is e 25 an roghainn bhunaiteach. Dèan cinnteach gur e sin an luach ris a bheil an t-Òstair SMTP agad an dùil.
- **Tèarainteachd SMTP** Is e *Gun dad* an roghainn bhunaiteach, ach tha e coltach gum feum thu STARTTLS.
- **Dearbhadh SMTP** Dh’fhaoidte nach bi feum air seo ma tha thu a’ cleachdadh lìonra dachaigh a tha an dùil nach bi feum air dearbhadh airson puist-d a-mach. Air neo:
- **Ainm-cleachdaiche SMTP** agus **Facal-faire SMTP** cuir a-steach na luachan a chleachdas tu gus inntrigeadh fhaighinn don chunntas phuist-d agad tron eadar-lìon.
- Tagh am putan **Cuir Post-deuchainn**.

## A’ cleachdadh Gmail

Ma tha cunntas Gmail obrachail agad, faodaidh tu Gmail a chleachdadh mar fhrithealaiche a’ phuist agad le bhith ga shuidheachadh san rèiteachadh choitcheann.

Air taba an fhrithealaiche, suidhich na leanas:

- Mailer: SMTP
- Òstair SMTP: smtp.gmail.com
- Port SMTP 465
- Tèarainteachd SMTP: SSL/TLS
- Dearbhadh SMTP: Tha
- Suidhich an ath dhà loidhne leis an fhiosrachadh agad. Feumaidh tu facal-faire sònraichte airson aplacaid (ASP) a chleachdadh, air a mhìneachadh gu h-ìosal.
- Ainm-cleachdaiche SMTP: an t-ainm-cleachdaiche Gmail agad
- Facal-faire SMTP: am facal-faire sònraichte airson na h-aplacaid (ASP) a chruthaich thu, air a mhìneachadh gu h-ìosal.

Tha na cothlamachaidhean a leanas ag obair cuideachd:

- Port SMTP 587
- Tèarainteachd SMTP: STARTTLS
- Port SMTP 25
- Tèarainteachd SMTP: STARTTLS

Chan fheum am modal SSL a bhith an comas ann an Apache.

Feumaidh an leudachan OpenSSL a bhith an comas ann am PHP. Gheibhear am mion-fhiosrachadh air [duilleag stàlaidh php.net](https://www.php.net/manual/en/openssl.installation.php).

Ma tha thu a’ cleachdadh WAMP air Windows, chan eil am modal openssl an comas mar bhun-roghainn agus feumaidh tu a chur an comas. Gus seo a dhèanamh:

1.  Fosgail am faidhle php.ini agus thoir air falbh am beachd bhon loidhne `extension=php_openssl.dll` le bhith a’ toirt air falbh an leth-chòilean ; bho thoiseach na loidhne.
2.  Sàbhail am faidhle php.ini agus ath-thòisich seirbheis Apache.

Thoir an aire ma chleachdas tu dearbhadh 2-cheum ann an Gmail, gum feum thu facal-faire ùr a chur ris ann an Settings - Accounts - Change accounts settings - Other Google Account settings - Security - 2-step verification - Manage your application specific passwords.

Nuair a nochdas am Facal-faire Sònraichte airson na h-Aplacaid (ASP) ùr ann am buidhnean de cheithir caractaran air an sgaradh le beàrnan, dèan cinnteach nach cuir thu **na beàrnan a-steach idir** don fhacal-faire SMTP ann an roghainnean frithealaiche a’ phuist ann an Joomla.

- Faclan-faire Sònraichte airson Aplacaidean (ASPan): Faic duilleag Taic Google leis an tiotal
  [Clàraich a-steach le Faclan-faire Aplacaid](https://support.google.com/accounts/answer/185833).
- Dearbhadh 2-cheum: Faic duilleag Taic Google leis an tiotal 
  [Cuir Dearbhadh 2-cheum an comas](https://support.google.com/accounts/answer/185839).

## Fuasgladh dhuilgheadasan

Mura tèid am post a chur no mura ruig e a cheann-uidhe gu bràth:

- Tagh **Plugins** on **Deas-bhòrd Dachaigh → pannal na Làraich**. 
- Lorg agus cuir an comas am plugan **Siostam - Dì-bhugachadh**, agus rèitich e:
- Suidhich **Buidhnean Ceadaichte** gu *Super Users* gus toradh an dì-bhugachaidh a chuingealachadh ris an t-seisean logaidh a-steach agad fhèin an dà chuid sa backend agus san frontend. Mura h-eil thu airson logadh a-steach don frontend mar Super User, cruthaich buidheann chleachdaichean shònraichte airson na gnìomhan deuchainn agad agus tagh a’ bhuidheann sin de luchd-cleachdaidh bhon liosta de bhuidhnean chleachdaichean ceadaichte.
- **Sàbhail agus Dùin**

- Tagh **Rèiteachadh Coitcheann** on **Deas-bhòrd Dachaigh → pannal na Làraich**. 
- Ann an taba an *t-Siostaim*, suidhich **Dì-bhugachadh an t-Siostaim** gu *Tha*.
- Ann an taba an *Fhrithealaiche*, suidhich **Aithris Mhearachdan** gu *As àirde*.
- Ann an taba an *Logaidh*, thoir fa-near susbaint *Slighe gu Pasgan nan Logaichean*, mar as trice *\[rudeigin\]/administrator/logs*. 
- Suidhich **Logaich Cha mhòr a h-uile càil** gu *Tha*.
- Anns a’ phannal *Logadh gnàthaichte*, suidhich an raon *Roinnean nan Logaichean* gu *mail* (gun chomharran-luirg).
- **Sàbhail** gus na roghainnean dì-bhugachaidh a shàbhaladh.
- Ann an taba an **Fhrithealaiche**, tagh am putan *Cuir Post-deuchainn* aig bonn na duilleige.

Ma tha duilgheadasan sa chòd rè an deuchainn, bu chòir dhut *Trace Staca* fhaighinn a chuidicheas thu fhèin no daoine eile leis an duilgheadas a lorg. Cuideachd, coimhead airson faidhle sa phasgan logaichean le ainm mar *administrator/logs/everything.php* agus fosgail e le deasaiche teacsa. Dh’fhaodadh e a bhith feumail faicinn dè chaidh a chlàradh nuair a chaidh an teachdaireachd a chur.

*Air eadar-theangachadh le openai.com*