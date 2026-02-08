Suggerimenti
============

Gestione dello SPAM
-------------------

La lotta allo SPAM può avere successo solo se si opera su più fronti: lato server e lato utente.

Sui server di posta avvengono dei processi automatici, generalmente notturni, che:

- classificano come indesiderate tutte le email presenti nelle cartelle SPAM degli utenti
- classificano come desiderate tutte le email presenti nelle cartelle ARCHIVIO degli utenti
- cancellano le email più vecchie di 90 giorni presenti nelle cartelle SPAM degli utenti

Lato utente è quindi di fondamentale importanza:

- non cancellare o spostare nel cestino le email indesiderate, ma spostarle nella cartella SPAM, altrimenti il filtro antispam non impara a classificare la posta indesiderata
- utilizzare la funzione “Archivio” presente sia nelle più comuni webmail che nei client di posta (Outlook, Thunderbird, etc.) per tutte le email desiderate, in modo da evitare i falsi positivi del filtro antispam
- non archiviare mai le email indesiderate, altrimenti il filtro antispam classifica come *desiderata* anche la posta che dovrebbe essere *indesiderata*


Recupero e invio della posta esterna tramite Gmail
--------------------------------------------------

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
.. attention:: Gmail ha **dismesso il recupero della posta di terze parti tramite POP3**, leggi qui https://support.google.com/mail/answer/16604719.

Gmail permette l'aggiunta di ulteriori account di posta esterni a Gmail (*fetchmailing*) sia in arrivo che in uscita. 

È possibile quindi utilizzare Gmail per collegarsi ai server di posta `Frugan <https://frugan.it>`_, andando nelle impostazioni di Gmail:

.. image:: /assets/img/email/frugan/tips/gmail_account.png

e impostando gli stessi parametri riportati in :ref:`user-email-frugan-conf-ref1`, sia per la posta in arrivo:

.. image:: /assets/img/email/frugan/tips/gmail_incoming_1.png

.. image:: /assets/img/email/frugan/tips/gmail_incoming_2.png

che per la posta in uscita:

.. image:: /assets/img/email/frugan/tips/gmail_outgoing_1.png

.. image:: /assets/img/email/frugan/tips/gmail_outgoing_2.png


.. Errore *Connection refused* su Gmail 
.. --------------------------------------------------
.. 
.. Se si utilizza Gmail per collegarsi ai server di posta `Frugan <https://frugan.it>`_, è possibile riscontrare l'errore ``Connection refused`` con il .. parametro `pop.frugan.it` in abbinamento alla connessione SSL sulla porta 995.
.. 
.. Il problema su Gmail si presenta analogamente anche con la configurazione della posta in uscita per gli stessi account esterni. 
.. 
.. Come indicato `qui <https://productforums.google.com/forum/#!topic/gmail-it/HYLhxAMltXY/discussion>`_, l'errore sembra dipendere da problemi di .. risoluzione dei DNS da parte di Google.
.. 
.. .. image:: /assets/img/email/frugan/tips/gmail_incoming_fix.png
.. 
.. .. image:: /assets/img/email/frugan/tips/gmail_outgoing_fix.png
.. 
.. Temporanemente è possibile risolvere il problema utilizzando i seguenti parametri alternativi:
.. 
.. +-----------------------------------------+
.. | Posta in arrivo - POP3                  |
.. +======================+==================+
.. | Server               | mail.domain.tld  |
.. +----------------------+------------------+
.. | Porte                | 110              |
.. +----------------------+------------------+
.. | Connessione protetta | no               |
.. +----------------------+------------------+
.. | Autenticazione       | password normale |
.. +----------------------+------------------+
.. 
.. +-----------------------------------------+
.. | Posta in uscita - SMTP                  |
.. +======================+==================+
.. | Server               | mail.domain.tld  |
.. +----------------------+------------------+
.. | Porte                | 587              |
.. +----------------------+------------------+
.. | Connessione protetta | TLS              |
.. +----------------------+------------------+
.. | Autenticazione       | password normale |
.. +----------------------+------------------+
.. 
.. dove `domain.tld` corrisponde al dominio ospitato presso `Frugan <https://frugan.it>`_.
