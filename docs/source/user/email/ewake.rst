EWake
=====

Acceso alla webmail
-------------------

La webmail principale per accedere alle caselle email `EWake <https://ewake.it>`_ è raggiungibile al seguente indirizzo:

- `http://webmail.domain.tld` (Roundcube)

dove `domain.tld` corrisponde al dominio ospitato presso `EWake <https://ewake.it>`_.

.. image:: /assets/img/email/ewake/webmail/roundcube.png

Per autenticarsi è necessario digitare il proprio indirizzo email (ad es. `hello@domain.tld`) nel campo **Nome utente** e la password nel campo **Password**.

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
.. hint:: Si consiglia fortemente l'utilizzo, tramite l'app `Google Authenticator <https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2&hl=it>`_, del sistema di `autenticazione a due fattori <https://it.wikipedia.org/wiki/Autenticazione_a_due_fattori>`_ (Two-Factor authentication) attivabile nelle impostazioni della webmail principale.


Sono inoltre disponibili altre webmail secondarie ai seguenti indirizzi:

- `http://domain.tld/webmail2` (AfterLogic WebMail Lite)
- `http://domain.tld/webmail3` (RainLoop Webmail Community ed.)
- `http://domain.tld/webmail4` (SquirrelMail)

.. 
	- `http://domain.tld/webmail` (MailPile) https://www.mailpile.is Python opensource
	- `http://domain.tld/webmail` (Tutanota) https://tutanota.com NodeJs encryped mail opensource
	- `http://domain.tld/webmail` (Cypht) https://cypht.org PHP multiple accounts opensource
	- `http://domain.tld/webmail` (Horde) https://www.horde.org suite
	
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
.. note:: La disponibilità delle webmail secondarie può variare nel tempo per questioni tecniche;
	inoltre alcuni servizi aggiuntivi, come ad es. la modifica della propria password o l'utilizzo delle rubriche condivise tramite LDAP, 
   	non sono disponibili sulle webmail secondarie.
   	

Configurazione dei client di posta
----------------------------------

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
-----------------------------------------------------------

Di seguito sono elencate anche le istruzioni dettagliate per la configurazione sui principali dispositivi:

.. toctree:: 
   :maxdepth: 1

   ewake/conf/mobile
   ewake/conf/mobile_nokia_symbian
   ewake/conf/android
   ewake/conf/iphone_ipad_ios6
   ewake/conf/iphone_ipad_ios7
   ewake/conf/mail_osx
   ewake/conf/opera_mail
   ewake/conf/outlook_2003
   ewake/conf/outlook_2007
   ewake/conf/outlook_2010
   ewake/conf/outlook_2011_mac
   ewake/conf/outlook_2013
   ewake/conf/outlook_express
   ewake/conf/thunderbird
   ewake/conf/windows_live_mail
   ewake/conf/windows_live_mail_2011
   ewake/conf/windows_mail
   ewake/conf/windows_phone

.. toctree:: 
   :maxdepth: 2

   ewake/webmail
   ewake/conf
   ewake/ldap
