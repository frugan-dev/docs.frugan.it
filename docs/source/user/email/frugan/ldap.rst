Utilizzo delle rubriche LDAP
============================

Gli utenti che utilizzano il servizio LDAP fornito da `Frugan <https://frugan.it>`_ possono configurare sui loro dispositivi la connessione ai server LDAP per la condivisione delle loro rubriche tramite i seguenti parametri:

+--------------------------------------------------------------------------------------+
| Rubrica pubblica                                                                     |
+======================+===============================================================+
| Server               | ldap.frugan.it                                                 |
+----------------------+---------------------------------------------------------------+
| Porta                | 389                                                           |
+----------------------+---------------------------------------------------------------+
| Base DN              | `ou=public,ou=addressbook,dc=username,dc=it,dc=base`          |
+----------------------+---------------------------------------------------------------+
| DN associato         | `cn=Public,ou=users,ou=addressbook,dc=username,dc=it,dc=base` |
+----------------------+---------------------------------------------------------------+
| Connessione protetta | no                                                            |
+----------------------+---------------------------------------------------------------+
| Autenticazione       | password normale                                              |
+----------------------+---------------------------------------------------------------+

+----------------------------------------------------------------------------------------------------+
| Rubrica privata                                                                                    |
+======================+=============================================================================+
| Server               | ldap.frugan.it                                                               |
+----------------------+-----------------------------------------------------------------------------+
| Porta                | 389                                                                         |
+----------------------+-----------------------------------------------------------------------------+
| Base DN              | `ou=hello@domain.tld,ou=private,ou=addressbook,dc=username,dc=it,dc=base`   |
+----------------------+-----------------------------------------------------------------------------+
| DN associato         | `cn=hello@domain.tld,ou=users,ou=addressbook,dc=username,dc=it,dc=base`     |
+----------------------+-----------------------------------------------------------------------------+
| Connessione protetta | no                                                                          |
+----------------------+-----------------------------------------------------------------------------+
| Autenticazione       | password normale                                                            |
+----------------------+-----------------------------------------------------------------------------+

Dove `username` è il nome utente associato al servizio LDAP e `hello@domain.tld` corrisponde all'email ospitata presso `Frugan <https://frugan.it>`_.

Di seguito sono elencate anche le istruzioni dettagliate per la configurazione sui principali dispositivi:

.. toctree:: 
   :maxdepth: 1

   ldap/outlook_2007_addressbook
   ldap/thunderbird_addressbook