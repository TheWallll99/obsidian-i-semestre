Per rappresentare dei numeri che non sono potenze perfette di due, si approssima al bit successivo: $n=\log_{2}12\approx4$ 
Le informazioni che rappresentiamo con un computer sono:
- Numeri naturali (*unsigned integer*)
- Numeri interi (*integer*)
- Numeri reali (*floating point*)
- Testo (*characters*)
- Immagini 
- Suoni
- Video
## Numeri naturali: codifica naturale
Si rappresentano secondo la codifica del sistema posizionale scegliendo la base 2 come base:
	In base al numero $n$ di bit si possono rappresentare i numeri tra $0$ e $2^n -1$ (8 bit $\rightarrow$ numeri da 0 a 255)
Per ricavare il numero di bit si parte dal valore che devo rappresentare ($\log_{2}n+1$).
Se da una somma otteniamo un numero che sfora il numero di bit previsti si parla di **overflow**.
Se ho un numero fisso di bit, devo dichiararli **tutti** (101$\square\square\square$ non è accettabile)
## Numeri naturali: codifica BCD
Binary Coded Decimal: ogni cifra viene rappresentata da una sequenza di 4 bit, quindi un numero con $k$ cifre decimali viene rappresentato da $4\cdot k$ bit.
Ogni codifica è seguita da un numero che identifica il peso dei 4 bit:
- BCD8421: più a sinistra 8, poi 4, poi 2, poi 1
- BCD84-2-1: 8, 4, -2, -1
- in eccesso 3: si aggiunge tre al numero decimale che si vuole rappresentare
Esempio: 37 (in codifica BCD8421)
	Si dividono 3 e 7: 3 | 7
	Si rappresenta 3 e 7 separati: 0011 0111

## Numeri naturali: codifica di Gray
La codifica di Gray permette di far cambiare solo un bit alla volta, per ridurre il tempo di lettura del codice da parte del calcolatore:
DA BINARIO A GRAY
$1011_{B}\rightarrow????_{G}$ 
Si usa uno XOR tra le cifre: $B_{1}$ e $G_{1}$ rimane uguale, poi: $G_{2}=B_{1}\oplus B_{2}$ e così via.
Quindi: $1011_{B}=1110_{G}$
DA GRAY A BINARIO
Si fa sempre XOR ma $B_{2}=B_{1}\oplus G_{2}$ 
Quindi: $1110_{G}=1011_{B}$ 