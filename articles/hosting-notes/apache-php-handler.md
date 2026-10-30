<!--
{
    "source": "https://docs.joomla.org/J4.x:Apache_PHP_Handler",
    "title": "Luchd-l\u00e0imhseachaidh PHP Apache",
    "description": " ",
    "author": ""
}
-->

## Notaichean

Gus faighinn a-mach dè an dòigh a tha am frithealaiche-lìn agad a’ cleachdadh gus faidhlichean PHP a làimhseachadh, cleachd na ceanglaichean **Rianadair / Siostam / Fiosrachadh an t-Siostaim** agus tagh an taba Fiosrachadh PHP. Rannsaich an duilleag airson **Server API**. Am measg nan dòighean àbhaisteach anns am bi frithealaiche-lìn Apache a’ làimhseachadh fhaidhlichean PHP tha na leanas:

### DSO (mod_php)

- **Buannachd:** aon de na luchd-làimhseachaidh as luaithe a tha ri fhaighinn.
- **Eas-bhuannachd:** chan obraich e ach le aon tionndadh de PHP; ’s ann leis a’ chleachdaiche Apache a bhios na faidhlichean a shàbhaileas sgriobtaichean PHP **ach a-mhàin** nuair a thèid a chleachdadh còmhla ri mod_ruid2.
- **Gus aithneachadh:** Server API - Apache 2.0 Handler

### CGI/FastCGI

- **Buannachd:** bidh sgriobtaichean a’ ruith mar chleachdaiche an àrainn no an fho-àrainn; neach-làimhseachaidh glè luath.
- **Eas-bhuannachd:** nas slaodaiche na mod_php; chan urrainnear atharrachaidhean rèiteachaidh PHP a chur ann am faidhle .htaccess.
- **Gus aithneachadh:** Server API - CGI/FastCGI

### FPM/FastCGI

- **Buannachd:** glè luath, le ìre a bharrachd de shùbailteachd.
- **Eas-bhuannachd:** bidh e a’ cleachdadh barrachd cuimhne na a’ mhòr-chuid den fheadhainn eile; chan urrainnear atharrachaidhean rèiteachaidh PHP a chur ann am faidhle .htaccess.
- **Gus aithneachadh:** Server API - FPM/FastCGI

### LSAPI (mod_lsapi)

’S e eadar-aghaidh prògramadh aplacaidean frithealaiche LiteSpeed a th’ ann an LiteSpeed Server Application Programming Interface, agus chaidh a dhealbhadh gu sònraichte airson LiteSpeed Web Server, le cuideam air àrd-choileanadh agus èifeachdas.

- **Buannachdan:**
   - A’ toirt taic do thasgadh.
   - ’S e an neach-làimhseachaidh as èifeachdaiche a th’ ann, le glè bheag de chleachdadh cuimhne.
   - Chan eil feum air rèiteachadh.
   - Faodaidh e obrachadh le iomadh tionndadh de PHP ann an aon rèiteachadh.
   - Tha e a’ toirt taic do stiùiridhean rèiteachaidh PHP tro fhaidhlichean .htaccess.
   - Tèarainte oir bidh sgriobtaichean a’ ruith mar shealbhadair na h-àrainn.
- **Eas-bhuannachdan:**
   - Chan eil e a’ cur gach comas LSAPI ri làimh.
- **Gus aithneachadh:** Server API - ?

Air coimpiutair-glùine no coimpiutair deasg ionadail, faodaidh tu mod_php a chleachdadh, ach dh’fhaodadh gum feum thu an cleachdaiche Apache a shuidheachadh mar an t-ainm-cleachdaiche agad fhèin agus freumh nan sgrìobhainnean a chomharrachadh gu àite taobh a-staigh an àite-fhaidhlichean agad fhèin. Mur dèan thu sin, bidh duilgheadasan agad le ceadan fhaidhlichean agus phasganan.

Air seirbheis aoigheachd, feumaidh tu aon de na roghainnean FastCGI no LSAPI a chleachdadh. Dh’fhaodadh seirbheisean aoigheachd roghainn a thoirt dhut.

*Air eadar-theangachadh le openai.com*

