
## TIPOS DE ECUACIONES DIFERENCIALES:


#### - Ecuaciones diferenciales ordinarias (EDO):
Es una ecuación diferencial en la que hay solo una variable independiente de manera que todas las derivadas que paracen en ellas son derivadas ordinarias.

EJ:
## $\frac{d²y}{dx²}-4\frac{dy}{dx}+4y=4y²-2$ 


## $y'-4y=0$


### ECUACIONES DIFERENCIALES CON DERIVADAS PARCIALES
Es una ecuación diferencial que hace intervenir más de una variable independiente de manera que aparecen derivadas pariciales

EJ: 

## $\frac{d²z}{dx²}+\frac{d²z}{dy²}=0$


## Orden y linealidad de una EDO

- Se considera el orden de la derivada más alta en la ecuación para dar el orden a la EDO
- si $F$ es una función lineal de $Y$ si $F$ se compone solo de funciones lineales

EJ:

## $y'+7y=e^x$ (Lineal de orden 1)

## $3y''+4y'-3y=0$ (Lineal de orden 2)

## $y^{(3)}+y²=0$ (NO Lineal de orden 3)

## $\frac{d²y}{dx²}-sin(y)=0$ (NO Lineal de orden 2)




### OBS: 
Simbolicamente una EDO de orden n se ve como:

## $F(X, Y, Y', ..., Y^{(n)})=0$ 
(donde $F$ es una funcion de n+2 variables)

Asi, es equivalente decir que:

## $Y^{(n)}=f(X, Y, Y', ..., Y^{(N-1)})$ 
(donde $f$ es una función de n+1 variables)


EJ:

## $\frac{d²y}{dx²}+\frac{dy}{dx}+5y-10sin(x)=0=F(x, y, y', y'')$ 

esto tambien implica: 

## $\frac{d²y}{dx²}=-4\frac{dy}{dx}-5y+10sin(x)$ 




## SOLUCIÓN DE UNA EDO

def: Una función $\phi:I\subseteq R -> R$, que tiene al menos n derivadas continuas en I, que satisfacen la ecuación:

## $F(X, Y, Y', ..., Y^{(n)})=0$

es una solución de la ecuación en $I$ 
(*El intervalo $I$ se llama intervalo de existencia o dominio de solución)

EJ (tarea):

Compruebe que $y(x)=xe^x$ es solución de la EDO:

## $Y''-2Y'+Y=0$ en $\mathbb{R}$

¿Esta solución es unica? 




## Solución Trivial :O


Observe que, $y=0$ es solucion de la ecuación $y''-2y'+y=0$ del ejemplo anterior. la solucioón $y=0$ se llama solución trivial de la ecuación.


## Solución Implicita 

def: Se dice que la relación $g(x,y)=0$ es una solucion implicita de una EDO de orden n, $F(x, y, y', ..., y^{(n)})=0$ en un intervalo $I$, si existe al menos una función $\phi(x)$, y la ecuación en el intervalo $I$. 

EJ: La relación $x²+y²=1$ ($g(x,y)=x²+y²-1$), es una solución implicita de la siguiente ecuación: $y'=\frac{-x}{y}$ en el intervalo $]-1,1[$, ya que derivando g(x), obtenemos: 

## $2x+2yy'=0$ -> $y'=\frac{-x}{y}$ 


Note ademas que existen dos funciones diferenciables en $I$ que satisfacen la EDO, y ademas la relación $x²+y²=1$, a saber:

## $\phi_1(x)=\sqrt{1-x²}$ , $\phi_1(x)=-\sqrt{1-x² }$ 

## Solución particular

Una solucion sin parametros arbitrarios se llama solución particular:

EJ: 
## La familia $y=cx-xcos(x)$ ; c constante, es solución de la EDO lineal $xy'-y=x²$ (Verificar)

Considerando c = 0, obtenemos la solución particular $y=-xcos(x)$


## Solución Singular 

Def: Una solución que no es parte de la familia de soluciones de una EDO se llama Solución Singular.

EJ: 
## La familia $y=(\frac{1}{4}x²+c)²$ es solución de la EDO NO lineal de primer orden $y'=x\sqrt{y}$.

SIn embargo, la solución trivial y = 0 tambien es solución, y no se obtiene para ningun valor del parametro $c$ 

Así $y=0$ es una solución singular de la ecuación. 

## Solución General de una ecuación 

Si toda solución de una EDO lineal de orden $n$, $F(x, y, ..., y^{(n)})=0$ se puede obtener de una familia n-paramétrica de soluciones:

## $G(x,y,c_1,...,c_n)=0$ 

Se dice que esta familia es la solución general de la ecuación.

## Problemas de valores iniciales

def: Una ecuación diferencial sujeta a condiciones sobre $y=y(x)$ o sus derivadas en un punto $x_0\in{I}$, se llama problema de valor inicial (P.V.I), tiene la forma:

## $F(x,y,y',...,y^{(n)})=0$
## $y(x_0)=y_0,...,y^{(n-1)}(x_0)=y_{n-1}$ 

donde $y_0,y_1,y_{n-1}$ son constantes reales, las condiciones:

## $y(x_0)=y_0,...,y^{(n-1)}(x_0)=y_{n-1}$ 

se llaman condiciones iniciales. 

## Problemas de valor inicial de primer orden: 

## $y'=f(x,y);y(x_0)=y_0$  

al resolver el problema de valor inicial, buscamos una solución que pasa por $(x_0,y_0)$


## Problemas de valor inicial de segundo orden 

## $y''=f(x,y,y');y(x_0)=y_0;y'(x_0)=y_1$ 


EJ:

## La ecuacion de orden 1 $y'=y$ tiene como solución general la familia $y=ce^x$ donde $c$ es constante. Si imponemos la condición inicial y(0)=3, obtenemos $y(0)=c=3$. Por lo tanto $y=3e^x$ es solución del PVI:

## $y'=y;y(0)=3$ 

Ej:

## Sabiendo que $x(t)=c_1cos(4t)+c_2sin(4t)$ es una familia de soluciones de la ecuación $x''(t)+16x(t)=0$, encuentre la solución del P.V.I:

## $x''(t)+16x(t)=0$ 
## $x(\frac{\pi}{2})=2$ ;$x'(\frac{\pi}{2})=1$ 

## EDO de primer orden 

## $F(x,y,y')=0$ -> $y'=f(x,y)$ 

Note que $f:A\subseteq{R} -> R$ , Por lo tanto, el dominio de la EDO es un subconjunto de $R²$ 

## Teorema de existencia y Unicidad

Sea D un conjunto abierto de $R^2$ y $f:D\subseteq{R²}->R$ una función continua. Supongamos que $\frac{df}{dy}$ es continua en D. 
Sea $(x_0,y_0)\in{D}$. Entonces la EDO $\frac{dy}{dx}=f(x,y)$  tiene una unica solución $u:I\in{R}->R$, con $x_0\in{I}$, tal que $u(x_0)=y_0$. 

Nota: $\frac{df}{dy}$ denota la derivada parcial de f con respecto a $I$ .

### Es decir :

#### 1. Si $f(x,y)$ es continua en $(x_o,y_0)$, entonces el P.V.I tiene solución
#### 2. Si $\frac{df}{dy}$ es continua en $(x_0,y_0)$, entonces el P.V.I tiene solución UNICA. 

## EJERCICIO

## Dada la EDO de orden 1 ,$\frac{dy}{dx}=\frac{3}{\sqrt{x-y}}$; se pide: 

### a) aplicando teorema de existencia y unicidad , determine el conjunto donde el teorema asegura existencia y unicidad. 

### b) Decidir si existe solución que pasa por el punto $(-2,2)$. 


## Tipos de EDOS de primer orden 


#### Ecuaciones de variables separadas :

La EDO de orden 1 $\frac{dy}{dx}=f(x,y)$, se llama de variables separadas si se puede escribir de la siguiente forma:

## $\frac{dy}{dx}=g(x)h(x)=f(x,y)$  (1)

donde $g$ es una función que depende solo de $x$, y $h$ es una función que depende solo de la variable $y$ 


## 13/08/2025 


## obs: 
## Note que si existe $y_0$ tal que $h(y_0)=0$ entonces la función constante $y(x)=y_0$ , es solución de la ecuación diferencial. Se llama solución constante de la ecuación.

### Si $h(y)\not={0}\forall{y}$ etnocnes de (1) podemos escribir:

## $\frac{1}{h(y)}dy=g(x)dx$ 
## $<-> \int{\frac{1}{h(y)}}dy=\int{g(x)}dx +C$ 


## Ejemplo : Resolver :

### $\frac{dy}{dx}=y²sin(x)e^{cos(x)}$
### Ademas, encuentre soluciones constantes. 

## RESPUESTA : $g(x)sin(x)e^{cos(x)};h(y)=y²$ 

## Solución constante: $y²=0<->y=0$, por lo tanto $y(x)=0$ es la solución constante de la ecuación.

### para $h(y)\not=0$, tenemos: (Separamos variables)

## $\frac{1}{y²}dy=sin(x)e^{cos(x)}dx <-> \int{\frac{1}{y²}}=\int{sin(x)e^{cos(x)}dx}$ 

## Entonces : $-\frac{1}{y}=-e^{cos(x)}+D <-> y = \frac{1}{e^{cos(x)}+C}$ 
## es nuestra solución general. 

NOTA : La EDO de orden 1 $\frac{dy}{dx}=f(x,y)$ se puede escribir en la forma $M(x,y)dx+N(x,y)dy=0$ 

## EJERCICIO :

### Resolver $ydx+(x-3)dy=0;y(0)=1$ 

## <-> $(x-3)dy=-ydx$ 
## <-> $\frac{dy}{-y}=\frac{dx}{x-3}/\int()$ 
## <-> $ln(y)=-ln|x-3|+C$ (Solución general en su forma implicita)
## <-> $y=\frac{1}{|x-3|}e^{C}=\frac{D}{|x-3|};D\in{R⁺}$ (Solución general en su forma explicita)

## Aplicando $y(0)=1$: 

### ->$\frac{D}{3}=1$ -> $D=3$, entonces la solución del P.V.I es : $y=\frac{3}{|x-3|}$ 


## Ejemplo : Resuelva $y'=\frac{1}{x-y}+1=\frac{dy}{dx}$ 

#### Solución: 
#### Note que la ecuación dada no es de variables separadas (no se ppuede aplicar T.V.P), entonces:
### Sea $z=x-y$ -> $\frac{dz}{dx}=1-\frac{dy}{dx}$ -> $\frac{dz}{dx}=1-(\frac{1}{x-y}+1)=-\frac{1}{x-y}=-\frac{1}{z}$ -> $\frac{dz}{dx}=\frac{-1}{z}$ (variables separadas)

## luego -> $zdz=-dx/\int()$ 

## -> $\frac{z²}{z}=-x+C <-> \frac{(x-y)²}{z}=-x+C$ (Solución general en su forma implicita)

## Ejercicios : Resolver las siguientes ecuaciones :

### 1. $\frac{dy}{dx}=y²cos(x)$ 

### 2. $\frac{dy}{dx}=y(1-y)$ 
### 3. $(x²+1)\frac{dy}{dx}+2xy=1$ 

### 4. $(2x+1+2xy)dx + (x²+4y³)dy = 0$ 
### 5. $(3y²+4x)dx + (2xy)dy =0$ 


# ECUACIONES LINEALES DE PRIMER ORDEN CON FACTOR INTEGRANTE

### Forma:$a_1(x)\frac{dy}{dx}+a_2(x)y=g(x)$ , donde $a_1(x),a_2(x),g(x)$ son funciones de la variable $x$ 

## Forma estandar: al dividir ambos miembros de la igualdad por $a_1(x),a_1(x)\not=0$, se obtiene la forma estandar:

## $\frac{dy}{dx}+p(x)y=f(x)$ (1)


### OBS: 

#### 1. Buscamos una solución de (1) en un intervalo $I$ en el cual ambas funciones $p$ y $f$ son continuas 

#### 2. SI $f(x)=0$, la ecuación (1) se transforma en una ecuación homogénea, caso contrario no homogénea. Si la ecuación (1) es homogénea, esto es:

### $\frac{dy}{dx}+p(x)y=0$  (2)

#### Se obtiene una ecuación de variables separadas :

### $\frac{dy}{dx}=-p(x)y <-> \frac{dy}{y}=-p(x)dx/\int()$ 

### -> $ln(y)=\int{-p(x)dx}+k/e^{()}$ 
### -> $y(x)=C\dot{e^{-\int{p(x)dx}}}$ ; $C\in{R}$ (Solución general de la ecuación lineal homogénea)

# SOLUCIÓN GENERAL DE LA ECUACIÓN LINEAL NO HOMOGÉNEA 

## $y(x)=e^{-\int{p(x)dx}}[\int{f(x)e^{\int{p(x)dx}}}dx+c]$ 

## $\frac{dy}{dx}+p(x)y=f(x);f(x)\not=0$ (Solución general)

## OBS: La forma de la solución general de la ecuación (1), nos hace pensar que la ecuación lineal en su forma estándar se puede reducir a a una ecuación de variable separada, mediante el uso de un factor integrante.


# $\frac{dy}{dx}+p(x)y=f(x)/e^{\int{p(x)dx}}$ <- factor integrante

# $\frac{dy}{dx}e^{\int{p(x)dx}}+p(x)ye^{\int{p(x)dx}}=f(x)e^{\int{p(x)dx}}$ 

## -> $\frac{d}{dx}(y(x)e^{\int{p(x)dx}})=f(x)e^{\int{p(x)dx}}/\int()$
## -> $y(x)e^{\int{p(x)dx}}=\int{f(x)e^{\int{p(x)dx}}}+C$
## -> $y(x)=\frac{1}{e^{\int{p(x)dx}}}(\int{f(x)e^{\int{p(x)dx}}}+C)=e^{-\int{p(x)dx}}(\int{f(x)e^{\int{p(x)dx}}}+C)$ 
### Solución general de la EDO lineal de primer orden no homogénea 

## Ejercicio: Resolver la siguiente ecuación : 

### a) $\frac{dy}{dx}-3y=6$
### b) $(x²-9)\frac{dy}{dx}+xy=x$ 


# 20/08 

# Ecuaciones diferencuales exactas 

### Previo: 

### definición: Sea $z=f(x,y)$ una función con derivadas parciales de primer orden continuas en una región rectangular $R$ del plano $xy$, entonces se su diferencial total, denotada por $dz$ o $df$ , se define como: 

# $df=\frac{\delta f}{\delta x}dx + \frac{\delta f}{\delta y}dy$ 

### Ahora, si $f(x,y)=c$ ; $c$ constante, entonces :

# $df=\frac{\delta f}{\delta x} dx + \frac{\delta f}{\delta y}dy=0$ 

### de modo que la solución de la ecuación diferencial $df=0$, esta dada implicitamente por $f(x,y)=c$ ; $c$ constante.

## definición (Ec. diferencial Exacta) : 

### Consideremos la EDO: 

# $M(x,y)dx + N(x,y)dy=0$ (1) 

### donde $N$ y $M$ son funciones continuas en un conjunto abierto de $D\subseteq{R²}$. Diremos que la ecuación (1) es excacta en D, si existe una función diferenciable $f(x,y)$, tal que:

# $\frac{\delta f}{\delta x}=M(x,y) ; \frac{\delta f}{\delta y}=N(x,y); \forall{(x,y)\in{D}}$ 
## Note que en este caso 

# $df = M(x,y)dx + N(x,y)dy=0$ 
# -> $df=0$ -> $f$ es constante, esto es $f(x,y)=c$ con $c$ constante.

# Así: 

# $\frac{\delta M}{\delta y}=\frac{\delta}{\delta y}(\frac{\delta f}{\delta x}) = \frac{\delta N}{\delta x}$ 
## Se concluye que $\frac{\delta M}{\delta y}=\frac{\delta N}{\delta x}$ 

### Teorema: Sean M,N , $\frac{\delta M}{\delta y}$ , $\frac{\delta N}{\delta x}$ funciones continuas en una región rectangular $R$ del plano $xy$. entonces la ecuación: 

# $M(x,y)dx + N(x,y)dy=0$ 

### es exacta en $R$ si y solo si pasa lo siguiente: 

# $\frac{\delta M}{\delta y}(x,y)=\frac{\delta N}{\delta x} (x,y), \forall{(x,y)}\in{R}$ 


## Ejemplo: Resolver la ecuación: 

# $cos(y)dx-(xsin(y)-y²)dy=0$ (M(x,y) - N(x,y))


### Respuesta: $M(x,y) = cos(y) ; N(x,y)= -xsin(y)+y²$ 


# $\frac{\delta M}{\delta y}=-sin(y);\frac{\delta N}{\delta x}=-sin(y)$ 

# -> $\frac{\delta M}{\delta y}=\frac{\delta N}{\delta x}$ y por lo tanto la ecuación es dada exacta.

### Su solución se obtiene como sigue: 

### Como la ecuación es exacta, existe una función escalar $\mu(x,y)=c$, tal que: 

# $\frac{\delta \mu}{\delta x}=M(x,y)=cos(y)$ y $\frac{\delta \mu}{\delta y}=N(x,y)=-xsin(y)+y²$ 

### Tenemos: 

# $\mu(x,y)=\int{cos(y)dx}=xcos(y)+C(y)$ ; $C(y)$ es una función que depende de $y$ 

### Para que $\mu(x,y)$ sea solución de la ecuación, debe ocurrir también que: 

# $\frac{\delta \mu}{\delta y}=N(x,y)$ <-> $-xsin(y)+y²=-xsin(y)+C'(y)$ 
# -> $C'(y)=y²$ -> $C(y)=\frac{y³}{3}$ 

# Luego, $\mu(x,y)=xcos(y)+\frac{y³}{3}$ y por lo tanto: 

### $\mu(x,y)=xcos(y)+\frac{y³}{3}=C$ es solución de la ecuación en forma implicita 

#### Nota : $\vec{F}(x,y)=cos(y)î - (xsin(y)-y²)j$ 


## Ejemplo: Considere la EDO 

# $ydx+dy=0$ 

## Note que:  $M(x,y)=y ; N(x,y)=1$ 


# -> $\frac{\delta M}{\delta y}=1\not=0=\frac{\delta N}{\delta x}$, luego la ecuación dada no es exacta, pero: 

### Si multiplicamos la ecuación dada por $e^x$, tenemos: 

# $e^{x}ydx+e^{x}dy=0$ ; $P(x,y)=e^{x}ydx ; Q(x,y)=e^{x}dy$ 

# -> $\frac{\delta P}{\delta y}=e^x ; \frac{\delta Q}{\delta x}=e^x$, Así la ecuación es exacta, cuya solución es la siguiente: 

# $\mu(x,y)=\int{e^{x}y}dx = e^{x}y+C(y)$ 


## $\frac{\delta \mu}{\delta y}=e^x + C'(y)=Q(x,y)=e^x$ 

# -> $C'(y)=0$ -> $C(y)$ es cte. $=k$ 


### Luego la solución de la ecuación es: 

# $\mu(x,y)=ye^x + k=C$ 
# -> $ye^x = D ; D=C-K$ -> $y=De^{-x}$ ; $D$ cte



# Factores Integrantes

### Considere la EDO no exacta: 

# $M(x,y)dx+N(x,y)dy=0$ ; (1)

### esto es $\frac{\delta M}{\delta y}\not=\frac{\delta N}{\delta x}$ 

### PUEDE OCURRIR que multiplicando (1) por una función $p(x,y)$, ella se transforme en una EDO exacta:

# $P(x,y)M(x,y)dx+P(x,y)M(x,y)dy=0$ (2)

### Nuevo M y N 


### Cuando ocurre esto, decimos que P(x,y) es un factor integrante de la EDO (1), además las soluciones de la EDO (1) y (2) son iguales :O


### Como la ecuación (2) es exacta debe ocurrir que: 

# $\frac{\delta }{\delta y} (P\cdot{M})=\frac{\delta}{\delta x} (P\cdot{N})$ 


# -> $M\cdot{\frac{\delta P}{\delta y}}+P\frac{\delta M}{\delta y}=N\frac{\delta P}{\delta x}+P\frac{\delta N}{\delta x}$ (Ecuación diferencial parcial)

### En algunos casos $p(x,y)$ se puede calcular, se distinguen 2 casos: 

## 1. si $p$ depende solo de $x$: 

### $p=p(x)$ -> $\frac{\delta p}{\delta y}=0$ ; $\frac{\delta p}{\delta x}=\frac{dp}{dx}$ 

### Sustituyendo en la igualdad anterior, tenemos: 

## $P\frac{\delta M}{\delta y}=\frac{dp}{dx}N+p\frac{\delta N}{\delta x}$ 

## -> $\frac{dp}{dx}N=p(\frac{\delta M}{\delta y}-\frac{\delta N}{\delta x})$ 
## -> $\frac{dp}{p}=\frac{1}{N}(\frac{\delta M}{\delta y}-\frac{\delta N}{\delta x})dx$ 

## Si $\frac{1}{N}(\frac{\delta M}{\delta y}-\frac{\delta N}{\delta x})$ depende solo de $dx$ entonces: 

# $p(x)=e ^{\int\frac{1}{N}(\frac{\delta M}{\delta y}-\frac{\delta N}{\delta x})dx}$ 


# 2. Si $p$ depende solo de $y$, es decir $P=P(y)$ , entonces $\frac{\delta p}{\delta y}=0$ y $\frac{dp}{dy}=\frac{\delta p}{\delta y}$ 
## Sutituyendo en (*), se tiene: 

## $\frac{dp}{dy}\cdot{M}+p\frac{\delta M}{\delta y}=P\frac{\delta N}{\delta x}$ 


# -> $\frac{dp}{dy}M=P(\frac{\delta N}{\delta x}-\frac{\delta M}{\delta y})$ 

# ->$\frac{dp}{p}=\frac{1}{M}(\frac{\delta N}{\delta x}-\frac{\delta M}{\delta y})dy$ (B)

## SI $-\frac{1}{M}(\frac{\delta M}{\delta y}-\frac{\delta N}{\delta x})$ solo depende de y, la ecuación (B)es de variables separadas (se resuelve la ecuación), y en este caso el factor integrante es: 

# $p(y)=e^{\int{\frac{1}{M}(\frac{\delta N}{\delta x}-\frac{\delta M}{\delta y})dy}}$ 

## Ejercicio: Resuelva la ecuación:

### $2xyln(y)dx+(x²+y²\sqrt{y²+1})dy=0$ 

### Solución: en este caso tenemos 

## $M(x,y)=2xyln(x)$ ; $N(x,y)=x^2+y²\sqrt{y²+1}$ 

## entoces :

# $\frac{\delta M}{\delta y}=2x[ln(y)+y\frac{1}{y}]=2xln(y)+2x$ 
# $\frac{\delta N}{\delta x}=2x$ 

# -> $\frac{\delta M}{\delta y}\not=\frac{\delta N}{\delta x}$ y por lo tanto, la ecuación no es exacta.

### Entonces buscamos factor integrante

## i) $p(x)=e ^{\int\frac{1}{N}(\frac{\delta M}{\delta y}-\frac{\delta N}{\delta x})dx}$ 

## $\frac{1}{n}(\frac{\delta M}{\delta y}-\frac{\delta N}{\delta x})=\frac{1}{x²+y²\sqrt{y²+1}}[2xln(y)+2x-2x]$ 
## $=\frac{2xln(y)}{x²+y²\sqrt{y²+1}}$ (Expresión que no depende solo de $x$ ) (No es factor integrante)

# ii) $\frac{1}{M}(\frac{\delta N}{\delta y}-\frac{\delta M}{\delta x})=\frac{1}{2xyln(y)}\cdot{(2x-2xlny-2x)}$ 
## $=\frac{1}{2xyln(y)}\cdot[-2xln(y)]$ 

# $=-\frac{1}{y}$ (que depende solo de y)

### luego el factor integrante apropiado es 


# $p(y)=e ^{\int\frac{1}{N}(\frac{\delta M}{\delta y}-\frac{\delta N}{\delta x})dy}$

## $=e^{\int{-\frac{1}{y}}dy}=e^{-ln(y)}=\frac{1}{y}$ 

### luego $p(y)=\frac{1}{y}$ 

# $2xyln(y)dx+(x²+y²\sqrt{y²+1})dy=0$ 

## -> $2xln(y)dx+\frac{x²+y²\sqrt{y²+1}}{y}dy=0$ 

## entonces: $M=2xln(y)dx$ ; $N=\frac{x²+y²\sqrt{y²+1}}{y}dy$ 

## observe que esta ecuación es exacta, pues:

# $\frac{\delta M}{\delta y}=\frac{2x}{y}=\frac{\delta N}{\delta x}$ 

### por lo tanto, existe una función escalar $\phi(x,y)=c$, tal que su diferencial es:

# $d\phi=\frac{\delta\phi}{\delta x}dx+\frac{\delta\phi}{\delta y}dy=2xln(y)dx+(\frac{x²}{y}+y\sqrt{y²+1})=0$ ## comparando. 

## a) $\frac{\delta \phi}{\delta x}=2xln(y)$ y b) $\frac{\delta\phi}{\delta y}=\frac{x²}{y}+y\sqrt{y²+1}$ 


### integrando (a) con respecto a $x$: 

# $\phi(x,y)=\int{2xln(y)}dx=x²ln(y)+C(y)$ 
### derivando con respecto a $y$:

## $\frac{\delta \phi}{\delta y}=\frac{x²}{y}+C'(y)$

## comparando con (b), tenemos:

# $\frac{x²}{y}+C'(y)=\frac{x²}{y}+y\sqrt{y²+1}$

# -> $C'(y)=y\sqrt{y²+1}$ 

# -> $C(y)=\int{y\sqrt{y²+1}dy}=\frac{1}{2}\int{\sqrt{u}du}=\frac{1}{2}\frac{u^{\frac{3}{2}}}{\frac{3}{2}}+cte$ 
# = $\frac{1}{3}(y²+1)^{\frac{3}{2}}+cte$ 


## entonces, $C(y)=\frac{1}{3}\sqrt{(y²+1)³}+cte$ 

### luego, la solución de la ecuación es, en su forma implicita :

## $\phi(x,y)=x²ln(y)+\frac{1}{3}\sqrt{(y²+1)³}$ 


## Ejercicio Propuesto: 

## Resolver la ecuación: $(2xy+y⁴)dx+(3x²+6xy³)dy=0$ 

### respuesta: $\phi(x,y)=x²y²+xy⁶=C$ 


# Ecuaciones diferenciales Homogeneas

### def: FUnción homogenea, una función $f(x,y)$ se le dice homogenea de grado $n$, si $f(tx,ty)=t^{n}f(x,y)$ 

## ejemplo: Verificar si la función $f(x,y)=2x³-5xy²+4y³$ es homogénea y determine su grado


## Respuesta: 
# $f(tx,ty)=2(tx)³-5(tx)(ty)²+4(ty)³=2t³x³-5t³xy²+4t³y³=t³(2x³-5xy²+4y^3)=t³f(x,y)$ 
### por lo tanto, la función es homogenea de grado 3 


## Def: Ecuación diferencial Homogénea

### La ecuación $M(x,y)dx+N(x,y)dy=0$ se dice homogénea si $M$ y $N$ son funciones homogeneas 

### obs importante: La ecuación $M(x,y)dx+N(x,y)dy=0$ se puede escribir en la forma: 

# $\frac{dy}{dx}=-\frac{M(x,y)}{N(x,y)}$ o bien $\frac{dy}{dx}=G(x,y)$ 

## Por lo tanto, la ecuación $\frac{dy}{dx}=G(x,y)$ es homogénea si $G(x,y)$ es una función homogénea de grado 0, así la ecuación $\frac{dy}{dx}=G(x,y)$, será homogénea siempre que la función $G(x,y)$ no dependa de $x$ o de $y$ separadamente, sino que de su razón $\frac{y}{x}$ o $\frac{x}{y}$. Por lo tanto las ecuaciones homogeneas tienen la forma: 

# $\frac{dy}{dx}=f(\frac{y}{x})$ o $\frac{dy}{dx}=f(\frac{x}{y})$ 


## Metodo de solución: 

### Una ecuación homogénea. 

# $M(x,y)dx+N(x,y)dy=0$ , se resuelve reduciendola a una de variables separadas, usando cualquiera de las sustituciones:

# $v=\frac{y}{x}$ o bien $v=\frac{x}{y}$ 

### donde $v$ es una nueva variable. 

### obs: Cualquiera de las dos sustituciones anteriores reducen una ecuación homogénea a una de variables separadas. Se sugiere usar :

### - $y=vx$ si $N$ tiene una estructura más simple que $M$ 
### - $x=vy$ si $M$ tiene una estructura más simple que $N$ 


## Ejemplo: Resolver la ecuación siguiente:

# $(x³+y³)dx-xy²dy=0$ 

### Respuesta: Aquí el $M(x,y)=x³+y³$ y $N(x,y)=-xy²$ 
### Como $M$ y $N$ son funciones homogeneas de grado $3$ (Verificar), la ecuación dada es homogénea. Además $N$ tiene una estructura algebraica más sencilla que $M$, por lo tanto hacemos la susttución $y=vx$. de donde se obtiene. 

# $\frac{dy}{dx}=v+x\frac{dv}{dx}$ -> $dy=vdx+xdv$ 
### Sustituyendo en la ecuación queda: 

# $(x³+y³)dx-xy²dy=0$ 

# <-> $x³+(vx)³dx-x(vx)²\cdot{(vdx+xdv)}=0$ 
# -> $(x³+v³x³)dx-x³v²(xdv+vdx)=0$
# -> $x³(1+v³)dx-x³v²(xdv+vdx)=0$ 
# -> $(1+v³)dx-v²(xdv+vdx)=0$ 
# -> $dx+v³dx-xv²dv-v³dx=0$ 
# -> $dx-xv²dv=0$ (EDO de variables separadas)
# -> $\frac{dx}{x}=v²dv$ / $\int()$ 
# -> $ln|x|+ln|c|=\frac{v³}{3}$ 
# -> $ln|cx| =\frac{v³}{3}$ -> $v^3=3ln|cx|$ ; $c$ cte.
# -> $(\frac{y}{x})³=3ln|cx|$ -> $y=x\sqrt[3]{3ln|cx|}$ ; $c$ constante


### Ejemplo : Resolver la ecuación $2xydx+(y²-3x^2)dy=0$ 

## Respuesta: Aqui $M(x,y)=2xy$ ; $y³-3x²=N(x,y)$ 

### Note que $M$ tiene una estructura más simple que $N$. hacemos la sustitución $v=\frac{x}{y}$ -> $x=vy$ -> $\frac{dx}{dy}=v+y\frac{dv}{dy}$ -> $dx=vdy+ydv$ 

### Sustituyendo en la ED: 

### $2yvy(vdy+ydv)+(y²-3(yv)²)dy=0$ 
## -> $2y²v(vdy+ydv)+(y²-3y²v^2)dy=0$ 
## -> $2v^{2}y²dy+2y³vdv+y²dy-3y²v²dy=0$ 
# -> $2y³vdv+y^{2}dy-y²v²dy=0$ 
# -> $2vdv+dy-v²dy=0$ 
# -> $2vydv+(1-v^2)dy=0$ 
# -> $(1-v^2)dy=-2vydv$ (Variables separables)
# -> $\frac{dy}{y}=-\frac{2v}{1-v^2}dv/\int()$ 
# -> $ln|y|=ln|1-v^{2}|+ln|c1|$ 
### sustituyendo devuelta:
# -> $ln|y|=ln|1-\frac{x²}{y^2}|+ln|c1|$ 
# -> $ln|\frac{y³}{y²-x²}|=ln|C1|$ -> $|\frac{y^3}{y^2-x²}|=|c1|$ -> $|y³|=|c1(y²-x²)|$ 

### o bien $y³=c1(y^2-x^2)$ (solución implicita)

### OBS: nose lol







### Ejercicio: Resolver la ecuación: 

# $\frac{dy}{dx}=\frac{x+y+4}{x-y-6}$ (pista: buscar sustitución para convertirla en homogénea)

### Respuesta: Hacemos la sustitución:

### $x=z+h$ e $y=w+k$ donde $(h,k)$ es la solución del sistema: $x+y+4=0$ y $x-y-6=0$ <-> $x+y=-4$ y $x-y=6$ 

### -> $x=1$ y $y=-5$ 

### luego, $(h,k)=(1,-5)$ 
### entonces, $x=z+1$ , y $y=w-5$ -> $dx=dz$ y $dy=dv$ 


### luego, la ecuación queda: 

### $\frac{dw}{dz}=\frac{z+w}{z-w}=\frac{1+\frac{w}{z}}{1-\frac{w}{z}}=f(\frac{w}{z})$ (Ecuación homogenea) (1)

### Sea $v=\frac{w}{z}$ entonces, $w=vz$ -> $dw=vdz+zdv$ 

### Sustituyendo en (1):

### -> $\frac{dw}{dz}=\frac{z+w}{z-w}$
### <-> $\frac{vdz+zdv}{dz}=\frac{z+vz}{z-vz}$ 
### <-> $v+z\frac{dv}{dz}=\frac{z(1+v)}{z(1-v)}$ 
### <-> $v+z\frac{dv}{dz}=\frac{1+v}{1-v}$ y
### <-> $z\frac{dv}{dz}=\frac{1+v}{1-v}-v$ 
### <-> $z\frac{dv}{dz}=\frac{1+v²}{1-v}$ (Variables separables :0)

### -> $\int\frac{1-v}{1+v²}dv=\int\frac{dz}{z}+C$ 
### -> $\int\frac{1}{1+v²}dv-\int\frac{v}{1+v²}dv=\int\frac{dz}{z}+C$ 
### <-> $artan(v)-\frac{1}{2}ln|1+v²|=ln|z|+C$ 
### -> $arctan(\frac{w}{z})-\frac{1}{2}ln|1+(\frac{w}{z})²|=ln|z|+C$ 
### -> $arctan(\frac{y+5}{x-1})-\frac{1}{2}ln(1+(\frac{y+5}{x-1})²)=ln|x-1|+C$ (Solución general en su forma implicita)

### OBS: Si las rectas son paralelas, el metodo anterior no se puede aplicar. En este caso hacemos la sustitución $u=ax+by$ ; $du=adx+bdy$, dá origen a una EDO de variables separables. 

### Por ejemplo: Resolver la EDO: 
# $\frac{dy}{dx}=\frac{2x+3y+9}{4x+6y-7}$ (2)

### respuesta: Note que las rectas $2x+3y+9=0$ y $4x+6y-7=0$ son paralelas, entoncees hacemos la sustitución $u=ax+by=2x+3y$ 

# -> $du=2dx+3dy$ 
# -> $\frac{du}{dx}=2+3\frac{dy}{dx}$ 

# -> $\frac{dy}{dx}=(\frac{du}{dx}-2)\frac{1}{3}$ o bien 

# sustituyendo en (2):

# -> $\frac{dy}{dx}=\frac{u+9}{2u-7}=\frac{1}{3}(\frac{du}{dx}-2)$ 
# -> $\frac{du}{dx}=\frac{3u+2y}{2u-7}+2=\frac{7u+13}{2u-7}$ 
# -> $\frac{du}{dx}=\frac{7u+13}{2u-7}$ (Variables Separables)
# -> $\frac{2u-7}{7u+12}du=dx$ (Resolver)

# Ecuación de bernuli 
### Ejercicio: Considere la E.D no lineal: 
# $\frac{dy}{dx}+p(x)y=f(x)y^x$ ; $n\not=0$ y $n\not=1$ ; $n\in{R}$ (3)

### Muestre que el cambio de variable $z=y^{1-n}$ transforma la ecuación dada en una ecuación lineal.

### Respuesta: Sea $z=y^{1-n}$, derivando respecto a $x$:

# $\frac{dz}{dx}=(1-n)y^{-n}\frac{dy}{dx}$ 

### Remplazo en (3):
# -> $\frac{dz}{dx}=(1-n)y^{-n}\frac{dy}{dx}$ 
# -> $\frac{dz}{dx}=(1-n)y^{-n}[f(x)y^n-p(x)y]$ 
# $=(1-n)f(x)-(1-n)p(x)y^{1-n}$ 
# $=(1-n)f(x)-(1-n)p(x)z$ 
### luego: 
# $\frac{dz}{dx}=(1-n)f(x)-(1-n)p(x)z$ 
# -> $\frac{dz}{dx}+(1-n)p(x)z=(1-n)f(x)$ (EDO lineal de primer orden)
## La EDO (3), se llama ecuación de Bernulli:

# $\frac{dy}{dx}+p(x)y=f(x)y^{n};n\not=0;n\not=1;n\in{R}$ 
### $z=y^{1-n}$ 

## Ejercicio: 

### Encuentre la solución general de la EDO.:

# $x\frac{dy}{dx}+y+xy²=0$ 

### Respuesta : $x\frac{dy}{dx}+y+xy²=0 / \cdot\frac{1}{x};x\not=0$ 

# -> $\frac{dy}{dx}+\frac{1}{x}y=-y^{2}$ (Ecuación de Bernulli)

### Sea $z=y^{-1}$ -> $\frac{dz}{dx}=\frac{-1}{y²}\frac{dy}{dx}$ 
### -> $\frac{dz}{dx}=\frac{-1}{y²}(-y²-\frac{1}{x}y)$ 
### -> $\frac{dz}{dx}=1+\frac{1}{x}z$ 
### -> $\frac{dz}{dx}-\frac{1}{x}z=1$ (Edo lineal)
### Factor integrante: $\mu(x)=e^{-\int\frac{1}{x}dx}=e^{ln(x^{-1})}=\frac{1}{x}$ 
### -> $\frac{1}{x}\frac{dz}{dx}-\frac{1}{x²}z=\frac{1}{x}$ 
### -> $\frac{d}{dx}(\frac{1}{x}z)=\frac{1}{x}/\int$ 
### -> $\frac{1}{x}z=\int\frac{1}{x}dx+C$ 
### -> $\frac{1}{x}z=ln|x|+C$ (Solución en su forma implicita) ; $x\in{]0,+\infty[}$ 
### -> $z(x)=xln(x)+Cx$ 
### -> $\frac{1}{y}=xln(x)+Cx$ 
### -> $y(x)=\frac{1}{xln(x)+Cx}$ ; $C$ constante.

# Ecuaciones diferenciales lineales de orden n

Forma General:  $a_n(x)y^{(n)}+a_{n-1}(x)y^{(n-1)}+...+a_1(x)y'+a_0(x)y=R(x)$ 
Si las funciones $a_i(x)$ son constantes $\forall{i}$, la ecuación diferencial lineal de orden $n$, se llama de "coeficientes constantes", caso contrario de "coeficientes variables".

### Ejemplo : 
1. $5y'''+3y''-7y'+4=2e^{-x}+7x²$ (EDO lineal de coeficientes constantes de orden 3)
2. $xy''+3y'+x²y=x²-7$ (EDO lineal de orden 2 de coeficientes variables)

# Ecuación diferencial lineal de segundo orden

Forma General: $\frac{d²y}{dx²}+P(x)\frac{dy}{dx}+Q(x)y=R(x)$ (1)
Esta ecuación se llama "Ecuación lineal de segundo orden" en la variable $y$. 

Si $R(x)=0$, la ecuación se llama homogénea de segundo orden de coeficientes variables, caso contario no homogénea. 

### Teorema: 
Sean $P(x),Q(x)$ y $R(x)$ funciones continuas en el intervalo $[a,b]$. SI $x_0$ es cualquier punto de $[a,b]$ e $y_0$, $y'_0\in{R}$ son constantes arbitrarias, la ecuación (1) tiene una unica solución $y(x)$ en $[a,b]$, que satisface la condiciones iniciales: 
# $y(x_0)=y_0$ ; $y'(x_0)=y'_0$ 

# Ecuación diferencial lineal de segundo orden homogénea 

Forma General: $\frac{d²y}{dx²}+P(x)\frac{dy}{dx}+Q(x)y=0$ (2)
### Teorema: 
Si $y_1(x)$ e $y_2(x)$ son soluciones de (2), entonces $c_1y_1(x)+c_2y_2(x)$ tambien es solución de (2), para $c_1,c_2\in{R}$. 
### Teorema. 
Si $y_1(x)$ e $y_2(x)$ son soluciones linealmente independientes de (2) en un intervalo $[a,b]$, entonces la solución general de (2) es:
# $y_G(x)=c_1y_1+c_2y_2$ ; $c_1,c_2\in{R}$ 

### Def: 
Si $y_1,y_2$ son soluciones de la ecuación (2) ;  Se define el "Wronkiano" de $y_1$ e $y_2$, como:
# $W(y_1,y_2)=`\begin{vmatrix}   y_1 & y_2\\   y'_1 & y'_2    \end{vmatrix}`$ $=y_1y'_2-y_2y'_1$ 

### Teorema: Dos soluciones $y_1$ e $y_2$de la ecuación (2), son linealmente independientes si y solo si $W(y_1,y_2)\not=0$ 

### Ejemplo: Muestre que la ecuaciín $y''+y=0$ tiene solución general $y(x)=C_1sin(x)+C_2cos(x)$. Encuentre ademas la solución particular para la cual $y(0)=2$ y $y'(0)=3$ 

### Teorema: 
Si $y_1(x)$ es una solución de la ecuación homogenea: 
# $y''+P(x)y++Q(x)y=0$ 

entonces, una segunda solcuión linealmente independiente con $y_1(x)$, esta dada por:
# $y_2(x)=y_1\int\frac{1}{y_1²(x)}e^{\int{-p(x)dx}}dx$ 

### Demostración
Supongamos que podemos encontrar una función $v(x)$, tal que $y_2(x)=v(x)y_1(x)$, sea otra solución de la ecuación homogénea, tal que $y_1(x)$ e $y_2(x)$ sean linealmente independientes (l.i), tenemos:

## $y_2(x)=v(x)y_1(x)\rightarrow{y'_2(x)=v'y_1+vy_1' }$ 
## $\Rightarrow{y_2''(x)}=v''y_1+2v'y_1'+vy_1''$ 

Sustituyendo en la ecuación queda:

### $\Rightarrow{(v''y_1+2v'y_1'+vy_1'')+P(v'y_1+vy_1')+Q(vy_1)}=0$ 
### $\Rightarrow{v(y_1''+Py_1'+Qy_1)+v''y_1+v'(2y_1'+Py_1)}=0$ ; $y_1''+Py_1'+Qy_1=0$ (solución de (2)) 
### $\Rightarrow{v''y_1+v'(2y_1'+Py_1)}=0$ 
### $\Rightarrow{v''y_1}=-v'(2y_1'+Py_1)$ 
### $\Rightarrow{\frac{v''}{v'}}=-\frac{2y_1'+Py_1}{y_1}$ 
### $\Rightarrow\frac{v''}{v'}=-\frac{2y'}{y_1}-P$ / $\int()$ 
### $\Rightarrow{ln(v')}=-2ln(y_1)-\int{Pdx}$ / $e^{()}$
### $\Rightarrow{v'}=e^{-2ln(y_1)}e^{-\int{Pdx}}$ 
### $\Rightarrow{v'}=\frac{e^{-\int{Pdx}}}{y_1²}$ $\Rightarrow{v}=\int{\frac{e^{-\int{Pdx}}}{y_1²}dx}$ $\Rightarrow{y_2}=y_1\cdot{\int{\frac{e^{-\int{Pdx}}}{y_1²}}}$ 

### Falta demostrar que $y_1,y_2$ son l.i, esto es $W(y_1,y_2)\not=0$ 

### $\Rightarrow{W(y_1,y_2)}=e^{-\int{Pdx}}\not=0;\forall{x}$ 

# Ejercicio Propuesto: 

Para $x>-1$, resuelva la ecuación diferencial: 
# $(x+1)³y''+3(x+1)²y'+(x+1)y=0$

Sabiendo que $y_1(x)=\frac{1}{x+1}$ es solución de la ecuación.

### Respuesta: 

$(x+1)³y''+3(x+1)²y'+(x+1)y=0$ / $\frac{1}{(x+1)³}$ 
$\Rightarrow{y''}\frac{3}{x+1}y'+\frac{1}{(x+1)²}y=0$ 
como $y_1(x)=\frac{1}{x+1}$ es solución, entonces usando la formuma de Abel, determinemos $y_2(x)$.

### $y_2(x)=y_1\int\frac{1}{y_1²}e^{-\int{Pdx}}=\frac{1}{x+1}\int{e^{-\int{\frac{3}{x+1}dx}}}\frac{1}{\frac{1}{(x+1)²}}dx$ 
### $=\frac{1}{x+1}\int{(x+1)²}\frac{1}{(x+1)³}dx=\frac{1}{x+1}\int{\frac{1}{x+1}dx}=\frac{ln(x+1)}{x+1}=y_2(x)$ 

### faltaria probar que $y_1(x)$ e $y_2(x)$ $\forall{x}>-1$   son l.i :oo

### $W(y_1,y_2)=\frac{1}{(x+1)³}>0 ; \forall{x>-1}$


### Aplicaciones de las edos importantes: 
- Población (Variables separadas)
- Temperatura (Bernoulli)
- Estanques (Lineales de orden 1)


# Ejercicios Certamen 1

### 1. La ED $y'=y(1-y)$ modela el crecimiento de una población con restricción de recursos. Asuma que existe un limite al tamaño maximo de la población que el medio ambiente puede soportar, el cual es igual a 1 en nuestro modelo. Sea $y(t)$ el tamaño de ña población en el tiempo $t$, y la razón de cambio de la población $y'(t)$ es proporcional al tamaño existente de la población $y$ , y a la diferencia respecto de la población limite $1-y$ 

#### a) Obtenga la solución general de la EDO dada
#### b) Asuma $y(0)=\frac{1}{2}$. obtenga la solución particular a este P.V.I, y describa el comportamiento de la població cuando $t\to{\infty}$ 

### Solución (a):

$y'=y(1-y)$ $\Rightarrow{\frac{dy}{dx}}=y(1-y)\Rightarrow{\frac{dy}{y(1-y)}}=dt$ / $\int($ ) ; $y\not=1$ 
$\Rightarrow{\int{\frac{1}{y}+\frac{1}{1-y}}}dy=t+C$ 
$\Rightarrow{ln(y)-ln(1-y)}=t+C_1\Rightarrow{ln|\frac{y}{1-y}|}=t+C_1\Rightarrow{\frac{y}{1-y}}=Ce^{t}$ 
$\Rightarrow{y}=\frac{Ce^t}{1+Ce^t}$ (Solución General)
Note que, se tienen dos soluciones:
- $y=0$ (que se puede obtener de la solución general para $C=0$ )
- $y=1$ (Solución singular, no se obtiene a partir de la solución general)
### Solución (b):

si $y(0)=\frac{1}{2}$ $\Rightarrow{\frac{C}{1+C}}=\frac{1}{2}\Rightarrow{C=1}$
$\Rightarrow{y(t)}=\frac{e^t}{1+e^t}$, Así $t\to{\infty}\Rightarrow{y\to{1}}$ 
### 2. Resuelva la ecuación $y'=\frac{e^{\sqrt{x}}+x}{\sqrt{x}}$ 
Se tiene $\frac{dy}{dx}=\frac{e^{\sqrt{x}}+x}{\sqrt{x}}$ (de variables separables)
$\Rightarrow{dy}=\frac{e^{sqrt{x}}+x}{x}dx$ / $\int()$ 
$\Rightarrow{\int dy}=\int{\frac{e^{\sqrt{x}}+x}{\sqrt{x}}}dx+C$ ; Sea $z=\sqrt{x}$ $\Rightarrow{dz}=\frac{1}{2\sqrt{x}}dx$
$\Rightarrow{y}=\int{(e^{z}+z²)}dz$ $\Rightarrow{y}=2(e^{z}+\frac{z³}{3})+C$ (Remplazando z a la variable original, queda la solución en su forma general)


### 3. Resolver la EDO $\frac{dx}{dy}+\frac{2(1-y)}{y}x=\frac{e^{y}}{y}$ ; $P(y)=\frac{2(1-y)}{y}$ y $Q(y)=\frac{e^{y}}{y}$ 
Esta es una EDO lineal de primer orden, donde su factor integrante $\mu$ es:
$\mu(y)=e^{\int P(y)}dy=e^{\int\frac{2}{y}-2dy}=e^{2ln|y|-2y}=y²e^{-2y}$ 
$\Rightarrow{\frac{dx}{dy}+\frac{2(1-y)}{y}x=\frac{e^{y}}{y}}$ / $\mu(y)$ 
$\Rightarrow{\frac{d}{dy}(\mu(y)x)}=ye^{-y}$ / $\int()$ 
$\Rightarrow{\mu(y)x=}\int ye^{-y}dy+C$
$\Rightarrow y²e^{-2y}x=-e^{-y}(y+1)+C$ 
$\Rightarrow{x}=\frac{e^{y}(y+1)}{y²}+C_1$ (Solución General en forma explicita)

### 4. Resolver la EDO $(\frac{y}{x²}+2)dx+\frac{1}{x}(1+ln(xy))dy=0$ 

Note que $M(x,y)=(\frac{y}{x²}+2)$ y $N(x,y)=\frac{1}{x}(1+ln(xy))$ 
$\Rightarrow{\frac{\delta M}{\delta y}}=\frac{1}{x²}$ y $\frac{\delta N}{\delta x}=-\frac{ln(xy)}{x²}$ 
dado $\frac{\delta M}{\delta y}\not=\frac{\delta N}{\delta x}$ la ecuación no es exacta.
entonces, tenemos $\frac{\frac{\delta M}{\delta y}-\frac{\delta N}{\delta x}}{N}$ = $\frac{1}{x}$, entonces el factor integrante es $\mu(x)=e^{\int \frac{1}{x}dx}=ln|x|$  que solo depende de $x$. 

$(\frac{y}{x²}+2)dx+\frac{1}{x}(1+ln(xy))dy=0$ / $x$
$\Rightarrow$ $(\frac{y}{x}+2x)dx+(1+ln(xy))dy=0$ (exacta :0) ; $M(x,y)=\frac{y}{x}+2x$ y $N(x,y)=1+ln(xy)$ 
donde $\frac{\delta M}{\delta y}=\frac{1}{x}=\frac{\delta N}{\delta x}$ 
$\Rightarrow$ existe un $\phi(x,y)=C$ tal que:
$\frac{\delta \phi}{\delta x}=\frac{y}{x}+2x$ y $\frac{\delta\phi}{\delta y}=1+ln(xy)$ donde la más sencilla es $M(x,y)$ 


### 5. Resolver $\frac{dy}{dx}=\frac{xy+2y-x-2}{xy-3y+x-3}$ 

### 6. Resolver $(2xy+y⁴)dx+(3x²+6xy³)dy=0$ 











 