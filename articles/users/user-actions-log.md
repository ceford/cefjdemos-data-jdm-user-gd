<!--
{
    "source": "https://docs.joomla.org/J4.x:User_Actions_Log",
    "title": "Log Gn\u00ecomhan Cleachdaiche",
    "description": " ",
    "author": ""
}
-->

## Ro-ràdh

Tha co-phàirt Log Gnìomhan Cleachdaiche (com_actionlogs) a’ solarachadh
bun-structair airson log sgrùdaidh de ghnìomhan làraich-lìn a chruthachadh. Faodar
na gnìomhan a thèid a chlàradh a ghleusadh gu mionaideach le rianaire na làraich.
Tha leudachain treas-phàrtaidh comasach air ceangal ris a’ cho-phàirt gus teachdaireachdan
gnàthaichte a chur ris no gus toirt air an t-siostam gnìomhan rianaire àbhaisteach a phròiseasadh.

**Nota:** Chan eil cothrom aig ach Sàr-chleachdaichean air co-phàirt Log Gnìomhan Cleachdaiche.

## Log Gnìomhan Cleachdaiche

Gus liosta Log Gnìomhan Cleachdaiche fhaicinn:

- Tagh **Cleachdaichean → Log Gnìomhan Cleachdaiche** bho chlàr an Rianaire.

![duilleag liosta log ghnìomhan cleachdaiche](../../../gd/images/users/user-actions-log/01-user-actions-log-list.png)

Bhon duilleag seo, tha sealladh farsaing cruinneil aig Sàr-chleachdaiche air a h-uile gnìomh
cleachdaiche a chaidh a dhèanamh air làrach.

- Às-phortaich na chaidh a thaghadh mar CSV: às-phortaichidh am putan seo na nithean a chaidh a thaghadh a-mhàin
  san liosta fhaicsinneach.
- Às-phortaich na h-uile mar CSV: às-phortaichidh am putan seo a h-uile clàr. Thèid na criathragan
  a leigeil seachad.
- Sguab às: sguabaidh am putan seo às na nithean a chaidh a thaghadh.
- Falamhaich an Log: sguabaidh am putan seo às a h-uile inntrigeadh log.
- Roghainnean: foirm rèiteachaidh airson na roghainnean logaidh a shuidheachadh.

## Roghainnean

Tha am foirm Log Gnìomhan Cleachdaiche: Roghainnean a’ leigeil leis an t-Sàr-chleachdaiche taghadh dè na
tachartasan a thèid a chlàradh agus am bu chòir seòlaidhean IP a thoirt a-steach ann an dàta an loga.

![duilleag roghainnean log ghnìomhan cleachdaiche](../../../gd/images/users/user-actions-log/02-user-actions-log-options.png)

## Plugain

Tha an siostam logaidh ghnìomhan a’ cleachdadh grunn phlugan:

### Log Gnìomhan - Joomla

Nuair a tha am plugan an comas, clàraichidh e prìomh ghnìomhan nan cleachdaichean, a’ gabhail a-steach
gnìomhan leithid logadh a-steach/a-mach, ùrachadh artaigil agus modal a chur ris. Chan eil paramadairean
aig a’ phlugan,

### Siostam - Log Gnìomhan Cleachdaiche

Nuair a tha am plugan an comas, sònraichidh e an àireamh de làithean às dèidh sin a thèid na
logaichean a sguabadh às. Ma tha an luach neoni, cha tèid na logaichean a sguabadh às gu fèin-obrachail a-riamh.

### Prìobhaideachd - Logaichean Gnìomhan

Nuair a tha am plugan an comas, às-phortaichidh e dàta log nan gnìomhan airson iarrtas prìobhaideachd cleachdaiche.

## Modal nan Gnìomhan as Ùire

Chan eil am modal seo ri fhaicinn ach do Shàr-chleachdaichean ann an Deas-bhòrd na Dachaigh.

![modal log ghnìomhan cleachdaiche](../../../gd/images/users/user-actions-log/03-user-actions-log-module.png)

## Mar a cheanglas tu leudachan ris an t-siostam

Faodaidh tu an earrann seo a dheasachadh le bhith ga leasachadh no a’ ceartachadh mhearachdan innte.

### Sgriobt Stàlaidh na Co-phàirte

Cuir an leudachan ris a’ chlàr (`#__action_logs_extensions`) gus am bi e
a’ nochdadh ann an rèiteachadh Logaichean Gnìomhan Cleachdaiche.
```php
            $extension = 'com_mycomponent';
            $db = Factory::getDbo();
            $db->setQuery(' INSERT into #__action_logs_extensions (extension) VALUES ('.$db->Quote($extension).') ' );
            try {
                // If it fails, it will throw a RuntimeException
                $result = $db->execute();
            } catch (RuntimeException $e) {
                Factory::getApplication()->enqueueMessage($e->getMessage());
                return false;
            }
```

Cuir rèiteachadh an leudachain ris a’ chlàr (`#__action_log_config`) gus
am bi dàta nan gnìomhan agad air a ghlacadh.
```php
           $logConf = new stdClass();
            $logConf->id = 0;
            $logConf->type_title = 'transaction';
            $logConf->type_alias = $extension;
            $logConf->id_holder = 'id';
            $logConf->title_holder = 'trans_desc';
            $logConf->table_name = '#__mycomponent_transaction';
            $logConf->text_prefix = 'COM_MYCOMPONENT_TRANSACTION';

            try {
                // If it fails, it will throw a RuntimeException
                // Insert the object into the table.
                $result = Factory::getDbo()->insertObject('#__action_log_config', $logConf);
            } catch (RuntimeException $e) {
                Factory::getApplication()->enqueueMessage($e->getMessage());
                return false;
            }
```

Gu dearbh, bhiodh e na b’ fheàrr sgrùdadh a dhèanamh gus dèanamh cinnteach
nach eil an clàr ann mu thràth.

### Cuidear na Co-phàirte

San eisimpleir seo, thathar a’ cleachdadh cuidear na co-phàirte gus gnìomhan a stòradh.
```php
       /**
         * Record transaction details in log record
         * @param   object  $user    Saves getting the current user again.
         * @param   int     $tran_id  The transaction id just created or updated
         * @param   int     $id  Passed id reference from the form to identify if new record
         * @return  boolean True
         */
        public static function recordActionLog($user = null, $tran_id = 0, $id = 0)
        {
                // get the component details such as the id
            $extension =  MycomponentHelper::getExtensionDetails('com_mycomponent');
            // get the transaction details for use in the log for easy reference
            $tran = MycomponentHelper::getTransaction($tran_id);
            $con_type = "transaction";
            if ($id === 0) { $type = 'New '; } else { $type = 'Update '; }

            $message = array();
            $message['action'] = $con_type;
            $message['type'] = $type . $tran->tran_type . ' - '.$tran->tran_desc . ' $' . $tran->tran_amount;
            $message['id'] = $tran->id;
            $message['title'] = $extension->name;
            $message['extension_name'] = $extension->name;
            $message['itemlink'] = "index.php?option=com_mycomponent&task=transaction.edit&id=".$tran->id;
            $message['userid'] = $user->id;
            $message['username'] = $user->username;
            $message['accountlink'] = "index.php?option=com_users&task=user.edit&id=".$user->id;

            $messages = array($message);

            $messageLanguageKey = Text::_('COM_MYCOMPONENT_TRANSACTION_LINK');
            $context = $extension->name.'.'.$con_type;

            $fmodel = MycomponentHelper::getForeignModel('Actionlog', 'ActionlogsModel');

            $fmodel->addLog($messages, $messageLanguageKey, $context, $user->id);

            return true;
        }

        /**
         * Get the Model from another component for use
         * @param   string  $name    The model name. Optional. Default to my own for safety.
         * @param   string  $prefix  The class prefix. Optional
         * @param   array   $config  Configuration array for model. Optional
         * @return object   The model
         */
        public function getForeignModel($name = 'Transaction', $prefix = 'MycomponentModel', $config = array('ignore_request' => true))
        {
            \Joomla\CMS\MVC\Model\ItemModel::addIncludePath(JPATH_ADMINISTRATOR . '/components/com_actionlogs/models', 'ActionlogsModelActionlog');
            $fmodel = \Joomla\CMS\MVC\Model\ItemModel::getInstance($name, $prefix, $config);

            return $fmodel;
        }
```

### Foirm Gnothaich na Taobh Beulaibh

A-nis gu bheil na bunaitean suidhichte, chan eil againn ach am pròiseas a phiobrachadh.
Tha sinn a’ glacadh fiosrachaidh mu ghnothach a chaidh a chruthachadh no ùrachadh agus tha
modail againn air a bheil `transactionform.php`. ’S ann sa mhodh Save a tha sinn airson log a ghlacadh.
```php
       // So the code above this point checks and does what it should do and then after the successful save of the record, we check for the parameter setting to see if logging is required, we pass key elements to recordActionLog.
            $table = $this->getTable();

            if ($table->save($data) === true) {

                /* ---------------------------------------------------------------- */
                // trigger transaction log if required
                $act_log = $params->get('act_log', 0);
                if ($act_log && $table->id) {
                    // gather information and log in a new action log record
                    MycomponentHelper::recordActionLog($user, $table->id, $data['id']);
                }
                /* ---------------------------------------------------------------- */

                return $table->id;
            } else {
                return false;
            }
```

### Faidhle Cànain

Mu dheireadh, gus cuideachadh le Liosta nan Logaichean Gnìomhan ann an taobh rianachd
Joomla, tha sinn airson cuid de phrìomh eileamaidean dàta a shuidheachadh gus an tèid an taisbeanadh
anns an fhaidhle cànain en-GB/com_mycomponent.ini.
```ini
    COM_MYCOMPONENT_TRANSACTION_LINK="User {username} created a transaction ( {type} )"
```

*Air eadar-theangachadh le openai.com*