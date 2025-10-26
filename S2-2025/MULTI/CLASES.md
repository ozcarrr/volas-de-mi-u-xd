def: UNa función vectorial de una variable a valores en $\mathbb{R}^n$, es una función cuyo dominio es un conjunto de numeros reales, y su recorrido es un conjunto de vectores (o puntos de $\mathbb{R}^n$)

## Notación: $\vec{r}:\mathbb{R}->\mathbb{R}^n$, tal que, $\forall{t}\in{I},\vec{r}(t)=(f_1(t), ..., f_n(t))$ 

donde $f_i:I\subseteq{\mathbb{R}}->\mathbb{R}^n$ ; $i=1,2,...,n$ son funciones reales de una variable


las n-funciones $f_1, f_2, ..., f_n$ son llamadas "funciones componentes de la función vectorial $\vec{R}$" 

OBS: Si una función $\vec{r}$ describe el movimiento de una particula, el vector $\vec{r}(t)=(f_1(t), ..., f_n(t))$, nos indica la posición en el instante t.


EJ: sea $t\in{I}$ -> $\vec{r}(t)$ 

imagen...


Para el caso de $n=2$ o $n=3$ :

## $IM(\vec{r}) = {{\vec{r}(t)\in{\mathbb{R}^3}};t\in{I}}$       




EJ:  Considerando la siguiente función vectorial, $\vec{r}:\mathbb{R} -> \mathbb{R}^2$, dada por $\vec{r}(t)=(t, 3t)$ = $ti + 3tj$  

Notamos que la trayectoria de $\vec{r}$ es una recta de ecuaciones parametricas x(t) = t ; y(t) = 3t y con un vector director,$\vec{v}=(1,3)$ , entonces, la trayectoria es y = 3x

EJ: sea $\vec{r}(t)=(t,t²)=ti+t²j; t\in{[-1,3]}$ 

en este caso, la imagen de $r$ es la curva de ec. parametricas :

## $x(t)=t ; y(t)=t^2$ 

donde la trayectoria grafica de $\vec{r}$ coincide con $y=x²$

EJ: 

## $\vec{r}=cos(t)i+sin(t)j;t\in{[0,2\pi]}$ 


es una circunferecnia centrada en el origen de radio 1, donde su trayectoria es $x²+y²=1$ 







## Derivada de una función Vectorial

Def: Sea $\vec{r}(t)=(f_1(t), f_2(t),..., f_n(t))$ una función vectorial ; $t_0\in{dom(\vec{r})}\subseteq{R}$ 

Se define la derivada de $\vec{r}$ en $t_0$ como:

## $\vec{r}'(t) = \lim_{t\to{t_0}}\frac{\vec{r}(t-\vec{r}(t))}{t-t_0}$ 


### Entonces, si $h=t-t_0$, se tiene que $t=t_0+h$ y si $t\to{t_0}->h\to{0}$ 

Asi, el limite se escribe como:

## $\vec{r}'(t) = \lim{h\to{0}}\frac{\vec{r}(t_0+h)-\vec{r}(t_0)}{h}$ 



#### Teorema: sea $\vec{r}=(f_1,...,f_n)$ una función vectorial y $t_o\in{dom(\vec{r})}$, done $\vec{r}$ es derivable en $t_i;\forall{i}=1,2,...,n$ , entonces:

## $\vec{r}'(t)=(f_1'(t), f_2'(t),..., f_n'(t))$


#### EJEMPLO: Considere $\vec{r}(t)=(cos(t+\pi),2\frac{sin(t)}{t},e^{-t²})$ 

#### Note que $dom(\vec{r})=R-{0}$, ademas:

#### $\vec{r}'(t)=(-sin(t+\pi),2\frac{tcos(t)-sin(t)}{t²},-2te^{-t²})$ 


Teorema: Sean $\vec{u}(t)$ y $\vec{v}(t)$ funciones vectoriales derivables (son curvas especiales) se tiene:

## 1. $\frac{d}{dt}(\alpha\vec{u}(t))=\alpha\frac{d}{dt}(\vec{u}(t))$  

## 2. $\frac{d}{dt}(\vec{u}(t)+-\vec{v}(t))=\frac{d}{dt}(\vec{u}(t))+-\frac{d}{dt}(\vec(v(t))$ 

## 3. $(f(t)\vec{u}(t))'=f'(t)\vec{u}(t)+f(t)\vec{u}'(t)$  donde $f(t):R\to{R}$ 

## 4. $(\vec{u}\vec{v})'=\vec{u}'(t)\vec{v}(t)+\vec{u}(t)\vec{v}'(t)$   (El resultado seria un numero Real

## 5. $(\vec{u}(t)\times\vec{v}(t))'=\vec{u}'(t)\times\vec{v}(t)+\vec{u}(t)\times\vec{v}'(t)$  (Si y solo si $\vec{u}, \vec{v}\in\set{R³}$ 

## 6. $(\vec{u}(f(t)))'=\vec{u}'(f(t))f'(t)$ donde $f:R\to{R}$ 


### EJERCICIO:

Considere las siguientes funciones vectoriales :

## $\vec{u}(t)=(cos(t),sin(t),0)$ y $\vec{v}(t)=(1,arctan(t),-t²)$ 

determine :

## $\frac{d}{dt}(\vec{u}(t)\vec{v}(t))$ 

## $\frac{d}{dt}(\vec{u}(t)\times\vec{v}(t))$ 


## RECTA TANGENTE A UNA CURVA 

### Sea $\vec{r}=(x(t),y(t),z(t));t\in{I}$, una curva espacial, suponiendo que es derivable, la recta tangente a la funcion $\vec{r}$ en $t_0$ esta dada por: 

## $w=\vec{r}(t_0)+\alpha\vec{r}'(t_0);\alpha\in{R}$ 



## EJ: Dada la curva $\vec{r}(t)=(e^t,e^{-t},\sqrt{2}t)$ y el punto $p_0(1,1,0)$, encuentre la ecuación de la curva en el punto $p_0$ 


### dado que $\vec{r}$ es derivable, tenemos lo siguiente :

## $(e^t,e^{-t},\sqrt{2}t)=(1,1,0) -> t=0$ 


### luego $\vec{r'}(t)=(e^t,-e^{-t},\sqrt{2})$, entonces, con $t=0$, nuestro vector director es $\vec{r}'(0)=(1,-1,\sqrt{2})$  


## finalmente, la ecuacion de la recta es:

## $L: (1,1,0)+\alpha(1,-1,\sqrt{2});\alpha\in{R}$ 



## Vector tangente, nromal y binormal 


### Sea $C$ una curva "suave", dada por la función vectorial $\vec{r}(t);t\in{I}$, se definen los siguientes vectores: 

## 1. Vector tangente unitario a lo largo de $C$ :

## $T(t)=\frac{\vec{r}'(t)}{||\frac{d}{dt}\vec{r}(t)||}$ 


## 2. Vector normal a lo largo de $C$ :

## $N(t)=\frac{T'(t)}{||T'(t)||}$ 

## 3. Vector binormal unitario a lo largo de $C$:

## $B(t)=T(t)\times N(t)$ 



## OBS:

## $T(t)\times N(t)=B(t)$ | $TT=1$ 

## $T(t)\times B(t)=N(t)$ | $NN=1$ 

## $B(t)\times N(t)=T(t)$ | $BB=1$ 


## MICH 

# 13/08/25

### Teorema :

### Sea $C$ una curva suave dada por la función vectorial $\vec{r}(t);t\in{I}$, sea $t_0\in{I}$, tenemos:

#### 1. $\vec{B}(t_0)=\frac{\vec{r}'(t_0)\times{\vec{r}''(t_0)}}{||\vec{r}'(t_0)\times{\vec{r}''(t_0)}||}$ 

#### 2. $\vec{N}(t_0) = \frac{(\vec{r}'(t_0)\times{r}''(t_0))\times{\vec{r}'(t_0)}}{||(\vec{r}'(t_0)\times{r}''(t_0))\times{\vec{r}'(t_0)}||}$ 


## EJERCICIO PROPUESTO:
### Considere la helice dada por:

## $C: \vec{r}(t)=(cos(t),2t,sin(t))$ 

### a) Determine los vectores tangente unitario, normal unitario y binormal a $C$ en el punto $(-1,2\pi,0)$ 

### b) ¿Es el vector normal en cualquier punto de $C$, ortogonal a eje $y$? 

# Longitud de arco

### Def: sea $C$ una curva suave definida por la función vectorial $\vec{r}(t)=(x(t),y(t),z(t));t\in[a,b]$. Definimos la longitud de arco de $C$ como: 

## $L_C=\int_{t_0}^{t}{\vec{r}'(t)}Vdt=\int_{t_0}^{t}{\sqrt{(x'(t))²+(y'(t))²+(z'(t))²}}$  

### Ejemplo: sea $C$ una curva definida por la funcion vectorial $\vec{r}(t)=(\frac{t²}{2},sin(t)-tcos(t),cos(t)+tsin(t));t\in[0,\pi]$, calcule la longitud de curva de $C$:


## $\vec{r}'(t)=(t,cos(t)-(cos(t)-tsin(t)),-sin(t)+sin(t)+tcos(t))=(t,tsin(t),tcos(t))$

## $||\vec{r}'(t)||=\sqrt{t²+t²sin²(t)+t²cos²(t)}=\sqrt{2t²}=\sqrt{2}|t|=\sqrt{2}t$ 

### Entonces : $L_C=\int_{t_0}^{t}{||\vec{r}'(t)}dt=\sqrt{2}\int_{t_0}^{t}{t}dt=\frac{\sqrt{2}}{2}\pi²$  

# Función longitud de arco 

### Def: Sea $C$ una curva suave dada por la función vectorial $\vec{r}:I\subseteq{R}->R³$ ; $\vec{r}(t)=(x(t),y(t),z(t))$ 
### Supongamos que $\vec{r}$ es diferenciable; $t_0\in{I}$, se define la longitud de arco $\vec{r}(C)$, relativa a $t_0$, como: 

## $s(t)=\int_{t_0}^{t}{||\vec{r}'(u)||}du$ entrega la longitud de la curva, desde el punto inicial $\vec{r}(t_0)$ hasta el punto variable $\vec{r}(t)$ 
### OBS: Por el teorema fundamental del calculo (TFC) se tiene lo siguiente: 

## Si $F(u)$ es una primitiva de la $||\vec{r}'(u)||$, entonces:

## $s(t)=\int{||\vec{r}'(u)||}du=F(u)=F(t)-F(t_0)$ donde $F(t_0)$ es constante, entonces :

## $s'(t)=\frac{ds}{dt}=\frac{d}{dt}(\int{||\vec{r}'(u)}du)=||\vec{r}'(t)||$ Por lo tanto, $s$ es una función diferenciable, y $s'(t)=\frac{ds}{dt}=||\vec{r}'(t)||$, además :

## $ds=||\vec{r}'(t)||dt$ 

### Def: Una curva $C$ dada por $\vec{r}(t)=(x(t),y(t)z(t))$ se dice "parametrizada por la longitud de arco si y solo si $||\vec{r}'(t)||=1,\forall{t}$ "

### obs: Sea $C$ una curva suave, dada por $\vec{r}(t)=(x(t),y(t),z(t))$ ; suponga que $\vec{r}'(t)\not=0,\forall{t}$. 

## Como $s'(t)=\frac{ds}{dt}=||\vec{r}'(t)||>0,\forall{t}$, entonces $s$ es una función creciente de $t$, y por lo tanto invertible, con inversa $t=t(s)$, entonces:

## $s=s(t)<->t=t(s)$ ; La funcion $s$ siendo la longitud de arco y $t$ es la inversa de $s$. 

### Cuando sustituimos $t$ por $t(s)$ en las ecuaciones originales de $C$, obtenemos la reparametrización por la longitud de arco de la curva $C$: 

## $\beta(s)=x(s)i+y(s)j+z(z)k=(x(s),y(s),z(s))$  

## donde $||\beta'(s)||=1$ 

## Ejercicio :

### Considere la hélice $C$ dada por la función vectorial:

## $\vec{r}(t)=(5cos(t),5sin(t),12t),t\in{R}$ 

### Reparametrice la curva $C$ con respecto a la longitud de arco, medida a paritr del punto (5,0,0), en la dirección en que aumenta $t$. 

### Respuesta : $\vec{r}'(t)=(-5sin(t),5cos(t),12)$ entonces $||\vec{r}'(t)||=\sqrt{25sin²(t)+25cos²(t)+144}=13$ que es distinto de 1, entonces la curva $C$ no esta parametrizada por la longitud de arco. 

## Reparametricemos $C$ por la longitud de arco: 

### El punto $(5,0,0)$ corresponde a $t=0$, por lo tanto la función longitud de arco relativa a $t=0$ es:

## $s(t)=\int_{0}^{t}{||\vec{r}'(u)||du}=\int_{0}^{t}{\sqrt{169}du}=\int_{0}^{t}{13}du=13t$ 

## entonces: $s(t)=13t$, donde su inversa es $t(s)=\frac{s}{13}$ 
## Sustituyendo en las ecuaciones originales de $C$, $t$ por $\frac{s}{13}$, obtenemos: 

## $C: \vec{\beta}(s)=(x(\frac{s}{13}),y(\frac{s}{13}),z(\frac{s}{13}))=(5cos(\frac{s}{13}),5sin(\frac{s}{13}),12\frac{s}{13})$  

#### Note que $||\vec{\beta}'(s)||=1$, Verificar. 

## Ejercicio :

### Considere la curva $C$, dad por $\vec{r}(t)=(e^tcos(t),e^tsin(t),e^t),t\in[0,+\infty]$ 

### a) Determine $\vec{T},\vec{N},\vec{B}$ en el punto $P(0,e^{\frac{\pi}{2}},e^{\frac{\pi}{2}})$ 

### b) Parametrice $C$ con respecto al parametro longitud de arco. 


## RESPUESTA : $\vec{r}(t)=(e^tcos(t),e^tsin(t),e^t)=(0,e^{\frac{\pi}{2}},e^{\frac{\pi}{2}})$ 

## -> $e^{t}cos(t)=0 ; e^{t}sin(t)=e^{\frac{\pi}{2}} ; e^{t}=e^{\frac{\pi}{2}}$ -> $\vec{r}(\frac{\pi}{2})=(0,e^{\frac{\pi}{2}},e^{\frac{\pi}{2}})$ 

## Por otro lado : $\vec{r}'(t)=(e^t(cos(t)-sin(t)),e^t(sin(t)+cos(t)),e^t)$ 

## -> $\vec{r}''(t)=(-2e^tsin(t),2e^tcos(t),e^t)$ 

## $\vec{r}'(\frac{\pi}{2})=e^{\frac{\pi}{2}}(-1,1,1)$ 
## $\vec{r}''(\frac{\pi}{2})=e^{\frac{\pi}{2}}(-2,0,1)$  

## Por lo tanto $\vec{T}(t)= \frac{ \vec{r}'(t)}{||\vec{r}'(t)||}->\vec{T}(\frac{\pi}{2})=\frac{\vec{r}'(\frac{\pi}{2})}{||\vec{r}'(\frac{\pi}{2})||}=\frac{e^{\frac{\pi}{2}}(-1,1,1)}{e^{\frac{\pi}{2}}\sqrt{3}}=\frac{1}{\sqrt{3}}(-1,1,1)$ 

# 20/08 

# Plano osculador, normal y rectificante por un pounto de una curva. 

### Sea $C$ una curva dada por la función vectorial $\vec{r}(t)=(x(t),y(t),z(t))$; $t\in{I}$ y un punto $P=\vec{r}(t_0)$ 

## 1. Plano Osculador:  
### Este plano está dirigido (o generado) por los vectores $\vec{T}$ y $\vec{N}$ es ortogonal al vector $\vec{B}$. 

### $\vec{B}(t_0)=(b_1(t_0), b_2(t_0), b_3(t_0))$ 

### Luego, la ecuación del plano osculador de la curva $C$ en el punto $P=\vec{r}(t_0)$ esta dada por: 

# $\vec{B}(t_0)\cdot{(x-x(t_0),y-y(t_0),z-z(t_0))}=0$ 
# <-> $b_1(t_0)(x-x(t_0))+b_2(t_0)(y-y(t_0))+b_3(t_0)(z-z(t_0))=0$ 

## Plano Normal: 

### Este plano esta dirigido (o generado) por los vectores $\vec{N}$ y $\vec{B}$, por lo tanto, e es ortogonal al vector $\vec{T}$ (vector tangente).

# $\vec{r}'(t_0)=(x'(t_0),y'(t_0),z'(t_0))$ (Vector normal al plano Normal)

### Por lo tanto la ecuación del plano normal esta dada por. 

# $\vec{r}'(t_0)\cdot{(x-x(t_0),y-y(t_0),z-z(t_0))}=0$ <-> $x'(t_0)(x-x(t_0)) + y'(t_0)(y-y(t_0)) +z'(t_0) (z-z(t_0))=0$ 
# Plano Rectificante 

### Este plano esta dirigido (o generado) por los vectores $\vec{T}$ y el $\vec{B}$, entonces el es ortogonal al vector $\vec{N}$ (vector normal). 

# $\vec{N}(t_0)=(n_1(t_0),n_2(t_0),n_3(t_0))$ (Vector normal al plano rectificante) 

### Por lo tanto, la ecuación del plano rectificante a $C$ en el punto $P=\vec{r}(t_0)$ esta dada por:

# $n_1(t_0)\cdot{(x-x(t_0))}+n_2(t_0)\cdot{(y-y(t_0))}+n_3(t_0)\cdot{(z-z(t_0))}=0$ 

## Ejercicio :

### Determine las ecuaciones de los planos normal, osculador y rectificante de la helice $\vec{r}(t)=(2cos(t),2sin(t),t)$ ;$t\in{R}$ en el punto $P(0,2,\frac{\pi}{2})$ 

## Respuesta:
### Sea $t_0\in{R}$ tal que:

## $\vec{r}(t_0)=(0,2,\frac{\pi}{2})$ 

## -> $2cos(t_0)=0 ; 2sin(t_0)=2 ; t = \frac{\pi}{2}$ -> $t_0=\frac{\pi}{2}$ 


## luego, $P=\vec{r}(\frac{\pi}{2})$ 

## Tenemos: 

# $\vec{r}'(t)=(-2sin(t),2cos(t),1) ; \vec{r}''(t)=(-2cos(t),-2sin(t),0)$ 
# -> $\vec{r}'(\frac{\pi}{2})=(-2,0,1) ; \vec{r}''(\frac{ \pi}{2})=(0,-2,0)$ 


### Como el vector tangente es ortogonal al plano normal a la curva $C$ en $P$, entonces $\vec{r}'(\frac{\pi}{2})$ es ortogonal al plano normal, por lo tanto su ecuación es: 

# $\vec{r}'(\frac{\pi}{2})\cdot{(x-0,y-2,z-\frac{\pi}{2})}=0$ 
# -> $-2(x-0)+0(y-2)+1(z-\frac{\pi}{2})$ <-> $-2x+z-\frac{\pi}{2}=0$ (ecuación plano normal)


## luego, calculamos el vector $\vec{B}$ :

# $\vec{r}'(\frac{\pi}{2})\times\vec{r}''(\frac{\pi}{2})=(-2,0,1)\times(0,-2,0)=(2,0,4)$ 

# -> $\vec{B}(t_0)=\vec{r}'(\frac{\pi}{2})\times{\vec{r}''(\frac{\pi}{2})}$ / norma de $\vec{B}'(t_0)=\vec{r}'(\frac{\pi}{2})\times{\vec{r}''(\frac{\pi}{2})}$ = $\frac{1}{\sqrt{20}}\cdot(2,0,4)$ 


## La ecuación del plano osculador a $C$ es en el punto $P$ es : 

# $\vec{B}(\frac{\pi}{2})\cdot(x-0,y-2,z-\frac{\pi}{2})=0$ 
# <-> $\frac{2}{sqrt{20}}x+0(y-2)+\frac{4}{\sqrt{20}}(z-\frac{\pi}{2})=0$ 

# <-> $2x+4z-2\pi=0$  (ecuación plano osculador)

## 3. calcular plano rectificante lol oye mira tu



# Curvatura y torsión 

### def: La curvatura de una curva $C$ esta dada por: 

# $k=||\frac{dT}{ds}||$ 

### donde $T$ es el vector tangente unitario. 

#### Nota: Curvatura en terminos del parametro $t$ : 

# $\frac{dT}{dt}=\frac{DT}{ds}\cdot{\frac{ds}{dt}}$ -> $\frac{dT}{ds}=\frac{\frac{Dt}{dt}}{\frac{ds}{dt}}$ 


### Luego $k=||\frac{dT}{ds}||=||\frac{\frac{dT}{ds}}{\frac{ds}{dt}}||=\frac{||\frac{dT}{dt}||}{|| || \vec{r}(t) || ||}= \frac{||T'(t)||}{||\vec{r}'(t)||};\vec{r}(t)\not=\vec{0}$ 

### se supone que $C$ esta dada por la función vectorial $\vec{r}(t)=(x(t),y(t),z(t))$ 

# Teorema: La curvatura de una curva $C$ dada por la función vectorial $\vec{r}(t)$, esta dada por: 

# $k(t)=\frac{||\vec{r}'(t)\times\vec{r}''(t)||}{||\vec{r}'(t)||³}$ 


### Definición (Torsión) : Se define la torisón de una curva $C$, dada por la función vectorial $\vec{r}(t)=(x(t),y(t),z(t));t\in{I}$ como:

# $\tau(t)=\frac{(\vec{r}'(t)\times\vec{r}''(t))\cdot\vec{r}'''(t)}{|| \vec{r}'(t)\times\vec{r}''(t)||²}$ 


### Notas: "La torsión mide el grado de torcedura de la curva $C$". 
### "La torsión mide el desvio de la curva  respecto del plano oscular". 


# Componente tangencial y normal de la aceleración 

## Sea $C$ definida por $\vec{r}(t)=(x(t),y(t),z(t))$ 

### definición :

### Si el parametro $t$ es el tiempo entonces $\vec{r}''(t)$ es la aceleración de una particula con posición instantanea $\vec{r}(t)$. los coeficientes de los vectores $T$ y $N$ son respectivamente las componentes tangencial y normal de la aceleración

### De hecho :

# $T(t)=\frac{\vec{r}'(t)}{||\vec{r}'(t)}$ -> $\vec{r}'(t)=||\vec{r}'(t)||\cdot{T(t)}$ 


# $\Rightarrow$ $\vec{r}''(t)=\frac{d}{dt}(||\vec{r}'(t)||)\cdot{T(t)}+||\vec{r}'(t)||\cdot{T'(t)}$ 

## sabemos que $s'(t)=\frac{ds}{dt}=||\vec{r}'(t)||$ 

## -> $s''(t)=\frac{d}{dt}(||\vec{r}'(t)||)$ 

## $=s''(t)\cdot{T(t)}+||\vec{r}'(t)||\cdot{T'(t)}$ 

### además $N(t)=\frac{T'(t)}{||T'(t)||}$ 

## entonces : 

# $s''(t)\cdot{T(t)}+||\vec{r}'(t)||\cdot||T'(t)||\cdot{N(t)}$ 


## sabemos que $k(t)=\frac{||T'(t)||}{||\vec{r}'(t)||}$ (curvatura) y $s'(t)=||\vec{r}'(t)||$ 
## entonces :

# $=s''(t)\cdot{T(t)}+s'(t)\cdot||T'(t)||\cdot{N(t)}$ 

# $=s''(t)\cdot{T(t)}+s'(t)\cdot{k(t)\cdot||\vec{r}'(t)||}\cdot{N(t)}$ 

# -> $\vec{r}''(t)=s''(t)\cdot{T(t)}+(s'(t))²\cdot{k(t)}N(t)$ 

## obs: $s''(t)$ es la componente tangencial de la aceleración
### obs: $(s'(t))²\cdot{k(t)}$ es la componente normal de la aceleración


## Notación: 

# $a_T=s''(t)$  (componente tangencial)$a_N=(s'(t))²\cdot{k(t)}$ (componente normal)


## obs: Geometricamente si se proyecta $\vec{r}''(t)$ sobre los vectores $T$ y $N$, se puede concluir lo siguiente :

# $\vec{r}''(t)=[\vec{r}''\cdot{\vec{T}(t)}]+[\vec{r}''(t)\cdot{N(t)}]$ donde $\vec{r}''(t)\cdot{T(t)}$ y $\vec{r}''(t)\cdot{N(t)}$ son respectivamente las componentes tangencial y normal de la aceleración. 


## Proposición: Sean $a_T$ y $a_N$ las componentes tangencial y normal de la aceleración. Se tiene: 

# $a_T=\frac{\vec{r}'(t)\cdot{\vec{r}''(t)}}{||\vec{r}'(t)||}$ (Escalar)

# $a_N=\frac{||\vec{r}'(t)\times\vec{r}''(t)||}{||\vec{r}'(t)||}$ (Escalar)


## Bosquejo de demostración: 

### Sabemos que : 

# $a_T(t)=s''(t)=\vec{r}''(t)\cdot{T(t)}=\vec{r}''(t)\cdot{\frac{\vec{r}'(t)}{||\vec{r}'(t)||}}$ 

# $=\frac{\vec{r}''(t)\cdot{\vec{r}'(t)}}{||\vec{r}'(t)||}$ 

# = $\frac{\vec{r}'(t)\cdot{\vec{r}''(t)}}{||\vec{r}'(t)||}$ (Escalar (Numero real))
# $a_N = (s'(t))²\cdot{k(t)}=||\vec{r}'(t)||²\cdot{\frac{||\vec{r}'(t)\times\vec{r}''(t)|}{||\vec{r}'(t)||³}}$ 

## Finalmente : $\frac{||\vec{r}'(t)\times{\vec{r}''(t)}||}{||\vec{r}'(t)||}=a_N$ 


## Ejercicio considere la curva: $\vec{r}(t)=ti+cos²(t)j+sin²(t)k$ ; $t\geq{0}$ 
## Función vectorial que describe el movimiento de una particula en el espacio. 

### Calcule las componentes tangencial y normal de la aceleración 

# RESPUESTA :

### $\vec{r}(t)=(t,cos²(t),sin²(t));t\geq{0}$ 

### $\vec{r}'(t)=(1,-2sin(t)cos(t),2sin(t)cos(t))=(1,-sin(2t),sin(2t))$ 
### $\vec{r}''(t)=(0,-2cos(2t),2cos(2t))=2cos(2t)(0,-1,1)$ 



## Por otro lado: 

### Sea $s$ la función longitud de arco se tiene:

# $\frac{ds}{dt}=s'(t)=||\vec{r}'(t)||=\sqrt{1+2sin²(2t)}$ 

# -> $s''(t)=\frac{1}{2\sqrt{1+2sin²(2t)}}\cdot{4sin(2t)2cos(2t)}$ 

# $=\frac{4sin(2t)cos(2t)}{\sqrt{1+2sin²(2t)}}$ 

# = $2[\frac{2sin(2t)cos(2t)}{\sqrt{1+2sin²(2t)}}]$ 

# $=\frac{2sin(4t)}{\sqrt{1+2sin²(2t)}}$ 

## entonces, $a_T=s''(t)=\frac{2sin(4t)}{\sqrt{1+2sin²(2t)}}$ 

## Por otro lado $a_N=?$ 

# $a_N=s'(t)²\cdot{k(t)}$ 

# $\vec{r}'(t)\times{\vec{r}''(t)}=(1,-2sin(2t),2sin(2t))\times{(0,-2cos(2t),2cos(2t))}=(0,-2cos(2t),-2cos(2t))$ 
# $u$ 

## Luego, $k(t)=\frac{||\vec{r}'(t)\times{\vec{r}''(t)}||}{||\vec{r}'(t)||³}=\frac{2 \sqrt{2}cos(2t)}{(1+sin²(2t))^{\frac{3}{2}}}$ 


## Así: 

# $a_N=(s''(t))^2\cdot{k(t)}=(1+2sin²(2t))\cdot{\frac{2\sqrt{2}|cos(2t)}{(1+sin²(2t))^{\frac{3}{2}}}}$ 

# Funciones de varias variables 

### def: Llamaremos función real o escalar de varias variables a toda función del tipo: 

# $f: u\subseteq{R^{n}}\Rightarrow{R}$ ; $u=dom(f)$ 

#### $x\rightarrow{f(x)}$ 

### aqui:

## $x=(x_1,x_2,...,x_n)$ 
## $f(x)=f(x_1,...,x_n)$ 


### Ejemplos: 

### $f(x,y)=x²+y²$ 

### $f(x,y)=\sqrt{9-x²-y²}$

### $f(x,y,z)=\frac{\sqrt{49-z²}}{25+\sqrt{16-x²-y²}}$ 

### OBS: Dada la función $f: U\subseteq{R^{n}}->R$ 

### 1. Se entendera como dominio de $f$ al mayor subconjunto de $R^n$ , tal que $f(x)$ tenga sentido en $R$, esto es:

# $dom(f)={(x_1,x_2,x_n)}\in{R^{n}} | f(x)\in{R}$} 

### 2. Se entendera como recorrido de $f$ al siguiente conjunto: 

## $Rec(f)=$ conjunto de todos los valores que toma $f(x)$, para $x\in{dom(f)}$.

### Ejemplo:  Sea $f(x,y)=\sqrt{1-x²-y²}$. Tenemos: 

### $dom(f)=(x,y)\in{R²} | f(x,y)\in{R}=(x,y)\in{R²} | \sqrt{1-x²-y²}\in{R}$ 

### -> $dom(f)=(x,y)\in{R²} | x²+y²\leq{1}$ 

### -> $Rec(f(x,y)): f(x,y)=\sqrt{1-x²-y²}\geq{0}$ 

### -> $x²+y²+z²=1$ ; $z\geq{0}$ (Hemisferio norte de la esfera $x^2+y²+z²=1$ centrada en $(0,0,0)$ de radio $1$).

### -> $Rec(f)=[0,1]$ 

### Ejemplo : sea $f(x,y)=\frac{1}{\sqrt{x²-4y²}}$. en este caso: 

## $dom(f) = (x,y)\in{R²} | x²-4y²>0$ 

### -> $2|y|<|x|$ -> $-\frac{1}{2}|x|<y<\frac{1}{2}|x|$ 

### -> $dom(f)=(x,y)\in{R²} | -\frac{1}{2}|x|<y<\frac{1}{2}|x|$ 

### $Rec(f)=]0,+\infty[$ 

### ejercicio: Sea $f(x,y,z)=\frac{\sqrt{49-z²}}{25+\sqrt{16-x²-y²}}$. Determine el dominio y recorrido de $f$. 

# Grafico de una función de varias variables 

### sea $f:U\subseteq{R^n}->R$ una función escalar, se define el grafico de $f$, que anotamos $gra(f)$ como el conjunto; 

# $gra(f)=$ {$(x_1,x_2,...,x_n),f(x_1,x_2,..,x_n))$ | $(x_1,x_2,...,x_n)\in{dom(f)}$  } 

### Note que: $gra(f)\subseteq{R^{n+1}}$ 
#### Para el caso $n=1$ ; $f:U\subseteq{R²}->R$ ; $f(x,y)=z$ 


### Tenemos: 

# $gra(f)=$ {$(x,y,f(x,y))\in{R³}$ | $z=f(x,y) , (x,y)\in{dom(f)}$}

# = $gra(f)=$ {$(x,y,z)\in{R³} | z=f(x,y),(x,y)\in{dom(f)}$ }


![[Screenshot from 2025-08-30 17-07-43 1.png]]


### ejemplo: $f(x,y)=\sqrt{1-x²-y²}$ 

### $dom(f)=${$(x,y)\in{R²}$ | $x²+y²\leq{1},z\geq{0}$ } (disco unitario :O)

### $x=\sqrt{1-x²-y²}\geq{0}$ -> $x²+y²+z²=1$ 


![[Screenshot from 2025-08-30 17-09-06.png]]


# Conjuntos de nivel 

### def: Sea $f:U\subseteq{R^n}->R$ una función escalar. sea $C\in{R}$, el conjunto de nivel o valor $C$ en $f$ se define:

# $N_C(f)=$ {$(x_1,x_2,..,x_n)\in{dom(f)}$ | $f(x_1,x_2,...,x_n)=c$}

### note que $N_C\subseteq{dom(f)}$ 

### - Si $n=2$, nos referimos a "curvas de nivel"
### - Si $n=3$, nos referimos "Superficies de nivel" 
### - Si $n>3$, nos referimos a "Hiper-superficies de nivel"


## Ejemplo: Sea $f(x,y)=x²+y²$. Determine los conjuntos de nivel de $f$ (o curvas de nivel de $f$). Ademas, bosqueje la grafica de $f$ 
### Respuesta: $f(x,y)=z=x²+y²$ y $dom(f)=R²$ 

## $N_C=$ {$(x,y)\in{R²}$ | $f(x,y)=C$ }= {$(x,y)\in{R²}$ | $x²+y²=C$ }

### Tenemos:

### - Si $c<0$ -> $N_C(f)=\emptyset$ 
### - SI $c=0$ -> $N_C={(0,0)}$
### - Si $c>0$ -> $N_C(f)=$ {$(x,y)\in{R} | x²+y²=(\sqrt{c})²$}


### Si $c>0$, los conjuntos (o curvas) de nivel de $f$ son circunferencias centradas en el origen y radio $r=\sqrt{c}$ 

### Curvas de nivel  de $f$:

### insertar imagen lol

### Traza de una superficie: 
#### Son las secciones transversales que se generan cuando la superficie intersecta un plano paralelo a los planos cordenados.

#### Ejemplo: $T_{R_{X_Y}}:x²+y^2 = 0 -> (x,y=(0,0))$ 
### $T_{R_{x_z}}:x²=z$ (Parabola en el plano xz)
### $T_{R_{y_z}}:y²=z$ (Parabola en el plano yz)

![[Screenshot from 2025-08-30 17-10-42.png]]


# Ejercicio: Determine los conjuntos (superficies) de nivel de la función:

# $f(x,y,z)=ln(\frac{1+\sqrt{x²+y²+z²}}{1-\sqrt{x²+y²+z²}})$ 

### OBS (Integración de funciónes vectoriales): 

### Sea $\vec{r}(t)=(f_1(t),f_2(t),...,f_n(t))$ una función vectorial con $t\in{[a,b]}$, Entonces: 


# $\int_{a}^{b}\vec{r}(t)dt=\int_{a}^{b}f_1(t)dt+...+\int_{a}^{b}f_n(t)dt$ 

### La integral indefinida de $\vec{r}(t)$, queda:

# $\int{\vec{r}(t)}dt=\int{f_1(t)dt}+...+\int{f_n(t)dt}$ = $(\int{f_1(t)dt},...,\int{f_n(t)dt})$ ; donde las constantes de cada integral se anotan de manera $c_1,c_2,...,c_n$ 


### Ejercicio (aplicación): Determine los vectores velocidad y de posición de una particula que tiene aceleración $\vec{a}(t)=(0,0,-10)[\frac{m}{s²}]$, velocidad inicial $v(0)=(1,1,0)[\frac{m}{s}]$ y posición inicial $\vec{r}(0)=(0,0,0)$ 



# *Derivadas Parciales* 

### Sea $f:A\subseteq{R^n}->R$ una función; $A\not=\emptyset$ . $a=(a_1,a_2,...,a_n)$ ; $a\in{A}$ , la expresión 


## $\lim_{h_{k}->0}\frac{f(a_1,...,a_{k-1},a_k+h_k,a_{k+1},...,a_n)-f(a_1,...,a_n)}{h_k}$ 

#### Si existe, se denomina "derivada parcial de $f$, con respecto a la $k$-esima variable en el punto $a$"

#### SI el limite existe, lo denotariamos como: 

# $\frac{\delta f}{\delta x_k},f_k(a),f_{x_k}(a),D_kf(a)$ 



## Caso particular: $n=2$ 

### Sea $f:A\subseteq{R²}->R$ , $a=(x_0,y_0)\in{A}$, entonces: 

### 1. $\frac{\delta f}{\delta x}(x_0)(y_0)=\lim_{h->0}\frac{f(x_0+h,y_0)-f(x_0,y_0)}{h}$ 

### $\frac{\delta f}{\delta y}(x_0,y_0)=\lim_{h->0}\frac{f(x_0,y_0+h)-f(x_0,y_0)}{h}$ 

### En general, para $(x,y)\in{A}$, las derivadas de $f$ quedan escritas como: 

# $\frac{\delta f}{\delta x}(x,y)=\lim_{h->0}\frac{f(x+h,y)-f(x,y)}{h}$ 

# $\frac{\delta f}{\delta y}(x,y)=\lim_{h->0}\frac{f(x,y+h)-f(x,y)}{h}$ 

## Para fines de calculo: 

### Para encontrar $\frac{\delta f}{\delta x}(x,y)$, se considera la variable y constante, y se deriva $f(x,y)$ con respecto a $x$.

### Para encontrar $\frac{\delta f}{\delta y}(x,y)$, se procede de forma analoga. 

### Ejemplo: Sea $f(x,y)=sin(\frac{x}{1+y})$, encuentre $\frac{\delta f}{\delta x}(x,y)$ y $\frac{\delta f}{\delta y}(x,y)$ 

### -> $\frac{\delta f}{\delta x}(x,y)=cos(\frac{x}{1+y})\frac{1}{1+y}$ 
### -> $\frac{\delta f}{\delta y}(x,y)=cos(\frac{x}{1+y})\cdot{-\frac{x}{(1+y)²}}$ 

# Interpretación geometrica:

![[Screenshot from 2025-08-30 17-12-21.png]]

# *Derivadas parciales de orden superior*

### Si $f$ es una función de las variables $x$ e $y$, entonces sus derivadas parciales $\frac{\delta f}{\delta x}$ y $\frac{\delta f}{\delta y}$, también son funciones de las variables $x$ e $y$, de modo que podemos considerar sus derivadas parciales con respecto a $x$ y con respecto a $y$. 

### Estas derivadas reciben el nombre de "derivadas parciales de segundo orden de $f$". 

## Notaciones: 

### $\frac{\delta f}{\delta x}(\frac{\delta f}{\delta x})=\frac{\delta²f}{\delta x²}$ ~~~~~ > $f_{xx}$ 
### $\frac{\delta f}{\delta y}(\frac{\delta f}{\delta y})=\frac{\delta²f}{\delta y²}$ ~~~~ > $f_{yy}$ 
### $\frac{\delta }{\delta x}(\frac{\delta f}{\delta y})=\frac{\delta²f}{\delta x \delta y}$ ~~~~~ > $\frac{\delta z}{\delta x \delta y}$ ; $f_{yx}$ 
### $\frac{\delta }{\delta y}(\frac{\delta f}{\delta x})=\frac{\delta²f}{\delta y \delta x}$ ~~~~ > $\frac{\delta² z}{\delta y \delta x}$ ; $f_{xy}$ 


# *Teorema de Schwarz*

### Sea $f$ una función de las variables $x$ e $y$ tal que las derivadas parciales de segundo orden de son continuas en $D$. Entonces: 

# $\frac{\delta² f}{\delta x \delta y}(x,y)=\frac{\delta² f}{\delta y \delta x}(x,y)$ ; $(x,y)\in{D}$ 

### Ejemplo: 

### Sea $f(x,y)=x³+x²y²-2y²$, calcule $\frac{\delta² f}{\delta x\delta y}$ y $\frac{\delta² f}{\delta y \delta x}$ 
# Ejercicio Propuesto: 

### Pruebe que la función $f(x,y)=cos(x^2+y²)$ satisface la ecuación:

# $y\frac{\delta² z}{\delta x²}-x\frac{\delta² z}{\delta y \delta x}-\frac{\delta z}{\delta y}=0$ 


# *Plano Tangente a la gráfica de una función de dos variables* 

Sea $z=f(x,y)$ una función de dos variables y $P_0(x_0,y_0,z_0)$ un punto de la grafica de $f(f(x_0,y_0)=z_0),(x_0,y_0)\in{dom(f)}$ 

SI existe el plano tangente a la grafica de $f$ (que es una superficie en $R³$), en el punto $P_0$, entonces su ecuación, esta dada por:

### $P_t: z-z_0=\frac{\delta f}{\delta x}(x_0,y_0)(x-x_0)+\frac{\delta f}{\delta y}(x_0,y_0)(y-y_0)$ 
### <-> $\frac{\delta f}{\delta x}(x_0,y_0)(x-x_0)+\frac{\delta f}{\delta y}(x_0,y_0)(y-y_0)-(z-z_0)=0$ 

### obs: El vector normal a este plano es $(\frac{\delta f}{\delta x}(x_0,y_0),\frac{\delta f}{\delta y}(x_0,y_0),-1)$ 

# Interpretación Grafica: 
### *insertar dibujo rossel lol


# *Ejercicio*: 

Sea $f(x,y)=3x²y+2xy²$ determine la ecuación del plano tangente a la  superficie $S:z=f(x,y)$, en el punto $P_0(1,1,5)$.

SOlUCIÓN: $dom(f)=R²$ ; $f(1,1)=5$ 

$\Rightarrow{P_0(1,1,5)}\in{gra(f)}$ 

$\Rightarrow\frac{\delta f}{\delta y}=3x²+4xy$ y $\frac{\delta f}{\delta x}=6xy + 2y²$ 

$\Rightarrow{\frac{\delta f}{\delta x}(1,1)}=8$ y $\Rightarrow{\frac{\delta f}{\delta y}(1,1)}=7$ 

Entonces, la ecuación del plano tangenete a $S$ en $P_0$ es: 

# $P_T:8(x-1)+7(y-1)-(z-5)=0$ 


# *Ejercicio*: 
Determine los puntos en el paraboloide $z=4x²+y^2=f(x,y)$, en los cuales el plano tangente es paralelo al plano $\Pi$: $x+2y+z=6$ 

$\Rightarrow{\frac{\delta z}{\delta x}}=8x$ y $\frac{\delta f}{\delta y}=2y$ 
$\Rightarrow{(8x,2y,-1)}$ es un vector normal al paraboloide
$\Rightarrow{(1,2,1)}=\alpha(8x,2y,-1)$ ; $\alpha\in{R}$ ; dado $P_1=(1,2,1)$ es un vector normal al plano $\Pi$ y 
$(1,2,1)\parallel{(8x,2y,-1)}$  (son paralelos)

$\Rightarrow{\alpha}=-1; y_0=-1,x_0=-\frac{1}{8}$ 

Sea $y=f(x)$ una función derivable. La diferencial de $y=f(x)$ esta dada por: 
# $\frac{dy}{dx}=f'(x)\Rightarrow{dy}=f'(x)dx$ 

donde $\Delta y=f(x_0+\Delta_x)-f(x_0)\approx{dy}$ 
$\Rightarrow{f(x_0+\Delta_x)}\approx{f(x_0)+dy}$ 

# Diferencial Total

Para funciones de dos variables $z=f(x,y)$, se usa una terminología similar al caso de una función de una sola variable. Esto es, si $\Delta x$ y $\Delta y$ son los incrementos de $x$ y de $y$, el incremento de $z$, esto es $\Delta z$ esta dado por:

# $\Delta z=f(x+\Delta x,y+\Delta y)-f(x,y)$ 

si $z=f(x,y)$ es una función de las variables $x$ e $y$, $\Delta z$ y $\Delta y$ son los incrementos de $x$ y de $y$, entonces la diferencial total de la variable dependiente $z$, es: 

# $dz=\frac{\delta f}{\delta x}dx+\frac{\delta f}{\delta y}dy$ 

Para funciones de tres variables, $w=f(x,y,z)$ y $\Delta x$, $\Delta y$ y $\Delta z$ son los incrementos de $x$,$y$ y $z$ respectivamente, se tiene: 

# $dw=\frac{\delta f}{\delta x}dx+\frac{\delta f}{\delta y}dy+\frac{\delta f}{\delta z}dz$ 

# Calculos aproximados:
- Si $z=f(x,y)$ es una función diferenciable, la diferencial de $z$, se puede usar, como aproximación para el incremento de $z$, es decir :

# $\Delta z\approx{dz}$

$\Rightarrow{f(x+\Delta x,y+\Delta y)}-f(x,y)\approx{dz}$ 
$\Rightarrow{f(x+\Delta x,y+\Delta y)\approx{f(x,y)+dz}}$ 

para el caso de $w=f(x,y,z)$ se tendra: 

# $f(x+\Delta x, y+\Delta y, z+\Delta z)\approx{f(x,y,z)+dw}\approx f(x,y,z)+\nabla f(x,y,z)\cdot(\Delta x, \Delta y, \Delta z)$  

# *Ejercicio:*

Estimar el valor de $\sqrt{(2.10)²+(1.98)²+(1.05)²}$ 

Sea $w=f(x,y,z)=\sqrt{x^2+y²+z^2}$ ; $x_0=2, y_0=2,z_0=1$ $\Rightarrow \Delta x=0.1;\Delta y=-0.02;\Delta z=0.05$ 
$\Rightarrow{f_x}=\frac{x}{\sqrt{x²+y²+z²}}$ ; $f_y=\frac{y}{\sqrt{x²+y^2+z²}}$ ; $f_z=\frac{z}{\sqrt{x^2+y²+z²}}$ 
$\Rightarrow{f_x(2,2,1)}=\frac{2}{\sqrt{5}}$ ; $f_y(2,2,1)=\frac{2}{\sqrt{5}}$ ; $f_z(2,2,1)=\frac{1}{\sqrt{5}}$
$\Rightarrow \Delta w \approx\frac{2}{\sqrt{5}}0.1+\frac{2}{\sqrt{5}}(-0.02)+\frac{1}{\sqrt{5}}0.05$ 

# Ejercicios Certamen 1(hacer control 1)

### 1. Considere la curva definida por $\vec{r}(t)=(e^{-t}cos(t),e^{-t}sin(t),e^{-t})$ ; $t\in{[0,2\pi]}$ 

a) Demuestre que la esta contenida en el caso de ecuación $x^{2}+y^{2}=z²$ 
b) Calcule el triedio $\vec{T},\vec{N},\vec{B}$ 

### 2. La posición de una cierta particula en el plano esta dada por $\vec{r}(t)=(cos(t²),sin(t²)) [cm]$ 

Determine para $t=\frac{\sqrt{\pi}}{2}[s]$, las componentes escalares tangencial y normal de la aceleración.

### 3. 
a) Dibuje las curvas de nivel $z=k$ para las siguientes funciones, para los valores especificados de $k$:
- $z=x²+y²;k=0,1,2,3$
- $z=\frac{y}{x};k=-2,-1,0,1$ 

b) Dibuje e identifique las trazas en los planos coordenados de la superficie $x²+\frac{y²}{4}=\frac{z}{5}$ 


### 4. Verificar si la función $u(x,t)=sin(Cwt)\cdot{sin(wx)}$;$C\in{R}$  satisface la ecuación de la onda: 

#### $\frac{\delta² u}{\delta t²}=C²\frac{\delta²u}{\delta x²}$ 

# Gradiente: 

### Definición: 
Sea $f:A\subseteq{R^n}\rightarrow{R}$ ; $P\in{A}$ ; A conjunto abierto de $R^n$ . El vector gradiente de $f$ en $P$ , que detonamos $\nabla f(P)$, se define como: 

$\nabla f(P)=(\frac{\delta f}{\delta x_1}(P),\frac{\delta f}{\delta x_2}(P),...,\frac{\delta f}{\delta x_n})$ , Siempre que $\frac{\delta f}{\delta x_i}(p)$ existan, $\forall{i}=1,...,n$ 
característica
Ejemplo: Sea $f(x,y,z)=3x³y²z$ , $dom(f)=R³$ Calcule $\nabla f(1,2,3)$ 

SOlución: 

tenemos $\nabla f(x,y,z)=(9x²y²z,6x³yz,3x³y²)$ 

$\Rightarrow{\nabla f(1,2,3)}=\nabla f_{x=1,y=2,z=3}=(108,36,12)=12(9,3,1)$ 

### Propiedades

Sean $f$ y $g$ funciones de $n$ variables a valores en $R$, tal que $\frac{\delta f}{\delta x_i}$ y $\frac{\delta g}{\delta x_i}$ existen $\forall{i}=1,...,n$: 

- $\nabla (f\cdot{g})=f\nabla g + g\nabla f$ 
- $\nabla(\frac{f}{g})=\frac{g\nabla f-f\nabla g}{g²}$ 

### Interpretación Geométrica

Ejemplo: Sea $f(x,y)=x²+y²$ ; $dom(f)=R²$ ; $\nabla f(x,y)=(\frac{\delta f}{\delta x}(x,y),\frac{\delta f}{\delta y}(x,y))=(2x,2y)$ 

entonces $\nabla f(1,1)=(2,2)$ 

insertar imagen ola

Note que: $\nabla f(1,1)$ es un vector ortogonal a la curva de nivel de $f$ que pasa por el punto $(1,1)$ y posicionado en ese punto. 

En general, si $f$ es una función de $n$ variables a valores en $R$, el vector $\nabla f(x_1,x_2,...,x_n)$, es un vector ortogonal al conjunto de nivel de $f$ (o hipersuperficie de nivel de $f$) que pasa por el punto $P(x_1,x_2,...,x_n)\in{dom(f)}$ 

# Plano tangente a una superficie de nivel

Suponga que $S$ es una superficie con ecuación $F(x,y,z)=k$ ; $k\in{rec(f)}$ ; $k$ constante, donde $F$ es una función diferenciable. Suponga que $P(x_0,y_0,z_0)\in{S}$, esto es $F(x_0,y_0,z_0)=k$, si $\nabla F(x_0,y_0,z_0)\not=\vec{0}$, entonces el plano tangente a la superficie $S$ en $P$, tiene por ecuacion:

$\frac{\delta F}{\delta x}(x_0,y_0,z_0)(x-x_0)+\frac{\delta F}{\delta y}(x_0,y_0,z_0)(y-y_0)+\frac{\delta F }{\delta z}(x_0,y_0,z_0)(z-z_0)=0$ 

tambien se puede expresar como:

$\nabla F(x_0,y_0,z_0)\cdot (x-x_0,y-y_0,z-z_0)=0$

Recuerdo: $S$: $z=f(x,y)$ ; $(x,y)\in{dom(f)}$ , donde se mira a $S$ como la grafica de la fucnión $z=f(x,y)$ 

$\Rightarrow{F(x,y,z)}=f(x,y)-z=0$ 

Tambien podemos mirar la superficie $S$ como la superficie de nivel $0$ de la función $F(x,y,z)=f(x,y)-z$ 

Entonces una ecuación de un plano tangente a $S$ en el punto $(x_0,y_0,f(x_0,y_0))$ 

$\frac{\delta f}{\delta x}(x_0,y_0)(x-x_0)+\frac{\delta f}{\delta y}(x_0,y_0)(y-y_0)-(z-z_0)=0$ 

Además, la recta normal a la superficie $S$ en el punto $P(x_0,y_0,z_0)$, tiene como vector director $\nabla F(x_0,y_0,z_0)$. Por lo tanto las ecuaciones parametricas de la ==recta normal== a la superficie $S$ en el punto $P(x_0,y_0,z_0)$ son: 

$R_N$ : $x(t)=x_0+t\frac{\delta F}{\delta x}(x_0,y_0,z_0)$ ; $y(t)=y_0+t\frac{\delta F}{\delta y}(x_0,y_0,z_0)$ ; $z(t)=z_0+t\frac{\delta F}{\delta z}(x_0,y_0,z_0)$ 

Notación: $F_{p_0}$ es equivalente a decir "$F$ evaluado en en punto $p_0$"
### Ejemplo:

Encuentre la ecuación del plano tangente a la superficie de ecuación:

$S$ : $sin(xy)+sin(yz)+sin(xz)=1$ en el punto $P_0(1,\frac{\pi}{2},0)$. 

Además determine un conjunto de ecuaciónes parametricas de la ecuación de la recta normal a la superficie $S$ en $P_0$ 

Solución: Note que la superficie $S$, puede ser mirada como la superficie de nivel $0$ de la función: 

$F(x,y,z)=sin(xy)+sin(yz)+sin(xz)-1$ 

Así la ecuación del plano tangente a $S$ en el punto $P_0(1,\frac{\pi}{2},0)$ es: 

$\nabla F(1,\frac{\pi}{2},0)(x-1,y-\frac{\pi}{2},z)=0$ 

como: 

$\frac{\delta F}{\delta x}|_{p_0}=(ycos(xy)+zcos(xz)) _{P_0}=0$ 

$\frac{\delta F}{\delta y}|_{P_0}=(xcos(xy)+zcos(yz)) _{P_0}=0$ 

$\frac{\delta F }{\delta z}|_{P_0}=(ycos(yz)+xcos(xz)) _{P_0}=\frac{\pi}{2}+1$ 

Entonces la ecuación del plano tangente a $S$ en el punto $P_0$ es: 

$(0,0,\frac{\pi}{2}+1)(x-1,y-\frac{\pi}{2},z)=0$ <-> $z=0$ 

Además un conjunto de ecuaciones de parametrcias para la recta normal a la superficie $S$ en el punto $(1,\frac{\pi}{2},0)$ es:


$R_N$ : $x=1 ; y=\frac{\pi}{2}; z = (\frac{\pi}{2}+1)t$ ; $t\in{R}$ 

# Diferencibilidad 

Teorema: Sea $z=f(x,y)$ una funición de las variables $x$ e $y$. Sea $(x_0,y_0)\in{dom(f)}$. 
Si las derivadas parciales $\frac{\delta f}{\delta x}$ y $\frac{\delta f}{\delta y}$ existen en una vecindad (abierta) de $(x_0,y_0)$ y son continuas en $(x_0,y_0)$, entonces $f$ es diferenciable en $(x_0,y_0)$. 

# Regla de la cadena

- $(I)$ Sea $z=f(x,y)$ una función diferenciable. Si $x=f(t)$ y $y=g(t)$, son funciones derivables de $t$, entonces $z$ también es una función derivable de $t$, y: 
$$\frac{dz}{dt}=\frac{\delta z}{\delta x}\frac{dx}{dt}+\frac{\delta z}{\delta y}\frac{dy}{dt}$$

- $(II)$ Sea $z=f(x,y)$ una función diferenciable de las varibales $x$ e $y$. Si $x=g(s,t)$ e $y=h(s,t)$, son funciones diferenciables tales que $\frac{\delta x}{\delta s}, \frac{\delta x}{\delta t}$ y $\frac{\delta y}{\delta s},\frac{\delta y}{\delta t}$ existen, entonces $\frac{\delta z}{\delta s}$ y $\frac{\delta z}{\delta t}$ tambien existen, y ademas (Verificar esto en clases de rossel): 
$$\frac{\delta z}{\delta s}=\frac{\delta z}{\delta x}\frac{\delta x}{\delta s}+\frac{\delta z}{\delta y}\frac{\delta y}{\delta s}$$
$$\frac{\delta z}{\delta t}=\frac{\delta z}{\delta x}\frac{\delta x}{\delta t}+\frac{\delta z}{\delta y}\frac{\delta y}{\delta t}$$ En general: 

Si $w=f(x_1,...,x_n)$ y $x_i=g(t_1,t_2,...,t_n)$ con $i=1,...,n$, entonces: 

$$\frac{\delta w}{\delta t_1}=\frac{\delta w}{\delta x_1}\frac{\delta x_1}{\delta t_1}+\frac{\delta w}{\delta x_2}\frac{\delta x_2}{\delta t_1}+...+\frac{\delta w}{\delta x_n}\frac{\delta x_n}{\delta t_1}$$ entonces : 
$$\frac{\delta w}{\delta t_m}=\frac{\delta w}{\delta x_1}\frac{\delta x_1}{\delta t_m}+\frac{\delta w}{\delta x_2}\frac{\delta x_2}{\delta t_m}+...+\frac{\delta w}{\delta x_n}\frac{\delta x_n}{\delta t_m}$$
Entonces se forma una matriz (de m filas y n columnas): 

$$\Rightarrow \begin{pmatrix}   \frac{\delta x_1}{\delta t_1} & \frac{\delta x_2}{\delta t_1} & ... & \frac{\delta x_n}{\delta t_1}\\  .  & . & . & .\\ \frac{\delta x_1}{\delta t_m} & \frac{\delta x_2}{\delta t_m} & ... & \frac{\delta x_n}{\delta t_m}  \end{pmatrix} \begin{pmatrix}  \frac{\delta w}{\delta x_1} \\ \frac{\delta w}{\delta x_2} \\ ... \\ \frac{\delta 2}{\delta x_n}   \end{pmatrix} = \begin{pmatrix} \frac{\delta w}{\delta t_1}  \\ \frac{\delta w}{\delta t_2} \\ ... \\ \frac{\delta w}{\delta t_m}  \end{pmatrix}$$

### Ejercicio: Sea $w=f(x,y)$ una función que admite derivadas parciales de 2do orden continuas. Suponga que $x=u+v$ , $y=u-v$.Demuestre que: 
$$\frac{\delta² w}{\delta u \delta v}=\frac{\delta² w}{\delta x²}-\frac{\delta² w}{\delta y²}$$  Respuesta: 

$w=w(x(u,v),y(u,v))$ ; $x=u+v$ y $y=u-v$ 
$\frac{\delta² w}{\delta u \delta v}=\frac{\delta² w}{\delta x²}-\frac{\delta² w}{\delta y²}$ 

primero, $\frac{\delta w}{\delta v}=\frac{\delta w}{\delta x}\frac{\delta x}{\delta v}+\frac{\delta w}{\delta y}\frac{\delta y}{\delta v}=\frac{\delta w}{\delta x}-\frac{\delta w}{\delta y}$ 
$\Rightarrow =\frac{\delta² w}{\delta u \delta v}=\frac{\delta}{\delta u}(\frac{\delta w}{\delta v})=\frac{\delta }{\delta u}(\frac{\delta w}{\delta x}-\frac{\delta w}{\delta y})$ 
Pero: 
$\frac{\delta w}{\delta x}=\frac{\delta w}{\delta x}(x(u,v),y,(u,v))$ 
analogamente: 
$\frac{\delta w}{\delta y}=\frac{\delta w}{\delta y}(x(u,v),y(u,v))$ 
photo

Luego: 

(1) $\frac{\delta}{\delta u}(\frac{\delta w}{\delta x})=\frac{\delta² w}{\delta x²}\frac{\delta x}{\delta u}+\frac{\delta² w}{\delta y \delta x}\frac{\delta y}{\delta u}=\frac{\delta² w}{\delta x²}\frac{\delta² w}{\delta y \delta x}$ 

(2) $\frac{\delta}{\delta u}(\frac{\delta w}{\delta y})=\frac{\delta² w}{\delta x \delta y}\frac{\delta x}{\delta u}+\frac{\delta² w}{\delta y²}\frac{\delta y}{\delta u}=\frac{\delta² w}{\delta x \delta y}+\frac{\delta² w}{\delta y²}$ 

entonces, (1)-(2) = $\frac{\delta^2 w}{\delta x²}+\frac{\delta² w}{\delta y \delta x}-\frac{\delta² w}{\delta x \delta y}-\frac{\delta² w}{\delta y²}=\frac{\delta² w}{\delta x²}-\frac{\delta² w}{\delta y²}$ 

# Derivación implicita

### $I)$ Suponga que $y$ esta dada de forma implicita por la relacuón $F(x,y)=0$, como función diferenciable de las variables $x$ (se supone que $y=f(x)$). Entonces: 

$\frac{dy}{dx}=-\frac{\frac{\delta F}{\delta x}}{\frac{\delta F}{\delta y}}; \frac{\delta F}{\delta y}\not=0$ 

#### Demostración :  $F(x,y)=0$ 

$\Rightarrow dF=\frac{\delta F}{\delta x}dx+\frac{\delta F}{\delta y}dy=0$ 
Se supone que $y=f(x)$, entonces: 

$\frac{dy}{dx}=f'(x)\Rightarrow dy=f'(x)dx$ 

$\Rightarrow \frac{\delta F}{\delta x}dx+\frac{\delta F}{\delta y}(\frac{dy}{dx}dx)=0$ 
$\Rightarrow \frac{\delta F}{\delta x}dx+\frac{\delta F}{\delta y}(\frac{dy}{dx})dx=0$ 
$\Rightarrow \frac{\delta F }{\delta x}+\frac{\delta F}{\delta y}\frac{dy}{dx})dx=0$ 
$\Rightarrow \frac{\delta F}{\delta x}+\frac{\delta F}{\delta y}\frac{dy}{dx}=0 \Rightarrow \frac{dy}{dx}=-\frac{\frac{\delta F}{\delta x}}{\frac{\delta F}{\delta y}}; \frac{\delta F}{\delta y}\not=0$ 


### $II)$ Suponga que $z$ esta dada en forma implicita, por la relación $F(x,y,z)=0$ como función diferenciable de $x$ e $y$, (se supone que $z=f(x,y)$). Entonces: 

$$\frac{\delta z}{\delta x}=-\frac{\frac{\delta F}{\delta x}}{\frac{\delta F}{\delta z}}$$ $$\frac{\delta z}{\delta y}=-\frac{\frac{\delta F}{\delta y}}{\frac{\delta F}{\delta z}}$$

### Ejercicio: Sea $z=z(x,y)$ una función de $x$ e $y$, definida implicitamente por la ecuación: 

$$z²+\frac{2}{x}=\sqrt{y^2-z²}$$
Demuestre la igualdad siguiente: 

$$x²\frac{\delta z}{\delta x}+\frac{1}{y}\frac{\delta z}{\delta y}=\frac{1}{z}$$

## Control miercoles
- aproximación lineal
- plano tangente (a una función de dos variables o superficie de nivel) (recta normal)


# Clase 01/10 

# Derivada direccional 

Definición: Sea $z=f(x,y)$ una función ; $(x_0,y_0)\in{dom(f)}$. Sea $\vec{u}=(a,b)$ un vector unitario. La derivada direccional de $f$ en $(x_0,y_0)$ en la dirección del vector unitario $\vec{u}$, se define como: 

$$\lim_{h\to{0}} \frac{f(x_0+ha,y_0+hb)-f(x_0,y_0)}{h}$$
desde que este limite exista.

Notación: 
$$\frac{\delta f}{\delta \vec{u}}(x_0,y_0)=\lim_{t\to{0}} \frac{f(x_0+ta,y_0+tb)-f(x_0,y_0)}{t}=D_{\vec{u}}f(x_0,y_0)$$

GRAFICA ROSSEL INSERTAR 

La derivada direccional $\frac{\delta f}{\delta \vec{u}}(x_0,y_0)$es la razón de cambio de $z$, cuando $(x,y)$ se mueve desde el punto $(x_0,y_0)$ en la dirección del vector unitario $\vec{u}$ 

#### Observación: 
- La derivada direccional $\frac{\delta f}{\delta \vec{u}}(x_0,y_0)$, se denomina tambien "tasa de variación" de $f$ en el punto $(x_0,y_0)$.
-  Las derivadas parciales de $f$ en $(x_0,y_0)$, son casos particulares de derivadas direccionales. Esto es:
$$\frac{\delta f}{\delta \vec{i}}(x_0,y_0)=\lim_{t\to{0}} \frac{f(x_0+t,y_0)-f(x_0,y_0)}{t}=\frac{\delta f}{\delta x}(x_0,y_0)$$
$$\frac{\delta f}{\delta \vec{j}}(x_0,y_0)=\lim_{t\to{0}} \frac{f(x_0,y_0+t)-f(x_0,y_0)}{t}=\frac{\delta f}{\delta y}(x_0,y_0)$$
- Si $\frac{\delta f}{\delta \vec{u}}(x_0,y_0)<0$ , entonces la función $f$ es localmente decreciente desde el punto $(x_0,y_0)$, en la dirección del vector unitario $\vec{u}$ 
- Si $\frac{\delta f}{\delta \vec{u}}(x_0,y_0)>0$, entonces la fucnión $f$ es localmente creciente, desde el punto (x_0,y_0)$ en la dirección del vector unitario $\vec{u}$. 

### Teorema: 

Sea $f:A\subseteq{R²}\to{R}$ una función, donde $A$ es un conjunto abierto, ($x_0,y_0)\in{A};\vec{u}=(a,b)$ unitario.

a) Si $f$ es diferenciable en $(x_0,y_0)$, entonces:
- $f$ admite derivada direccional en $(x_0,y_0)$, en la dirección de $\vec{u}$ ; y además: 
$$\frac{\delta f}{\delta \vec{u}}(x_0,y_0)=\nabla f(x_0,y_0)\cdot{\vec{u}}$$

b) si $f$ es diferenciable en $(x_0,y_0)$ y además $\nabla f(x_0,y_0)\not=\vec{0}$, entonces, el valor máximo de $\frac{\delta f}{\delta \vec{u}}(x_0,y_0)$, ocurre cuando $\vec{u}=\frac{\nabla f(x_0,y_0)}{||\nabla f(x_0,y_0)||}$, y el valor máximo de $\frac{\delta f}{\delta \vec{u}}(x_0,y_0)$ es $||\nabla f(x_0,y_0)||$, de hecho:

$$|\frac{\delta f}{\delta \vec{u}}(x_0,y_0)|=|\nabla f(x_0,y_0)\cdot{\vec{u}}|\leq ||\nabla f(x_0,y_0||\cdot ||\vec{u}||$$
$\Rightarrow |\frac{\delta f}{\delta \vec{u}}(x_0,y_0)| \leq ||\nabla f(x_0,y_0)||$
$\Rightarrow -||\nabla f(x_0,y_0)|| \leq \frac{\delta f}{\delta \vec{u}}(x_0,y_0)\leq ||\nabla f(x_0,y_0)||$ (valores minimos y maximos de la derivada direccional de $f$)



#### ¿Cuando ocurre el valor máximo? 

Respuesta: Cuando $\vec{u}=\frac{\nabla f(x_0,y_0)}{||\nabla f(x_0,y_0)||}$ 

analogamente: 

$\frac{\delta f}{\delta \vec{u}}(x_0,y_0)=\nabla f(x_0,y_0)\frac{\nabla f(x_0,y_0)}{||\nabla f(x_0,y_0)||}$ 
$=\frac{1}{||\nabla f(x_0,y_0)||}(\nabla f(x_0,y_0)\nabla f(x_0,y_0))=||\nabla f(x_0,y_0)||$

entonces, como formula, el valor máximo de la derivada direccional $\frac{\partial f}{\partial \vec{u}}$ ocurre cuando: 
$$\frac{\partial f}{\partial \vec{u}}=||\nabla f(x_0,y_0)||$$

Esto es, $\frac{\delta f}{\delta \vec{u}}(x_0,y_0)$, asume su valor máximo cuando $\vec{u}$ tiene la dirección y sentido de el gradiente de $f$ ($\nabla f(x_0,y_0)$)

#### ¿Cuando ocurre el valor mínimo? 

Respuesta: Cuando $\vec{u}=-\frac{\nabla f(x_0,y_0)}{||\nabla f(x_0,y_0)||}$ 

analogamente: 

$\frac{\delta f}{\delta \vec{u}}(x_0,y_0)=-\nabla f(x_0,y_0)\frac{\nabla f(x_0,y_0)}{||\nabla f(x_0,y_0)||}$ 
$=-\frac{1}{||\nabla f(x_0,y_0)||}(\nabla f(x_0,y_0)\nabla f(x_0,y_0))=-||\nabla f(x_0,y_0)||$ 

entonces como formula, el valor mínimo de la derivada direccional $\frac{\partial f}{\partial \vec{u}}$ ocurre cuando: 
$$\frac{\partial f}{\partial \vec{u}}(x_0,y_0)=-||\nabla f(x_0,y_0)||$$
#### Ejercicio: Sea $V(x,y)=e^{-2x}cos(2y)$, donde $V$ indica el potencial electrico en un punto $(x,y)$ 

a) Encontrar la rapidez de cambio del potencial en el punto $(0,\frac{\pi}{4})$, en la dirección del vector unitario $\vec{u}=(cos(\frac{\pi}{6}),sin(\frac{\pi}{6}))$ 
b) Encontrar la dirección y magnitud de la máxima rapidez de cambio de $V$ en $(0,\frac{\pi}{4})$.

#### Respuesta:

a) $\frac{\delta V}{\delta \vec{u}}(0,\frac{\pi}{4})=\nabla V(0,\frac{\pi}{4})\vec{u}$ 

$\Rightarrow \nabla V(x,y)=(-2e^{-2x}cos(2y),-2e^{-2x}sin(2y))$ 

$\Rightarrow \nabla V(0,\frac{\pi}{4})=(0,-2)=-2ĵ$ 

luego, $\frac{\delta V}{\delta \vec{u}}(0,\frac{\pi}{4})=(0,-2)\cdot{(cos(\frac{\pi}{6}),sin(\frac{\pi}{6}))}=-1$ 

b) $||\nabla V(0,\frac{\pi}{4})||=||-2ĵ||=\sqrt{4}=2$ 
donde la dirección es $-ĵ=(0,-1,0)$ 



# Máximos y Mínimos.

### Puntos críticos:

Definición: Sea $f:U\subseteq{R^n}\to{R}$ una función ; $U$ conjunto abierto de $R^n$; $a\in{U}$. 

$a\in{U}$ se dice punto crítico de $f$, si y solamente si se verifica una de las siguientes afirmaciones: 

- $\frac{\delta f}{\delta x_i}(a)=0$ ; $\forall{i}=1,...,n$ ($ie, \nabla f(a)=\vec{0}$ )
- $\frac{\delta f}{\delta x_1}(a)$ o $\frac{\delta f}{\delta x_2}(a)$ o ... o $\frac{\delta f}{\delta x_n}(a)$ no existe

#### Ejemplo: Considere la función $f(x,y)=\frac{3x²+1}{2}-x(x²+y^2)$ , determine los puntos críticos de $f$. 
#### Solución: 

$\nabla f(x,y)=(3x-3x²-y²,-2xy)$ 

Tenemos : $3x-x²-y^2=0$ y $-2xy=0$ 

luego $x=0$ o $y=0$, entonces, si $x=0$:

$\Rightarrow -y²=0 \Rightarrow y=0$, entonces se obtiene el punto $(0,0)$ 

Si $y=0\Rightarrow x-x²=0\Rightarrow x=0$ o $x=1$ (Se obtienen los puntos (0,0) o (1,0))

Luego, los puntos criticos de $f$ son:

$(0,0)$ y $(1,0)$ 

# Matriz hessiana 

Sea $f:U\subseteq{R^n}\rightarrow{R}$ una función; $U$ conjunto abierto de $R^n$ ; $P\in{U}$. 
Supongamos que todas las derivadas parciales de segundo orden de $f$ existen en $P$. 
La matriz de orden $n\times n$, que denotamos po $H(P)=(a_{ij})$ ; $i,j=1,2,...,n$,
donde $a_{ij}=\frac{\delta²f}{\delta x_i \delta y_j}(P)$ se llama la matriz Hessiana de $f$ en $P$. 

### Casos particulares 

- SI $n=2$ ; $f:U\subseteq{R^2}\rightarrow R$ ; $P_0(x_0,y_0)\in U$ 
La matriz esta dada por

$$H(x_0,y_0)=\begin{pmatrix}   \frac{\delta²f}{\delta x²}(x_0,y_0)  & \frac{\delta² f}{\delta y \delta x}(x_0,y_0)\\   \frac{\delta²f}{\delta x \delta y}(x_0,y_0)  & \frac{\delta²f}{\delta y²}(x_0,y_0)  \end{pmatrix}=H(x_0,y_0)=\begin{pmatrix}   f_{xx}(x_0,y_0)  & f_{xy}(x_0,y_0)\\   f_{yx}(x_0,y_0)  & f_{yy}(x_0,y_0)  \end{pmatrix}$$

- Si $n=3$ 
$$H(x_0,y_0)=\begin{pmatrix} \frac{\delta²f}{\delta x²}(x_0,y_0) & \frac{\delta²f}{\delta y \delta x}(x_0,y_0)  & \frac{\delta² f}{\delta z \delta x}(x_0,y_0)\\   \frac{\delta²f}{\delta x \delta y}(x_0,y_0)  & \frac{\delta²f}{\delta y²}(x_0,y_0) & \frac{\delta²f}{\delta z \delta y}(x_0,y_0) \\ \frac{\delta²f}{\delta x \delta z}(x_0,y_0) & \frac{\delta²f}{\delta y \delta z}(x_0,y_0) & \frac{\delta²f}{\delta z²}(x_0,y_0) \end{pmatrix}  $$

### Definición: 

$$A_n=\begin{pmatrix}   a_{11} & a_{12} & ...&a_{1n}\\   a_{21} & a_{22} &...& a_{2n} \\.. .\\ ...\\ a_{n1} & a_{n2} & ... & a_{nn}  \end{pmatrix}$$
Se definen las siguientes submatrices $A_k$ de $A_n$:

$$A_1=a_{11};A_2=\begin{pmatrix}   a_{11} & a_{12} \\   a_{21} & a_{22}    \end{pmatrix};A_n=\begin{pmatrix}   a_{11} & a_{12} & ...&a_{1n}\\   a_{21} & a_{22} &...& a_{2n} \\.. .\\ ...\\ a_{n1} & a_{n2} & ... & a_{nn}  \end{pmatrix}$$
# Teorema (condición suficiente para la existencia de extremos locales )

Sea $f:U\subseteq{R^n}\rightarrow R$ una función. Sea $P$ un punto critico de $f$. Suponga que además las derivadas parciales de 2do orden de $f$ son continuas en una vecindad de $P$. 


### i) Si todas las submatrices de $A_k$ de la matriz Hessiana $H(P)$, definidas en "definición anterior" tienen determinante positivo, entonces $f$ tiene un minimo local en $P$ 

### ii) Si todas las submatrices $A_k$ de la matriz Hessiana $H(P)$, tienen determinante de signos alternados, comenzando con $|A_1| <0$, entonces $f$ alcanza (o tiene) un máximo local en $P$. 

### iii) Si el determinante de las submatrizes no cumplen ninguno de los criterios anteriores, se dice a $P$ un "punto de silla de $f$ "

### iv) Si uno de los determinantes es nulo ($det(A_k)=0$), el criterio no asegura nada
### Caso particular (para $n=2$ )
Sea $f:U\subseteq R^n\rightarrow R$ una función y $P(x_0,y_0)$ un punto crítico de $f$. Suponga que además que $f$ admite derivadas parciales de 2do orden continuas en una vecindad de $P(x_0,y_0)$, entonces: 


#### i) Si $\frac{\delta^2 f}{\delta x^2}(x_0,y_0)>0$ y $det(H(x_0,y_0))>0$, entonces $f$ tiene un minimo local en $P(x_0,y_0)$ 
#### ii) Si $\frac{\delta^2 f}{\delta x²}(x_0,y_0)<0$ y $det(H(x_0,y_0))>0$, entonces $f$ tiene (o alcanza) un máximo local en $P(x_0,y_0)$ 
#### iii) Si $det(H(x_0,y_0))<0$, entonces $P(x_0,y_0)$ es un punto de silla de $f$ 
#### iv) Si $det(H(x_0,y_0))=0$, el criterio no entrega info 

#### Nota: De acuerdo a enunciado, tenemos: 

$$det(H(x_0,y_0))=\frac{\delta²f}{\delta x²}(x_0,y_0)\frac{\delta²f}{\delta y²}(x_0,y_0) - (\frac{\delta²f}{\delta x \delta y}(x_0,y_0))²$$
Dado que, como $f$ admite derivadas parciales de segundo orden continuas en una vecindad de $P(x_0,y_0)$, la matriz $H(x_0,y_0)$, resulta ser simetrica. 

### Ejercicio: 
Sea $f(x,y)=x³+y³-3x-3y+4$. Clasifique los puntos críticos de $f$. 

tenemos que, $\frac{\delta f}{\delta x}=3x²-3=0$ y $\frac{\delta f}{\delta y}=3y²-3=0$ $\Rightarrow x=+-1$ y $y=+-1$
Entonces, los puntos criticos de $f$ son:

$$P_1(1,1);P_2(1,-1);P_3(-1,1);P_4(-1,-1)$$
Además: 
$$H(x,y)=\begin{pmatrix}   \frac{\delta²f}{\delta x²}  & \frac{\delta² f}{\delta y \delta x}\\   \frac{\delta²f}{\delta x \delta y}  & \frac{\delta²f}{\delta y²}  \end{pmatrix}=\begin{pmatrix} 6x & 0 \\ 0 & 6y  \end{pmatrix}$$
entonces, $det(H(x,y))=36xy$

luego, note que $P_2$ y $P_3$ son puntos de silla, ya que:

$det(H(P_2))=0$ y $det(H(P_3))<0$ 

Luego para, $P_1(1,1)$ :
$\frac{\delta² f}{\delta x²}(1,1)=6$ , $det(H(1,1))=36>0$, entonces, es un mínimo local de $f$ 

NOTA: Note que $P_1(1,1)$ no es un mínimo global de $f$, ya que la $f(-3,0)=-14<0=f(1,1)$ 

Luego, para $P_4(-1,-1)$ : 
$\frac{\delta² f}{\delta x²}(-1,-1)=-6<0$  y $det(H(-1,-1))=36>0$ 

por lo tanto, el punto $P_4(-1,-1)$ es un máximo local de $f$. 

Note que $P_4(-1,-1)$ no es un máximo global de $f$, ya que: 

$f(4,0)=56>8=f(-1,-1)$ 

### Ejercicio:
Encuentre y clasifique los puntos críticos (estacionarios) de la función: 

$$f(x,y,z)=x³-3x^2-4y²-2z²+4yz+z+2$$

# Maxímos y mínimos Globales

Sea $f$:$D\subseteq{R^n}\to R$ una función ; $P_0\in dom(f)=D$ 

i) $f$ tiene un máximo absoluto (o global) en $P_0$, si:
$$f(P_0)\geq f(x);\forall x\in D$$
ii) $f$ tiene un minimo absoluto (o global ) en $P_0\in dom(f)$ si:
$$f(P_0)\leq {f(x);\forall x\in D}$$

# Conjuntos compactos

Definición: $A\subseteq{R^n}$, se dice compacta si y solo si $A$ es un conjunto cerrado y acotado. 

### Ejemplo: 

1. En $R$ al intervalo $[a,b]$ ; $a<b$ es un conjunto compacto.

2. El conjunto $A$={$(x,y)\in{R²}/x²+y²\leq{1}$} es un conjunto compacto.


### Teorema (De Weirstrass)

Sea $f:A\subseteq{R^n}\to{R}$ una función continua en $A$; $A$ conjunto compacto de $R^n$, entonces:
existen $P_1$ y $P_2$ en $A$ tales que:
$$f(P_1)\geq{f(p)};\forall{P}\in{A}$$
$$f(P_2)\leq{f(P)};\forall{P\in{A}}$$ esto es, $f$ alcanza sus valores máximos y minimos globales en $A$. 


### Teorema: Multiplicadores de Lagrange (Generalizado)

Sean $f,g_2,g_2,...,g_k:U\subseteq{R^n}\to{R}$, funciones que admiten derivadas parciales de primer orden continuas. Sea $a\in{U}$ tal que $g_{j}(a)=0$ ; $j=1,...,k$ ; $k\leq{n}$.
Sea $S=$ {$x\in{U}|g_{j}(x)=0;j=1,...,k$}.
Suponga además que $\nabla g_j(a)\not=0$ ; $\forall{j}$.

Si $f|_{S}$ ($f$ restringido a $S$) tiene un extremo relativo en $a$, entonces existen $\lambda_1,...,\lambda_k;\lambda_k\in{R}$ tal que:
$$\nabla f(a)=\lambda_1\nabla g_1(a)+...\lambda_k\nabla g_k(a)$$
Las constantes $\lambda_1,...,\lambda_k$ se denominan multiplicadores de Lagrange 


#### Observación: 

1) En la practica, para determinar los puntos extremos de $f$, se resuelve el sistema de $n+k$ ecuaciones, formado por las $k$ ecuaciones de las condiciones $g_j(a)=0$, y las $n$ ecuaciones determinadas por la relación: 
$$\nabla f(x)=\lambda_1\nabla g_1(x)+...+\lambda_k \nabla g_k(x)$$
2) El sistema se resuelve respecto a las $n+k$ incognitas, $x_1,...,x_n$ y $\lambda_1,...,\lambda_k$ 
3) Los puntos críticos se encuentran en las soluciones del sistema
##### Ejemplo: 
Encuentre los valores máximos y mínimos de la función $f(x,y)=y²-x²$ sobre la elipse de ecuación $\frac{x²}{4}+y²=1$. 

#### Respuesta: 
Sea $g(x,y)=x²+4y²=4$ (Restricción)

Por teorema anterior, se resuelve el sistema:
$$\nabla f(x,y)=\lambda\nabla g(x,y)$$
$$g(x,y)=0$$

$\Rightarrow (-2x,2y)=\lambda(2x,8y)$ ; $x²+4y²=4$ 

$\Rightarrow -2x=2\lambda z$ (1) y $2y= 8\lambda y$ (2) ; $x²+4y²=4$ (3)

En (1), si $x\not=0$ $\Rightarrow \lambda=-1$ , sustituyendo en (2) queda $y=0$. Pero $x²+4y²=4$, de donde $x=+-2$. se obtienen los puntos:

$$P_1(2,0) ; P_2(-2,0)$$
SI $y\not=0$ en (2), obtenemos $\lambda=\frac{1}{4}$. Sustituyendo en (1), queda $x=0$, y de (3) se obtiene $y=+-1$. Y se obtienen los puntos críticos: 

$$P_3(0,1);P_4(0,-1)$$
Evaluando obtenemos:
$f(P_1)=f(2,0)=-4$ 
$f(P_2)=f(-2,0)=-4$ 
$f(P_3)=f(0,1)=1$
$f(P_4)=f(0,-1)=1$ 

Como el conjunto $S=$ {$(x,y)\in{R²}/\frac{x²}{4}+y²=1$} es un conjunto cerrado y acotado (compacto) de $R²$, y además la función $f$ es continua en $R²$, y en particular en $S$, entonces se tiene que:

- En $P_1$ y $P_2$, $f$ alcanza su valor mínimo, a saber $-4$ 
- En $P_3$ y $P_4$, $f$ alcanza su valor máximo, a saber $1$ 

#### Ejercicio Propuesto:
Usando multiplicadores de lagrange encuentre el valor máximo y valor mínimo de:
$$f(x,y,z)=x²+y²+z²$$
cuando $(x,y,z)$ recorre la curva de intersección entre el cilindro $x²+y²=50$, y el plano $x+y+z=12$.

#### Respuesta: 
Función adjetivo: $f(x,y,z)=x²+y²+z²$ 
Restricciones: $x²+y²=50$ y, $g_1(x,y,z)=x²+y²-50$ ; $x+y+z=12,g_2(x,y,z)=x+y+z-12$ 

Usando Teorema anterior, se resuelve el sistema:
$\nabla f=\lambda_1\nabla g_1+\lambda_2\nabla g_2$ (1)
$g_1(x,y,z)=0$ (2)
$g_2(x,y,z)=0$ 

$\Rightarrow (2x,2y,2z)=\lambda_1(2x,2y,0) + \lambda_2(1,1,1)$ (1)
$x²+y²=50$ (2)
$x+y+z=12$ (3)


$\Rightarrow$ $2x=\lambda_1x+\lambda_2$ ; $2y=2\lambda_1y+\lambda_2$ ; $2z=\lambda_2$ ; $x²+y²=50$ ; $x+y+z=12$ 

(ecuaciones (1), (2), (3), (4) y (5), respectivamente)


de (1): $2xy=2\lambda_1 xy+\lambda_2 y$ 
de (2): $2xy=2\lambda_1 xy+\lambda_2 x$ 

Restando (1) y (2): 

$\Rightarrow 0=\lambda_2(x-y)$ 
$\Rightarrow$ $\lambda_2=0$ o $x=y$

- SI $\lambda_2=0$, de (3), tenemos $z=0$, sustituyendo en (5), tenemos:
$x+y=12\Rightarrow{y=12-x}$
Sustituyendo en (4), se obtiene:
$x²+(12-x)²=50$ 

$\Rightarrow x²+144-24x +x²=50$ 
$\Rightarrow 2x²-24x+64=0$ $\Rightarrow x²-12x+47=0$ 
Note que $\Delta=-44<0$, por lo que no hay solución real.

#### Ejercicio: 
Sea $w=f(x,y)$ una función que admite derivadas parciales de 2do orden continuas, suponga que $x=u+v$ e $y=u-v$. Determine $\frac{\partial^2w}{\partial x\partial y}$ en terminos de las derivadas parciales con respecto a $u$ y $v$. 

#### Respuesta
de $x$ e $y$ $\Rightarrow x+y=2u\Rightarrow u=\frac{1}{2}(x+y)$ (sumando las ecuaciones)
y sacamos $x-y=2v\Rightarrow v=\frac{1}{2}(x-y)$ 

luego, $w=f(u(x,y),v(x,y))$ 

entonces, $\frac{\partial² w}{\partial x\partial y}=\frac{\partial}{\partial x}(\frac{\partial w}{\partial y})$ 

donde $\frac{\partial w}{\partial y}=g(x(u,v),y(u,v))$ 

luego sale más facil calcular la derivada parcial.

#### Ejercicio: Determine y clasifique los puntos criticos de la función:
$$f(x,y)=x³+2y³-27x-54y+4$$
#### Ejercicio: 
Sea $G=f(x+3y,2x-y)$, donde $f:R²\to{R}$ es una función diferenciable. Si $\nabla f(0,0)=(4,-3)$, determine la derivada direccional de $G$ en el origen en la dirección del vector $\vec{v}=(1,1)$ 



# Sub-superficies de una superficie




# Integrales dobles

### Definición:
Sea $z=f(x,y)$ una función integrable sobre el rectangulo $R=[a,b]\times{[c,d]}$ se define la integral doble de $f$ sobre el recangulo $R$ como:
$$\iint_{R}f(x,y)dA=\sum_{i=1}^{n}\sum_{j=1}^{m}f(x_{ij}^{*},y_{ij}^{*})\Delta A$$
Siempre que el limite exista


### Observavción

#### i) 
Cuando $f(x,y)\geq{0};\forall(x,y)\in{R}$, entonces, la inegral donle de $f$ sobre el rectangulo $R$, nos proprciona el volumen del solido que está por encima de $R$, y por debajo de la superficie $S:z=f(x,y)$ 

Esto es:
$$V=\iint_{R}f(x,y)dA$$
#### ii) 
Si $f(x,y)\equiv{1}$ en $R$, la integral $\iint_{R}dA$, nos proporciona el área de $R$.

## Teorema de Fubini

Si $z=f(x,y)$ es continua sobre el rectangulo $R=[a,b]\times[c,d]$, entonces:

$$\iint_R f(x,y)dA=\int_{a}^{b}[\int_{c}^{d}f(x,y)dy]dx=\int_{c}^{d}[\int_{a}^{b}f(x,y)dx]dy$$

#### Ejercicio propuesto

Calcular $\iint_R (4x³+6xy²)dA$ donde $R=[1,3]\times[-2,1]$ 



### Ejercicios

#### 1) 
Una polilla es atraida por la luminosidad de una ampolleta, lo que aumenta en proporción inversa a la en proporción inversa a la distancia del insecto al centro de la fuente de luz, que se considera el origen. La luminosidad a $30cm$ de la ampolleta es de $900lum$ 

##### a) 
Demuestre que en cualquier punto la dirección en que la luminosidad aumenta más rapido, apunta hacia la ampolleta

##### b)
Determine la razón de cambio de la luminosidad en el punto $(1,2,2)$ en la dirección del punto $(5,2,5)$. 

#### Solución:

##### a) 
Sea $L(x,y,z)$ la función que indicia la luminosidad en un punto $(x,y,z)$ (medido en cm) del espacio. Se tiene:
$$L(x,y,z)=\frac{k}{\sqrt{x²+y²+z^2}}(lum)$$
Además, $L(30,0,0)=900\Rightarrow{k=27.000}$,
por lo tanto $L(x,y,z)=\frac{27.000}{\sqrt{x²+y²+z²}}$ 

La dirección en que la luminosidad aumenta más rápido esta dada por $\nabla L(x,y,z)$ 

como $\frac{\partial L}{\partial x}(x,y,z)=-\frac{27.000x}{(x²+y²+z^2)^{\frac{3}{2}}}$ 

Así por simetria:
$$\nabla L(x,y,z)=-\frac{27.000}{(x²+y²+z²)^{\frac{3}{2}}}<x,y,z>=\lambda \cdot <x,y,z>$$

Como $<x,y,z>$ es el vector posición del punto $(x,y,z)$, concluimos que el vector, $\lambda<x,y,z>$ , $\lambda<0$; y por lo tanto la dirección de máximo crecimiento de la luminosidad, siempre apunta hacia el origen del espacio (la ampolleta).

##### b)
$\vec{u}=(5,2,5)-(1,2,2)=(4,0,3)$

entonces $û=\frac{<4,0,3>}{||<4,0,3>||}=\frac{1}{5}<4,0,3>$ 

por lo tanto:
$$\frac{\partial L}{\partial û}(1,2,2)=\nabla L(1,2,2)û=(-1000,-2000,-2000)=\frac{1}{5}<4,0,3>=-2000 (lum/cm)$$
# Integrales dobles sobre regiones más generales (Regiones elementales del plano)


### $I$) Región verticalmente simple

$f:R\subseteq{\mathbb{R}}\to{\mathbb{R}}$; f integrable. $R=\{(x,y)\in{R}/a\leq{x}\leq{b};g_1(x)\leq y\leq g_2(x)\}$
donde $g_1$ y $g_2$ son funciones continuas en $[a,b]$.

![[Pasted image 20251026203921.png]]

En este caso:
$$\iint_Rf(x,y)dA=\int_{x=a}^{x=b}[\int_{y=g_1}^{y=g_2}f(x,y)dy]dx$$

### $II$) Región horizontalmente simple
Sea $f:R\subseteq{\mathbb{R²}}\to\mathbb{R}$ una función integrable en la región $R=\{(x,y)\in\mathbb{R²}/c\leq{y}\leq{d};h_1(y)\leq x\leq h_2(y)\}$
donde $h_1$ y $h_2$ son funciones continuas en $[a,b]$ 
![[Pasted image 20251026204350.png]]
En este caso:
$$\iint_Rf(x,y)dA=\int_{y=c}^{y=d}[\int_x={h_1}^{x=h_2}f(x,y)dx]dy$$

### Ejercicio: 
Calcule el área de la región $R$ del plano $xy$, acotada por la recta $y=x$ y la parábola $y=x²-2x$ 

#### SOlución:

$y=x²-2x=x\Rightarrow x=0$ o $x=3\Rightarrow y=0$ o $y=3$ 

que son los puntos $(0,0),(3,3)$

entonces: $R=${$(x,y)\in\mathbb{R²}|0\leq{x}\leq{3};x²-2x\leq y\leq x$}


entonces, por teorema:

$$A(R)=\int_{x=0}^{x=3}[\int_{y=x²-2x}^{y=x}dydx]$$

### Ejercicio: 
Calcular la integral:
$$I=\int_{0}^{1}\int_{x²}^{1} 4x³ssin(y³)dydx$$
cambiando el orden de integración 

#### Solución:

$R:0\leq{x}\leq{1};x²\leq{y}\leq{1}$ que es verticalmente simple

Imagen rossel

La región $R$, mirada como región HORIZONTALMENTE simple es:

$R:0\leq{y}\leq{1};0\leq{x}\leq{\sqrt{y}}$ 

entonces:
$$I=\int_{y=0}^{y=1}\int_{x=0}^{x=\sqrt{y}} 4x³sin(y³)dxdy$$


### Ejercicios propuestos:

1) Determine el volumen del sólido, cuya base es la región del plano $xy$, que limitan la parabola $y=4-x²$ y la recta $y=3x$, mientras que su tejado es el plano $z=x+5$

SOlución 1):
sacando la intersección de ambos:
$y=4-x²=3x\Rightarrow x=-4$ o $x=1\Rightarrow y=-12$ o $y=3$ 

lo que da los puntos: $(-4,-12);(1,3)$ 
![[Pasted image 20251022132108.png]]

donde $f(x,y)=z=x+5$ que, evaluando en el valor minimo de $x$ de la región, tenemos que $f(x,y)=1$, entonces:

$R=${$(x,y)\in\mathbb{R²}|-4\leq{x}\leq{1};3x\leq{y}\leq{4-x²}$ } y $f(x,y)=x+5\geq{0}$ 

finalmente: 
$$V=\iint_R f(x,y)dA=\int_{-4}^{1}\int_{3x}^{4x²}(x+5)dydx=V(B)$$

podemos definir el volumen como:

$B=${$(x,y,z)\in\mathbb{R³}|0\leq{z}\leq{f(x,y)};(x,y)\in R$}
### Ejercicio:

Invierta el orden de integración en la siguiente integral doble:
$$I=\int_{0}^{1}\int_{e^{y-1}}^{e^{y}}f(x,y)dxdy$$

#### Respuesta:
Región de integración: $R: 0\leq{y}\leq{1};e^{y-1}\leq{x}\leq{e^{y}}$ ![[Screenshot from 2025-10-22 13-34-36.png]]

donde, los puntos "importantes" son: $(\frac{1}{e},0);(1,0)$ y $(e,1);(1,1)$, entonces:
$$I=\int_{x=\frac{1}{e}}^{x=1}\int_{y=0}^{y=ln(x)+1} f(x,y)dydx+\int_{x=1}^{x=e}\int_{y=ln(x)}^{y=1}f(x,y)dydx$$

# Cambio de variable

### Jacobiano:

Sean $x=g(u,v)$ e $y=h(u,v)$ con $g$ y $h$ funciones con derivadas parciales continuas en una región $S$ del plano. Entonces el Jacobiano de $x$ e $y$ con respecto a $u$ y $v$ se define como:

$$\frac{\partial (x,y)}{\partial (u,v)}=\begin{vmatrix}   \frac{\partial x}{\partial u} &  \frac{\partial x}{\partial v} \\    \frac{\partial y}{\partial u} &  \frac{\partial y}{\partial v}   \end{vmatrix}$$

### Teorema (Cambio de variable en la integral doble):
Sean $R$ y $S$ regiones de los planos $xy$ y $UV$ respectivamente, relacionados por $x=g(u,v)$ e $y=h(u,v)$, tales que cada punto de $R$ es imagen de un unico punto de $S$. Si $f(x,y)$ es continua en $R$, y $g$ e $h$ tienen derivadas parciales continuas en $S$, y además el Jacobiano no es nulo ($\frac{\partial (x,y)}{\partial (u,v)}\not=0$ )en $S$, entonces:
$$\iint_Rf(x,y)dA=\iint_Sf(g(u,v),h(u,v))\cdot|\frac{\partial (x,y)}{\partial (u,v)}|dudv$$
donde $dA=|\frac{\partial (x,y)}{\partial (u,v)}|dudv$ 

### Ejercicio:
Calcule $\iint_R\frac{cos(x-y){sin(x+y)}}dxdy$ donde $R$ es el trapecio $1\leq x+1\leq2;x\geq0;y\geq0$ 

#### Solución:

La región $R$ es: $1\leq{x+1}\leq2$ con $x$ e $y$ positivos en el plano $xy$ 

(Insertar grafico rossel)


##### Cambio de variable

$$\psi:\biggl\{u=x-y;v=x+y\Rightarrow\psi^{-1}:\biggl\{x=\frac{u}{2}+\frac{v}{2};y=\frac{v}{2}-\frac{u}{2}$$

Note que la transformación:
$$(u,v)=\psi(x,y)=(x-y,x+y)$$ transforma de acuerdo a la siguiente tabla:


| Plano $xy$ | Plano $UV$ |
| ---------- | ---------- |
| $x+y=1$    | $v=1$      |
| $x+y=2$    | $v=2$      |
| $y=0$      | $v=u$      |
| $x=0$      | $v=-u$     |
|            |            |
calculando:

$$\frac{\partial (u,v)}{\partial (x,y)}=\begin{vmatrix}   \frac{\partial u}{\partial x} &  \frac{\partial u}{\partial y} \\    \frac{\partial v}{\partial x} &  \frac{\partial v}{\partial y}   \end{vmatrix}=\begin{vmatrix} 1   &-1   \\  1   &   1  \end{vmatrix}=2$$
entonces:
$$\frac{\partial (x,y)}{\partial (u,v)}=\begin{vmatrix}   \frac{\partial x}{\partial u} &  \frac{\partial x}{\partial v} \\    \frac{\partial y}{\partial u} &  \frac{\partial y}{\partial v}   \end{vmatrix}=\begin{vmatrix} 0.5   &-0.5   \\  0.5   &   0.5  \end{vmatrix}=\frac{1}{2}$$

Transforma;
Plano $UV$ 
(insertar plano)



entonces, tenemos;

###### $\iint_{R_{xy}}\frac{cos(x-y)}{sin(x+y)} dA=\iint_{R_{uv}}\frac{cos(u)}{sin(v)}|\frac{1}{2}|dudv$ 

##### $=\frac{1}{2}\iint_{R_{uv}}=\frac{cos(u)}{sin(v)}dudv=\frac{1}{2}\int_{v=1}^{v=2}\int_{u=-v}^{u=v}\frac{cos(u)}{sin(v)}dudv$ 
##### $=\frac{1}{2}\int_{v=1}^{v=2}\frac{1}{sin(v)}(sin(u))|_{-v}^{v}dv$
##### $=\frac{1}{2}\int_{1}^{2}\frac{1}{sin(v)}(sin(v)+sin(v))dv$ 
##### $=\int_{1}^{2}2dv=\int_{1}^{2}dv=1$ 


### Ejercicio:
Calcule:
$$\iint_R\frac{1}{3x+y}cos(\frac{x-y}{2})dA$$
donde $R$ es la región del plano $XY$, acotdada por las graficas de las funciones (o rectas):
$$y=x;y=x-\pi;y=3-3x;y=6-3x$$

#### Respuesta:

note que graficando $R$:


![[Pasted image 20251024133110.png]]

![[Pasted image 20251024133134.png]]


##### Cambio de variable:
$$\Phi:\bigg\{ u=x-y;v=3x+y;\frac{\partial (u,v)}{\partial (x,y)}=\begin{vmatrix} 1 & -1   \\  4   &   1  \end{vmatrix}=4$$ 
entonces, la transformacion se da por:


| Plano $XY$ | Plano $UV$ |
| ---------- | ---------- |
| $x-y$      | $u=0$      |
| $x-y=\pi$  | $u=\pi$    |
| $3x+y=3$   | $v=3$      |
| $3x+y=6$   | $v=6$      |
|            |            |

plano $UV$:

(insertar plano ola)




entoinces:
$$\iint_R\frac{1}{3x+y}cos(\frac{x-y}{2})dA=\iint_S\frac{1}{v}cos)(\frac{u}{2})\cdot |\frac{1}{4}|dudv$$

