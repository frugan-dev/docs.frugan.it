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

Disattivazione delle conferme di lettura
----------------------------------------

Le conferme di lettura (in inglese `Return Receipts` o `Read Receipts`) sono notifiche automatiche che il client del destinatario invia al mittente quando un messaggio viene aperto.

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
.. attention:: Le caselle ospitate presso `Frugan <https://frugan.it>`_ sono soggette a limiti sul numero di messaggi inviabili. Anche le conferme di lettura rientrano nel conteggio dei messaggi inviati, quindi si consiglia di **disattivarne l'invio automatico** sul proprio client di posta per evitare di superare inutilmente tali limiti.

La disattivazione rilevante è quella lato destinatario, cioè evitare che il proprio client di posta risponda automaticamente alle richieste di conferma presenti nei messaggi in arrivo.

Mozilla Thunderbird
~~~~~~~~~~~~~~~~~~~

Aprire **Impostazioni** e scorrere la sezione **Generale** fino a trovare le opzioni relative alle **Conferme di lettura** (in inglese *Return Receipts*).

Alla voce **Quando arriva un messaggio che richiede una conferma di lettura** selezionare **Non inviare mai una conferma di lettura**.

In alternativa è possibile configurare il comportamento per singolo account in **Impostazioni account** → **<account>** → **Conferme di lettura**, spuntando **Personalizza le conferme di lettura per questo account** e selezionando le opzioni desiderate.

Microsoft Outlook
~~~~~~~~~~~~~~~~~

Aprire **File** → **Opzioni** → **Posta** e cercare la sezione **Verifica messaggi**.

Alla voce **Per qualsiasi messaggio ricevuto che includa una richiesta di conferma di lettura** selezionare **Non inviare mai una conferma di lettura**.

Webmail
~~~~~~~

Nella webmail principale `Frugan <https://frugan.it>`_ (Roundcube), aprire **Impostazioni** → **Preferenze** → **Visualizzazione messaggi**, e alla voce **Su richiesta per la ricevuta di ritorno** selezionare **ignora la richiesta**.

Anche nelle webmail secondarie l'opzione di disattivazione delle conferme di lettura è generalmente disponibile in una sezione analoga delle preferenze utente.

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
