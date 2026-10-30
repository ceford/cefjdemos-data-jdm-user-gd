<!--
{
    "source": "https://docs.joomla.org/How_do_you_password_protect_directories_using_htaccess%3F",
    "title": "D\u00econ E\u00f2lairean le Facal-faire",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

’S dòcha gum bi thu airson eòlaire no làrach slàn a dhìon bho inntrigeadh poblach. ’S e
aon adhbhar airson seo inntrigeadh poblach gu làrach Leasachaidh a dhiùltadh. Is e dìreach an fheadhainn
a tha eòlach air an ainm-chleachdaiche agus am facal-faire a gheibh inntrigeadh. ’S e adhbhar eile
paranoia — mar eisimpleir, pasgan an rianaire a dhìon gus am feum luchd-cleachdaidh
ainm-chleachdaiche agus facal-faire a chur a-steach dìreach airson inntrigeadh fhaighinn dhan fhoirm
logaidh a-steach aig Rianaire Joomla.

Tha an dòigh a tha air a mhìneachadh an-seo airson frithealaichean Apache a tha a’ cleachdadh faidhle *.htaccess*.

### Rabhadh bho Apache.org

Cha bu chòir dearbhadh bunaiteach a mheas tèarainte fo mhìneachadh
gu sònraichte teann sam bith air “tèarainte”. Ged a tha am facal-faire
air a stòradh air an fhrithealaiche ann an cruth crioptaichte, dh’fhaodadh gun
tèid a chur bhon chleachdaiche dhan fhrithealaiche ann an teacsa lom tron lìonra. Bidh comas aig duine sam bith
a tha ag èisteachd le seòrsa sam bith de ghlacadair phacaidean an t-ainm-chleachdaiche agus
am facal-faire a leughadh fhad ’s a tha iad a’ dol thairis.

Thèid an t-ainm-chleachdaiche agus am facal-faire a chur leis gach iarrtas,
chan ann dìreach nuair a chuireas an cleachdaiche a-steach iad an toiseach. Mar sin chan fheum an glacadair phacaidean
a bhith ag èisteachd aig àm ro-innleachdail sònraichte, ach dìreach fada gu leòr airson iarrtas singilte sam bith fhaicinn a’ tighinn
thairis air an uèir.

A bharrachd air sin, tha an t-susbaint fhèin cuideachd a’ dol thairis air an lìonra
ann an cruth soilleir, agus mar sin ma tha fiosrachadh mothachail air an làrach-lìn, bhiodh
an glacadair phacaidean sin cuideachd comasach air an fhiosrachadh sin fhaighinn, fiù ’s mura deach an t-ainm-chleachdaiche
agus am facal-faire a chleachdadh gus inntrigeadh dìreach fhaighinn dhan làrach-lìn.

Na cleachd dearbhadh bunaiteach airson rud sam bith a dh’fheumas fìor thèarainteachd.
Tha e na ana-cothrom don mhòr-chuid de luchd-cleachdaidh, oir cha ghabh ach glè bheag de dhaoine an
trioblaid, no bidh am bathar-bog no an uidheamachd riatanach aca, gus faclan-faire
fhaighinn a-mach. Ach, nam biodh miann aig cuideigin faighinn a-steach, cha toireadh e
ach glè bheag oidhirp dhaibh sin a dhèanamh.

Ach bidh dearbhadh bunaiteach thairis air ceangal SSL tèarainte,
oir thèid a h-uile càil a chrioptachadh, a’ gabhail a-steach an t-ainm-chleachdaiche agus
am facal-faire.

## A’ cleachdadh cPanel

Ma tha thu a’ cleachdadh seirbheis òstachaidh, bu chòir dhut an dòigh aice airson dìon eòlairean
a chleachdadh. Mar eisimpleir, tha roghainn aig cPanel air a bheil Directory Privacy. Nuair a
thaghas tu e, faodaidh tu seòladh gu eòlaire sam bith agus ainm a shuidheachadh air. Bidh
cothrom agad an uair sin Ainm Cleachdaiche agus Facal-faire cleachdaiche a chruthachadh airson an
eòlaire ainmichte. Sìmplidh?

Ma choimheadas tu a-nis san eòlaire a dhìon thu, gheibh thu faidhle .htaccess ùr
anns a bheil rudeigin coltach ris an t-suidheachadh a leanas gus pasgan api Joomla a dhìon:

```
#----------------------------------------------------------------cp:ppd
# Section managed by cPanel: Password Protected Directories     -cp:ppd
# - Do not edit this section of the htaccess file!              -cp:ppd
#----------------------------------------------------------------cp:ppd
AuthType Basic
AuthName "API"
AuthUserFile "/home/username/.htpasswds/public_html/[jroot]/api/passwd"
Require valid-user
#----------------------------------------------------------------cp:ppd
# End section managed by cPanel: Password Protected Directories -cp:ppd
#----------------------------------------------------------------cp:ppd
```

Tha e cudromach a bhith mothachail gum faod dìon eòlaire cPanel an aon
faidhle .htaccess a chleachdadh ’s a tha Joomla a’ cleachdadh airson adhbharan eile.

Ma choimheadas tu san fhaidhle passwd ainmichte, chì thu an t-Ainm Cleachdaiche a thug thu seachad
agus an tionndadh crioptaichte den fhacal-faire.

Faodar an dìon a thoirt air falbh le bhith ag ath-aithris a’ phròiseis agus a’ toirt air falbh an comharradh bhon
bhogsa-seic `Dìon an eòlaire seo le facal-faire.` Bheir sin air falbh an earrann dearbhaidh bhon fhaidhle .htaccess. Cha toir
e air falbh am faidhle .htaccess!

## Riaghailtean .htaccess

Faodaidh tu gach ceum riatanach a dhèanamh le làimh. Dh’fhaodadh an t-inneal seo do chuideachadh:

<a href="https://www.htaccessredirect.net/"
 rel="nofollow noreferrer noopener"><em>gineadair</em>
.htaccess</a>

Cruthaichidh e na faidhlichean riatanach dhut. Feumaidh tu an t-ainm-cleachdaiche,
am facal-faire agus an t-slighe a shònrachadh.

Lìon a-steach an dà earrann: **Faidhle Dìon le Facal-faire** agus **Gineadair htpasswd**
agus an uair sin tagh am putan `Cruthaich Còd`. Gheibh thu air ais teacsa an
faidhle .htaccess agus teacsa an fhaidhle .htpasswd ann am bogsaichean fa leth.
Eisimpleirean:
```
//Password Protect file
<Files /admin>
AuthName "Prompt"
AuthType Basic
AuthUserFile /home/user/.htpasswd
Require valid-user
</Files>
```

```
John:$apr1$a3dbt6j7$KJQr137CY9QuN6tYl6M4Z1
```

*Air eadar-theangachadh le openai.com*

