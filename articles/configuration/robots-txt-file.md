<!--
{
    "source": "https://docs.joomla.org/Robots.txt_file",
    "title": "Am faidhle robots.txt",
    "description": " ",
    "author": ""
}
-->

## Mu dheidhinn innealan-fuadain

’S e prògraman a th’ ann an innealan-fuadain-lìn, ris an canar cuideachd
luchd-sgùabaidh, luchd-coiseachd-lìn no damhain-allaidh, a bhios a’
seòladh na lìn gu fèin-obrachail. Am measg iomadh cleachdaidh, bidh
einnseanan-luirg gan cleachdadh gus susbaint na lìn a chlàr-amais.

Tha am faidhle robots.txt a’ cur an gnìomh am 
[Pròtacal Toirmeasg nan Innealan-fuadain](https://en.wikipedia.org/wiki/Robots_exclusion_standard),
a leigeas le rianaire làraich-lìn mìneachadh dè na pàirtean den làrach nach bu chòir
do riochdairean cleachdaiche innealan-fuadain sònraichte a sgrùdadh. Mar eisimpleir,
tha cead ga thoirt mar as trice faighinn gu susbaint nan duilleagan poblach, ach
gu tric thathar a’ toirmeasg faighinn gu pasgain cgi, phrìobhaideach agus
shealach nach bu chòir na duilleagan aca a chlàr-amais.

## Far an cuirear am faidhle *robots.txt*

Tha faidhle àbhaisteach *robots.txt* air a ghabhail a-steach ann am freumh Joomla. Feumaidh am
faidhle *robots.txt* a bhith ann am freumh an àrainn no an fho-àrainn agus
feumaidh e a bhith air ainmeachadh `robots.txt`.

### Joomla ann am Fo-phasgan

Chan eil faidhle robots.txt a tha ann am fo-phasgan dligheach. Cha dèan innealan-fuadain
sgrùdadh air an fhaidhle seo ach ann am freumh an àrainn. Ma tha làrach Joomla air
a stàladh ann am fo-phasgan mar *example.com/joomla/*, feumaidh am faidhle
*robots.txt* a bhith air a ghluasad gu freumh na làraich aig
*example.com/robots.txt*.

**Nota:** Anns an fhaidhle robots.txt, feumaidh ainm an fho-phasgain a bhith air thoiseach air
slighean Joomla sam bith nach eil ceadaichte. Mar eisimpleir, feumar an riaghailt toirmisg airson a’ phasgain `/administrator/`
atharrachadh gus `Disallow: /joomla/administrator/` a leughadh.

## Susbaint *robots.txt* Joomla

Seo susbaint [faidhle robots.txt àbhaisteach Joomla](https://raw.githubusercontent.com/joomla/joomla-cms/refs/heads/5.2-dev/robots.txt.dist):

```
# If the Joomla site is installed within a folder
# eg www.example.com/joomla/ then the robots.txt file
# MUST be moved to the site root
# eg www.example.com/robots.txt
# AND the joomla folder name MUST be prefixed to all of the
# paths.
# eg the Disallow rule for the /administrator/ folder MUST
# be changed to read
# Disallow: /joomla/administrator/
#
# For more information about the robots.txt standard, see:
# https://www.robotstxt.org/orig.html

User-agent: *
Disallow: /administrator/
Disallow: /api/
Disallow: /bin/
Disallow: /cache/
Disallow: /cli/
Disallow: /components/
Disallow: /includes/
Disallow: /installation/
Disallow: /language/
Disallow: /layouts/
Disallow: /libraries/
Disallow: /logs/
Disallow: /modules/
Disallow: /plugins/
Disallow: /tmp/
```

## Toirmeasg nan Innealan-fuadain

Faodaidh tu pasgain a thoirmeasg no casg a chur air innealan-fuadain bhon làrach agad le bhith a’ cur
riaghailt Disallow ris an fhaidhle *robots.txt*. Mar eisimpleir, gus casg a chur air innealan-fuadain sam bith bho bhith a’ tadhal air
a’ phasgan */tmp*, cuir an riaghailt seo ris:

    Disallow: /tmp/

Faic cuideachd:

- [Cuir casg air faighinn chun t-susbaint agad](https://support.google.com/webmasters/topic/4598466?hl=en&amp;ref_topic=9427949)
  ann an Ionad Cuideachaidh Google.

## Sgrùdadh Co-chàradh

Airson co-chàradh a sgrùdadh, faodaidh tu dearbhadair airson faidhlichean *robots.txt* a chleachdadh. Feuch
aon dhiubh seo:

- [Dèan deuchainn air do <em>robots.txt</em> leis an Deuchadair robots.txt](https://support.google.com/webmasters/answer/6062598) aig Google.
- [Dearbhadair <em>robots.txt</em>](http://www.searchenginepromotionhelp.com/m/robots-text-tester/robots-checker.php) le Search Engine Promotion Help.

### Fiosrachadh Coitcheann

- Is e [Duilleagan Innealan-fuadain na Lìn](http://www.robotstxt.org/) am prìomh làrach-lìn airson *robots.txt*.
- Is e [Inbhe airson Toirmeasg Innealan-fuadain](http://www.robotstxt.org/orig.html) an t-inbhe thùsail.
- [Sònrachaidhean taga meta Robots, data-nosnippet agus X-Robots-Tag](https://developers.google.com/search/docs/advanced/robots/robots_meta_tag)

*Air eadar-theangachadh le openai.com*

