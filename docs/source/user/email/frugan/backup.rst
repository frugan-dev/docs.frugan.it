.. _user-email-frugan-backup-ref1:

Backup locale della posta IMAP
==============================

Quando si utilizza il protocollo IMAP, i messaggi rimangono sul server e lo stato (letto/non letto, cartelle, etichette) viene gestito centralmente. Questa modalità è molto comoda per consultare la posta da più dispositivi, ma **non costituisce un backup**: in caso di cancellazioni accidentali, esaurimento dello spazio della casella o problemi al server, i messaggi possono andare persi.

Per questo motivo è consigliato configurare il proprio client di posta in modo da mantenere una **copia locale** dei messaggi ricevuti e inviati, indipendente dal server.

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
.. note:: La configurazione descritta in questa pagina rappresenta un'alternativa più pulita all'uso combinato di IMAP e POP3 sullo stesso account, che è generalmente sconsigliato perché i due protocolli hanno modelli di gestione diversi e possono generare incoerenze sullo stato dei messaggi (ad es. messaggi non letti che appaiono come letti dopo lo scarico via POP3).


Mozilla Thunderbird *(consigliato)*
-----------------------------------

In Thunderbird esistono due approcci complementari per mantenere una copia locale dei messaggi: la sincronizzazione offline e i filtri di backup nelle Cartelle locali.


Sincronizzazione offline
~~~~~~~~~~~~~~~~~~~~~~~~

L'opzione più semplice è abilitare la sincronizzazione offline, che mantiene una copia in cache di tutti i messaggi del server.

#. Selezionare l'account IMAP
#. Andare in **Impostazioni account** → **Sincronizzazione e spazio su disco**
#. Spuntare **Mantieni i messaggi per questo account su questo computer**

.. note:: Questa modalità **non protegge dalle cancellazioni**: se un messaggio viene rimosso dal server, alla successiva sincronizzazione viene rimosso anche dalla cache locale. È quindi un backup parziale, utile per la consultazione offline ma non sufficiente come archivio storico indipendente.


Filtri di backup nelle Cartelle locali
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Per un backup vero e proprio, indipendente dal server, è possibile configurare due filtri che copiano automaticamente ogni messaggio ricevuto e ogni messaggio inviato all'interno delle **Cartelle locali** di Thunderbird.


Struttura delle cartelle
^^^^^^^^^^^^^^^^^^^^^^^^

Prima di creare i filtri, è utile predisporre la struttura delle cartelle locali, ad es.::

   Cartelle locali
   └── Backup
       └── info@domain.tld
           ├── Ricevuta
           └── Inviata

dove `info@domain.tld` corrisponde all'indirizzo email ospitato presso `Frugan <https://frugan.it>`_.

Le cartelle si creano tramite tasto destro su **Cartelle locali** → **Nuova sottocartella**.

.. tip:: Suddividere il backup per anno (ad es. ``Ricevuta/2026``, ``Ricevuta/2027``, ecc.) è una buona pratica per mantenere i file mbox di Thunderbird di dimensioni gestibili ed evitare il rischio di corruzione su file di grandi dimensioni. Vedi `Suddivisione per anno`_.


Filtro per la posta ricevuta
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

#. Aprire **Strumenti** → **Filtri messaggi**
#. Selezionare l'account IMAP nel menu a tendina **Filtri per**
#. Cliccare su **Nuovo...**
#. Configurare il filtro come segue:

   - **Nome del filtro:** ``Backup posta ricevuta``
   - **Applica filtro quando:**

     - ✔ Durante il controllo della posta
     - ✔ Manualmente

   - **Applica il filtro se:** ``Tutte incondizionatamente``
   - **Esegui le seguenti azioni:** ``Copia il messaggio in`` → ``Cartelle locali / Backup / info@domain.tld / Ricevuta``

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
.. attention:: La voce ``Tutte incondizionatamente`` va selezionata dal menu a tendina in alto. Non lasciare una riga di condizione vuota (ad es. ``Oggetto contiene <vuoto>``), perché Thunderbird la interpreta come "oggetto contiene una stringa vuota" e il filtro può non attivarsi correttamente.


Filtro per la posta inviata
^^^^^^^^^^^^^^^^^^^^^^^^^^^

I messaggi inviati non transitano dalla casella di posta in arrivo, quindi il filtro precedente non li intercetta. È necessario creare un secondo filtro che si attiva sull'evento di invio:

#. Sempre nell'account IMAP, in **Strumenti** → **Filtri messaggi**, cliccare su **Nuovo...**
#. Configurare il filtro come segue:

   - **Nome del filtro:** ``Backup posta inviata``
   - **Applica filtro quando:**

     - ✔ Dopo l'invio
     - ✔ Manualmente

   - **Applica il filtro se:** ``Tutte incondizionatamente``
   - **Esegui le seguenti azioni:** ``Copia il messaggio in`` → ``Cartelle locali / Backup / info@domain.tld / Inviata``


Verifica del funzionamento
^^^^^^^^^^^^^^^^^^^^^^^^^^

Per verificare che i filtri funzionino correttamente:

#. Inviarsi una mail di prova
#. Controllare che:

   - il messaggio compaia normalmente nella **Posta in arrivo** del server IMAP
   - una copia compaia in ``Cartelle locali / Backup / info@domain.tld / Ricevuta``
   - una copia del messaggio inviato compaia in ``Cartelle locali / Backup / info@domain.tld / Inviata``

Se entrambe le copie sono presenti, la configurazione è corretta.


Backup retroattivo della posta esistente
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

I filtri appena creati operano solo sui nuovi messaggi. Per copiare nelle Cartelle locali anche la posta già presente sul server è possibile eseguire i filtri manualmente:

#. Selezionare la cartella di origine (ad es. **Posta in arrivo**)
#. **Strumenti** → **Esegui filtri sulla cartella**

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
.. caution:: Se la casella contiene molti GB di posta, l'esecuzione retroattiva del filtro può richiedere molto tempo e in alcuni casi bloccare temporaneamente Thunderbird. Per archivi grandi è preferibile procedere a blocchi (ad es. per anno o per cartella), oppure selezionare manualmente i messaggi e usare **Copia in...** → **Cartelle locali / ...**.


Suddivisione per anno
^^^^^^^^^^^^^^^^^^^^^

Thunderbird non supporta la creazione dinamica di cartelle in base alla data del messaggio: la cartella di destinazione di un filtro deve essere già esistente. Per organizzare il backup per anno ci sono due strategie possibili.

**Strategia 1 - un filtro per ogni anno**

Si creano filtri separati per ciascun anno, con condizioni sulla data:

- ``Data`` → ``è dopo`` → ``31/12/2025``
- ``Data`` → ``è prima`` → ``01/01/2027``

con destinazione ``Backup / info@domain.tld / Ricevuta / 2026``.

L'ordine dei filtri va dal più recente al più vecchio, eventualmente seguito da un filtro "fallback" senza condizioni di data per evitare che eventuali messaggi non rientranti negli intervalli rimangano senza backup.

**Strategia 2 - cambio manuale annuale** *(consigliata)*

Si mantiene un solo filtro per la posta ricevuta e uno per la posta inviata. Una volta all'anno (ad es. a gennaio) si crea la cartella del nuovo anno e si modifica la destinazione dei filtri.

Questa strategia richiede una piccola manutenzione annuale ma è molto più semplice da gestire e meno soggetta a errori di configurazione.


Posizione del backup su disco
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Le Cartelle locali di Thunderbird sono salvate nel profilo utente, in file in formato `mbox <https://it.wikipedia.org/wiki/Mbox>`_ (un file per cartella, senza estensione). Il percorso del profilo varia in base al sistema operativo:

- **Windows:** ``%APPDATA%\Thunderbird\Profiles\<profilo>\Mail\Local Folders\``
- **macOS:** ``~/Library/Thunderbird/Profiles/<profilo>/Mail/Local Folders/``
- **Linux:** ``~/.thunderbird/<profilo>/Mail/Local Folders/``

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
.. important:: È fortemente consigliato includere questi file in un backup periodico del sistema (ad es. su disco esterno o storage cloud), perché in caso di guasto del PC o corruzione del profilo Thunderbird i messaggi archiviati localmente **non sono recuperabili dal server**.


Altri client
------------

La configurazione di filtri di backup analoghi è possibile anche su altri client di posta (Microsoft Outlook, Apple Mail, ecc.), ma la procedura varia significativamente da un'applicazione all'altra. Per assistenza su client diversi da Thunderbird è possibile contattarci ai `seguenti recapiti <https://frugan.it>`_.
