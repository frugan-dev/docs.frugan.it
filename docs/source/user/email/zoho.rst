Zoho
====

Accesso alla webmail
--------------------

La webmail per accedere alle caselle email `G Suite di Google <https://gsuite.google.com>`_ è raggiungibile al seguente indirizzo:

- `http://mail.domain.tld` (GMail)

dove `domain.tld` corrisponde al dominio ospitato presso `EWake <https://ewake.it>`_.

Per autenticarsi è necessario digitare il proprio indirizzo email (ad es. `hello@domain.tld`) e successivamente la password.

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
.. important:: Si consiglia fortemente l'utilizzo del sistema di `autenticazione a due fattori <https://support.google.com/accounts/answer/185839?hl=it>`_ (Two-Factor authentication) tramite l'app `Google Authenticator <https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2&hl=it>`_.


Configurazione dei client di posta
----------------------------------

I parametri necessari per l'autenticazione ai server di posta `G Suite di Google <https://gsuite.google.com>`_ tramite i comuni client di posta elettronica (ad es. Outlook, Thunderbird, ecc.) sono uguali per tutte le caselle ospitate presso `EWake <https://ewake.it>`_:

+-----------------------------------------+
| Posta in arrivo - IMAP                  |
+======================+==================+
| Server               | imap.gmail.com   |
+----------------------+------------------+
| Porta                | 993              |
+----------------------+------------------+
| Connessione protetta | SSL/TLS          |
+----------------------+------------------+
| Autenticazione       | password normale |
+----------------------+------------------+

+---------------------------------------------------------------------------+
| Posta in arrivo - POP3                                                    |
+======================+====================================================+
| Server               | pop.gmail.com *(consigliato)* o pop.googlemail.com |
+----------------------+----------------------------------------------------+
| Porta                | 995                                                |
+----------------------+----------------------------------------------------+
| Connessione protetta | SSL/TLS                                            |
+----------------------+----------------------------------------------------+
| Autenticazione       | password normale                                   |
+----------------------+----------------------------------------------------+

+-----------------------------------------------------------------------------+
| Posta in uscita - SMTP                                                      |
+======================+======================================================+
| Server               | smtp.gmail.com *(consigliato)* o smtp.googlemail.com |
+----------------------+------------------------------------------------------+
| Porte                | 465 *(consigliata)* o 587                            |
+----------------------+------------------------------------------------------+
| Connessione protetta | SSL/TLS *(consigliata)* o STARTTLS                   |
+----------------------+------------------------------------------------------+
| Autenticazione       | password normale                                     |
+----------------------+------------------------------------------------------+

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
.. note:: A prescindere dal dominio utilizzato, l'autenticazione ai server di posta `G Suite di Google <https://gsuite.google.com>`_ avviene sempre tramite hostname del tipo `*.gmail.com` o `*.googlemail.com`.


Maggiori informazioni
---------------------

- https://support.google.com/mail 
- https://gsuite.google.com/intl/it/support/