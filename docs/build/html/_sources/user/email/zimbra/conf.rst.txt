Configurazione dei client di posta
==================================

I parametri necessari per l'autenticazione ai server di posta Zimbra gestiti da `Frugan <https://frugan.it>`_ tramite i comuni client di posta elettronica (ad es. Outlook, Thunderbird, ecc.) sono uguali per tutte le caselle Zimbra ospitate presso `Frugan <https://frugan.it>`_:

+-----------------------------------------+
| Posta in arrivo - POP3                  |
+======================+==================+
| Server               | pop.frugan.it    |
+----------------------+------------------+
| Porte                | 995              |
+----------------------+------------------+
| Connessione protetta | SSL/TLS          |
+----------------------+------------------+
| Autenticazione       | password normale |
+----------------------+------------------+

+-----------------------------------------+
| Posta in arrivo - IMAP                  |
+======================+==================+
| Server               | imap.frugan.it   |
+----------------------+------------------+
| Porte                | 993              |
+----------------------+------------------+
| Connessione protetta | SSL/TLS          |
+----------------------+------------------+
| Autenticazione       | password normale |
+----------------------+------------------+

+-----------------------------------------+
| Posta in uscita - SMTP                  |
+======================+==================+
| Server               | smtp.frugan.it   |
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
.. note:: A prescindere dal dominio utilizzato, l'autenticazione ai server di posta Zimbra gestiti da `Frugan <https://frugan.it>`_ avviene sempre tramite hostname del tipo `*.frugan.it`.


Le istruzioni dettagliate per la configurazione sui principali dispositivi sono disponibili qui :ref:`user-email-frugan-conf-ref1`.


Maggiori informazioni
---------------------

- https://wiki.zimbra.com/wiki/Accessing_Zimbra_Collaboration_Server_with_Thunderbird
- https://wiki.zimbra.com/wiki/Download_the_Zimbra_Connector_for_Outlook_(ZCO)