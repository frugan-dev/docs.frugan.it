G Suite
=======

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
.. hint:: Si consiglia fortemente l'utilizzo, tramite l'app `Google Authenticator <https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2&hl=it>`_, del sistema di `autenticazione a due fattori <https://support.google.com/accounts/answer/185839?hl=it>`_ (Two-Factor authentication) attivabile nelle impostazioni dell'account Google.
	


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


Suggerimenti
------------

Password per le app
~~~~~~~~~~~~~~~~~~~

Le password per le app consentono agli utenti che utilizzano la verifica in due passaggi di accedere ai loro account GSuite attraverso il proprio client email (Outlook, Thunderbird, Mail, etc.). 

Per maggiori informazioni vedi https://security.google.com/settings/security/apppasswords. 


App meno sicure
~~~~~~~~~~~~~~~

Alcuni dispositivi e app utilizzano una tecnologia di accesso meno sicura, che rende più vulnerabile il tuo account. Puoi disattivare l'accesso per queste app (soluzione consigliata) oppure attivare l'accesso se desideri utilizzarli nonostante i rischi. 

Per maggiori informazioni vedi https://www.google.com/settings/security/lesssecureapps.


Condivisione account POP3
~~~~~~~~~~~~~~~~~~~~~~~~~

Se un account POP3 viene condiviso fra più utenti, si può utilizzare l'impostazione `recent:mail@domain.tld` per autenticarsi ai server di Google tramite il proprio client di posta, simulando alcune funzionalità del protocollo IMAP.


Filtro posta inviata
~~~~~~~~~~~~~~~~~~~~
 
G Suite ha un unico contenitore in cui finiscono tutti i messaggi, compresa la posta inviata che viene salvata in automatico.
Per evitare che il proprio client email (Outlook, Thunderbird, Mail, etc.) scarichi la posta inviata “credendola” posta ricevuta è possibile creare un filtro apposito andando in **Strumenti** → **Filtri**, inserendo la proprio email nel campo **Mittente** e selezionando **Posta inviata** nel campo **Sposta il messaggio in**.


Maggiori informazioni
---------------------

- https://support.google.com/mail 
- https://gsuite.google.com/intl/it/support/