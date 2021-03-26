Configurazione dei client di posta
==================================

I parametri necessari per l'autenticazione ai server di posta certificata `EWake <https://ewake.it>`_ tramite i comuni client di posta elettronica (ad es. Outlook, Thunderbird, ecc.) sono uguali per tutte le caselle PEC ospitate presso `EWake <https://ewake.it>`_:

+-----------------------------------------+
| Posta in arrivo - IMAP                  |
+======================+==================+
| Server               | mail.twtcert.it  |
+----------------------+------------------+
| Porta                | 993              |
+----------------------+------------------+
| Connessione protetta | SSL/TLS          |
+----------------------+------------------+
| Autenticazione       | password normale |
+----------------------+------------------+

+-----------------------------------------+
| Posta in arrivo - POP3                  |
+======================+==================+
| Server               | mail.twtcert.it  |
+----------------------+------------------+
| Porta                | 995              |
+----------------------+------------------+
| Connessione protetta | SSL/TLS          |
+----------------------+------------------+
| Autenticazione       | password normale |
+----------------------+------------------+

+-----------------------------------------+
| Posta in uscita - SMTP                  |
+======================+==================+
| Server               | smtp.twtcert.it  |
+----------------------+------------------+
| Porte                | 465              |
+----------------------+------------------+
| Connessione protetta | SSL/TLS          |
+----------------------+------------------+
| Autenticazione       | password normale |
+----------------------+------------------+

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
.. note:: A prescindere dal dominio utilizzato, l'autenticazione ai server di posta certificata `EWake <https://ewake.it>`_ avviene sempre tramite hostname del tipo `*.twtcert.it`.


.. _user-email-pec-conf-ref1:

Certificato Agenzia per l'Italia digitale (ex DigitPA)
------------------------------------------------------

Tutti i gestori di PEC firmano i messaggi, le ricevute e gli avvisi con un certificato digitale rilasciato da `Agenzia per l'Italia digitale <http://www.agid.gov.it>`_ (ex DigitPA).

Per fare in modo che il vostro client di posta (Outlook, Thunderbird, Eudora, Apple Mail, ecc.) riconosca la validità di questo certificato è necessario installarlo o importarlo scaricandolo dal seguente link https://public.ewake.it.

Per installare il certificato cliccare semplicemente su **Installa certificato** (**Install certificate**) dopo aver cliccato sul file del certificato.
