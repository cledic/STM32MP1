# *Installazione de "X-LINUX-AI OpenSTLinux Expansion Package"*

Il link da seguire per l'installazione di questo package è il seguente: [X-LINUX-AI](https://wiki.st.com/stm32mpu/wiki/X-LINUX-AI_OpenSTLinux_Expansion_Package#Configure_the_AI_OpenSTLinux_package_repository)

Ma la prima cosa da fare è seguire [questo link](https://wiki.st.com/stm32mpu/wiki/Getting_started/STM32MP1_boards/STM32MP157x-DK2/Let%27s_start/Populate_the_target_and_boot_the_image) per scaricare ed installare l'ultima immagine disponibile; quella che ho scaricato è la seguente: "en.FLASH-stm32mp1-openstlinux-5-4-dunfell-mp1-20-06-24.tar.xz"

La scrittura dell'immagine sulla SDCard avviene tramite il programma [STM32CubeProgrammer](https://www.st.com/en/development-tools/stm32cubeprog.html). Quello che ho utilizzato io è la versione 2.4.0

In pratica, la board viene riavviata in modalità *DFU* (BOOT= e BOOT2 su *OFF*) e poi fatta collegare al CubeProgrammer che provvederà alla scrittura dell'immagine scaricata.


