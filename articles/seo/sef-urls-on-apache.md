<!--
{
    "source": "https://docs.joomla.org/Enabling_Search_Engine_Friendly_(SEF)_URLs_on_Apache",
    "title": "SEF URLs air Apache",
    "description": " ",
    "author": ""
}
-->

## Dearbhaich gu bheil .htaccess an comas

Dèan cinnteach gu bheil rèiteachadh Apache agad a’ ceadachadh tar-sgrìobhadh
.htaccess. Feumaidh tu dèanamh cinnteach gu bheil tar-sgrìobhaidhean an
comas, air neo thèid am faidhle .htaccess ann am prìomh eòlaire Joomla!
a leigeil seachad no adhbharaichidh e mearachd. Anns an earrainn de
fhaidhle rèiteachaidh an òstair bhrìgheil agad, no sa phrìomh fhaidhle
rèiteachaidh (`httpd.conf`), feumaidh rudeigin coltach ris an eisimpleir
gu h-ìosal a bhith agad a’ cur tar-sgrìobhaidhean an comas:

```bash
<Directory "/home/user/public_html">
  AllowOverride All
</Directory>

<Directory "/path/to/htdocs">
  AllowOverride All Options=[an option],[an option],...
</Directory>
```

Tha dòighean eile ann gus dearbhadh a bheil `.htaccess` an comas mura h-eil
cothrom agad air faidhlichean rèiteachaidh na làraich agad. Thoir sùil air
an [oideachadh .htaccess](http://httpd.apache.org/docs/current/howto/htaccess.html) 
air làrach-lìn *The Apache Software Foundation* airson barrachd fiosrachaidh.

## Ceum air Cheum

Seo stiùireadh ceum air cheum. Lean iad san òrdugh
anns a bheil iad air an taisbeanadh an seo. Ma dh’fhàillig ceum, **na**
lean air adhart gus am bi thu air an duilgheadas fhuasgladh.

1.  Ath-ainmich am faidhle `htaccess.txt` ann am pasgan bunaiteach Joomla! agad gu `.htaccess`.
2.  *’S dòcha nach bi feum air a’ cheum seo.* Fosgail `.htaccess` ann an deasaiche teacsa.
    Thoir beachd air falbh bho `RewriteBase /` (thoir air falbh a’ chiad charactar, \#). Ma tha
    Joomla air a stàladh na phasgan fhèin, cuir ainm pasgan Joomla
    às dèidh na slaise air adhart. m.e. `RewriteBase /yourjoomlafolder`.
3.  Log a-steach don Chùlaibh agad agus fosgail an Rèiteachadh Cruinneil.
4.  Cuir an roghainn **Cleachd mod_rewrite Apache/Ath-sgrìobhadh URL** an comas agus
    *Sàbhail*. Cleachdaidh an roghainn seo gnìomh *mod_rewrite* Apache gus
    am pàirt "index.php" den URL a thoirt air falbh.

    Dèan cinnteach a bheil an làrach agad ag obair mar bu chòir. Bu chòir do na URLan agad
    a bhith coltach ri seo a-nis:

        `http://www.example.com/the-­news/1­-latest-­news/1-­welcome-­to­-joomla`

    Ma dh’adhbharaicheas an roghainn seo mearachdan, faic
    [Mar a nì thu dearbhadh a bheil mod rewrite an comas air an fhrithealaiche agad](https://docs.joomla.org/How_to_check_if_mod_rewrite_is_enabled_on_your_server).

    - Mura h-eil e an comas agus ma tha cothrom agad air an fhaidhle
      `apache/conf/httpd.conf`, fosgail am faidhle sin agus dèan cinnteach a bheil an loidhne
      `LoadModule rewrite_module modules/mod_rewrite.so` gun bheachd.
      Ma tha feum air, thoir beachd air falbh bhon loidhne agus ath-thòisich frithealaiche-lìn Apache.
    - Mura gabh *mod_rewrite* a chur an comas, fàg an roghainn seo dheth. Chan eil
      e gu diofar ma dh’fhàgas tu am faidhle `.htaccess` air ath-ainmeachadh.
5.  *Ma tha thu den bheachd gu bheil feum air seo*, cuir **Cuir iar-leasachan ri URLan** an comas agus
    *Sàbhail*. Cuiridh an roghainn seo `.html` ri deireadh nan URLan. Tha
    diofar bheachdan ann a thaobh a bheil seo riatanach no fiù ’s feumail.
    Chan eil coltas gu bheil cùram aig einnseanan-luirg a bheil na URLan agad a’ crìochnachadh ann an `.html` no
    nach eil.
6.  Fosgail Manaidsear nam Plugan agus cuir am **Siostam - Plugan SEF** an comas.
    Cuiridh am plugan seo taic SEF ri ceanglaichean anns na h-artaigilean Joomla agad. Bidh e
    ag obrachadh gu dìreach air an HTML agus chan eil taga sònraichte a dhìth.

*Air eadar-theangachadh le openai.com*