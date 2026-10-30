<!--
{
    "source": "https://docs.joomla.org/How_do_you_block_direct_hot_linking_to_image_files_using_htaccess%3F",
    "title": "Cuir casg air ceangal teth ri dealbhan",
    "description": " ",
    "author": ""
}
-->

## Mìneachadh

Is e ceangal teth an cleachdadh far a bheil ceangal ri dealbh air aon làrach-lìn
bho artaigil air làrach-lìn eile. Faodaidh e a bhith na chleachdadh glè
fheumail. Bidh an làrach-lìn seo a’ cleachdadh mòran dhealbhan a tha
suidhichte air làrach-lìn docs.joomla.org. Sàbhalaidh seo an ùine agus an oidhirp
a tha riatanach airson glacadh-sgrìn a chruthachadh, agus leud-bann na làraich
seo. Ach, faodaidh cùisean dlighe-sgrìobhaidh èirigh agus dh’fhaodadh gum bi
thu airson casg a chur air na dealbhan agad a bhith gan cleachdadh san dòigh seo.

Tha an dòigh a tha air a mhìneachadh an seo a’ cleachdadh faidhle *.htaccess*,
a tha na fheart de fhrithealaiche Apache. Dh’fhaodadh frithealaichean-lìn eile
dòighean eile a thoirt seachad gus casg a chur air ceangal teth.

## Stiùiridhean

Cuir an còd a leanas ann am faidhle *.htaccess* na prìomh-eòlaire agad.
```
<IfModule mod_rewrite.c>
    RewriteEngine on
    RewriteCond %{HTTP_REFERER} !^$
    RewriteCond %{HTTP_REFERER} !^http(s)?://(www\.)?yourdomain.com [NC]
    RewriteCond %{HTTP_REFERER} !^http(s)?://(www\.)?google.com [NC]
    RewriteRule \.(jpg|jpeg|png|gif|webp|svg)$ - [NC,F,L]
</IfModule>
```

### Mìneachadh

* Tha a’ chiad RewriteCond a’ ceadachadh iarrtasan dìreach a’ cleachdadh URL — gun referer.
* Tha an dàrna RewriteCond a’ ceadachadh iarrtasan bhon àrainn agad fhèin. Tha am bratach *\[NC\]*
    a’ ciallachadh *No Case*, is e sin, maidseadh charactaran ann an litrichean mòra agus beaga.
* Tha an treas RewriteCond a’ ceadachadh iarrtasan bho Google, gus am faod na dealbhan agad
    nochdadh fhathast ann an toraidhean luirg. Faodaidh tu loidhnichean coltach ris a chur ris airson làraichean
    sam bith eile a tha thu airson a cheadachadh.
* Bidh an RewriteRule a’ bacadh iarrtasan airson faidhlichean dhealbhan bho gach àrainn nach deach
    a cheadachadh roimhe. Tha am bratach F ag innse don bhrabhsair bann-cinn Forbidden (403) a thilleadh. Tha L a’ seasamh airson riaghailt mu dheireadh.

### Cuir casg air ceangal teth bho àrainnean sònraichte

Gus stad a chur air ceangal teth bho àrainnean sònraichte a-mhàin, leithid *myspace.com*,
*blogspot.com* agus *livejournal.com*, fhad ’s a tha thu a’ ceadachadh do làraichean-lìn eile
ceangal teth a dhèanamh ris na dealbhan agad, cleachd an còd a leanas:

```
<IfModule mod_rewrite.c>
    RewriteEngine On
    RewriteCond %{HTTP_REFERER} ^http(s)?://(.+\.)?myspace\.com/ [NC,OR]
    RewriteCond %{HTTP_REFERER} ^http(s)?://(.+\.)?blogspot\.com/ [NC,OR]
    RewriteCond %{HTTP_REFERER} ^http(s)?://(.+\.)?livejournal\.com/ [NC]
    RewriteRule \.(jpg|jpeg|png|gif|webp|svg)$ - [NC,F,L]
</IfModule>
```

Faodaidh tu na h-uimhir de dh’àrainnean eadar-dhealaichte ’s a thogras tu a chur ris. Bu chòir do gach loidhne *RewriteCond*
ach an tè mu dheireadh crìochnachadh leis na brataichean *\[NC,OR\]*. Tha *NC*
a’ ciallachadh gun tèid aire a thoirt do chùis nan litrichean. Tha *OR* a’ ciallachadh “No an ath fhear”, is e sin,
maidseadh na loidhne seo **no** an ath loidhne. Bidh an *RewriteCond* mu dheireadh a’ fàgail a-mach bratach *OR* gus stad a chur air
maidseadh às dèidh an *RewriteCond* mu dheireadh.

*Air eadar-theangachadh le openai.com*