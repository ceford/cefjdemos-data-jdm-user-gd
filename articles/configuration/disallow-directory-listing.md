<!--
{
    "source": "https://docs.joomla.org/How_do_you_block_directory_scans_using_htaccess%3F",
    "title": "Cuir casg air liostadh e\u00f2lairean",
    "description": " ",
    "author": ""
}
-->

## Cùl-fhiosrachadh

Gu bunaiteach, air frithealaiche-lìn Apache, seallaidh eòlaire anns nach eil
faidhle index a tha air a mhìneachadh san rèiteachadh (index.html no index.php)
liosta de na faidhlichean agus na fo-eòlairean uile san eòlaire. Faodaidh seo a
bhith feumail air frithealaiche deuchainn pearsanta, ach tha e na chunnart mòr
do thèarainteachd air frithealaiche riochdachaidh beò.

San àm a dh’fhalbh, bha e na chleachdadh cumanta faidhle index.html falamh a
chur anns a h-uile eòlaire Joomla gus casg a chur air an duilgheadas seo nochdadh
air frithealaichean nach robh air an rèiteachadh ceart. Chan eil seo fìor tuilleadh.
Thathar an dùil gum bi rèiteachadh ceart air an fhrithealaiche, an dara cuid ann
am faidhlichean rèiteachaidh an fhrithealaiche no ann am faidhlichean .htaccess
fa leth. ’S fheàrr a’ chiad roghainn, oir thèid a chur an sàs air gach làrach-lìn
air an fhrithealaiche.

Ach, faodaidh làraichean ann an àrainneachd aoigheachd cho-roinnte a bhith an
dùil gun atharraich gach làrach rèiteachadh an fhrithealaiche le faidhlichean
.htaccess. Feumaidh am frithealaiche a bhith air a shuidheachadh gu
AllowOverride Options" or "AllowOverride All" gus leigeil le faidhlichean
.htaccess faighinn thairis air na roghainnean.

## A’ cleachdadh .htaccess

Faodar am faidhle htaccess.txt a gheibhear le Joomla a chleachdadh air
frithealaichean Apache le bhith ga ath-ainmeachadh no ga lethbhreacadh gu .htaccess.
Tha mòran shuidheachaidhean ann gus cur an aghaidh ionnsaighean luchd-brisidh air
làraichean Joomla. Am measg shuidheachaidhean eile, chì thu na roghainnean a
leanas gus casg a chur air liostadh eòlairean:

```
Options -Indexes

## No directory listings
<IfModule mod_autoindex.c>
    IndexIgnore *
</IfModule>
```

## Dèan deuchainn air an làrach agad

Is e aon dòigh air an làrach agad a dhearbhadh URL pasgan nan ìomhaighean agad a
chur a-steach do bhàr URL a’ bhrabhsair: `https://yourdomain.com/images/`. Leis
nach bi faidhle index.html no index.php mar as trice ann am pasgan nan ìomhaighean,
bu chòir dhut duilleag gu tur falamh fhaicinn. Ma chì thu liosta de na faidhlichean
agus na pasganan uile, chan eil thu a’ cur casg air sganadh nan eòlairean airson
pàirt sam bith den làrach agad. Ceartaich e!

*Air eadar-theangachadh le openai.com*