Sulla circonferenza $x^2+y^2=1$, l'angolo si misura come _lunghezza dell'arco_, quindi $\cos \theta=x$ e $\sin \theta = y$ in radianti.
Proprietà immediate:
- $\sin^2x+\cos^2x=1$ 
- seno e coseno sono periodiche su $2\pi$, il seno è dispari e il coseno è pari
- $-1\le\sin,\cos\le 1$ 
- $\tan x =\frac{\sin x}{\cos x}$, definita per $x\neq \frac{\pi}{2}+k\pi$ 
FORMULE DI ADDIZIONE:
- $\sin(a\pm b)=\sin a\cos b\pm \cos a\sin b$
- $\cos(a\pm b)=\cos a\cos b\mp \sin a\sin b$ 
- $\tan(a\pm b)=\frac{\tan a\pm \tan b}{1\mp \tan a\tan b}$ 
DUPLICAZIONE E BISEZIONE:
- $\sin 2a=2\sin a\cos a$
- $\cos 2a=\cos^2a-\sin^2a=2\cos^2a-1=1-2\sin^2a$
- $\sin^2\frac{a}{2}=\frac{1-\cos a}{2}$
- $\cos^2\frac{a}{2}=\frac{1+\cos a}{2}$ 
PROSTAFERESI:
$\sin p+\sin q=2\sin\frac{p+q}{2}\cos\frac{p-q}{2}$
$\cos p+\cos q=2\cos\frac{p+q}{2}\cos\frac{p-q}{2}$ 
PARAMETRICHE(con $t=\tan \frac{x}{2}$):
$\sin x=\frac{2t}{1+t^2}$
$\cos x=\frac{1-t^2}{1+t^2}$
$dx={2dt}{1+t^2}$
Utili perchè trasformano gli integrali razionali in seno e coseno di un integrale di funzione razionale.
LIMITE NOTEVOLE
$$
\lim_{ x \to 0 }\frac{\sin x}{x}=1 
$$
Moltiplicando per $\frac{1+\cos x}{1+\cos x}$ Si ottiene
$$
\lim_{ x \to 0 }\frac{1-\cos x}{x^2}=\frac{1}{2}
$$
DERIVATE
$(\sin x)'=\cos x$
$(\cos x)'=-\sin x$
$(\tan x)'=\frac{1}{\cos^2}=1+\tan^2x$
$(\arcsin x)',(\arccos x)'=\pm\frac{1}{\sqrt{ 1-x^2 }}$

## LIMITI
$$
\forall \epsilon>0 \exists \delta>0:0<|x-x_{0}|<\theta\Rightarrow|f(x)-L|<\epsilon
$$
Il limite può non essere definito in: salti, esplosioni in segni opposti e oscillazioni infinite.
Operazioni con l'infinito:
$\infty +\infty=\infty$
$\infty \times \infty=\infty$
$\frac{n}{\infty}=0$
$\frac{n}{0}=\pm \infty$
Le forme indeterminate sono situazioni in cui si trova a quale infinito va l'operazione contando il grado dell'operazione iniziale: $\infty-\infty:x^2-x$ per $x\rightarrow \infty$ allora fa $\infty$ perchè $x^2$ cresce più in fretta.
Per risolvere una forma indeterminata, oltre che considerare la Gerarchia degli infiniti, possiamo:
1. Raccogliere il termine di grado più alto
2. Semplificare o fattorizzare
3. Razionalizzare se ci sono radici
4. Usare i limiti notevoli
La **GERARCHIA DEGLI INFINITI** dice che 
$$
\ln x\ll potenze\ x^n\ll esponenziali\ c^x\ll n!\ll n^n
$$
Inoltre possiamo ricorrere ad approssimazioni in cui sostituiamo le funzioni complicate con quelle più semplici.
Ad esempio:
$$
\lim_{ x \to 0 }\frac{\sin(3x)}{\ln(1+2x)}\sim\frac{3x}{2x}=\frac{3}{2}
$$
ma si può fare SOLO in prodotti e quozienti.
REGOLA DI TAYLOR:
$\sin x=x-\frac{x^3}{6}+\cdots$
$\cos x=1-\frac{x^2}{2}+\cdots$
$e^x=1+x+\frac{x^2}{2}+\cdots$
e si può utilizzare per risolvere forme indeterminate del tipo $\frac{0}{0}$
Sempre per risolvere questi limiti e quelli di forma $\frac{\infty}{\infty}$ si può utilizzare il TEOREMA DI DE L'HOPITAL:
$$
\text{se }\frac{f'(x)}{g'(x)}\text{esiste, allora}\lim \frac{f}{g}=\lim\frac{f'}{g'}  
$$
I limiti possono essere usati per verificare la continuità delle funzioni e per trovarne gli asintoti:
CONTINUITA':
	$\text{poniamo}\lim_{ x \to x_{0} }f(x)=f(x_{0})$; se questo non è verificato allora possiamo avere discontinuità di:
		ELIMINABILE: un buco nel grafico, il limite esiste ma il valore nel punto è diverso.
		PRIMA SPECIE: di salto, i limiti da destra e sinistra sono diversi.
		SECONDA SPECIE: almeno uno dei due limiti non esiste o è infinito
ASINTOTI:
	VERTICALE: $\lim_{ x \to x_{0} }$, se va a $\infty$ 
	ORIZZONTALE: $\lim_{ x \to \infty }$ se va a 0
	OBLIQUO: $\lim_{ x \to \infty }\frac{f(x)}{x}=m$ , $\lim_{ x \to \infty }(f(x)-mx)=q$ 

