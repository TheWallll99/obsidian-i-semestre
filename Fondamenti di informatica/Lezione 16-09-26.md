Un algoritmo è la sequenza di passi necessari alla risoluzione di un compito. Un computer è un esecutore di algoritmi. Deve essere espresso come una sequenza di istruzioni che il computer può eseguire. Un programma è un algoritmo scritto in un linguaggio comprensibile al computer. Deve essere **corretto** e **efficiente**: Svolge il compito senza errori e con uso ottimale delle risorse.

Un computer è un dispositivo composto da hardware e software. 
Ci sono due tipi di computer: 
	Embedded: fa un compito solo (calcolatrice)
	Programmabili: è autoesplicativo (computer smartphone bla bla bla)
La struttura di Von Neumann riassume tutte le componenti di un computer: 
	Periferiche I/O <-> Bus <-> CPU e Memorie
	Memoria centrale:
		Contiene i programmi da eseguire e i relativi dati.
		E' una sequenza di celle (bit) che possono essere accesi o spenti (1 o 0)
		Ogni cella ha un indirizzo a cui si rifà la CPU
	CPU:
		Estrae, decodifica ed esegue le istruzioni in memoria (le istruzioni possono comportare il trasferimento da e nella memoria centrale).
		Fatta da:
			Unità di controllo: preleva e decodifica informazioni, invia segnali
			Clock: metronomo per la CPU
			Unità aritmetico-logica: operazioni aritmetiche e logiche
			Registri: memorie rapide come cache per informazioni richieste dall'U. di controllo
	Bus:
		Insieme di connessioni che trasmette le informazioni e i segnali.
		Comprende bus dati, bus indirizzi e bus controlli

La CPU ha un proprio linguaggio chiamato Linguaggio Macchina. In linguaggio macchina le istruzioni sono rappresentate da:
	Codice operativo: 4 bit
	Indirizzo operando: 12 bit
Ogni famiglia di processori ha il suo Instruction Set predefinito.
L'algoritmo è la sequenza di operazioni base per risolvere un problema. Per programmare un computer bisogna tradurre l'algoritmo in una sequenza di istruzioni leggibile dal computer, scritta in linguaggio macchina. 
Il linguaggio Assembler (Assembly) è la versione simbolica, facile da memorizzare, del linguaggio macchina.
Assembly
	Istruzioni di trasferimento:
		READ 
		WRITE
		LOAD ***
		STORE *** ***
	Istruzioni aritmetiche:
		ADD ***
		SUB ***
		MULT ***
		DIV ***
	Istruzioni di controllo:
		JUMP label
Il linguaggio macchina presenta però degli svantaggi, ovvero la grande quantità di informazioni specifiche da ricordare per il programmatore e la difficoltà di comprensione dei programmi. Intervengono perciò i linguaggi ad alto livello (di astrazione), più vicini al linguaggio parlato ma che hanno bisogno di un compilatore e di un interprete per tradurre il linguaggio in istruzioni comprensibili dal computer.