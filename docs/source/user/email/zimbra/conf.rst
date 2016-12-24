Configurazione dei client di posta
==================================

I parametri necessari per l'autenticazione ai server di posta Zimbra gestiti da `EWake <https://ewake.it>`_ tramite i comuni client di posta elettronica (ad es. Outlook, Thunderbird, ecc.) sono uguali per tutte le caselle Zimbra ospitate presso `EWake <https://ewake.it>`_:

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
.. note:: A prescindere dal dominio utilizzato, l'autenticazione ai server di posta Zimbra gestiti da `EWake <https://ewake.it>`_ avviene sempre tramite hostname del tipo `*.ewake.it`.


Istruzioni sui principali dispositivi
-------------------------------------

Le istruzioni dettagliate per la configurazione sui principali dispositivi sono uguali a quelle delle email ordinarie `EWake <https://ewake.it>`_ disponibili qui :ref:`user-email-ewake-conf-ref1`.


Maggiori informazioni
---------------------

- https://wiki.zimbra.com/wiki/Accessing_Zimbra_Collaboration_Server_with_Thunderbird
- https://wiki.zimbra.com/wiki/Download_the_Zimbra_Connector_for_Outlook_(ZCO)