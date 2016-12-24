Zoho
====

Accesso alla webmail
--------------------

La webmail per accedere alle caselle email `Zoho <https://www.zoho.com>`_ è raggiungibile al seguente indirizzo:

- `http://mail.domain.tld` (Zoho mail)

dove `domain.tld` corrisponde al dominio ospitato presso `EWake <https://ewake.it>`_.

Per autenticarsi è necessario digitare il proprio indirizzo email (ad es. `hello@domain.tld`) nel campo **Email / Phone** e la password nel campo **Password**.

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
.. hint:: Si consiglia fortemente l'utilizzo, tramite l'app `Google Authenticator <https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2&hl=it>`_, del sistema di `autenticazione a due fattori <https://www.zoho.com/accounts/help/tfa-overview.html>`_ (Two-Factor authentication) attivabile nelle impostazioni dell'account Zoho.
	


Configurazione dei client di posta
----------------------------------

I parametri necessari per l'autenticazione ai server di posta `Zoho <https://www.zoho.com>`_ tramite i comuni client di posta elettronica (ad es. Outlook, Thunderbird, ecc.) sono uguali per tutte le caselle ospitate presso `EWake <https://ewake.it>`_:

+-------------------------------------------------------------------------+
| Posta in arrivo - IMAP                                                  |
+======================+==================================================+
| Server               | imappro.zoho.com *(consigliata)* o imap.zoho.com |
+----------------------+--------------------------------------------------+
| Porta                | 993                                              |
+----------------------+--------------------------------------------------+
| Connessione protetta | SSL/TLS                                          |
+----------------------+--------------------------------------------------+
| Autenticazione       | password normale                                 |
+----------------------+--------------------------------------------------+

+-----------------------------------------------------------------------+
| Posta in arrivo - POP3                                                |
+======================+================================================+
| Server               | poppro.zoho.com *(consigliata)* o pop.zoho.com |
+----------------------+------------------------------------------------+
| Porta                | 995                                            |
+----------------------+------------------------------------------------+
| Connessione protetta | SSL/TLS                                        |
+----------------------+------------------------------------------------+
| Autenticazione       | password normale                               |
+----------------------+------------------------------------------------+

+-----------------------------------------------------------+
| Posta in uscita - SMTP                                    |
+======================+====================================+
| Server               | smtp.zoho.com                      |
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
.. note:: A prescindere dal dominio utilizzato, l'autenticazione ai server di posta `Zoho <https://www.zoho.com>`_ avviene sempre tramite hostname del tipo `*.zoho.com`.


Accesso tramite Exchange ActiveSync (EAS)
-----------------------------------------

Di seguito i parametri per l'autenticazione ai server di posta `Zoho <https://www.zoho.com>`_ tramite Exchange ActiveSync (EAS):

+----------------------+------------------+
| Server               | msync.zoho.com   |
+----------------------+------------------+
| Dominio              | *lasciare vuoto* |
+----------------------+------------------+
| Connessione protetta | SSL/TLS          |
+----------------------+------------------+
| Autenticazione       | password normale |
+----------------------+------------------+

Per maggiori informazioni vedi http://zsync.zohosites.com.


Maggiori informazioni
---------------------

- https://www.zoho.com/mail/help/
