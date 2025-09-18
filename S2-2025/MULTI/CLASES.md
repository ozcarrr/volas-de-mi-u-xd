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

### $P_t: z-z_0=\frac{\delta f}{\delta x}(x_0,y_0)(x-x_0)+\frac{\delta f}{\delta y}(x_0,y_0)(y-y_0)=0$ 
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

$\Rightarrow$ el punto donde el plano tangente de la paraboloide es paralelo al plano $\Pi$ es  $(-\frac{1}{8},-1,f(-\frac{1}{8},-1))=(-\frac{1}{8},-1,\frac{1}{16}+1)$ 


# La diferencial 

### Recuerdo :
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

# $f(x+\Delta x, y+\Delta y, z+\Delta z)\approx{f(x,y,z)+dw}$ 

# *Ejercicio:*

Estimar el valor de $\sqrt{(2.10)²+(1.98)²+(1.05)²}$ 


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


























 






