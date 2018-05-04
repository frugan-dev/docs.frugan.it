Configurazione dei client WebDAV
================================

Se si dispone di un account WebDAV `EWake <https://ewake.it>`_ è possibile autenticarsi sia tramite browser che tramite le risorse di rete del proprio sistema operativo:

+--------------------------------------------------------------------------------------------+
| WebDAV                                                                                     |
+======================+=====================================================================+
| Server               | davs://`domain.tld`/webdav/`directory` - *(Mac/Linux)*              |
|                      |                                                                     |
|                      | davs://`username` @ `domain.tld`/webdav/`directory` - *(Mac/Linux)* |
|                      |                                                                     |
|                      | https://`domain.tld`/webdav/`directory` - *(Windows, browser)*      |
+----------------------+---------------------------------------------------------------------+
| Autenticazione       | password normale                                                    |
+----------------------+---------------------------------------------------------------------+

Dove `domain.tld`, `directory` e `username` sono i parametri associati al proprio account WebDAV presso `EWake <https://ewake.it>`_.

Di seguito sono elencate anche le istruzioni dettagliate per la configurazione sui principali dispositivi:

.. toctree:: 
   :maxdepth: 1

   webdav/mac
   webdav/windows
   webdav/linux