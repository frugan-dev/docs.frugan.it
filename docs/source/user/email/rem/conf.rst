Configurazione dei client di posta
==================================

I parametri necessari per l'autenticazione ai server di posta certificata `Frugan <https://frugan.it>`_ tramite i comuni client di posta elettronica (ad es. Outlook, Thunderbird, ecc.) sono uguali per tutte le caselle PEC ospitate presso `Frugan <https://frugan.it>`_:

+-------------------------------------------+
| Posta in arrivo - POP3                    |
+======================+====================+
| Server               | pop3s.pec.aruba.it |
+----------------------+--------------------+
| Porta                | 995                |
+----------------------+--------------------+
| Connessione protetta | SSL/TLS            |
+----------------------+--------------------+
| Autenticazione       | password normale   |
+----------------------+--------------------+

+-------------------------------------------+
| Posta in arrivo - IMAP                    |
+======================+====================+
| Server               | imaps.pec.aruba.it |
+----------------------+--------------------+
| Porta                | 993                |
+----------------------+--------------------+
| Connessione protetta | SSL/TLS            |
+----------------------+--------------------+
| Autenticazione       | password normale   |
+----------------------+--------------------+

+-------------------------------------------+
| Posta in uscita - SMTP                    |
+======================+====================+
| Server               | smtps.pec.aruba.it |
+----------------------+--------------------+
| Porte                | 465                |
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
.. note:: A prescindere dal dominio utilizzato, l'autenticazione ai server di posta certificata `Frugan <https://frugan.it>`_ avviene sempre tramite hostname del tipo `*.pec.aruba.it`.

.. .. _user-email-rem-conf-ref1:
.. 
.. Certificato Agenzia per l'Italia digitale (ex DigitPA)
.. ------------------------------------------------------
.. 
.. Tutti i gestori di PEC firmano i messaggi, le ricevute e gli avvisi con un certificato digitale rilasciato da `Agenzia per l'Italia digitale <http://.. www.agid.gov.it>`_ (ex DigitPA).
.. 
.. Per fare in modo che il vostro client di posta (Outlook, Thunderbird, Eudora, Apple Mail, ecc.) riconosca la validità di questo certificato è .. necessario installarlo o importarlo scaricandolo dal seguente link https://public.frugan.it.
.. 
.. Per installare il certificato cliccare semplicemente su **Installa certificato** (**Install certificate**) dopo aver cliccato sul file del certificato.
