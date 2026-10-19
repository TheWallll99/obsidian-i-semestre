## DERIVATE
La derivata misura quanto velocemente cambia una funzione in un punto. Geometricamente è la retta tangente al grafico in un punto $x_{0}$.

DEFINIZIONE
Prendendo due punti sul grafico: $x_{0}$ e $x_{0}+h$ (h è l'incremento), La pendenza della retta secante che li congiunge è il **rapporto incrementale**:
$$
\frac{f(x_{0}+h)-f(x_{0})}{h} 
$$
facendo tendere h a 0, la retta diventa tangente:
$$
\lim_{ h \to 0 } \frac{f(x_{0}+h)-f(x_{0})}{h} 
$$
Se questo limite è definito allora la funzione $f$ è derivabile in $x_{0}$ Se f è derivabile in $x_{0}$ allora è continua in $x_{0}$, NON il contrario. 
I punti in cui una funzione non è derivabile sono tre:
	Punti Angolosi: derivata destra e sinistra sono diverse.
	Cuspidi: Le pendenze tendono da una parte a $+\infty$ e dall'altra a $-\infty$
	Flesso a Tangente Verticale: La derivata tende a $\pm \infty$ 
DERIVATE IMMEDIATE:
	$c \rightarrow 0$
	$x^n \rightarrow nx^{n-1}$
	$e^x \rightarrow e^x$
	$a^x \rightarrow a^x\cdot \ln a$ 
	$\ln x\rightarrow \frac{1}{x}$
	$\sin x \rightarrow \cos x$
	$\cos x \rightarrow -\sin x$
	$\tan x \rightarrow \frac{1}{\cos^2x}$
	$\arctan x \rightarrow \frac{1}{1+x^2}$
	$\arcsin x \rightarrow \frac{1}{\sqrt{1-x^2}}$
REGOLE DI CALCOLO:
	Somma: $(f+g)' =f'+g'$
	Prodotto: $(fg)'=f'g+fg'$
	Quoziente: $(f/g)'= \frac{f'g-fg'}{g^2}$
	Funzioni composte: $(f(g(x)))'=f'(g(x))\cdot g'(x)$
TEOREMI:
	Fermat: Se $x_{0}$ è un punto di massimo o minimo relativo, e la funzione è derivabile in $x_{0}$, allora $f'(x_{0})=0$
	Rolle: Se f è continua e derivabile in $[a,b]$ e $f(a)=f(b)$, esiste almeno un punto c tale che $f'(c)=0$
	Lagrange: