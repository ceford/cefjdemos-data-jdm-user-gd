<!--
{
    "source": "https://docs.joomla.org/J4.x:Assorted_Issues",
    "title": "C\u00f9isean Measgaichte",
    "description": " ",
    "author": ""
}
-->

## Cùis Ath-stiùiridh an dèidh Ùrachadh gu 4.0.6

’S e buga a tha sin! Loidhne 243 de *plugins/system/redirect/redirect.php*:

       $db->updateObject('#__redirect_links', $redirect, 'id');

bu chòir dhi a bhith

       $this->db->updateObject('#__redirect_links', $redirect, 'id');

## Tha Duilleag a’ Nochdadh gun Stoidhleachadh

Adhbhar a dh’fhaodadh a bhith ann: Tha earrann gzip ann an *.htaccess* a’ dlùthadh
nam faidhlichean CSS agus JavaScript a tha air an dlùthadh mu thràth.

Faic an earrann seo den fhaidhle *.htaccess*:

    ## These directives are only enabled if the Apache mod_headers module is enabled.
    ## This section will check if a .gz file exists and if so will stream it
    ##     directly or fallback to gzip any asset on the fly
    ## If your site starts to look strange after enabling this, and you see
    ##     ERR_CONTENT_DECODING_FAILED in your browser console network tab,
    ##     then your server is already gzipping css and js files and you don't need this
    ##     block enabled in your .htaccess

    ...

Ma tha e ann, cuir beachd air no thoir air falbh e.

## Tha Liosta nam Modal Làraich Falamh

Adhbhar a dh’fhaodadh a bhith ann: Dh’fhaodadh meud bufair seòrsachaidh MySQL a bhith ro bheag.

A’ cleachdadh phpMyAdmin, rach gu **Dachaigh **→** Caochladairean **→** Meud bufair seòrsachaidh**.

Bu chòir dha a bhith co-dhiù 256K agus, mas fheàrr, 512K. Air cuid de sheirbheisean
aoigheachd cho-roinnte, dh’fhaodadh e a bhith air a shuidheachadh gu 128K. Iarr air an
t-seirbheis aoigheachd a mheudachadh.

## Fàilligidh an Ùrachadh an dèidh Ùrachadh gu 4.0.4

Adhbhar: atharrachadh riatanach don mhodh-obrachaidh Ùrachaidh a tha a’ toirt
buaidh air àireamh bheag de luchd-cleachdaidh.

Coimhead ann an *.htaccess* airson na loidhne seo:

    RewriteRule ^administrator/components/com_joomlaupdate/restore\.php$ - [L]

Atharraich i gu:

    RewriteRule ^administrator\/components\/com_joomlaupdate\/extract\.php$ - [L]

Airson tuilleadh fiosrachaidh, faic:

<a
href="https://www.joomla.org/announcements/release-news/5850-changes-to-update-process-that-you-need-to-be-aware-of.html"
rel="noreferrer noopener">Atharrachaidhean
don Mhòid-Obrach Ùrachaidh air am feum thu a bhith mothachail</a>

## Artaigilean Rim Faicinn san Stòr-dàta agus air an Aghaidh-aghaidh ach Gun a bhith Rim Faicinn san Backend

Bidh seo a’ tachairt nuair a thèid artaigilean a thoirt a-steach dìreach don stòr-dàta, rud a dh’obraich gu math ann an Joomla 3 ach nach eil ag obair ann an Joomla 4. Seo fuasgladh aon neach-cleachdaidh:

    I imported articles directly in the database into the #__content table like I often did in Joomla 3.
    However in Joomla 4 they were not visible.

    In Content > Categories, the category item counters counted the imported articles.
    But they were not visible in Content > Articles.

    I solved it by creating the necessary references in the #__workflow_associations table for each imported article:
    item_id = article ID, stage_id = 1 and extension = com_content.article.

Le seo bho neach-cleachdaidh eile:

Bu chòir don cheist seo a dhèanamh dhut. Cuir an ro-leasachan stòr-dàta agad fhèin an àite \#\_\_.

Bidh a’ cheist seo a’ cur casg air nithean dùblaichte ann an clàr nan co-cheanglaichean srutha-obrach

    INSERT INTO #__workflow_associations (item_id, stage_id, extension) 
    SELECT c.id as item_id, '1', 'com_content.article' FROM #__content AS c 
    WHERE NOT EXISTS (SELECT wa.item_id FROM #__workflow_associations AS wa WHERE wa.item_id = c.id);

*Air eadar-theangachadh le openai.com*

