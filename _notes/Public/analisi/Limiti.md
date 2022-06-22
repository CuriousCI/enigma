# Limiti e continuità

## Introduzione all'analisi e funzioni
### Che cos'è l'analisi matematica
L'analisi nacque nel **XVII** secolo per affrontare tre categorie di problemi:
- la ricerca di soluzioni ottimali
- la ricerca della retta tangente a una curva
- calcolo di superfici dai contorni curvilinei

#### Problemi di ottimizzazione
Un esempio, nel **XVII**, è quello di [Galileo Galilei](../notabili/Galileo%20Galilei) e della **gittata massima del cannone** nel vuoto, che si ottiene a 45°. Nel **1626** [Willebrord Snell](../notabili/Willebrord%20Snell) scoprì la **legge di rifrazione** $\frac{\sin i}{\sin r} = \frac{v_1}{v_2}$, che fu dimostrata da Pierre de Fermat con il **cammino minimo ottico**, un altro problema di ottimizzazione.

#### Problema della retta tangente
Uno dei problemi legati alla tangente è quello di dare un senso alla **velocità istantanea**. Era semplice definire la **velocità media** in un intervallo di tempo $[t_0, t_1]$, avendo $v_{media} = \frac{\Delta s}{\Delta t}$, il problema si pone quando $\Delta s = \Delta t = 0$, che risulta in $\frac{0}{0}$, il che non ha significato! Si notò che $\frac{\Delta s}{\Delta t}$ non era altro che il **coefficiente angolare** della retta **tangente** in un determinato punto.

#### Il problema della misura
Il problema era già noto a [Archimede](../notabili/Archimede) con il metodo di **esaustione**, ma, nel **1600** un gruppo di matematici elaborò il metodo degli **indivisibili** *(Geometria degli indivisibili **1635**, Bonaventura Cavalieri)*, che vedeva le aree come infiniti segmenti indivisibili, e i volumi come infiniti fogli indivisibili, da cui [Isaac Newton](../notabili/Isaac%20Newton) riprese alcuni concetti per sviluppare gli **integrali**.

#### Il concetto di limite
Tutti gli studi e le analisi del **1600**, con la revisione di **numero reale** e di **funzione**, culminarono alla fine del **XVIII** secolo con la definizione formale di **limite**.

### L'insime R: richiame e complementi
#### L'insieme R
- L'insime di espandere l'**insime Q** deriva dal problema di introdurre i **numeri irrazionali** come $\sqrt{2}$ 
- Bisgona introdurre i **numeri irrazionali** *($\pi, \sqrt{3}$)* 

> Ogni numero (positivo o negativo) la cui rappresentazione decimale è illimitata e non periodica si dice **irrazionale** 

Si può quindi definire l'insieme **R**

> L'insieme formato dall'unione dell'insieme dei numeri razionali e dell'insieme dei numeri irraionali veine chiamatao insieme dei numeri **reali** e viene indicato con la lettera **R**

- l'insieme **R** rispetto a **Q** è **completo**

#### Massimo e minimo, estremo inferiore ed estremo superiore
Considreando un insieme $A$ non vuoto, esiste in $\mathbb{R}$ un numero $M$ **maggiore o uguale** a tutti gli elementi di $A$. In tal caso, $M$ si dice **maggiorante** e $A$ si dice **superiormente limitato**. 

Il numero real $m$ è un **minorante** di $A$ se è **minore o uguale** a tutti gli elementi dell'insieme, e, in tal caso, l'insieme $A$ si chiama **inferiormente limitato**. 

> $\{x \in \mathbb{R}:x\geq1\}$  è inferiormente limitato; il minorante più grande è 1, ma ne esistono infiniti altri

Un insieme sia **inferiormente** che **superiormente** limitato, si dice **limitato**.

> $A = (-1, 2] \cup  (4, 5]$ ammette sia un minorante e un maggiorante e si dice limitato

 Per cui:
 
 >Sia $A$ un sottoinsieme non vuoto in $\mathbb{R}$.
> 
 >1. Un numero reale $M$ si dice **massimo** di $A$ (e si scrive $M = max A$) quando sono verificate entrambe le seguenti condizioni
  >    - $M$ appartiene ad $A$;
  >    - $M$ è un maggiorante di $A$.
 > 
  >2. In maniera analoga, un numero reale $m$ si dice **minimo**  di $A$ (e si srive $m = min A$) quando appartiene ad $A$ ed è minorante di $A$.

Ma non si hanno in tutti i casi **minimi** e **massimi**, infatti:

>Sia $A$ un sottoinsieme non vuoto di $\mathbb{R}$
>
>1. Si chiama **estremo superiore** di $A$ (e si scrive $sup A$), se esiste, il minimo dell'insieme dei maggioranti di $A$.
>2. Si chiama **estremo inferiore** di $A$ (e si scrive $infA$), se esiste, il massimo dell'insieme dei minoranti di $A$.

#### I simboli di più infinito e meno infinito
Si può estendere l'insieme $\mathbb{R}$ con due nuovi elementi per attribuire l'**insieme inferiore** e **superiore** di insiemi non **limitati**:

>- $+\infty$  l'estremo superiore di ogni insieme superioremente illimitato
>- $-\infty$ l'estremo inferiore di ogni insieme inferiormente illimitato

Per cui, il **sistema ampliato dei numeri reali** si definisce come:

> $\mathbb{R}^* = \mathbb{R}  \cup  \{\pm \infty\}$  

### Dominio e studio del segno
#### Definizione e funzioni elementari
> Si chiama funzione $f$ di **dominio** $A$ e **codominio** $B$  una relazione che associa a **ogni** elemento di $A$ **uno e un solo** elemento di $B$ (si scrive $f:A\rightarrow B$) 

Se $A$ e $B$ sono sottoinsiemi di $\mathbb{R}$, la funzione si dice **reale** di **variabile reale**, e $f:\mathbb{R} \rightarrow\mathbb{R}$ si può scrivere con due notazioni:

>- $y = f(x)$, equazione di una funzione
>- $f(x) = \; ...$  espressione analitica della funzione

#### Classificazione
- **algebriche**, composte da *addizzione, sottrazione, moltiplicazione, divisione, elevamento a potenza*;
- **transcendenti**, tutte le altre *(come $y = lnx$, $y = e^x$, $y = \sin x$)*;
- **intere** *(polinomiali)*, se l'incognita non compare al denominatore;
- **frazionarie**, se l'incognita compare al denominatore;
- **razionali**, in cui l'incognita non compare sotto alcuna radice;
- **irrazionali**, in cui l'incognita compare sotto radice.

#### Dominio
%% TODO: indicazioni per determinare il dominio di una funzione %%

> Due funzioni $f$ e $g$ si dicono **uguali** se hanno lo stesso dominio $D$ e risulta: 
> $f(x) = g(x) \; \forall \; x \in D$

#### Il segno di una funzione
1. bisogna fare l'intersezione fra gli **assi** e la **funzione**;
2. ponendo $y = 0$, si trovano gli **zeri** della funzione;
3. è necessario stabilire per quali valori di $x$ risulta $f(x) > 0$ *(positiva)* e per quali $f(x) < 0$ *(negativa)*

### Prime proprietà
#### Immagine, massimo, minimo, estremo superiore ed estremo inferiore di una funzione
L'**insieme immagine** *(o semplicemente **immagine**)* della funzione è formato invece dai valori assunti da $y$ al variare di $x$ nel dominio della funzione:

> $y = \sin x$ al variare di $x \in \mathbb{R}$ ha come immagine l'intervallo $[-1, 1]$

> 1. Sia $f: D \rightarrow \mathbb{R}$ una funzione e sia $I$ l'insieme immagine della funzione. L'estremo superiore e l'estremo inferiore dell'insieme $I$ vengono chiamati rispettivamente **estremo superiore** ed **estremo inferiore della funzione** e si indicano con i simboli: $\sup f(x)$ e $\inf f(x)$ 
>
> 2. Analogmante, se esistono il massimo o il minimo dell'insieme $I$, vengono chiamati **massimo**  e **minimo (assoluti) della funzione** e si indicano con i simboli: $\max f(x)$ e $\min f(x)$ 

> Sia $f: D \rightarrow \mathbb{R}$ una funzione. La funzione si dice:
>
>1. **superiormente limitata**, se il suo estremo superiore è un numero reale;
>2. **inferiormente limitata**, se il suo estremo inferiore è un numero reale;
>3. **limitata**, se è sia superiormente limitata sia inferiormente limitata.

#### Funzioni crescenti e funzioni decrescenti
> Sia $I$ un sottoinsieme del dominio della funzione $y = f(x)$.
> 1. $f$ si dice **strettamente crescente** in $I$ se:
>	$x_1 < x_2 \Rightarrow f(x_1) < f(x_2) \; \forall \; x_1, x_2 \in I$
> 2. $f$ si dice **strettamente decrescente** in $I$ se:
>	$x_1 < x_2 \Rightarrow f(x_1) > f(x_2) \; \forall \; x_1, x_2 \in I$

Si possono intendere queste definizioni anche in senso **lato**:

> Sia $I$ un sottoinsieme del dominio della funzione $y = f(x)$.
> 1. $f$ si dice **crescente in senso lato** in $I$ se:
>	$x_1 < x_2 \Rightarrow f(x_1) \leq f(x_2) \; \forall \; x_1, x_2 \in I$
> 2. $f$ si dice **decrescente in senso lato** in $I$ se:
>	$x_1 < x_2 \Rightarrow f(x_1) \geq f(x_2) \; \forall \; x_1, x_2 \in I$

Le funzioni crescenti o decrescenti, in senso lato o in senso stretto, nel **dominio** prendono l'appellativo comune di funzioni **monotòne**.

#### Funzioni pari, funzioni dispari e funzioni periodiche
Il grafico di una funzione può presentare **simmetrie** o **ripetizioni** a intervalli regolari:

>Sia data una funzione $y = f(x)$, avente dominio $D$, tale che $\forall \; x \in D$ anche $-x \in D$.
> 1. Se risulta: $f(-x) = f(x) \; \forall \; x \in D$ 
>	la funzione si  dice **pari** e il suo grafico è simmetrico rispetto all'asse $y$.
> 2. Se invece: $f(-x) = -f(x) \; \forall \; x \in D$  
> 	la funzione si dice **dispari** e il suo grafico è simmetrico rispetto all'origine.

> Una funzione $f: D \rightarrow \mathbb{R}$ si dice **periodica** se e solo se esiste un numero $T > 0$  tale che $f(x) = f(x + T) \; \forall \; x \in D$. Il minimo valore di $T$, se esiste, per cui è verificata questa proprietà si dice **periodo (minimo)** della funzione $f$.

#### Funzione inversa
Una condizione *sufficiente* perché una funzione, **definita in un intervallo**, sia *invertibile* è che essa sia **strettamente crescente** (o **strettamente descrescente**).

> Una funzione $f$ si dice **invertibile** se e solo se esiste una **corrispondenza biunivoca** tra il dominio della funzione e il suo insieme immagine. In tal caso, si chiama funzione **inversa** di $f$, che si indica con il simbolo $f^{-1}$, la funzione che associa a ciascun elemento dell'immagine di $f$ la sua (unica) controimmagine.

Inoltre il grafico di $f$ e della sua inversa $f^{-1}$ sono simmetrici rispetto alla bisettrice del primo e del terzo quadrante.

Una volta determinato che $f(x)$ è **invertibile**, per determinare l'equazione inversa si possono seguire i seguenti passaggi:
1. nell'equazione $y = f(x)$ si sostituisce $y$ al posto di $x$ e $x$ al posto di $y$, ottenendo così l'equazione $x = f(y)$ 
2. se possibile, si risolve l'equazione $x = f(y)$ rispetto a $y$ in modo da ottenere l'equazione *esplicita* di $f^{-1}$.

Viene effettuata una **restrizione** della funzione quando la funzione non è invertibile in tutto il dominio, ma solo in un intervallo.

#### Funzione composta
La **composizione** permette di definire una nuova funzione partendo da due funzioni assegnate $f$ e $g$.

>Date due funzioni $f$ e $g$, si dice **funzione composta** di $f$ e $g$, e si indica con il simbolo $g \circ f$ (che si legge "$g$ composto $f$") la funzione definita da:
>	$(g \circ f)(x) = g(f(x))$

%% TODO: specificare dominio %%

Bisogna notare che $f \circ g \neq g \circ f$.

## Limiti di funzioni reali di variabile reale
### Il concetto di limite
### La definizione generale di limite
### Le definizioni particolari
### Teoremi di esistenzà e unicità sui limiti
### Le funzioni continue e l'algebra dei limiti
### Forme di indecisione di funzioni algebriche
### Forme di indecisione di funzioni transcendenti
### Infinitesimi e infiniti

## Successioni e principio di induzione
### Le successioni
### Progressioni aritmetiche e geometriche
### Limiti di successioni
### Principio di induzione

## Continuità
### Funzioni continue
### Punti singolari e la loro classificazione
### Proprietà delle funzioni continue
### Asintoti e grafico probabile di una funzione


