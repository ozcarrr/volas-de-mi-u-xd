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

## $T(t)=\frac{\vec{r}(t)}{||\frac{d}{dt}\vec{r}(t)||}$ 


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

## $L_C=\int{\vec{r}'(t)}Vdt=\int{\sqrt{(x'(t))²+(y'(t))²+(z'(t))²}}$ 

### Ejemplo: sea $C$ una curva definida por la funcion vectorial $\vec{r}(t)=(\frac{t²}{2},sin(t)-tcos(t),cos(t)+tsin(t));t\in[0,\pi]$, calcule la longitud de curva de $C$:


## $\vec{r}'(t)=(t,cos(t)-(cos(t)-tsin(t)),-sin(t)+sin(t)+tcos(t))=(t,tsin(t),tcos(t))$

## $||\vec{r}'(t)||=\sqrt{t²+t²sin²(t)+t²cos²(t)}=\sqrt{2t²}=\sqrt{2}|t|=\sqrt{2}t$ 

### Entonces : $L_C=\int{||\vec{r}'(t)}dt=\sqrt{2}\int{t}dt=\frac{\sqrt{2}}{2}\pi²$ 

# Función longitud de arco 

### Def: Sea $C$ una curva suave dada por la función vectorial $\vec{r}:I\subseteq{R}->R³$ ; $\vec{r}(t)=(x(t),y(t),z(t))$ 
### Supongamos que $\vec{r}$ es diferenciable; $t_0\in{I}$, se define la longitud de arco $\vec{r}(C)$, relativa a $t_0$, como: 

## $s(t)=\int{||\vec{r}'(u)||}du$ entrega la longitud de la curva, desde el punto inicial $\vec{r}(t_0)$ hastael punto variable $\vec{r}(t)$ 
### OBS: Por el teorema fundamental del calculo (TFC) se tiene lo siguiente: 

## Si $F(u)$ es una primitiva de la $||\vec{r}'(u)||$, entonces:

## $s(t)=\int{||\vec{r}'(u)||}du=F(u)=F(t)-F(t_0)$ donde $F(t_0)$ es constante, entonces :

## $s'(t)=\frac{ds}{dt}=\frac{d}{dt}(\int{||\vec{r}'(u)}du)=||\vec{r}'(t)$ Por lo tanto, $s$ es una función diferenciable, y $s'(t)=\frac{ds}{dt}=||\vec{r}'(t)||$, además :

## $ds=||\vec{r}'(t)||dt$ 

### Def: Una curva $C$ dada por $\vec{r}(t)=(x(t),y(t)z(t))$ se dice "parametrizada por la longitud de arco si y solo si $||\vec{r}'(t)||=1,\forall{t}$ "

### obs: Sea $C$ una curva suave, dada por $\vec{r}(t)=(x(t),y(t),z(t))$ ; suponga que $\vec{r}'(t)!=0,\forall{t}$. 

## Como $s'(t)=\frac{ds}{dt}=||\vec{r}'(t)||>0,\forall{t}$, entonces $s$ es una función creciente de $t$, y por lo tanto invertible, con inversa $t=t(s)$, entonces:

## $s=s(t)<->t=t(s)$ ; La funcion $s$ siendo la longitud de arco y $t$ es la inversa de $s$. 

### Cuando sustituimos $t$ por $t(s)$ en las ecuaciones originales de $C$, obtenemos la reparametrización por la longitud de arco de la curva $C$: 

## $\beta(s)=x(s)i+y(s)j+z(z)k=(x(s),y(s)z(s))$  

## donde $||\beta'(s)||=1$ 

## Ejercicio :

### Considere la hélice $C$ dada por la función vectorial:

## $\vec{r}(t)=(5cos(t),5sin(t),12t),t\in{R}$ 

### Reparametrice la curva $C$ con respecto a la longitud de arco, medida a paritr del punto (5,0,0), en la dirección en que aumenta $t$. 

### Respuesta : $\vec{r}'(t)=(-5sin(t),5cos(t),12)$ entonces $||\vec{r}'(t)||=\sqrt{25sin²(t)+25cos²(t)+144}=13$ que es distinto de 1, entonces la curva $C$ no esta parametrizada por la longitud de arco. 

## Reparametricemos $C$ por la longitud de arco: 

### El punto $(5,0,0)$ corresponde a $t=0$, por lo tanto la función longitud de arco relativa a $t=0$ es:

## $s(t)=\int{||\vec{r}'(u)||du}=\int{\sqrt{169}du}=\int{13}du=13t$ 

## entonces: $s(t)=13t$, donde su inversa es $t(s)=\frac{s}{13}$ 
## Sustituyendo en las ecuaciones originales de $C$, $t$ por $\frac{s}{13}$, obtenemos: 

## $C: \vec{\beta}(s)=(x(\frac{s}{13}),y(\frac{s}{13}),z(\frac{s}{13}))=(5cos(\frac{s}{13}),5sin(\frac{s}{13}),12\frac{s}{13})$  

#### Note que $||\vec{\beta}(s)||=1$, Verificar. 

## Ejercicio :

### Considere la curva $C$, dad por $\vec{r}(t)=(e^tcos(t),e^tsin(t),e^t),t\in[0,+\inf]$ 

### a) Determine $\vec{T},\vec{N},\vec{B} en el punto $P(0,e^{\frac{\pi}{2}},e^{\frac{\pi}{2}})$ 

### b) Parametrice $C$ con respecto al parametro longitud de arco. 


## RESPUESTA : $\vec{r}(t)=(e^tcos(t),e^tsin(t),e^t)=(0,e^{\frac{\pi}{2}},e^{\frac{\pi}{2}})$ 

## -> $e^{t}cos(t)=0 ; e^{t}sin(t)=e^{\frac{\pi}{2}} ; e^{t}=e^{\frac{\pi}{2}}$ -> $\vec{r}(\frac{\pi}{2})=(0,e^{\frac{\pi}{2}},e^{\frac{\pi}{2}})$ 

## Por otro lado : $\vec{r}'(t)=(e^t(cos(t)-sin(t)),e^t(sin(t)+cos(t)),e^t)$ 

## -> $\vec{r}''(t)=(-2e^tsin(t),2e^tcos(t),e^t)$ 

## $\vec{r}'(\frac{\pi}{2})=e^{\frac{\pi}{2}}(-1,1,1)$ 
## $\vec{r}''(\frac{\pi}{2})=e^{\frac{\pi}{2}}(-2,0,1)$  

## Por lo tanto $\vec{T}(t)=\frac{\vec{r}'(t)}{||\vec{r}'(t)||}->\vec{T}(\frac{\pi}{2})=\frac{e^{\frac{\pi}{2}}{\sqrt{3}e^{\pi}{2}}=\frac{(-1,1,1)}{\sqrt{3}}$ 













 






