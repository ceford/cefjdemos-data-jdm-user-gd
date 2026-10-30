<!--
{
    "source": "https://docs.joomla.org/Purging_expired_cache_files",
    "title": "Glan an tasgadan a dh\u2019fhalbh an \u00f9ine",
    "description": " ",
    "author": ""
}
-->

## Faidhlichean Tasgadain

’S e faidhlichean sealach a th’ ann am faidhlichean tasgadain a thèid a chruthachadh gus coileanadh na làraich agad a leasachadh. Feumaidh tu dèanamh cinnteach gun tèid faidhlichean tasgadain a dh’fhalbh an ùine, agus mar sin nach eil feum orra tuilleadh, a thoirt air falbh bhon t-siostam. Air neo, ruithidh tu a-mach à àite diosga mu dheireadh thall.

Faodar faidhlichean tasgadain a dh’fhalbh an ùine a ghlanadh bhon eadar-aghaidh Rianadair no bhon eadar-aghaidh Loidhne-àithne (CLI).

## Glanadh - Dòigh an Rianadair

Bhon *Deas-bhòrd Dachaigh*
* Tagh an roghainn **Tasgadan** sa phannal *Siostam*.
* Air an duilleig *Cumail suas: Glan an tasgadan*, tagh am putan **Glan an tasgadan a dh’fhalbh an ùine**
sa Bhàr-inneal.

## Glanadh - Dòigh na Loidhne-àithne

Fosgail uinneag crìochnachaidh agus cleachd `cd` gus gluasad dhan phasgan cli ann am bun-eòlaire na làraich agad.
Mura h-eil fios agad dè na h-àitheantan CLI a tha rim faighinn, ruith an àithne a leanas:
```bash
php joomla.php
```

Chì thu liosta de na h-àitheantan a tha rim faighinn. ’S e seo an àithne `cache`:
```bash
php joomla.php cache:clean
```

Bu chòir dhut teachdaireachd dearbhaidh uaine fhaicinn, no ’s dòcha teachdaireachd mhearachd maròin.

## Faidhlichean Tasgadain a’ Glanadh Gu Fèin-obrachail

Faodaidh tu faidhlichean tasgadain a dh’fhalbh an ùine a ghlanadh gu fèin-obrachail a’ cleachdadh obair cron. Bidh seirbheisean aoigheachd a’ dèanamh seo furasta le bhith a’ toirt seachad foirm gus taghadh dè cho tric ’s a ruitheas obair agus dè an àithne a thèid a chleachdadh. Mar sin, dh’fhaodadh tu cron a shuidheachadh gus ruith aig 05:00 gach latha leis an àithne a leanas:
```
 /usr/local/bin/ea-php82 /home/username/public_html/cli/joomla.php cache:clean
 ```

Leigidh a’ mhòr-chuid de mhanaidsearan obraichean *cron* leat seòladh puist-d a chur a-steach far an tèid toradh cron a chur. Mura h-eil thu ag iarraidh teachdaireachd a chur, cuir ` > /dev/null 2>&1`
ris an àithne.

Gu tric bidh an tionndadh de PHP a thathar a’ cleachdadh air an loidhne-àithne eadar-dhealaichte bhon fhear a thathar a’ cleachdadh airson làrach-lìn a lìbhrigeadh. Dh’fhaodadh e a bhith neo-fhreagarrach ri Joomla. Mar sin, cleachd an t-slighe slàn dhan tionndadh de PHP a tha thu airson a chleachdadh seach `php` leis fhèin.

*Air eadar-theangachadh le openai.com*