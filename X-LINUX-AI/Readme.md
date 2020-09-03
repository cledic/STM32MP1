# *Installazione de "X-LINUX-AI OpenSTLinux Expansion Package"*

Il link da seguire per l'installazione di questo package è il seguente: [X-LINUX-AI](https://wiki.st.com/stm32mpu/wiki/X-LINUX-AI_OpenSTLinux_Expansion_Package#Configure_the_AI_OpenSTLinux_package_repository)

La descrizione del package la si può trovare [qui](https://www.st.com/en/embedded-software/x-linux-ai.html?ecmp=tt17172_gl_enews_aug2020&cid=stmDM32396&bid=333380117&uid=uuVB07gLbgb9q2s894UsErJne1j82j1X5MLBcHlJc00=)

# *Aggiornare l'immagine della Board*
La prima cosa da fare è seguire [questo link](https://wiki.st.com/stm32mpu/wiki/Getting_started/STM32MP1_boards/STM32MP157x-DK2/Let%27s_start/Populate_the_target_and_boot_the_image) per scaricare ed installare l'ultima immagine disponibile; quella che ho scaricato è la seguente: "en.FLASH-stm32mp1-openstlinux-5-4-dunfell-mp1-20-06-24.tar.xz"

La scrittura dell'immagine sulla SDCard avviene tramite il programma [STM32CubeProgrammer](https://www.st.com/en/development-tools/stm32cubeprog.html). Quello che ho utilizzato io è la versione 2.4.0

In pratica la board viene riavviata in modalità **DFU** (switch *BOOT0* e *BOOT2* su **OFF**) e poi fatta collegare al **STM32CubeProgrammer** che provvederà alla scrittura dell'immagine scaricata. Io ho eseguito l'installazione usando un PC con windows8 e non ho avuto problemi. 

La board dovrà essere collegata con un cavo "USB Type A to Type C" per l'alimentazione, ed un cavo "USB Type A to Type C" per il download dell'immagine.

La **console** seriale è disponibile tramite il connettore USB "USB ST-Link".

Una volta terminata l'installazione dell'immagine e ripristinati i due siwtch su **ON**, si deve riavviare e collegare la board ad Internet, e seguire le istruzioni di [X-LINUX-AI](https://wiki.st.com/stm32mpu/wiki/X-LINUX-AI_OpenSTLinux_Expansion_Package#Configure_the_AI_OpenSTLinux_package_repository) per installare il package.

Una volta installato il package e riavviata la board, il "weston menu" si sarà ampliato delle App di AI.

Per il collegamento con il **WiFi** ho seguito [queste indicazioni](https://wiki.somlabs.com/index.php/Connecting_to_WiFi_network_on_VisionSOM-STM32MP1)

A questo [link](https://wiki.st.com/stm32mpu/wiki/X-LINUX-AI_application_samples_zoo) si possono trovare i script del pacchetto.
