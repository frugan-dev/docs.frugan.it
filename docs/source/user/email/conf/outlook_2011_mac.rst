Microsoft Outlook 2011 per Mac
==============================
	
	
Passaggio 1: verifica di avere l’ultima versione
------------------------------------------------

| Verifica di avere l’ultima versione di **Outlook for Mac 2011**.
| Dopo aver aperto Outlook, fai clic su  **Help** nel menu principale e quindi su **Check for Updates**.
| L’applicazione ti informa se ci sono aggiornamenti disponibili. Segui le istruzioni per passare alla pagina di installazione aggiornamenti.
| Per ulteriore assistenza riguardo all’aggiornamento del software Microsoft, consulta il supporto in linea di Microsoft a questo indirizzo: <http://support.microsoft.com>

.. image:: /assets/img/email/outlook_2011_mac/check_for_updates.png
	
Passaggio 2: Aggiungi il tuo account di posta elettronica
---------------------------------------------------------

Fai clic su **Tools** nel menu principale e quindi su **Accounts**.

.. image:: /assets/img/email/outlook_2011_mac/add_account.png
	
Fai clic sul pulsante **più (+)**situato nell’angolo sinistro e quindi su **E-mail...** nel menu a discesa che compare.

.. image:: /assets/img/email/outlook_2011_mac/click_on_plus_button.png
	
Passaggio 3: Immetti le tue informazioni account
------------------------------------------------

Immetti l’indirizzo di posta elettronica (che desideri impostare) nel campo **E-mail address** e la relativa password nel campo **Password**. Quando inizi a digitare la password, il resto della finestra di espande visualizzando altre opzioni.

.. image:: /assets/img/email/outlook_2011_mac/enter_account_information.png
	
Nella finestra espansa, immetti le seguenti informazioni relative al tuo account:

- **E-mail address:** immetti l’indirizzo da aggiungere - in questo esempio `name@example.com`
- **Password:** è quella che usi per accedere al Webmail relativo a questo account.
- **User name:** `name@example.com`
- **Type:** IMAP
- **Incoming Server:** imap.ewake.it
- Seleziona la casella: **Use SSL to connect (recommended)**
- **Incoming server port:** 993
- **Outgoing server:** smtp.ewake.it
- Seleziona la casella: **Override default port**
- Seleziona casella: **Use SSL to connect (recommended)**
- Digita **465** nel campo porta situato a destra del campo **Outgoing server**.

Dopo aver immesso tutte le informazioni, fai clic su **Add Account**.

.. image:: /assets/img/email/outlook_2011_mac/click_on_add_account.png
	
Passaggio 4: Immetti un nome e una descrizione
----------------------------------------------

| Immetti nel campo **Account description** un nome che descrive il tuo account.
| Quindi immetti nel campo **Full name** un nome che sarà visualizzato come mittente.
| Verifica che le informazioni personali e le informazioni sul server relative al tuo account siano giuste; quindi fai clic sul pulsante **More Options...** situato nella parte inferiore della finestra di dialogo.

.. image:: /assets/img/email/outlook_2011_mac/click_on_more_options.png
	
Passaggio 5: Seleziona il metodo di autenticazione
--------------------------------------------------

| A questo punto ti viene chiesto di selezionare un metodo di autenticazione.
| Nel campo **Authentication**, seleziona **User name and Password** nel menu a discesa.

.. image:: /assets/img/email/outlook_2011_mac/select_authentication_method.png
	
| Nel campo **User Name**, digita lo stesso indirizzo di posta elettronica che hai già immesso in precedenza; nel campo **Password**, digita la relativa password. Lascia in bianco il campo **Unqualified domain**.
| Fai clic su **OK**.

.. image:: /assets/img/email/outlook_2011_mac/enter_user_name_and_password.png

| Impostazione dell’account di posta elettronica in Outlook 2011 per Mac completata. I dati del tuo account vengono caricati nell’applicazione.
| I passaggi seguenti spiegano come sia possibile eseguire la sincronizzazione delle cartelle IMAP.
	
Passaggio 6: Sincronizzazione delle cartelle IMAP
-------------------------------------------------

| **IMAP** consente a più clienti di accedere alla stessa cassetta postale e mantiene disponibili sul server i messaggi accessibili via Webmail o tramite altri dispositivi.
| Per gestire le cartelle IMAP ti consigliamo di utilizzare queste impostazioni sin dall’inizio.
| Verifica di avere installata l’ultima versione di **Microsoft Outlook 2011 for Mac**. Per ulteriori informazioni su come aggiornare il software, leggi il <a href="#step1">primo passo di questa guida</a>.
| Fai clic su **Tools** nel menu principale e quindi su **Accounts...**.

.. image:: /assets/img/email/outlook_2011_mac/add_account.png
		
Fai clic sul pulsante **Advanced** situato nell’angolo in basso a destra della finestra di dialogo.

.. image:: /assets/img/email/outlook_2011_mac/click_on_advanced.png
	
| Fai clic sulla scheda **Server**.
| Digita la parola **INBOX** - scritta in maiuscolo - nel campo **IMAP Root Folder**.

.. image:: /assets/img/email/outlook_2011_mac/click_on_server.png
	
Fai clic sulla scheda **Folders**.

.. image:: /assets/img/email/outlook_2011_mac/click_on_folders.png
	
Per conservare i messaggi nella cartella appropriata, procedi come segue:

- Nel riquadro **Sent**, imposta **Store sent messages in this folder:** su **Sent (Server)** nel menu a discesa.
- Nel riquadro **Drafts**, imposta **Store draft messages in this folder:** su **Drafts (Server)** nel menu a discesa.
- Nel riquadro **Junk**, imposta **Store junk messages in this folder:** su **Junk E-mail (Server)** nel menu a discesa.
- Nel riquadro **Move**, seleziona **Move deleted messages to this folder:** e quindi **Trash (Server)** nel menu a discesa.

Fai clic su **OK**.
	
Altri suggerimenti
------------------

Come eliminare un account
~~~~~~~~~~~~~~~~~~~~~~~~~

| Per eliminare un account, fai clic su **Tools** nel menu principale e quindi su **Accounts**.
| Seleziona l’account da eliminare facendo clic sul corrispettivo nome nella panoramica.
| Fai clic sul pulsante **meno (-)** nell’angolo in basso a sinistra e quindi sul pulsante **Delete** per la conferma.

.. image:: /assets/img/email/outlook_2011_mac/delete_account.png
	
Risoluzione dei problemi
------------------------

Che cosa fare se Outlook non riesce a stabilire una connessione protetta
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Se cerchi di scrivere un messaggio di posta elettronica e ricevi il messaggio di errore **A secure connection cannot be established with the server imap.example.com**, fai clic su **Cancel**.

.. image:: /assets/img/email/outlook_2011_mac/secure_connection_cannot_be_established.png
	
| Per risolvere questo problema, fai clic su **Tools** nel menu principale e quindi su **Accounts**.
| Nella finestra che compare, seleziona il tuo account  e verifica che nel campo **Incoming server** sia indicato **imap.ewake.it** (e non imap.example.com).

.. image:: /assets/img/email/outlook_2011_mac/check_that_correct_imap_server_is_used.png
	
Come visualizzare il registro errori
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

| Se non riesci a configurare il tuo account, invia un’acquisizione schermo delle tue impostazioni ed eventuali messaggi di errore al nostro servizio di assistenza clienti che ti aiuterà a trovare una soluzione.
| Inoltre puoi verificare il registro errori dell’applicazione, facendo clic su **Window** nel menu principale e quindi su **Error Log**.
| Compare una panoramica degli errori registrati dall’applicazione. Le informazioni del registro possono essere utili quando ci contatti in caso di eventuali problemi.

.. image:: /assets/img/email/outlook_2011_mac/check_the_error_log.png
