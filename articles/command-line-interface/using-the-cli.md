<!--
{
    "source": "https://docs.joomla.org/J4.x:Using_the_CLI",
    "title": "A\u2019 cleachdadh an CLI",
    "description": " ",
    "author": ""
}
-->

## Eadar-aghaidh na Loidhne-àithne (CLI)

Ma tha cothrom agad air ceann-uidhe an fhrithealaiche a tha a’ ruith na làraich-lìn agad, faodaidh tu an Joomla CLI a chleachdadh gus gnìomhan àbhaisteach a choileanadh gun fheum air teisteanasan logaidh a-steach cleachdaiche Joomla. Fiù ’s às aonais cothrom air ceann-uidhe, mar a thachras le cuid de chunntasan aoigheachd cho-roinnte, faodaidh tu òrdughan CLI a ruith a’ cleachdadh obraichean cron. Gu tric tha òrdughan CLI nas luaithe no nas goireasaiche na na co-ionnanachdan a thèid a choileanadh tro eadar-aghaidh Rianaire Joomla (no cPanel). Tha lethbhreac-glèidhidh na làraich agus suidheachadh na làraich far loidhne/no loidhne nan eisimpleirean far am b’ fheàrr leat an CLI a chleachdadh.

Tha mu 30 òrdugh feumail aig cridhe Joomla agus faodaidh tu barrachd a chur ris le leudachain a bharrachd. Mar eisimpleir, dh’fhaodadh tu dàta bhon taobh a-muigh fhaighinn, leithid dàta Geolocation no ìrean iomlaid, airson co-phàirt ghnàthaichte.

## A’ cleachdadh an CLI

Tha an CLI air a chleachdadh le bhith a’ gairm an fhaidhle-ruith php loidhne-àithne. Gu tric tha seo eadar-dhealaichte bhon fhear a chleachdas frithealaiche-lìn leithid Apache. Ma tha thu a’ cleachdadh obair cron, ’s dòcha gum feum thu an t-slighe iomlan dhan fhaidhle-ruith php a thoirt seachad, mar seo:

    /usr/local/bin/php /home/username/public_html/[optional subfolder]/cli/joomla.php

Air neo, nuair a tha thu a’ cleachdadh loidhne-àithne a’ chrìoch-uidhe, atharraich an t-eòlaire dhan eòlaire cli aig Joomla agus tòisich le bhith a’ ruith an òrduigh gun pharamadairean:

    cd /home/username/public_html/[optional subfolder]/cli
    php joomla.php

![Liosta nan òrdughan](../../../en/images/command-line-interface/using-the-cli/01-cli-command-list.png)

Agus feuch cuid de dh’òrdughan cuideachaidh gus fàs eòlach air na bu chòir a bhith an dùil:

    php joomla.php help
    php joomla.php list
    php joomla.php help cache:clean
    php joomla.php help config:get

Tha gach tuairisgeul Cuideachaidh agus sreang cleachdaidh air an còdachadh gu cruaidh ann am faidhlichean leabharlann Console no ann am plugain treas-phàrtaidh.

Feuch cuid de dh’òrdughan gnìomha sìmplidh:

    php joomla.php config:get debug
    php joomla.php cache:clean
    php joomla.php site:down
    php joomla.php site:up

## Roghainnean

Ma tha thu a’ gairm òrdughan bho cron, ’s dòcha nach eil thu airson toradh sam bith fhaicinn:

    php joomla.php -q cache:clean

Thoir an aire gum faod roghainnean beàrn no soidhne = a chleachdadh, ach feumaidh caochladairean soidhne = a chleachdadh:

    php joomla.php session:gc --application administrator
    php joomla.php session:gc --application=administrator

    php joomla.php config:set debug=true

## Òrdughan

Mìneachadh goirid air gach prìomh òrdugh.

### Tasgadan

Glan inntrigidhean a dh’fhalbh an ùine bhon tasgadan shiostaim:

    php joomla.php cache:clean --help
    php joomla.php cache:clean

![Toradh glanadh an tasgadain](../../../en/images/command-line-interface/using-the-cli/02-cli-cache-clean.png)

php joomla.php cache:clean expired

![Toradh glanadh nan inntrigidhean a dh’fhalbh an ùine](../../../en/images/command-line-interface/using-the-cli/03-cli-cache-clean-expired.png)

### Rèiteachadh

Faigh no suidhich caochladair rèiteachaidh, aon de na caochladairean ann an configuration.php no buidheann de chaochladairean. ’S iad na buidhnean dligheach db, session, mail,

    php joomla.php config:get debug --help
    php joomla.php config:get debug

![Toradh config get debug](../../../en/images/command-line-interface/using-the-cli/04-cli-get-debug.png)

php joomla.php config:set debug=true

![Toradh config set debug](../../../en/images/command-line-interface/using-the-cli/05-cli-set-debug.png)

php joomla.php config:get --group session

![Toradh config get group session](../../../en/images/command-line-interface/using-the-cli/06-cli-config-get-group-session.png)

### Bun-stèidh

Thoir sùil airson ùrachaidhean no ùraich Joomla.

    php joomla.php core:check-updates --help
    php joomla.php core:check-updates

![Toradh sgrùdadh ùrachaidhean a’ bhun-stèidh](../../../en/images/command-line-interface/using-the-cli/07-cli-check-updates.png)

php joomla.php core:update --help
    php joomla.php core:update

![Toradh ùrachadh a’ bhun-stèidh](../../../en/images/command-line-interface/using-the-cli/08-cli-core-update.png)

### Stòr-dàta

Às-phortaich no ion-phortaich an stòr-dàta. Faodaidh tu na clàran uile no clàr taghte às-phortadh no ion-phortadh. Na cleachd am feart seo gus na clàran uile de làrach ioma-chànanach ion-phortadh. Tha duilgheadas ann a dh’fhaodadh stad a chur air Smart Search ag obair gu tur.

    php joomla.php database:export --help
    php joomla.php database:export --table f4rc2_banners --folder /home/username/tmp/mydb (one table)
    php joomla.php database:export --folder /home/username/tmp/mydb (all tables)

    php joomla.php database:import --help
    php joomla.php database:import --table /home/username/tmp/mydb/f4rc2_banners (one table)
    [ERROR] The /home/username/tmp/mydb/f4rc2_banners.xml file does not exist.
    php joomla.php database:import --folder /home/username/tmp/mydb (all tables in this folder)

### Leudachan

Dèan liosta, lorg, stàlaich no thoir air falbh leudachain.

    php joomla.php extension:list --help
    php joomla.php extension:list
    php joomla.php extension:list --type component
    php joomla.php extension:list --type file
    php joomla.php extension:list --type language
    php joomla.php extension:list --type library
    php joomla.php extension:list --type module
    php joomla.php extension:list --type package
    php joomla.php extension:list --type plugin
    php joomla.php extension:list --type template

    php joomla.php extension:discover --help
    php joomla.php extension:discover
    php joomla.php extension:discover:list
    php joomla.php extension:discover:install --eid=

    php joomla.php extension:install --help
    php joomla.php extension:install --path=
    php joomla.php extension:install --url=

    php joomla.php extension:remove --help
    php joomla.php extension:remove

### Lorgaire

Glan agus ath-thog an clàr-amais (thèid na criathragan luirg a ghleidheadh).

    php joomla.php finder:index --help
    php joomla.php finder:index
    php joomla.php finder:index purge

![Toradh glanadh clàr-amais an lorgaire](../../../en/images/command-line-interface/using-the-cli/09-cli-finder-index-purge.png)

### Clàraiche

Dèan liosta de ghnìomhan clàraichte, atharraich an staid aca no ruith iad.

    php joomla.php scheduler:list --help
    php joomla.php scheduler:list

    php joomla.php scheduler:state --help
    php joomla.php scheduler:state (interactive prompt for task id)

    php joomla.php scheduler:run --help
    php joomla.php scheduler:run --id ID
    php joomla.php scheduler:run --all

### Seisean

Dèan cruinneachadh sgudail an t-seisein.

    php joomla.php session:gc --help
    php joomla.php session:gc
    php joomla.php session:gc --application administrator

    php joomla.php session:metadata:gc --help
    php joomla.php session:metadata:gc

### Làrach

Cuir an làrach far loidhne no air loidhne.

    php joomla.php site:down --help
    php joomla.php site:down

    php joomla.php site:up --help
    php joomla.php site:up

### Ùrachadh

Sgrùdaidh e airson ùrachaidhean leudachan a tha ri thighinn. Bheir e air falbh seann fhaidhlichean a bu chòir a bhith air an sguabadh às rè ùrachadh Joomla.

    php joomla.php update:extensions:check --help
    php joomla.php update:extensions:check

    php joomla.php update:joomla:remove-old-files --help
    php joomla.php update:joomla:remove-old-files

![Toradh toirt air falbh seann fhaidhlichean Joomla às dèidh ùrachaidh](../../../en/images/command-line-interface/using-the-cli/10-cli-update-remove-old-files.png)

### Cleachdaiche

Dèan liosta de luchd-cleachdaidh agus stiùir iad.

    php joomla.php user:list --help
    php joomla.php user:list

    php joomla.php user:add --help
    php joomla.php user:add --username cinderella --name Cinderella --email cinders@localhost --usergroup Manager (prompt for password)
    php joomla.php user:add (prompts for data)

![Toradh cur cleachdaiche ris le molaidhean](../../../en/images/command-line-interface/using-the-cli/11-cli-add-user.png)

php joomla.php user:addtogroup --help
    php joomla.php user:addtogroup (prompts for data)
    php joomla.php user:addtogroup --usernam=cinderella --group=Manager

    php joomla.php user:removefromgroup --help
    php joomla.php user:removefromgroup (prompts for data)
    php joomla.php user:removefromgroup --usernam=cinderella --group=Manager

    php joomla.php user:reset-password --help
    php joomla.php user:reset-password (prompts for data)
    php joomla.php user:reset-password --username=cinderella (prompts for password)

    php joomla.php user:delete --help
    php joomla.php user:delete (prompts for username)
    php joomla.php user:delete --username=cinderella (prompts for confirmation - y to confirm)

*Air eadar-theangachadh le openai.com*