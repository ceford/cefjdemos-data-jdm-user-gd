<!--
{
    "source": "https://docs.joomla.org/J4.x:Optional_Technical_Requirements",
    "title": "Riatanasan Teicnigeach Rogainneil",
    "description": " ",
    "author": ""
}
-->

Tha an duilleag seo a’ liostadh *riatanasan teicnigeach roghainneil* nach eil riatanach airson Joomla! a stàladh agus a ruith, ach a tha riatanach airson cuid de APIan a-staigh. Chaidh an liosta a chruthachadh airson Joomla 4.

| Nì                       | Tuairisgeul                                                                                                                                     |
|---------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| **Iarrtas**               |                                                                                                                                                 |
| JApplicationDaemon        | Feumaidh e ext/pcntl agus ext/posix PHP                                                                                                          |
| **Tasglann**              |                                                                                                                                                 |
| BZ2                       | Feumaidh e ext/bz2 PHP                                                                                                                           |
| GZip                      | Feumaidh e ext/zlib PHP                                                                                                                          |
| Zip                       | Feumaidh e ext/zip no ext/zlib PHP                                                                                                                |
| **Tasgadan**              |                                                                                                                                                 |
| APC                       | Feumaidh e ext/apc PHP air PHP 5.3 no 5.4, ext/apcu air PHP 5.5 no 5.6, gun taic air PHP 7.x (Nota: FEUMAIDH SEO A BHITH AIR A SGRÙDADH)                |
| APCu                      | Feumaidh e ext/apcu PHP air PHP 5.3+                                                                                                             |
| CacheLite                 | Feumaidh e pasgan PEAR Cache_Lite (air a dhearbhadh air 1.7.16, obraichidh e le 1.8)                                                             |
| Memcache                  | Feumaidh e ext/memcache PHP agus frithealaiche Memcache (Nota: Chan eil an leudachan Memcache co-chòrdail ri PHP 7.x)                            |
| Memcached                 | Feumaidh e ext/memcached PHP agus frithealaiche Memcached                                                                                         |
| Redis                     | Feumaidh e ext/redis PHP agus frithealaiche Redis                                                                                                 |
| Wincache                  | Feumaidh e ext/wincache PHP (Windows a-mhàin)                                                                                                     |
| XCache                    | Feumaidh e ext/xcache PHP                                                                                                                         |
| **Adaptaran cliant**      |                                                                                                                                                 |
| LDAP                      | Feumaidh e ext/ldap PHP                                                                                                                           |
| HTTP/Curl                 | Feumaidh e ext/curl PHP                                                                                                                           |
| HTTP/Socket               | Feumaidh gnìomh fsockopen() PHP a bhith an comas                                                                                                  |
| HTTP/Stream               | Feumaidh e gnìomh fopen() PHP agus allow_url_fopen a bhith an comas                                                                                |
| **Criptografaidheachd**   |                                                                                                                                                 |
| JCrypt                    | Feumaidh e ext/mcrypt PHP airson a h-uile cipher ach a-mhàin SodiumCipher, a dh’fheumas ext/sodium                                                |
| JKeychain                 | Feumaidh e ext/openssl PHP                                                                                                                        |
| **Stòr-dàta**              |                                                                                                                                                 |
| Microsoft SQL Azure       | Feumaidh e ext/sqlsrv PHP (chan eil leudachan PHP 5.x a’ cur taic ach ri Windows; tha tionndadh den leudachan a tha co-chòrdail ri Linux ri fhaighinn airson PHP 7.x) |
| Microsoft SQL Server      | Feumaidh e `ext/sqlsrv` aig PHP (chan eil an leudachan PHP 5.x a’ cur taic ach ri Windows; tha tionndadh dhen leudachan a tha co-chòrdail ri Linux ri fhaighinn airson PHP 7.x) |
| MySQL                     | Feumaidh e `ext/mysql` aig PHP (chan eil taic ann air PHP 7.x)                                                                                             |
| MySQLi                    | Feumaidh e `ext/mysqli` aig PHP                                                                                                                     |
| Oracle                    | Feumaidh e `ext/pdo` aig PHP le taic Oracle (ri fhaighinn airson 3PD a-mhàin; cha ruith an CMS leis)                                                |
| PDO MySQL                 | Feumaidh e `ext/pdo` aig PHP le taic MySQL                                                                                                     |
| PostgreSQL                | Feumaidh e `ext/pgsql` aig PHP                                                                                                                      |
| SQLite                    | Feumaidh e `ext/pdo` aig PHP le taic SQLite (ri fhaighinn airson 3PD a-mhàin; cha ruith an CMS leis)                                                |
| **Ìomhaigh**                 |                                                                                                                                                 |
|                           | Feumaidh e `ext/gd` aig PHP                                                                                                                         |
|                           | Feumaidh e `ext/fileinfo` aig PHP                                                                                                                   |
| **Seisean**               |                                                                                                                                                 |
| APC                       | Feumaidh e `ext/apc` aig PHP 5.3 no 5.4, `ext/apcu` aig PHP 5.5 no 5.6, gun taic air PHP 7.x (Nota: FEUMAIDH SEO A BHITH AIR A SGRÙDADH)               |
| Memcache                  | Feumaidh e `ext/memcache` aig PHP agus frithealaiche Memcache (Nota: chan eil an leudachan Memcache co-chòrdail ri PHP 7.x)                               |
| Memcached                 | Feumaidh e `ext/memcached` aig PHP agus frithealaiche Memcached                                                                                           |
| Wincache                  | Feumaidh e `ext/wincache` aig PHP (Windows a-mhàin)                                                                                                    |
| XCache                    | Feumaidh e `ext/xcache` aig PHP                                                                                                                     |
| **LEASACHAIDHEAN ROGHAINNEIL** |                                                                                                                                                 |
| **Sreang**                |                                                                                                                                                 |
| mbstring                  | Cuir an comas `ext/mbstring` aig PHP gus an leabharlann phputf8 na gnìomhan dùthchasach a chleachdadh                                                                     |

*Air eadar-theangachadh le openai.com*