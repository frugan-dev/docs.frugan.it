Microsoft Office 365
====================

Accesso alla webmail
--------------------

La webmail per accedere alle caselle email di `Microsoft Office 365 <https://www.zoho.com>`_ è raggiungibile al seguente indirizzo:

- `http://mail.domain.tld`

dove `domain.tld` corrisponde al dominio ospitato presso `EWake <https://ewake.it>`_.

Per autenticarsi è necessario digitare il proprio indirizzo email (ad es. `hello@domain.tld`) nel campo **Email** e la password nel campo **Password**.

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
.. hint:: Si consiglia fortemente l'utilizzo, tramite l'app `Google Authenticator <https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2&hl=it>`_, del sistema di `autenticazione a due fattori <https://support.microsoft.com/it-it/help/12408/microsoft-account-about-two-step-verification>`_ (Two-Factor authentication) attivabile nelle impostazioni dell'account Microsoft.
	


Configurazione dei client di posta
----------------------------------

I parametri necessari per l'autenticazione ai server di posta `Microsoft <https://www.zoho.com>`_ tramite i comuni client di posta elettronica (ad es. Outlook, Thunderbird, ecc.) sono uguali per tutte le caselle ospitate presso `EWake <https://ewake.it>`_:

+----------------------------------------------+
| Posta in arrivo - IMAP                       |
+======================+=======================+
| Server               | outlook.office365.com |
+----------------------+-----------------------+
| Porta                | 993                   |
+----------------------+-----------------------+
| Connessione protetta | SSL/TLS               |
+----------------------+-----------------------+
| Autenticazione       | password normale      |
+----------------------+-----------------------+

+----------------------------------------------+
| Posta in arrivo - POP3                       |
+======================+=======================+
| Server               | outlook.office365.com |
+----------------------+-----------------------+
| Porta                | 995                   |
+----------------------+-----------------------+
| Connessione protetta | SSL/TLS               |
+----------------------+-----------------------+
| Autenticazione       | password normale      |
+----------------------+-----------------------+

+-------------------------------------------+
| Posta in uscita - SMTP                    |
+======================+====================+
| Server               | smtp.office365.com |
+----------------------+--------------------+
| Porte                | 587                |
+----------------------+--------------------+
| Connessione protetta | SSL/TLS            |
+----------------------+--------------------+
| Autenticazione       | password normale   |
+----------------------+--------------------+

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
.. note:: A prescindere dal dominio utilizzato, l'autenticazione ai server di posta `Microsoft <https://www.zoho.com>`_ avviene sempre tramite hostname del tipo `*.office365.com`.


Accesso tramite Exchange ActiveSync (EAS)
-----------------------------------------

Di seguito i parametri per l'autenticazione ai server di posta `Microsoft <https://www.zoho.com>`_ tramite Exchange ActiveSync (EAS):

+----------------------+-----------------------+
| Server               | outlook.office365.com |
+----------------------+-----------------------+
| Dominio              | *lasciare vuoto*      |
+----------------------+-----------------------+
| Connessione protetta | SSL/TLS               |
+----------------------+-----------------------+
| Autenticazione       | password normale      |
+----------------------+-----------------------+

.. trovare un link di help migliore

Per maggiori informazioni vedi https://support.office.com/it-it/article/Impostazioni-POP-e-IMAP-per-Outlook-in-Office-365-per-le-aziende-7fc677eb-2491-4cbc-8153-8e7113525f6c.


Maggiori informazioni
---------------------

- https://support.office.com
