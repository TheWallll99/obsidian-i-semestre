## Numeri razionali in codifica BCD
Può essere utile ad esempio per la rappresentazione dei prezzi, che hanno sempre una parte razionale di 2 cifre.
Semplicemente si utilizzano 8 bit per rappresentare le due cifre con la classica codifica BCD.
Ad esempio: 69,69 euro sono 0110 1001, 0110 1001 euro
## Codifica in virgola mobile (floating point)
Per rappresentare un numero a virgola non fissa posso utilizzare ad esempio la notazione scientifica:
$152,73 = 1,5273\cdot 10^2$ come $101,0111=1,010111\cdot 2^2$. Così facendo abbiamo scritto il numero in **forma normale**, ovvero il numero con la virgola subito dopo la prima cifra. L'1 è implicito, quindi ci basta conservare la parte decimale e l'esponente. Quindi: 1 bit per il segno, $n_{m}$ bit per la **mantissa** (la parte decimale) e $n_{e}$ bit per l'esponente. Dobbiamo però accordare una certa codifica per questi valori, perchè ci occorre un numero finito di bit: la **mantissa** si esprime in codifica naturale, e l'esponente con la codifica eccesso k ($k=2^{n_{e}-1}-1$) con n il numero di bit dell'esponente.
Es: 
	$17,42_{(10)}=10001,0110101\cdots = 1,00010110101 \cdot 2^4$
	$0 (\text{per il segno}), e=4+7=11_{ecc}=1011_{2} \text{(esponente)},00010110(\text{mantissa})$
	$17,42_{10}=0101100010111_{2}$ 
Per la conversione al contrario si fa così:
	0101100010111
	0 = segno = +
	1011 = esponente (eccesso k, se bit sono 4 allora k = 7) = 11-7 = 4
	quindi il numero sarà $1,00010111\cdot 2^4$, ovvero 10001,0111, e quindi $\approx$ 17,42. 
Se l'esponente è uguale a 0 periodico allora è un numero denormalizzato.
Se l'esponente é uguale a 1 periodico e la mantissa uguale a 0 periodico allora è infinito.
Se l'esponente è uguale a 1 periodico e la mantissa diversa da 0 periodico allora é NaN.