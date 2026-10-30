<!--
{
    "source": "https://docs.joomla.org/Enabling_Search_Engine_Friendly_(SEF)_URLs_on_Nginx",
    "title": "URLan SEF air Nginx",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Tha URLan a tha càirdeil do dh’innealan-rannsachaidh (SEF), a ghabhas leughadh le daoine no glan, nan URLan a tha ciallach do dhaoine agus do dh’innealan-rannsachaidh le chèile, oir tha iad a’ mìneachadh na slighe chun na duilleige shònraichte air a bheil iad a’ comharrachadh. Tha Joomla! comasach air URLan a chruthachadh agus a pharsadh ann an cruth sam bith, a’ gabhail a-steach URLan SEF. Chan eil seo an eisimeil ath-sgrìobhadh URL a nì am frithealaiche-lìn, agus mar sin obraichidh e fiù ’s ma tha Joomla! a’ ruith air frithealaiche seach Apache leis a’ mhodal mod_rewrite. Bidh na URLan SEF a’ leantainn pàtran shuidhichte shònraichte, ach faodaidh an cleachdaiche teacsa ghoirid thuairisgeulach (alias) a mhìneachadh airson gach earrann den URL.

Taobh a-staigh, canar slighe ri pàirt ionadail URL SEF (am pàirt às dèidh ainm an àrainn). Mar sin, thathar a’ toirt iomradh air cruthachadh agus giullachd URLan SEF mar stiùireadh shlighean, agus canar router ris a’ chòd iomchaidh.

Tha an artaigil seo a’ dèiligeadh ri URLan SEF fon fhrithealaiche-lìn Nginx, a tha mòr-chòrdte agus fosgailte.

## Ceumannan airson frithealaichean NginX¶

- Cuir an còd a leanas ri rèiteachadh an fhrithealaiche agad (vhost) san fhaidhle nginx.conf:

```
    # Support Clean (aka Search Engine Friendly) URLs
    location / {
       try_files $uri $uri/ /index.php?$args;
    }
```

- Mura obraich na tha gu h-àrd, cuir an còd a leanas ri rèiteachadh an fhrithealaiche agad san fhaidhle nginx.conf: (Dh’obraich seo le nginx 1.4.6 air Ubuntu.)
```
    server {
      ....
      location / {
      expires 1d;

      # Enable joomla SEF URL's inside Nginx
      try_files $uri $uri/ /index.php?$args;
      }
      ....
    }
```

- Clàraich a-steach don Backend agad agus fosgail an Rèiteachadh Choitcheann
- Cuir an comas an roghainn **URLan a tha càirdeil do dh’innealan-rannsachaidh** agus sàbhail. Tionndaidhidh an roghainn seo na URLan bhon chruth dùthchasach Joomla! gu cruth SEF. Dearbhaich gu bheil an làrach agad ag obrachadh mar bu chòir. Bu chòir na URLan agad a bhith a’ coimhead mar `http://www.example.com/index.php/the-­news/1-­latest­-news/1­-welcome­-to­-joomla` a-nis. Mura h-obraich an làrach agad mar bu chòir, faic [Carson a thèid an làrach agad troimhe chèile nuair a chuireas tu SEF (URLan a tha càirdeil do dh’innealan-rannsachaidh) air?](https://docs.joomla.org/Why_does_your_site_get_messed_up_when_you_turn_on_SEF_(Search_Engine_Friendly_URLs)%3F)
- Cuir an comas an roghainn **Cleachd Apache mod_rewrite/Ath-sgrìobhadh URL** agus sàbhail. Cleachdaidh an roghainn seo gnìomh Apache mod_rewrite gus am pàirt *index.php* den URL a thoirt air falbh Dearbhaich gu bheil an làrach agad ag obrachadh mar bu chòir. Bu chòir na URLan agad a bhith a’ coimhead mar `http://www.example.com/the-­news/1­-latest-­news/1-­welcome-­to­-joomla` a-nis. Ma dh’adhbharaicheas an roghainn seo mearachdan, faic [Mar a nì thu sgrùdadh a bheil mod rewrite an comas air an fhrithealaiche agad](https://docs.joomla.org/How_to_check_if_mod_rewrite_is_enabled_on_your_server). Mura h-eil e an comas agus ma tha cothrom agad air an fhaidhle `apache/conf/httpd.conf`, fosgail am faidhle sin agus dearbhaich nach eil an loidhne `LoadModule rewrite_module modules/mod_rewrite.so` air a cur ann am beachd. Ma tha feum air, thoir air falbh an comharra beachd bhon loidhne agus ath-thòisich am frithealaiche-lìn Apache. Mura gabh *mod_rewrite* a chur an comas, fàg an roghainn seo dheth. Chan eil e gu diofar ma dh’fhàgas tu am faidhle `.htaccess` air ath-ainmeachadh.
- *Ma tha thu den bheachd gu bheil seo riatanach*, cuir an comas **Cuir iar-leasachan ri URLan** agus *Sàbhail*. Cuiridh an roghainn seo `.html` ri deireadh nan URLan. Tha diofar bheachdan ann a thaobh a bheil seo riatanach no fiù ’s feumail. Chan eil coltas gu bheil dragh air innealan-rannsachaidh ma chrìochnaicheas na URLan agad ann an `.html` no nach crìochnaich.
- Fosgail Manaidsear nam Plugan agus cuir an comas am plugan **Siostam - SEF**. Cuiridh am plugan seo taic SEF ri ceanglaichean sna h-artaigilean Joomla agad. Bidh e ag obrachadh dìreach air an HTML agus chan eil taga sònraichte a dhìth.

*Air eadar-theangachadh le openai.com*