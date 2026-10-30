<!--
{
    "source": "https://docs.joomla.org/How_do_you_put_a_module_inside_an_article%3F",
    "title": "Modalan taobh a-staigh Artaigilean",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Mar as trice bidh thu airson modalan a cheangal ri artaigilean ann an dòigh air choreigin.
Mar as trice thèid modalan a shònrachadh do shuidheachaidhean mhodalan, agus nochdaidh
suidheachaidhean nam modalan an àiteigin air an duilleag-lìn mar a tha air a dhearbhadh leis an teamplaid. Ach,
uaireannan tha e feumail modal a chur a-steach gu dìreach taobh a-staigh
artaigil. Tha plugan air a bheil *Content - Load Modules* aig Joomla airson sin a dhèanamh. Nuair a bhios e
air a chomasachadh, faodar modal a chur a-steach ann an artaigil ann an trì dòighean eadar-dhealaichte:

```
    {loadposition position,[style]}
    {loadmodule mod_type,the title,[style]}
    {loadmoduleid moduleId}
```

Far a bheil `style` mar aon de na luachan airson Stoidhle a’ Mhodaill bhon taba Adhartach den
fhoirm airson dàta a’ mhodail a chur a-steach, mar eisimpleir html, outline, table, card no noCard.

## loadposition

Gus modal a chur a-steach taobh a-staigh artaigil, foillsich am modal gu
suidheachadh agus luchdaich an suidheachadh sin san artaigil mar a leanas:

1.  Cruthaich modal agus suidhich a shuidheachadh gu ***myposition***.
    Faodaidh ***myposition*** a bhith na luach sam bith nach eil a’ dol an aghaidh suidheachadh teamplaid a tha ann mu thràth. Ann am foirm deasachaidh a’ mhodail, taip a-steach an suidheachadh ***myposition*** agus brùth air enter an àite a bhith ga thaghadh
    bhon liosta tuiteam-sìos.
2.  Sònraich am modal do **All** na Nithean Clàr-taice. Nì seo cinnteach
    gum bi e an-còmhnaidh ri fhaicinn, ge bith ciamar a ràinig an neach-tadhail an
    artaigil. Cha nochd am modal mura cleachd thu an àithne airson am modal a
    luchdachadh ann an artaigil.
3.  Deasaich an artaigil agus cuir a-steach an teacsa ***{loadposition myposition}*** aig
    an àite far a bheil thu airson gun nochd am modal.

**Nòta:** Ma tha am plugan *Content - Load Modules* à comas, nochdaidh an teacsa
*{loadposition myposition}* gun atharrachadh san artaigil. Cuideachd, bu chòir ainm
an t-suidheachaidh a bhith uile ann an litrichean beaga. Fàilligidh CamelCapitalization.

## loadmodule

Tha an co-chàradh *{loadmodule yyy}* a’ lorg a’ chiad mhodail aig a bheil an **seòrsa**
a’ maidseadh ris an t-sreang ‘yyy’. Mar sin, dh’fhaodadh tu modal *mod_login* a luchdachadh le
{loadmodule login} a chur san teacsa agad. Chan eil an seòrsa cho follaiseach sin! Mar
eisimpleir, ’s e **languages** an seòrsa airson Switcher Cànain. Gus an seòrsa a lorg, feumaidh tu coimhead tron liosta de phasganan mhodalan le manaidsear fhaidhlichean/eplorer agus am pàirt *mod_* den ainm pasgain a thoirt air falbh.

Ma tha thu airson eisimpleir shònraichte de mhodal a luchdachadh, leis gu bheil barrachd
na aon mhodal logaidh a-steach agad, mar eisimpleir leis na tiotalan Login 1, Login 2, msaa, feumaidh tu
{loadmodule mod_modType, modTitle} a chleachdadh, far am biodh **mod_modType** mar mod_login agus
**modTitle** mar an t-ainm/tiotal a chaidh a thoirt don eisimpleir agad den mhodal.
Mar sin, san eisimpleir gu h-àrd, gheibh thu **{loadmodule mod_login Login 2}**.

Faodaidh tu cuideachd an stoidhle a thèid a chleachdadh airson am modal a dheasachadh a chur ris. Gus
sin a dhèanamh, cuir an stoidhle ris mar an treas paramadair, mar ann an {loadmodule login,Login 2,xhtml}.
Mura cuir thu stoidhle ris, cha tèid gin a chleachdadh.

## loadmoduleid

Tha an co-chàradh *{loadmoduleid z}* a’ lorg a’ mhodail aig a bheil an `id` a’ maidseadh ris an
àireamh `z`. Mar sin, dh’fhaodadh tu am modal leis an id 200 a luchdachadh le
*{loadmoduleid 200}* a chur san teacsa agad. Chan eil an caochladh seo a’ cleachdadh pharamadairean a bharrachd leithid am paramadair `style`.

## Putan an Deasaiche

Ma tha am plugan editor-xtd *Button - Module* air a ghnìomhachadh, faodaidh tu am
putan deasaiche *Module* a chleachdadh gus na tagaichean a chaidh a mhìneachadh gu h-àrd a chur a-steach nas fhasa ann an teacsa an deasaiche. Tha putan aig liosta nam Modal anns a’ cholbh Tiotal gus cur a-steach a rèir id, agus putan anns a’ cholbh Suidheachaidh gus cur a-steach a rèir suidheachaidh.

## Modalan taobh a-staigh Mhodalan

Tha e comasach modal a chur a-steach taobh a-staigh modal *Custom HTML*. Tha iad
air an giullachd le plugain susbaint san aon dòigh ri artaigilean.

Dh’fhaodadh cùisean cruthachaidh èirigh leis gum bi stoidhle a’ mhodail *Custom HTML*
a’ cuairteachadh stoidhle a’ mhodail a chaidh a chur a-steach. Sin an t-adhbhar nach eil am putan
deasaiche *Module* ri fhaighinn ann am modalan den t-seòrsa *Custom*.

*Air eadar-theangachadh le openai.com*