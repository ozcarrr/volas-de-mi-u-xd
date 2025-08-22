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

## $\vec{r}'(t) = \lim{t\to{t_0}}\frac{\vec{r}(t-\vec{r}(t))}{t-t_0}$ 


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

### Considere la curva $C$, dad por $\vec{r}(t)=(e^tcos(t),e^tsin(t),e^t),t\in[0,+\inf]$ 

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


## La ecuación del plano osculador a $C$$ es en l punto $P$ es : 

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

### se supone que $C$ esta dada por la función vectorial $r'(t)=(x(t),y(t),z(t))$ 

# Teorema: La curvatura de una curva $C$ dad por la función vectorial $\vec{r}(t)$, esta dada por: 

# $k(t)=\frac{||\vec{r}'(t)\times\vec{r}''(t)||}{||\vec{r}'(t)||³}$ 


### Definición (Torsión) : Se define la torisón de una curva $C$, dada por la función vectorial $\vec{r}(t)=(x(t),y(t),z(t));t\in{I}$ como:

# $\tau(t)=\frac{(\vec{r}'(t)\times\vec{r}''(t))\cdot\vec{r}'''(t)}{|| \vec{r}'(t)\times\vec{r}''(t)||²}$ 


### Nota: La torsión mide el grado de torcedura de la curva $C$. 

### La torsión mide el desvio de la curva  respecto del plano oscular. 


# Componente tangencial y normal de la aceleración 

## Sea $C$ definida por $\vec{r}(t)=(x(t),y(t),z(t))$ 

### definición :

### Si el parametro $t$ es el tiempo entonces $\vec{r}''(t)$ es la aceleración de una particula con posición instantanea $\vec{r}(t)$. los coeficientes de los vectores $T$ y $N$ son respectivamente las componentes tangencial y normal de la aceleración

### De hecho :

# $T(t)=\frac{\vec{r}'(t)}{||\vec{r}'(t)}$ -> $\vec{r}'(t)=||\vec{r}'(t)||\cdot{T(t)}$ 


# -> $\vec{r}''(t)=\frac{d}{dt}(||\vec{r}'(t)||)\cdot{T(t)}+||\vec{r}'(t)||\cdot{T'(t)}$ 

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


## Proposición: Sean a_T y a_N las componentes tangencial y normal de la aceleración. Se tiene: 

# $a_T=\frac{\vec{r}'(t)\cdot{\vec{r}''(t)}}{||\vec{r}'(t)||}$ 

# $a_N=\frac{||\vec{r}'(t)\times\vec{r}''(t)}{||\vec{r}''(t)||}$ 


## Bosquejo de demostración: 

### Sabemos que : 

# $a_T(t)=s''(t)=\vec{r}''(t)\cdot{T(t)}=\vec{r}''(t)\cdot{\frac{\vec{r}'(t)}{||\vec{r}'(t)||}}$ 

# $=\frac{\vec{r}''(t)\cdot{\vec{r}'(t)}}{||\vec{r}'(t)||}$ 

# = $\frac{\vec{r}'(t)\cdot{\vec{r}''(t)}}{||\vec{r}'(t)||}$ 
# $a_N = (s'(t))²\cdot{k(t)}=||\vec{r}'(t)||²\cdot{\frac{||\vec{r}'(t)\times\vec{r}''(t)||{||\vec{r}'(t)||³}}}$ 

## FInalemtne : $\frac{||\vec{r}'(t)\times{\vec{r}''(t)}||}{||\vec{r}'(t)||}=a_N$ 


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
# $||\vec{r}'(t)\times{\vec{r}''(t)||}=2\sqrt{2}|cos(2t)|$ 

## Luego, $k(t)=\frac{||\vec{r}'(t)\times{\vec{r}''(t)}||}{||\vec{r}'(t)||³}=\frac{2 \sqrt{2}|cos(2t)}{(1+sin²(2t))^{\frac{3}{2}}}$ 


## Asi: 

# $a_N=(s''(t))^2\cdot{k(t)}=(1+2sin²(2t))\cdot{\frac{2\sqrt{2}|cos(2t)}{(1+sin²(2t))^{\frac{3}{2}}}}$ 














































 






