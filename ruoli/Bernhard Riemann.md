# Bernhard Riemann
## Vita
Nacque il **17 settembre 1826** e morì il **20 luglio 1866**. Fu un'importante *matematico* tedesco, con un'importante contributo in:
* analisi
* teoria dei numeri
* geometria differenziale

Il padre combatté nelle **guerre napoleoniche**. 

Già da piccolo dimostrò grandi abilità nel calcolo. Nel **1846** fu mandato all'Università Göttingen, dove fu allievo di **Carl Friedrich Gauss**. Sucessivamente, diventò professore presso l'Università Göttingen nel **1854** e capo del dipartimento di matematica nel **1859**.

Morì per tubercolosi nel **1866** dopo la fuga dalla guerra fra Hanover e Prussia.

## Lavori
Oltre al suo lavoro sulle *serie di Fourier* nel campo dell'*analisi reale* è noto per la prima formulazione rigorosa dell'integrale: l'**integrale di Riemann**.

### Somma di Riemann

Sia $f: [a, b] \to R$.

Consideriamo i punti $a = x_0, x_1, x_2, \cdots, x_{n-1}, x_n = b$
che suddividono l'intervallo $[a, b]$ in $n$ intervalli aventi la stessa ampiezza, uguale a:

$\Delta x = \frac{b - a}{n}$

Scelto in ciascuno degli $n$ intervalli $[x_{i-1}, x_i]$ un punto arbitrario $c_i$, chiamiamo **somma di Riemman** della funzione $f$ nell'intervallo $[a, b]$ la somma: 

$S_n = \sum_{i=1}^{n} f(c_i)\Delta x$

### Integrale definito
Se $f: [a, b] \to R$  è una funzione continua, si potrebbe dimostrare che $\displaystyle \lim_{n \to +\infty} S_n$ **esiste finito** ed **è indipendente dalla scelta dei punti $c_i$**. Ha senso quindi dare la seguente definizione.

Sia $f: [a, b] \to R$ una funzione continua. Si chiama **integrale definito** della funzione $f$ nell'intervallo $[a, b]$ il $\displaystyle \lim_{n \to +\infty} S_n$, essendo $S_n$ una somma di Riemann della funzione $f$ nell'intervallo $[a, b]$. L'integrale definito della funzione $f$ nell'intervallo $[a, b]$ vine indicato con il simbolo:

$\int_{a}^{b} f(x)dx$

che si legge *"integrale da $a$ a $b$ di $f(x)$ in $dx$"*.