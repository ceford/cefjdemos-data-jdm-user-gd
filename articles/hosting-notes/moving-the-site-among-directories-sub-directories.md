<!--
{
    "source": "https://docs.joomla.org/Moving_the_site_among_directories",
    "title": "A' Gluasad E\u00f2laire St\u00e0laidh",
    "description": " ",
    "author": ""
}
-->

Glè thric bidh thu a' stàladh Joomla ann am fo-eòlaire agus an uair sin ag iarraidh
a ghluasad gu eòlaire aig ìre nas àirde; seo oideachadh goirid air mar a nì thu sin.

Can gu bheil thu air Joomla a stàladh sa phasgan a leanas:
public_html/tryjoomla. A-nis gu bheil thu riaraichte leis an làrach, bidh thu
ag iarraidh a ghluasad gu public_html.

1. Gluais na faidhlichean uile bhon fho-eòlaire (i.e.,
    public_html/tryjoomla) chun an eòlaire aig an ìre as àirde (i.e., public_html).
    Faodaidh tu an cliant FTP as fheàrr leat a chleachdadh no am pannal-smachd a
    bheir an t-seirbheis aoigheachd agad dhut.
2. Luchdaich sìos am faidhle configuration.php agus fosgail e ann an deasaiche teacsa.
3. Dìreach thoir air falbh ainm a' phasgain tryjoomla bhon t-slighe. Coimhead airson
    na loidhnichean a leanas
    ```
    var $live_site = '';
    var $log_path = '/home/username/public_html/tryjoomla/administrator/logs';
    var $tmp_path = '/home/username/public_html/tryjoomla/tmp';
    var $ftp_root = 'public_html/tryjoomla';
    ```

    Atharraich gu:
    ```
    var $live_site = '';
    var $log_path = '/home/username/public_html/administrator/logs';
    var $tmp_path = '/home/username/public_html/tmp';
    var $ftp_root = 'public_html';
    ```

    N.B. Is ann ainneamh a dh'fheumas luach a bhith air a thoirt don chaochladair \$live_site. Ach ma
    chaidh luach a thoirt dha rè an stàlaidh, deasaich an t-slighe sin cuideachd.
    ```
    var $live_site = 'http://www.example.com/tryjoomla';
    ```

    Atharraich gu:
    ```
    var $live_site = 'http://www.example.com';
    ```

4. Thoir sùil air faidhle .htaccess na làraich agad. Bu chòir am fo-phasgan a thoirt air
    falbh às an sin cuideachd. Bu chòir an stiùireadh RewriteBase a bhith air a chur ann am
    beachd. Coimhead airson RewriteRule anns a bheil an seann fho-eòlaire.
5. Dearbhaich nach eil òrdughan ath-stiùiridh chun an t-seann fho-eòlaire nan àite
    ann am pannal-smachd na seirbheise aoigheachd agad.
6. Ma tha tasgadh air a chomasachadh, log a-steach do chùlaibh an rianaire (a bhios
    a-nis aig `http://www.example.com/administrator` agus chan ann aig
    `http://www.example.com/tryjoomla/administrator`). Rach gu
    Siostam / Tasg agus sguab às na faidhlichean tasgaidh uile.

*Eadar-theangaichte le openai.com*