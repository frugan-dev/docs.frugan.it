Configurazione dei client di posta
==================================

I parametri necessari per l'autenticazione ai server di posta `EWake <https://ewake.it>`_ tramite i comuni client di posta elettronica (ad es. Outlook, Thunderbird, ecc.) sono uguali per tutte le caselle ospitate presso `EWake <https://ewake.it>`_:

+-----------------------------------------------------------+
| Posta in arrivo - IMAP                                    |
+======================+====================================+
| Server               | imap.ewake.it                      |
+----------------------+------------------------------------+
| Porte                | 993 *(consigliata)* o 143          |
+----------------------+------------------------------------+
| Connessione protetta | SSL/TLS *(consigliata)* o STARTTLS |
+----------------------+------------------------------------+
| Autenticazione       | password normale                   |
+----------------------+------------------------------------+

+-----------------------------------------------------------+
| Posta in arrivo - POP3                                    |
+======================+====================================+
| Server               | pop.ewake.it                       |
+----------------------+------------------------------------+
| Porte                | 995 *(consigliata)* o 110          |
+----------------------+------------------------------------+
| Connessione protetta | SSL/TLS *(consigliata)* o STARTTLS |
+----------------------+------------------------------------+
| Autenticazione       | password normale                   |
+----------------------+------------------------------------+

+-----------------------------------------------------------+
| Posta in uscita - SMTP                                    |
+======================+====================================+
| Server               | smtp.ewake.it                      |
+----------------------+------------------------------------+
| Porte                | 465 *(consigliata)* o 587          |
+----------------------+------------------------------------+
| Connessione protetta | SSL/TLS *(consigliata)* o STARTTLS |
+----------------------+------------------------------------+
| Autenticazione       | password normale                   |
+----------------------+------------------------------------+

.. 
	attention (Attenzione)
	caution (Attenzione)
	danger (Pericolo)
	error (Errore)
	hint (Consiglio)
	important (Importante)
	note (Nota)
	tip (Suggerimento)
	warning (Avvertimento)
	admonition (non visibile)
	title (diventa il titolo della pagina)
.. note:: A prescindere dal dominio utilizzato, l'autenticazione ai server di posta `EWake <https://ewake.it>`_ avviene sempre tramite hostname del tipo `*.ewake.it`.


.. _user-email-ewake-conf-ref1:

Istruzioni per la configurazione sui principali dispositivi
===========================================================

Di seguito sono elencate anche le istruzioni dettagliate per la configurazione sui principali dispositivi:

.. toctree:: 
   :maxdepth: 1

   conf/mobile
   conf/mobile_nokia_symbian
   conf/android
   conf/iphone_ipad_ios6
   conf/iphone_ipad_ios7
   conf/mail_osx
   conf/opera_mail
   conf/outlook_2003
   conf/outlook_2007
   conf/outlook_2010
   conf/outlook_2011_mac
   conf/outlook_2013
   conf/outlook_express
   conf/thunderbird
   conf/windows_live_mail
   conf/windows_live_mail_2011
   conf/windows_mail
   conf/windows_phone