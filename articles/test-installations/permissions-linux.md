<!--
{
    "source": "https://docs.joomla.org/Verifying_permissions",
    "title": "Ceadan Fhaidhlichean: Linux",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Tha am fiosrachadh a leanas airson frithealaichean stèidhichte air Linux. Ma tha an
frithealaiche-lìn agad stèidhichte air Microsoft Windows (IIS), bu chòir dhut
[Permissions: Windows](jdocmanual?article=user/test-installations/permissions-windows) fhaicinn.

A rèir rèiteachadh tèarainteachd an fhrithealaiche-lìn agad, is iad na ceadan
bunaiteach a thathar a’ moladh:

- 755 airson pasgain
- 644 airson faidhlichean
- 444 airson an fhaidhle `configuration.php` (nuair a thèid atharrachadh air
  Rèiteachadh na Cruinne a shàbhaladh, bidh Joomla an toiseach ag atharrachadh a’ chead gu 644,
  a’ sàbhaladh an atharrachaidh agus an uair sin ag atharrachadh a’ chead air ais gu 444)

<div class="alert alert-warning">
Rabhadh!

Na cleachd 777 gu bràth mura h-eil fios agad dè tha thu a’ dèanamh! Na cleachd leudachain a
dh’fheumas ceadan 777!
</div>

## Mar a Lorgar na Ceadan

Tha diofar dhòighean rim faighinn gus ceadan fhaidhlichean no phasganan làraich-lìn fhaicinn agus
atharrachadh. Bu chòir do bhrobhsair fhaidhlichean pannal-smachd an aoigheachd no prògram cumanta
[File Transfer Protocol (FTP)](https://en.wikipedia.org/wiki/File_Transfer_Protocol)
dòigh a thoirt seachad airson ceadan fhaidhlichean is phasganan fhaicinn agus atharrachadh. Tha an
loidhne-àithne feumail dhaibhsan aig a bheil cothrom air ceann-uidhe agus eòlas air òrdughan an t-siostaim.

A rèir na tha thu a’ cleachdadh, bu chòir dhut rudeigin mar an ìomhaigh seo de phàirt de shiostam
fhaidhlichean freumh Joomla fhaicinn mar a chithear ann an cPanel:

![a’ dearbhadh cheadan ann an cPanel](../../../en/images/test-installations/permissions-linux/01-verifying-permissions-cpanel.png)

Tha na ceadan aig an fhìor làimh dheis agus neoni romhpa gus innse gur e àireamhan ochdail a th’ annta.
Bu chòir foirm a bhith ann gus ceadan aon nì no barrachd a thagh thu atharrachadh:

![ag atharrachadh cheadan ann an cPanel](../../../en/images/test-installations/permissions-linux/02-verifying-permissions-cpanel-change.png)

Ann an uinneag ceann-uidhe, tha ceadan fhaidhlichean is phasganan air an taisbeanadh mar bhuidhnean
litrichean seach àireamhan (tha an `d` aig toiseach a’ nochdadh gur e pasgan a th’ anns an nì):

```sh
drwxr-xr-x   20 ceford  staff     640 14 Oct 22:23 components
-r--r--r--    1 ceford  staff    3485 27 Oct 06:56 configuration.php
drwxr-xr-x    2 ceford  staff      64 20 Oct 14:21 files
-rw-r--r--    1 ceford  staff    6899 30 Sep 09:27 htaccess.txt
drwxr-xr-x   15 ceford  staff     480 24 Oct 12:19 images
```

## Àireamhan nan Ceadan

Ann an taisbeanadh cheadan den chruth 777, tha gach digiteach ochdail a’ freagairt ri trì litrichean
airson trì buidhnean luchd-cleachdaidh eadar-dhealaichte:

- A’ chiad digiteach = sealbhadair (sealbhadair an nì - `ceford` anns an liosta loidhne-àithne gu h-àrd)
- An dàrna digiteach = buidheann (a’ bhuidheann aig a bheil cead inntrigidh - `staff` anns an liosta gu h-àrd)
- An treas digiteach = feadhainn eile (a h-uile duine eile air a’ choimpiutair seo)

## Brìgh nan àireamhan

Is e gach digiteach ochdail suim nan ceadan a chaidh a bhuileachadh:
```sh
     r = Read    = 4
     w = Write   = 2
     x = Execute = 1
```

Cuir na h-àireamhan airson gach cead a tha a dhìth leis a’ bhuidheann chleachdaichean iomchaidh:

| \# “Ochtail” | (r)ead | (w)rite | e(x)ecute | Cleachdaiche no Buidheann no Eile |
|------------|--------|---------|-----------|-------------------------|
| 0          | chan eil | chan eil | chan eil | `---` 0+0+0 = 0         |
| 1          | chan eil | chan eil | tha       | `--x` 0+0+1 = 1         |
| 2          | chan eil | tha     | chan eil  | `-w-` 0+2+0 = 2         |
| 3          | chan eil | tha     | tha       | `-wx` 0+2+1 = 3         |
| 4          | tha      | chan eil | chan eil  | `r--` 4+0+0 = 4         |
| 5          | tha      | chan eil | tha       | `r-x` 4+0+1 = 5         |
| 6          | tha      | tha     | chan eil  | `rw-` 4+2+0 = 6         |
| 7          | tha      | tha     | tha       | `rwx` 4+2+1 = 7         |

## Eisimpleirean

- Tha 755 co-ionann ri rwx (sealbhadair), r-x (buidheann) agus r-x (feadhainn eile), no ann am faclan eile,
  faodaidh a h-uile duine leughadh agus cur an gnìomh (ruith), ach chan fhaod ach an sealbhadair
  (thu fhèin) atharrachaidhean a dhèanamh air an fhaidhle. Bhiodh e coltach ri seo nuair a chuireadh
  a h-uile càil ri chèile: `-rwxr-xr-x`. Is e seo an suidheachadh àbhaisteach airson phasganan.
- Tha 644 co-ionann ri rw-, r--, r--, no faodaidh A H-UILE DUINE am faidhle a leughadh, ach chan fhaod ach an
  sealbhadair sgrìobhadh dhan fhaidhle, no `-rw-r--r--`. Is e seo an suidheachadh àbhaisteach airson fhaidhlichean.
- Tha 777 no `-rwxrwxrwx` a’ ciallachadh gum faod A H-UILE DUINE faidhle SAM BITH a leughadh, a sgrìobhadh agus a chur an gnìomh
  <div class="alert alert-warning">
  Seo rud nach eil thu **A CHAOIDH** airson a cheadachadh air an fhrithealaiche/làrach-lìn agad
  mura h-eil thu buileach cinnteach gu bheil fios agad dè tha thu a’ dèanamh.
  </div>

Thathar a’ cleachdadh cheadan airson pasgain a bharrachd air faidhlichean, agus is e sin as coireach
gum faic thu `drwxr-xr-x` far a bheil an `d` a’ seasamh airson pasgan.

Airson mìneachadh slàn, leugh an t-artaigil Wikipedia air
[Ceadan an t-siostaim-fhaidhlichean](https://en.wikipedia.org/wiki/Filesystem_permissions)

*Air eadar-theangachadh le openai.com*