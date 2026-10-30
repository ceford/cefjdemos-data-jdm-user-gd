<!--
{
    "source": "https://docs.joomla.org/Keyboard_Shortcuts",
    "title": "Ath-ghoiridean Meur-chl\u00e0ir",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Faodar am meur-chlàr a chleachdadh ann an eadar-aghaidh an Rianaire gus cuid
de na gnìomhan a nì thu mar as trice leis an luchag no leis a’ phada a chur an
gnìomh. Mar eisimpleir, tha ath-ghoiridean meur-chlàir ann airson an duilleag
làithreach a shàbhaladh, a dhol gu *Deas-bhòrd na Dachaigh* no foirm
*Roghainnean* fhosgladh. 

Tha sealladh farsaing ann de na h-ath-ghoiridean uile, a thèid fhosgladh le
taghadh meur-chlàir de **J** agus **X** ann an sreath (chan ann aig an aon àm
agus na cleachd an iuchair Shift a chleachdar mar as trice airson litrichean
mòra). Mura h-atharraich thu roghainnean a’ phlugain, feumaidh tu na h-iuchraichean
a bhrùthadh taobh a-staigh 2 dhiog.

Tha am feart air a chomasachadh gu bunaiteach. Faodar a chur à comas no a
rèiteachadh fo **Rianaire → Siostam → Plugain → Siostam - Ath-ghoiridean
Meur-chlàir**. Aig an àm seo ’s e an ùine-às-dhàin an aon rèiteachadh: dè cho
fad ’s a dh’fheitheas an siostam airson an ath chur-a-steach agad bhon
mheur-chlàr. Gu bunaiteach, bidh e a’ feitheamh 2000 millisgeund (2 dhiog).

## Ath-ghoiridean Bunaiteach ann an Joomla

- J + A - Sàbhail an t-susbaint làithreach
- J + S - Airson Sàbhail agus Dùin
- J + Q - Sguir dhen duilleag làithreach
- J + N - Brùth am putan *Ùr*
- J + F - Suidhich am fòcas air raon an Lorg
- J + O - Rach gu Roghainnean
- J + H - Fosglaidh uinneag na Cobhair (faodaidh seo rabhadh mu uinneag bhrobhsaireir a chur an gnìomh)
- J + M - Tog am bàr clàr-taice air no dheth
- J + X - Seall liosta nan Ath-ghoiridean a tha rim faighinn
- J + D - Rach gu dìreach gu Deas-bhòrd na Dachaigh

## Ath-ghoiridean Treas-phàrtaidhean - Fiosrachadh do Luchd-leasachaidh

Faodaidh luchd-leasachaidh eile na h-ath-ghoiridean aca fhèin a chur ris
cuideachd. Bidh plugan Joomla a’ gairm an tachartais *onLoadShortcuts*, a
ghabhas cleachdadh le plugain eile cuideachd. Feumar an tachartas a chur ris
an liosta de *getSubscribedEvents* taobh a-staigh a’ phlugain. Dh’fhaodadh an
gnìomh a chaidh a shònrachadh coimhead mar seo:

```php
    public function onLoadShortcuts(EventInterface $event): void {
       $shortcuts = $event->getArgument('shortcuts');
       $exampleShortcuts = array('example' => (object)['shortcut' => 'E', 'title' => 'Great Example', 'selector' => '#menu-collapse']);
       $event->setArgument('shortcuts',  array_merge($shortcuts, $exampleShortcuts));
    }
```

Thoir aire shònraichte don phàirt array_merge: Nuair nach eil na
h-ath-ghoiridean a tha ann mu thràth air an co-aonadh leis na feadhainn ùra,
thèid sgrìobhadh thairis air na seann fheadhainn.

Faodaidh luchd-leasachaidh sreath de nithean ath-ghoirid a thoirt seachad:

    { shortcut: string, selector: string, title: string }

- Feumaidh an *Shortcut* a bhith na chur-a-steach meur-chlàir, air a sgaradh
  le plus, m.e. `Y` no `ALT + Z + 7` (an-dràsta chan eil sìoladh sam bith ann
  dha-rìribh). Cumaibh nur n-inntinn gun tòisich gach sreath ath-ghoirid le
  **J**.
- ’S e luchd-taghaidh CSS no URLan a th’ anns na *Selectors* gus an targaid a
  shònrachadh. Mas e eileamaid cuir-a-steach a th’ ann, bheir an ath-ghoirid
  fòcas dha, mar a thachras le raon an lorg. Air neo, thèid briogadh air an
  eileamaid no thèid an URL a ghairm.
- Thèid an *Title* a thaisbeanadh san t-sealladh fharsaing. Dh’fhaodadh gur e
  ainm na targaide a bhiodh ann, mar eisimpleir.

## Adhbharan airson J + X a chleachdadh

Dh’fhaodadh cuid iongnadh a dhèanamh mun cho-dhùnadh ath-ghoiridean
leantainneach a chleachdadh, no **J** mar thoiseach an àite Ctrl no rudeigin
eile. ’S iad ruigsinneachd agus seachnadh briseadh a-steach le bathar-bog eile
na prìomh adhbharan. Mar eisimpleir, bhiodh *Ctrl + S* feumail airson artaigil
a shàbhaladh, ach tha e air a chleachdadh leis na brobhsairean mu thràth.
Faodaidh an aon rud tachairt le leughadairean-sgrìn no manaidsearan faclan-
faire. Mar sin, b’ e an roghainn nas sàbhailte rudeigin a bha sònraichte do
Joomla a chleachdadh, leithid **J** aig an toiseach.

A-nis, ’s e an duilgheadas eile nach eil e an-còmhnaidh comasach barrachd air
aon iuchair a bhrùthadh aig an aon àm. Tha modh Sticky Key aig Windows airson
seo, ach chan obraich e ach airson iuchraichean atharrachaidh leithid Shift,
Ctrl agus Alt. Mar sin, bidh am plugan a’ cleachdadh cur-a-steach ann an
sreath bhon toiseach, rud a nì e comasach do bharrachd dhaoine a chleachdadh
eadhon às aonais cuideachadh bho mhòdan an t-siostaim-obrachaidh.

*Air eadar-theangachadh le openai.com*

