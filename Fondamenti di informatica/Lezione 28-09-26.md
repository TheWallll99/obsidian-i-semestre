## Numeri razionali in binario
Per rappresentare i numeri razionali, il metodo per ogni cifra successiva alla virgola è uguale al normale, ma invece di moltiplicare per $2^n$ si moltiplica per $2^{-n}$ 
es.
	3.14 = 11.001
Per la conversione si usa il metodo delle **moltiplicazioni successive** fino a quando il risultato delle moltiplicazioni non è un numero intero. (quindi, un numero che in base 10 è finito, in base 2 può essere periodico).
Ma in un computer abbiamo un numero finito di bit $\rightarrow$ non possiamo rappresentare numeri periodici. Quindi si usa:
### Codifica a virgola fissa
Mettiamo caso di avere 5 bit disponibili prima della virgola:
$\square\square\square\square\square$ parte intera $\square\square\square$ parte decimale
E di rappresentare in questa codifica 27.3:
27=11011 0.3=010$\cdots \Rightarrow$ 27.3 = 11011.010
Per passare poi da binario a decimale possiamo convertire separatamente parte intera e frazionaria:
	11011 = 27 $\approx$ 0.25
	Ovviamente dovremmo contare un'approssimazione, e quindi calcolare un errore che può essere: ASSOLUTO ($E_{a}=|27.3-27.25|=0.05$) o RELATIVO ($E_{r}=\frac{E_{a}}{27.3}=0.18\%$) 
Per rappresentare i numeri razionali negativi basta aggiungere un 1 all'inizio come nella codifica Modulo e segno.