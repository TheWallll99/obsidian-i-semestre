$\pi$, e, $\sqrt2$ sono numeri decimali Aperiodici (non presentano ripetizioni all'infinito), diversi da i classici numeri periodici come 3,333.....
## Numeri complessi
il numero z, è definito 
$$
z=(x,y) \in R^2
$$
quindi come una coppia di coordinate. 
Nell'insieme R abbiamo (R, +, x, <), nell'insieme $R^2$ abbiamo ($R^2, +, \cdot$) 
	 ADDIZIONI: 
	 $z_{1}+ z_{2} =(x_{1}+x_{2}, y_{1}+y_{2})$ 
	 MOLTIPLICAZIONI:
	 $z_{1} \cdot z_{2}=(x_{1}x_{2}-y_{1}y_{2}, x_{1}y_{2}-x_{2}y_{1})$ 
$(R^2,+,\cdot)$ è un **campo** oppure insieme $C$ (che non è ordinabile)
$z = (x,0)+(0,y)=x\cdot(1,0)+y\cdot(0,1)$, (1,0) è comunemente considerato 1, e (0,1) $i$ 
$i^2=-1$ e z si scrive $z=x+iy$  
Modulo: $|z|=\sqrt{x^2+y^2}$, La distanza del punto dall'origine
Argomento: $\arg z = \theta$, l'angolo con l'asse reale positivo. Se $x\neq 0$ allora $\tan \theta=\frac{y}{x}$ 

FORMA TRIGONOMETRICA
Avendo modulo e argomento possiamo scrivere:
	$x = r\cos\theta$ 
	$y=r\sin\theta$ 
e quindi:
$$
z=r(\cos \theta+i \sin \theta)
$$

FORMULA DI EULERO
$$
e^{i\theta}=\cos \theta+i \sin \theta
$$
e quindi: $z=r\cdot e{i\theta}$, forma esponenziale
La famosa identità di Eulero è quindi $e^{i\pi}+1=0$, ossia il caso in cui $\theta = \pi$
La forma esponenziale è utile ai fini della moltiplicazione:
	per esempio:
	$z_{1}=r_{1}\cdot e^{i\theta_{2}}$ e $z_{2}=r_{2}\cdot e^{i\theta_{2}}$: 
	$z_{1} \cdot z_{2}=r_{1}r_{2} \cdot e^{i(\theta_{1}+\theta_{2})}$, quindi $|z_{1}z_{2}|=|z_{1}||z_{2}|$ e $arg(z_{1}z_{2})=arg(z_{1})+arg(z_{2})$ 
	per la divisione, semplicemente:
	$\frac{z_{1}}{z_{2}}=\frac{r_{1}}{r_{2}}\cdot e^{i(\theta_{1}-\theta_{2})}$ 

CONIUGATO
Se $z=x+iy$, il coniugato è:
$$
\neg z=x-iy
$$ 
e, importante proprietà é:
$$
z\neg z=|z|^2
$$

DIVISIONE DI COMPLESSI IN FORMA ALGEBRICA
Per dividere $\frac{{2+i}}{{3-2i}}$
	1. Moltiplichiamo numeratore e denominatore per il coniugato del denominatore: $\frac{{2+i}}{3-2i}\cdot\frac{3+2i}{3+2i}$ 
	2. Otteniamo: $\frac{(2+i)(3+2i)}{(3-2i)(3+2i)}$, svolgendo i calcoli: $\frac{6+3i+4i+2i^2}{3^2+2^2}=\frac{4+7i}{13}=\frac{4}{13}+\frac{7}{13}i$ 


FORMULA DI DE MOIVRE PER LE POTENZE
Se abbiamo $z=r(\cos \theta+i\sin \theta)$, allora $z^n$=:
$$
z^n=r^n[\cos(n\theta)+i\sin(n\theta)] 
$$

RADICI COMPLESSE
Consideriamo $z^n=w$ 
Se $w=re^{i\theta}$ 
allora le soluzioni sono:
$$
z_{k}=\sqrt[n]r \cdot e^{i\frac{\theta+2k\pi}{n}} 
$$
con $k=0,1,\cdots,n-1$ 
TEOREMA FONDAMENTALE DELL'ALGEBRA
		*Ogni polinomio non costante a coefficienti complessi di grado $n$ possiede esattamente $n$ radici complesse, contando le molteplicità.*

## Parabola
Una parabola è il luogo geometrico dei punti equidistanti da un punto fisso (fuoco) e una retta fissa (direttrice), di equazione:
$$
y=ax^2+bx+c, a\neq 0
$$
ma la forma canonica geometricamente è:
$$
(x-h)^2=4p(y-k)
$$
Il vertice é: $V=(h,k)$, Il fuoco $F=(h,k+p)$, la direttrice è $y=k-p$ 

## Ellisse
L'ellisse è il luogo geometrico dei punti tali che la somma delle distanze da due punti fissi sia costante.
La condizione è:
$$
PF_{1}+PF_{2}= 2a
$$
dove $a$ è il semiasse maggiore.
La forma canonica, con centro nell'origine e asse maggiore orizzontale è:
$$
\frac{x^2}{a^2}+\frac{y^2}{b^2}=1
$$
con $a>b>0$, e i vertici sono $(\pm a, 0),(0,\pm b)$.

I **fuochi** sono $F_{1}=(-c,0), F_{2}=(c,0)$, quindi se abbiamo $c^2=a^2-b^2$ allora $c=\sqrt{a^2-b^2}$.

L'**eccentricità** è una quantità fondamentale, si indica con $e$ e ha le seguenti proprietà:
$$
e=\frac{c}{a}, 0<e<1
$$
Più l'eccentricità è vicina a 0 e più somiglierà ad una circonferenza.
## Iperbole
L'iperbole è il luogo geometrico dei punti per cui il **valore assoluto della differenza** delle distanze tra i due fuochi è costante.
$$
|PF_{1}-PF_{2}|= 2a
$$
e di forma canonica:
$$
\frac{x^2}{a^2}-\frac{y^2}{b^2}=1
$$
Qui abbiamo $c^2=a^2+b^2$, quindi l'eccentricità sarà per forza maggiore a 1
## Classificazione delle coniche in base all'eccentricità
Se prendiamo un fuoco $F$ e una direttrice $d$, allora possiamo considerare i punti $P$ tali che $\frac{PF}{d(P,direttrice)}=e$, abbiamo così che a seconda di e possiamo riconoscere tutti i quattro tipi di coniche:
- se $e=0 \Rightarrow$ circonferenza
- se $0<e<1 \Rightarrow$ ellisse
- se $e=1\Rightarrow$ parabola
- se $e>1\Rightarrow$ iperbole
## Equazione generale di una conica
$$
Ax^2+Bxy+Cy^2+Dx+Ey+F=0
$$
E' l'equazione generale di una conica.
Essendo un polinomio di secondo grado possiamo quindi ricavarne il discriminante $\Delta=B^2-4AC$, e in base al segno troviamo che
- $<0$ = ellisse/circonferenza
- $=0$ = parabola
- $>0$ = iperbole.
