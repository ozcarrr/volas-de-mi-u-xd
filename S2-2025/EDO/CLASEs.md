
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


# $p(y)=e ^{\int\frac{1}{N}(\frac{\delta N}{\delta x}-\frac{\delta M}{\delta y})dy}$

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
# $\frac{dy}{dx}+p(x)y=f(x)y^n$ ; $n\not=0$ y $n\not=1$ ; $n\in{R}$ (3)

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

### Respuesta : $x\frac{dy}{dx}+y+xy²=0 / \cdot\frac{1}{x};x>0$ 

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
# $W(y_1,y_2)=\begin{vmatrix}   y_1 & y_2\\   y'_1 & y'_2    \end{vmatrix}$ $=y_1y'_2-y_2y'_1$ 

### Teorema: Dos soluciones $y_1$ e $y_2$de la ecuación (2), son linealmente independientes si y solo si $W(y_1,y_2)\not=0$ 

### Ejemplo: Muestre que la ecuación $y''+y=0$ tiene solución general $y(x)=C_1sin(x)+C_2cos(x)$. Encuentre ademas la solución particular para la cual $y(0)=2$ y $y'(0)=3$ 

### Teorema: 
Si $y_1(x)$ es una solución de la ecuación homogenea: 
# $y''+P(x)y'+Q(x)y=0$ 

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
$\Rightarrow{y''}+\frac{3}{x+1}y'+\frac{1}{(x+1)²}y=0$ 
como $y_1(x)=\frac{1}{x+1}$ es solución, entonces usando la formuma de Abel, determinemos $y_2(x)$.

### $y_2(x)=y_1\int\frac{1}{y_1²}e^{-\int{Pdx}}=\frac{1}{x+1}\int{e^{-\int{\frac{3}{x+1}dx}}}\frac{1}{\frac{1}{(x+1)²}}dx$ 
### $=\frac{1}{x+1}\int{(x+1)²}\frac{1}{(x+1)³}dx=\frac{1}{x+1}\int{\frac{1}{x+1}dx}=\frac{ln(x+1)}{x+1}=y_2(x)$ 

### faltaria probar que $y_1(x)$ e $y_2(x)$ $\forall{x}>-1$   son l.i :oo

### $W(y_1,y_2)=\frac{1}{(x+1)³}\not=0 ; \forall{x>-1}$


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


# Ecuación diferencial lineal de 2do orden homogenea de coeficientes constantes: 


### Forma : $y''+Py'+Qy=0$ (1)
donde $P$ y $Q$ son constantes, recuerde que la solución general de (1) en $[a,b]$, tiene la forma: 

$y_G(x)=C_1y_1+C_2y_2$, $C_1,C_2$ constantes 

donde $y_1$ e $y_2$ son soluciones l.i de la ecuación (1). 


OBS : Note  que para encontrar la solución general de (1), solo necesitamos encontrar dos soluciones indpependientes de la ecuación. 

Buscaremos soluciones del tipo exponencial, esto es, de la forma $y=e^{mx}$; $m\in{R}$. Tenemos: 

$y'=me^{mx}$ ; $y''=m²e^{mx}$ 

Por lo tanto, si $y=e^{mx}$ satisface la ecuación (1) ; $y''+Py'+Qy=0$, se tendra: 

$y''+Py'+Qy=m²e^{mx}+Pme^{mx}+Qe^{mx}$ 
$=e^{mx}(m²+Pm+Q)=0$ ; dado $e^{mx}>0;\forall{x}$ 
$\Rightarrow m²+Pm+Q=0$ 

Definición: Llamaremos "Ecuación característica" asociada a la edo (1), a la ecuación cuadratica: 
$$m²+Pm+Q=0$$
Como la ecuación cuadrática tiene $3$ posibilidades de solución, que dependen de su discriminante: 

$$\Delta = P²-4Q$$
Se distinguen tres casos: 

- "Raices reales diferentes" $\Delta>0$ 
Si la ecuación característica tiene dos soluciones reales distintas, digamos $m_1$ y $m_2$ , entonces, la solución general de la EDO (1) es: 
$$y_G(x)=C_1e^{m_1x}+C_2e^{m_2x}$$
donde $C_1$ y $C_2$ son constates y: 
$$y_1=e^{m_1x},y_2=e^{m_2x}$$
Son soluciones l.i de la edo (1)

- "Raices imaginarias" $\Delta<0$ 
en este caso, $m_1=a-bi$ y $m_2=a+bi$ 
$\Rightarrow y_1(x)=e^{(a-bi)x}$ e $y_2(x)=e^{(a+bix)}$ son soluciones complejas de la edo (1)
Para encontrar las soluciones reales, las expresamos en su forma polar: 

$$y_1(x)=e^{ax}e^{-bi}=e^{ax}(cos(bx)-isin(bx))$$
$$y_2(x)=e^{ax}e^{bi}=e^{ax}(cos(bx)+isin(bx))$$
Entonces, la solución general queda de la forma: 
$$y_G(x)=e^{ax}(C_1cos(bx)+C_2sin(bx))$$

- "Raices iguales" $\Delta=0$ 
En este caso, hay raiz real de multiplicidad 2, donde $m=-\frac{p}{2}$, entonces: 
$$y_1(x)=e^{-\frac{p}{2}x}$$
Para encontrar $y_2$ usamos la formula de abel: 
$$y_2(x)=y_1(x)\int\frac{e^{-\int p(x)dx}}{y_1²(x)}dx;p(x)=p\in{R}$$
$$\Rightarrow y_2(x)=xe^{-\frac{p}{2}x}$$
$$\Rightarrow y_G(x)=e^{-\frac{p}{2}x}(C_1+C_2x)$$
Donde $C_1$ y $C_2$ son constantes
Ejercicios :

$I)$ Encuentre la solución del problema de valor inicial: 
$$y''-6y'+5y=0;y(0)=3;y'(0)=11$$
$II)$ Encuentre la solución general de: 
$$2y''-4'+8y=0$$
$III)$ Resuelva el P.VI:
$$y''+6y'+9y=0;y(0)=0;y'(0)=6$$

# Ecuación diferencial lineal de 2do orden no homogénea: 

### Forma: $\frac{d²y}{dx²}+P(x)\frac{dy}{dx}+Q(x)y=R(x)$ 
donde $P(x),Q(x),R(x)$ son funciónes de $x$. 
### Ecuación lineal de 2do orden no homogénea de coeficientes constantes 
#### Forma: $y''+py'+qy=r(x)$ ; $p,q$ constantes (1)

#### Solución general de (1): 

$y_G(x)=y_h(x)+y_p(x)$ 

donde $y_H(x)$ es solución general de la edo (1) en un cierto intervalo $[a,b]$, e $y_p(x)$ es una solución particular de la edo (1). 

#### OBS:
- Para resolver la ecuación homogénea asociada, se estudian las raices de la ecuación caracteristica. 
- Para encontrar la solución general de (1), solo necesitamos encontrar una solución  particular de ella. 
### Metodo de los coeficientes indeterminados

Los coeficientes indeterminados Se usan para encontrar una solución particular de la EDO lineal de 2do orden no homogénea de coeficientes constantes: 

$$y''+py'+qy=r(x);p,q\in{R}$$
#### OBS: 
Si $r(x)$ es del tipo exponencial, seno, coseno, polinomial o es suma y productos de estas. Es decir, es de la forma: 
$$r(x)=e^{\alpha x}(p(x)cos(\beta x)+q(x)sin(\beta x))$$
donde $p(x),q(x)$ son polinomios, entonces podemos suponer que una solución particular tiene la misma forma. 

#### Ejemplo: 
Para la ecuación de segundo orden:
$$y''-y'-2y=4x²$$
es esperable que su solución particular sea un polinomio de grado 2, de la forma:
$$y_p(x)=A+Bx+Cx²;A,B,C\in{R}$$
En este caso, basta derivar dos veces $y_p(x)$ y sustituir en la ecuación, obteniendo $y_p(x)=-3+2x-2x²$ (verificar).

#### Casos:
En el método de coeficientes indeterminados se distiguen 3 casos:

##### Caso 1: $r(x)=ae^{\lambda x}$ 
- si $\lambda\not=m_1$ y $\lambda\not=m_2$, donde $m_1$ y $m_2$ son las raices del polinomio caracteristico, entonces la solución particular queda de la forma: 

$$y_p(x)=Ae^{\lambda x}$$
dodne $A$ es una constante a determinar. 

- Si $\lambda =m_1$ y $\lambda\not=m_2$ , entonces la solución particular queda de la forma: 
$$y_p(x)=Axe^{\lambda x}$$
donde $A$ es una cte a determinar.

- Si $\lambda=m_1$ y $\lambda=m_2$, entonces la solución particular queda:
$$y_p(x)=Ax²e^{\lambda x}$$
donde $A$ es una constate a determinar. 

Nota: si $\lambda=m_1=m_2=...=m_n$, entonces :
$$y_p(x)=Ax^ne^{\lambda x}$$
##### Caso 2: $r(x)=A_0+A_1x+A_2x²+...+A_nx^n$ 

- Si $q\not=0\Rightarrow y_p(x)=B_0+B_1x+...+B_nx^n$ 
donde los $B$ son constates a determinar

- Si $q=0\Rightarrow y_p(x)=x(B_0+B_1x+...+B_nx^n)$ 
donde los $B$ son constantes a determinar.

##### Caso 3: $r(x)=sin(\lambda x)$ o $r(x)=cos(\lambda x)$ 
obs: $m=a+bi$ 
- Si $\lambda\not=b\Rightarrow y_p(x)=Asin(x)+Bcos(x)$ 
- SI $\lambda=b\Rightarrow y_p(x)=x(Asin(\lambda x)+Bcos(\lambda x))$ 
donde $A$ y $B$ son constantes a determinar


### Ejercicio: 
Rsolver la ecuación:
$$y''-y'-2y=4x^2 (1)$$
Solución: 
En este caso, $r(x)=4x²$ (polinomio de grado 2)

Ec. característica: $m²-m-2=0$ 

$\Rightarrow (m-2)(m+1)=0\Rightarrow m_1=2;m_2=-1$ 
entonces, $y_H(x)=C_1e^{2x}+C_2e^{-x}$ ; $C_1$ y $C_2$ constantes  (Solución general de la homogénea asociada)

La solución particular de la no homogénea tiene la forma:
$$y_p(x)=A+Bx+Cx²;A,B,C\in{R}$$
Tenemos:

$y_p'=B+2Cx$ ; $y_p''=2C$ 
Sustituyendo en (1):

$2C-(B+2C)-2(A+Bx+Cx²)=4x²$ 
$\Rightarrow (2C-B-2A)-(2C+2B)x-2Cx²=4x²$ 
Por igualdad de polinomios tenemos: 

$2C-B-2A=0$ 
$-2C-2B=0$ 
$-2C=4$ 

$\Rightarrow$ $C=-2$ ; $B=2$ ; $A=-3$ 

POr lo tanto: $y_p(x)=-3+2x-2x²$ 

Luego, la solución general de la no homogénea es:
$$y(x)=y_h(x)+y_p(x)=C_1e^{2x}+C_2e^{-x}+(-3+2x-2x²)$$
donde $C_1$ y $C_2$ son constantes. 

# Sustitución adecuada (bajar el orden de la EDO)

### Ejercicio: Resolver la EDO: 

$$xy''=y'ln(\frac{y'}{x});x>0$$

#### Solución

$\Rightarrow x\frac{d²y}{dx²}=\frac{dy}{dx}ln(\frac{y'}{x})$ 
Note que falta la variable dependiente $y$ (tiene que estar 'libre' de otras funciones) por ende hacemos la sustitución $z=y'$ $\Rightarrow z'=y''$ 
Sustituyendo en la edo queda:
$$xz'=zln(\frac{z}{x}) (*)$$
Ecuación de orden 1 homogénea 

Sea $u=\frac{z}{x}\Rightarrow z=ux\Rightarrow z'=u'x+u$ 
$\Rightarrow \frac{dz}{dx}=u'x+u$ 
Sustituyendo en $(*)$, queda: 

$u'x+u=uln(u)\Rightarrow u'x=u(ln(u)-1)$ que es de variables separables
$\Rightarrow \frac{du}{u(ln(u)-1)}=\frac{dx}{x}$ ; $u(ln(u)-1)\not=0$ 

1) si $u(ln(u)-1)=0$ entonces $u=0$ o $u=e$ 

si $u=0$ $\Rightarrow z=0\Rightarrow y(x)=c_1;c_1\in{R}$ 
si $u=e$ $\Rightarrow z= ex\Rightarrow y'=ex\Rightarrow y(x)=e\frac{x²}{2}+c_2$ ; $c_2\in{R}$ 

2) Si $u(ln(u)-1)\not=0$ separamos variables:

$\Rightarrow \frac{du}{u(ln(u)-1)}=\frac{dx}{x}$ / $\int$ 


#### Ejercicio: Resolver la ecuación: 
$$yy''+(y')²=0$$
#### Respuesta: 

Notamos que falta la variable independiente $x$, por ende, usamos la sustitución $z=y'$ , tenemos:
$$y'=z\Rightarrow y''=z'=\frac{dz}{dy}\frac{dy}{dx}=z\frac{dz}{dy}$$
Sustituyendo: 

$$yz\frac{dz}{dy}+z²=0\Rightarrow z(y\frac{dz}{dy}+z)=0$$
entonces $z=0$ o $y\frac{dz}{dy}+z=0$ 

1) Si $z=0\Rightarrow \frac{dy}{dx}=0\Rightarrow y=c$ ; $c$ constante
2) Si $z\not=0$ tenemos:
$y\frac{dz}{dy}+z=0\Rightarrow y\frac{dz}{dy}=-z$ que es de variables separadas
$\Rightarrow ln|z|=-ln|y|+C_1$ $\Rightarrow yz=c_2$ ; $C_1=ln(c_2)$ 
además $z=\frac{dy}{dx}$ $\Rightarrow y\frac{dy}{dx}=C_2$ (variables separadas)

$$\Rightarrow \frac{y²}{2}=C_2x+C_3$$ 
# Continuación (Materia)

### Teorema (Principio de superposición):

SI $y_1$ e $y_2$ son soluciones l.i de:
$$y''+py'+qy=R_1(x)$$ y :
$$y''+py'+qy=R_2(x)$$
Respectivamente, entonces $y_1+y_2$ es solución de: 
$$y''+py'+qy=R_1(x)+R_2(x)$$

### Ejercicio: Resolver la edo:
$$y''-2y'-3y=x-x²+e^{x}$$
#### Respuesta:
1) $y''-2y'-3y=x-x²=R_1(x)$ (1)
2) $y''-2y'-3y=e^{x}=R_2(x)$ (2)

Ec. caracteristica: 
$$m²-2m-3=0$$ $\Rightarrow m_1=3$ v $m_2=-1$ 
entonces, la solución general de la edo homogénea es:
$$y_H(x)=C_1e^{3x}+C_2e^{-x}$$ Solución particular de (1):

- $$y_{p_1}(x)=Ax²+Bx+C\Rightarrow y'_{p_1}=2Ax+B\Rightarrow y''_{p_1}=2A$$
Sustituyendo en la EDO (1), tenemos:

$$2A-2(2Ax+B)-3(Ax²+Bx+C)=x-x²$$
$\Rightarrow 2A-2B-3C=0$ ; $-4A-3B=1$ ; $-3A=-1$ 

$\Rightarrow A=\frac{1}{3}$ ; $B=-\frac{7}{9}$ ; $C=\frac{20}{27}$ 

Entonces: 
$$y_{p_1}(x)=\frac{x²}{3}-\frac{7}{9}x+\frac{20}{27}$$
Luego, por encontrar $y_{p_2}(x)$, note que $y''-2y'-3y=e^x$ $\Rightarrow \lambda=1\not=-1$ y $\lambda\not=3$  

entonces :
$$y_{p_2}(x)=Ae^{x}$$ donde $A$ es constante, entonces, sustituyendo en la ecuación, queda:
$$Ae^x-2Ae^x-3Ae^x=e^x$$
$\Rightarrow A=-\frac{1}{4}$ 
entonces $y_{p_2}(x)=-\frac{1}{4}e^x$ 

finalmente: 
$$y_g(x)=y_{h_1}(x)+y_{p_2}{x}=C_1e^{3x}+C_2e^{-x}+y_{p_1}(x)+y_{p_2}(x)=C_1e^{3x}+C_2e^{-x}+\frac{x²}{3}-\frac{7}{9}x+\frac{20}{27}-\frac{1}{4}e^x$$ 

# Variación de parametros 

Consideremos la ecuación lineal de segundo orden no homogénea de coeficientes variables: 
$$y''+P(x)y'+Q(x)y=R(x)(*)$$
Sabemos que ella tiene como solución general:
$$y_G=y_H+y_P=C_1y_1+C_2y_2+y_P $$
donde $y_H$ es la general de la homogénea asociada y $y_P$ es la solución particular de la no homogénea

Este método consiste en sustituir las constantes $C_1$ y $C_2$ por funciones $v_1(x)$ y $v_2(x)$ tal que $y(x)_P=v_1y_1+v_2y_2$ sea una solución particular de la ecuación no homogénea. 

tomamos entonces:

$y=v_1y_1+v_2y_2 \Rightarrow y'=v_1'y_1+v_1y_1'+v_2'y_2+v_2y_2'$ 
entonces, $y'=v_1'y_1+v_2'y_2+(v_1y_1'+v_2y_2')$ 

asumimos $v_1y_1+v_2'y_2=0$ para simplificar (evitar segundas derivadas de $v_1$ y $v_2$ )

$\Rightarrow y'=v_1y_1'+v_2y_2'$ 
$\Rightarrow y''=v_1'y_1'+v_1y_1''+v_2'y_2'+v_2y_2''$ 
sustituyendo en $(*)$:

$(v_1'y_1'+v_1y_1''+v_2'y_2'+v_2y_2'')+P(v_1y_1'+v_2y_2')+Q(v_1y_1+v_2y_2)=R$ 
$\Leftrightarrow v_1(y_1''+Py_1'+Qy_1)+v_2(y_2''+Py_2'+Qy_2)+(v_1'y_1'+v_2'y_2')=R$ 
luego , $y_1''+Py_1'+Qy_1=0$ y $y_2''+Py_2'+Qy_2=0$ ya que $y_1$ y $y_2$ son soluciones independientes de la EDO homogénea. 

$\Rightarrow v_1'y_1'+v_2'y_2'=R$ 

Asi se obtiene el sistema: 

$v_1'y_1+v_2'y_2=0$ y $v_1'y_1'+v_2'y_2'=R$ 

$$\Rightarrow \begin{pmatrix}   y_1 & y_2 \\   y_1' & y_2'   \end{pmatrix}\cdot \begin{pmatrix}   v_1'\\   v_2'  \end{pmatrix}= \begin{pmatrix}   0\\   R(x)  \end{pmatrix}
$$

Usando la regla de cramer: 

$$\Rightarrow v_1'=\frac{\begin{vmatrix}   0 & y_2\\   R(x) & y_2  \end{vmatrix}}{\begin{vmatrix}   y_1 & y_2 \\   y_1' & y_2'    \end{vmatrix}}=\frac{-y_2R(x)}{W(y_1,y_2)}$$
y 
$$\Rightarrow v_2'=\frac{\begin{vmatrix}   y_1 & 0\\   y_1' & R(x)  \end{vmatrix}}{\begin{vmatrix}   y_1 & y_2 \\   y_1' & y_2'    \end{vmatrix}}=\frac{y_1R(x)}{W(y_1,y_2)}$$

Luego:

$v_1(x)=\int\frac{-y_2R(x)}{W(y_1,y_2)}dx$ 
$v_2(x)=\int\frac{y_1R(x)}{W(y_1,y_2)}dx$

FInalmente, la solución particular de la no homogénea es:

$y_P=v_1y_1+v_2y_2=y_1\int\frac{-y_2R(x)}{W(y_1,y_2)}dx+y_2\int\frac{y_1R(x)}{W(y_1,y_2)}dx$


### Ejercicios 

Resolver: 

a) $y''+2y'+y=e^{-x}ln(x)$

b) Para $x>-1$ :
$(x+1)³y''+3(x+1)²y'+(x+1)y=6ln(x+1)$, sabiendo que$y_1(x)=\frac{1}{x+1}$ es solución de la EDO homogénea. 

#### Respuesta a)

Ec. característica:
$m²+2m+1=0\Leftrightarrow (m+1)²=0$ 
$\Rightarrow m=-1$ 
entonces, $y_H(x)=C_1e^{-x}+C_2xe^{-x}$ ; $y_1(x)=e^{-x}$ y $y_2(x)=xe^{-x}$ 

Calculando el wronkiano: 

$W(y_1,y_2)=e^{-x}(e^{-x}-xe^{-x})+xe^{-2x}=e{-2x}-xe^{-2x}+xe^{-2x}=e^{-2x}>0\forall x$, por ende, son l.i.

##### Calculo de $v_1(x)$ y $v_2(x)$ :

$v_1=\int\frac{-y_2R(x)}{W}dx=\int\frac{xe^{-x}e^{-x}ln(x)}{e^{-2x}}dx=-\int xln(x)dx=\frac{x²}{4}-\frac{x²}{2}ln(x)$ 

analogamente: 

$v_2=\int\frac{y_1R(x)}{W}dx=\int\frac{e^{-x}e^{-x}ln(x)}{e^{-2x}}dx=\int ln(x)dx=xln(x)-x$ 

Luego: 

$y_P(x)=v_1y_1+v_2y_2=(\frac{x^2}{4}-\frac{x²}{2}ln(x))e^{-x}+(xln(x)-x)xe^{-x}=-\frac{3}{4}e^{-x}+\frac{x^2}{2}ln(x)e^{-x}$ 

entonces, la solución general de la edo queda: 

$$y_G(x)=C_1e^{-x}+C_2xe^{-x}+(-\frac{3}{4}e^{-x}+\frac{x²}{2}ln(x)e^{-x})$$
Observación: El metodo variación de parámetros puede extenderse a ecuaciones diferenciales de orden arbitraria.

Dada la ecuación diferencial:

$y^{(n)}+a_{n-1}y^{(n-1)}+...+a_1(x)y'+a_0y=R(x)$ , entonces:

$y_P(x)=y_1\int \frac{V_1R(x)}{W}+y_2\int \frac{V_2R(x)}{W}dx+...+y_n\int\frac{V_nR(x)}{W}dx$ 

es la solución particular buscada, donde $V_k$ es el determinante obtenido de $W$ al sustituir la columna $k$ por el vector $\begin{pmatrix}   0\\   0 \\ 0\\ 0\\...\\1   \end{pmatrix}$

### Ejercicio: Resolver la ecuación:
$$3y'''+5y''-2y'=e^{x}$$

# Ecuación de euler 

### Ejercicio: Considere la EDO: 
$$a_0x²y''+a_1xy'+a_2y=0$$
donde los $a_k$ son ctes.
Pruebe que el cambio de variable $x=e^{t}$, transforma la ecuación dada en una del tipo:
$$b_0\frac{d²y}{dt²}+b_1\frac{dy}{dt}+b_2y=0$$
donde los $b_k$ son constantes.

#### Respuesta: 
Aplicamos sustitución $x=e^t$, donde buscamos $\frac{d²y}{dx²}=?$ y $\frac{dy}{dx}=?$ 

i) Notamos que y esta en función de x y x esta en función de t.
entonces $\frac{dy}{dt}=\frac{dy}{dx}\frac{dy}{dt}\Rightarrow\frac{dy}{dx}=\frac{\frac{dy}{dt}}{\frac{dx}{dt}}$, pero $x=e^t$, por lo tanto:
$\frac{dx}{dt}=e^{t}\Rightarrow\frac{dt}{dx}=e^{-t}$
notemos que ademas, $\frac{dy}{dx}=\frac{dy}{dt}\frac{dt}{dx}=e^{-t}\frac{dy}{dt}$
Luego, para la segunda derivada:
$$\frac{d}{dt}(\frac{dy}{dx})=\frac{d²y}{dx²}\frac{dx}{dt}$$
$\Rightarrow$  $\frac{d²y}{dx^2}=\frac{\frac{d}{dt}(\frac{dy}{dx})}{\frac{dx}{dt}}=\frac{d}{dt}(\frac{dy}{dx})\cdot\frac{dt}{dx}=\frac{d}{dt}(e^{-t}\frac{dy}{dt})\cdot\frac{dt}{dx}=-e^{-t}(\frac{dy}{dt}+e^{-t}\frac{d²y}{dt²})e^{-t}=e^{-2t}\frac{dy}{dt}+e^{-2t}\frac{d²y}{dt²}=e^{-2t}\frac{d²y}{dt²}-e^{-2t}\frac{dy}{dt}$ 
Sustituyendo en:
$a_0x²y''+a_1xy'+a_2y=0$ 
se obtiene:

$a_0e^{2t}(e^{-2t}\frac{d²y}{dt²}-a_0\frac{dy}{dt}+a_1\frac{dy}{dt}+a_2y=0)$

$\Rightarrow a_0\frac{d²y}{dt²}-a_0\frac{dy}{dt}+a_1\frac{dy}{dt}+a_2y=0$ 
$\Rightarrow a_0\frac{d²y}{dt²}+(a_1-a_0)\frac{dy}{dt}+a_2y=0$ 
$\Rightarrow b_0\frac{d^2y}{dt²}+b_1\frac{dy}{dt}+b_2y=0$ donde $b_0=a_0;b_1=a_1-a_0;b_2=a_2$ 

$$a_2x²y+a_1xy'+a_2y=0$$
Recibe el tipo de nombre "ecuación de euler"
### Ejercicios:

1. Resuelva la ecuación $x²y''+3xy'+2y=0$ 
2. Resuelva la ecuación: $x²y''-xy'+y=2x$ 

#### Respuesta 1:
hacemos la sustitución $x=e^{t}$, y obtenemos:
$y''(t)+2y'(t)+2y=0$ donde $a_0=1;a_1=3;a_2=2$ 

Resolvemos esta ultima ecuación caracteristica (homogénea de coef constantes):

$m²+2m+2=0$ $\Rightarrow m= \frac{-2\pm\sqrt{4-8}}{\alpha}$ $\Rightarrow m=-1\pm i$ 

La solución general es:

$y(t)=e^{-t}(C_1cos(t)+C_2sin(t))$ 

como $x=e^{t}\Rightarrow t=ln(x)$, sustituyendo queda:

$y(x)=e^{-ln(x)}(C_1cos(ln(x))+C_2sin(ln(x)))=\frac{1}{x}(C_1cos(ln(x))+C_2sin(ln(x)))$ 

### Respuesta 2: $x²y''-xy'+y=2x$ 
Resolvemos: $x²y''-xy'+y=0$, usando sustitución $x=e^t$
$\Rightarrow y''(t)+(-1-1)y'(t)+y(t)=0$ 
$\Rightarrow y''(t)-2y'(t)+y(t)=0$ 
donde la ec. caracteristica es $m^2+2m+1=0$ $\Rightarrow m=1$ 
entonces, $y_H(t)=C_1e^{t}+C_2te^{t}$ 

Resolvemos ahora:

$y''(t)-2y'(t)+y(t)=2e^{t}$ 

Usamos variación de parametros:

$W(y_1,y_2)=det(\begin{pmatrix}   e^{t}& te^t \\   e^t & e^t+te^t    \end{pmatrix})$ =$e^{2t}$ 

Calculamos: $v_1(t)$ y $v_2(t)$ 

$\Rightarrow v_1(t)=-\int\frac{2e^{t}te^{t}}{e^{2t}}dt=-2\int{tdt}=-t²$ 
$\Rightarrow v_2(t)=\int\frac{2e^te^t}{e^{2t}}dt=2\int dt=2t$ 

entonces: $y_p(t)=-t²e^{t}+2t²e^t=t²e^t$ 

Luego, $y_G=C_1e^t+C_2te^t+t²e^t$ 

Volviendo a la variable original:

$\Rightarrow y_G(x)=C_1x+C_2xln(x)+2xln(x)$ (Respuesta final)


### Ejercicio Propuesto (materia pasada)
1) Resolver la ecuación :

$y^{(6)}+2y^{(4)}+y^{(2)}=0$ 

2) Resolver la ecuación:

$y^{(4)}+8y'=4x$ 

3) Considere la ecuación:

$x²y''+xy'-4y=0$. 

Suponga que la ecuación admite solución del tipo $y=x^{n}$. Determine $n$ y resuelva la ecuación.


# Transformada de Laplace 

Definición: Sea $f:[0,+\infty[\to{R}$ una función. Se define la transformada de Laplace de $f$ como la función $F$ definida por:  
$$F(s)=\int_{0}^{\infty}e^{-st}f(t)dt$$ Siempre que la integral impropia sea convergente. Los valores de $s$ para los cuales la integral impropia converge, constituyen el dominio de $F$ .

#### Notación: La transformada de Laplace de una función $f$, la denotaremos por:
$L${$f(t)$}$(s)$ o $F(s)$ 

##### Ejemplo: Calcule $L${$1$}$(s)$

Respuesta:
$L${$1$}$(s)$=$\int_{0}^{\infty}e^{-st}\cdot 1dt=lim_{n\to\infty}\int_{0}^{N}e^{-st}dt$ 
$=\lim_{N\to\infty}(-\frac{1}{s}e^{-st})|_0^{N}=\lim_{N\to\infty}-\frac{1}{s}(e^{-sN}-1)$ 
$=\frac{1}{s}$ si $s>0$ o diverge si $s\leq{0}$ 

entonces, $L${$1$}$(s)$=$\frac{1}{s}$ ; $s>0$ 

### Ejemplo: Calcule $L${$e^{at}$}$(s)$;$a\in{R}$ ; $a\not=0$ 

#### Solución:
 $L${$e^{at}$}$(s)=\int_{0}^{\infty}e^{-st}e^{at}dt=\lim_{N\to{\infty}}\int_{0}^{N}e^{-st}e^{at}dt$
 $=\lim_{N\to\infty}(\frac{1}{a-s}e^{(a-s)t}-1)|_0^{N}$ 
 note que  $L${$e^{at}$}$(s)=\frac{1}{s-a};a-s<0$ y diverge para $a-s>0$ 

entonces,  $L${$e^{at}$}$(s)=\frac{1}{s-a}$ para $s>a$ 


# Transformada de algunas funciones básicas

$f(t)$ y $L${$e^{f(t)}$}$(s)=F(s)$ 
$1$ y $\frac{1}{s}$ para $s>0$ 
$t^n$ y $\frac{n!}{s^{n+1}}$ para $s>0$ 
$e^{at}$ y $\frac{1}{s-a}$ para $s>a$ 
$cos(at)$ y $\frac{s}{s²+a^2}$ para $s>0$ 
$sin(at)$ y $\frac{a}{s²+a²}$ para $s>0$ 
$sinh(at)$ y $\frac{a}{s²-a²}$ para $s>|a|$ 
$cosh(at)$ y $\frac{s}{s²-a²}$ para $s>|a|$ 
#### Teorema: 
La transformada de laplace es un operador lineal, es decir: 
$L${$\alpha f(t)+\beta g(t)$}$(s)$=$\alpha$$L${$f(t)$}$(s)$+$\beta L${$g(t)$}$(s)$

### Condiciones suficientes para la existencia de la transformada de Laplace: 


##### Definición

i) $f$ es una función continua por tramos en un intervalo $I$, si tiene una cantidad finita de discontinuidades, a lo más de tipo salto en $I$.

ii) Se dice que $f$ es de orden exponencial $\alpha$, si existen constantes $M,t_0,\alpha$, tales que:
$$|f(t)|>Me^{\alpha t}$$ para todo $t>t_0$ 

#### Teorema: Si $f$ es una función continua a tramos en el intervalo $[0,+\infty[$, y de orden exponencial $\alpha$, entonces  $L${$f(t)$}$(s)$ existe $\forall{s>\alpha}$. ádemas, $\lim_{s\to\infty}F(s)=0$


#### OBS: 
Note que las condiciones del teorema anterior son suficientes pero no necesarias, es decir existen funciones que no satisfacen su hipotesis y tienen transformada de Laplace, por ejemplo, la función $f(t)=\frac{1}{\sqrt{t}}$ 


# Primer Teorema de traslación

Sea $f$ una función de orden exponencial $\alpha$. Si $F(s)=L${$f(t)$}$(s)$ y $a\in{R}$, entonces:

$L${$e^{at}f(t)$}$(s)=F(s-a)=L${$f(t)$}$_{s\to{s-a}}$ 


### Demostración:

$L${$e^{at}f(t)$}$(s)$=$\int_0^{\infty}e^{-st}e^{at}f(t)dt=\int_0^{\infty}e^{-(s-a)t}f(t)dt=F(s-a)$ 

##### Ejemplo: Calcular $L${$e^{at}f(t)$}$(s)$, usando el primer teorema de traslación.

#### Respuesta: 
Aquí $f(t)=1$, y además sabemaos que $L${$f(t)$}$(s)$=$L${1}$(s)$=$\frac{1}{s}$ 

entonces, por laplace: 

$L${$e^{at}$}$(s)$=$L${$e^{at}\cdot 1$}$(s)=F(s-a)=\frac{1}{s-a}$ 

##### Ejemplo: Calcule $L${$e^{at}sin(bt)$}$(s)$ 

##### Respuesta:
Aquí $f(t)=sin(bt)$. Además sabemos que $F(s)=L${$f(t)$}$(s)=\frac{b}{s²+b²}$ 

luego, $L${$e^{at}sin(bt)$}$(s)=F(s-a)=\frac{b}{(s-a)²+b²}$ ; $s>a$ 

analogamente, $L${$a^{at}cos(bt)$}$(s)=\frac{s-a}{(s-a)²+b²}$ 

#### Ejercicio: Calcule $L${$e^{5t}t³$}$(s)$ 

#### solución: aquí $f(t)=t³$ 
entonces, $L${$f(t)$}$(s)$=$L${$t³$}$(s)=\frac{3!}{s^4}=F(s)$ 
luego, $L${$e^{5t}t³$}$(s)$=$F(s-5)=\frac{3!}{(s-5)⁴}$ para $s>5$ 


#### Ejercicio: $L${$2e^{-3t}-4sin(2t)$}$(s)$ (se sacan las constantes como si fueran constantes nomas lol)
 note que $L${$2e^{-3t}-4sin(2t)$}$(s)=2L${e^{-3t}}

### Función Escalón Unitario 

#### Definición: 
Se llama función escalón unitario o función de Heauiside, a la función $\mu(t)$, dada por:

$\mu(t)=1$ si $t\geq{0}$ y $0$ si $t<0$ 

Si trasladamos la función escalón a un punto $t=a$, tenemos:

$\mu(t-a)=1$ si $t\geq{a}$ y 0 si $t<a$ 

Insertar graficos rossel lol :OO
#### Notación: 
$\mu(t),\mu(t-a),H(t),H(t-a)$ 


### Transformada de la función escalón unitario

$L${$\mu(t-a)$}$(s)=\frac{1}{s}e^{-as}$ para $s>0$ 
##### Nota: $L${$\mu(t-a)$}$(s)=\frac{1}{s}$ para $s>0$ 

#### Demostración:
$L${$\mu(t-a)$}$(s)=\int_{0}^{\infty}e^{-st}\mu(t-a)dt=\int_{a}^{\infty}e^{-st}dt=\lim_{N\to\infty}\int_a^{\infty}e^{-st}dt=lim_{N\to\infty}-\frac{1}{s}e^{-st}|_a^{N}=\lim_{N\to\infty}-\frac{1}{s}[e^{-sN}-e^{-sa}]$ $=\frac{1}{s}e^{-sa}$ ; $s>0$ 


#### Observación: La función escalón unitario nos permite calcular la transformada de laplace de otras funciones definidas por tramos:

### Por ejemplo:

$f(t)=g(t)$ si $0\leq{t}<a$ y $h(t)$ si $t\geq{a}$ 

Se puede expresar en términos de la función escalón, como sigue:

$f(t)=g(t)+$ {$0$ si $0\leq{t}<a$ y $h(t)-g(t)$ si $t\geq{a}$}
$=g(t)+(h(t)-g(t))\mu(t-a)$ 

### Ejercicio: Calcule la transformada de Laplace de la función: 

$f(t)=3$ si $t<2$ y $-2$ si $2\leq{t}<5$ y $1$ si $t\geq{5}$ 

### Respuesta: 

$f(t)=3-5\mu(t-2)+3\mu(t-5)$ 

luego, $L${$f(t)$}$(s)$=$L${$3-5\mu(t-2)+3\mu(t-5)$}$(s)$
$=3L${1}$(s)$-$5L${$\mu(t-2)$}$(s)$+$3L${$\mu(t-5)$}$(s)$ 

luego usando la tabla, sacamos el valor


### Ejercicio: 
Calcule la transformada de laplace de la función:
$$f(t)=3;0\leq{t}<\pi\cos(t);\pi\leq{t}<2\pi v sin(t);t\geq{2\pi}$$
Respuesta. escribimos $f$ en terminos de la función escalon unitario:

$$f(t)=3+(cos(t)-3)\mu(t-\pi)+)(sin(t)-cos(t))\mu(t-2\pi)$$
$=3+\mu(t-\pi)cos(t)-3\mu(t-\pi)+\mu(t-2\pi)sin(t)-\mu(t-2\pi)cos(t)$ 


entonces:
$L${$f(t)$}$(s)=3L${$1$}$(s)+L${$cos(t)\mu(t-\pi)$}$(s)-3L${$\mu(t-\pi)$}$(s)+L${$sin(t)\mu(t-2\pi)$}$(s)-L${$cos(t)\mu(t-2\pi)$}$(s)$ 

#### Observación:
Notemos que para obtener la transformada de laplace de $f(t)$ (ejercicio anterior), necesitamos calcular la transformadada de algunos productos, tales como $L${$cos(t)\mu(t-\pi)$}$(s)$,...

Para ello, necesitamos el siguiente Teorema:
#### Teorema: Segundo teorema de traslación 
Si $F(s)=L${$f(t)$}$(s)$ entonces:

$L${$f(t-a)\mu(t-a)$}$(s)=e^{-as}F(s)$ 

##### Observación: 
Para calcular la transformada de $f(t-a)\mu(t-a)$, procedemos como sigue:

$L${$f(t)\mu(t-a)$}$(s)=L${$f(t+a-a)\mu(t-a)$}$(s)=e^{-as}L${$f(t+a)$}$(s)$ 

##### Ejemplo: 
$L${$cos(t)\mu(t-\pi)$}$(s)=L${$cos[(t+\pi)-\pi]\mu(t-\pi$}$(s)=e^{-\pi s}L${$cos(t+\pi)$}$(s)=e^{-\pi s}L${$-cos(t)$}$(s)=e^{-\pi s}\cdot -\frac{s}{s²+1}$ 

analogamente:

$L${$cos(t)\mu(t-2\pi)$}$(s)=e^{-2\pi s}L${$cos(t+2\pi)$}$(s)=e^{-2\pi s}L${$cos(t)$}$(s)=e^{-2\pi s}\frac{s}{s²+1}$ 

del mismo modo: 

$L${$sin(t)\mu(t-2\pi)$}$(s)=e^{-2\pi s}L${$sin(t+2\pi)$}$(s)=e^{-2\pi s}L${$sin(t)$}$(s)=e^{-2\pi s}\frac{1}{s²+1}$ 


#### Ahora puedes temrinar ejercicios anteriores :O




# Transformada de la derivada

### Teorema: 
Sea $f:[0,\infty[\to\mathbb{R}$ una función continua y de orden exponencial $\alpha$. Si $f'$ es continua a tramos, entonces $L${$f'(t)$}$(s)$ existe para $s>\alpha$, y:

### $L${$f'(t)$}$(s)$=$sL${$f(t)$}$(s)-f(0)$

es decir, si llamamos $F(s)=L${$f(t)$}$(s)$, se tiene que: 

### $L${$f'(t)$}$(s)=sF(s)-f(0)$ 


Si $f'$ es continua y de orden exponencial $\alpha$, y la segunda derivada es continua a tramos, entonces:

### $L${$f''(t)$}$(s)=s²F(s)-sf(0)-f'(0)$ donde $F(s)=L${$f(t)$}$(s)$

en general:
Si $f\in nose$($[0,+\infty[$) (es decir, $f$ pertenece al conjunto de todas las funciones $f:[0,\infty[\to\mathbb{R}$ que admiten derivada hasta el orden $n-1$, continuas en $[0,+\infty[$)

y además $f,f',f'',...,f^{(n-1)}$ son de orden exponencial $\alpha$, y $f^{(n)}$ es continua a tramos en $[0,+\infty[$ entonces, $L${$f^{(n)}(t)$}$(s)$ existe para $s>\alpha$, y:

### $L${$f^{(n)}(t)$}$(s)=s^{n}F(s)-s^{n-1}f(0)-s^{n-2}f'(0)-...-f^{(n-1)}(0)$ 


# Transformada inversa de Laplace

Definición: 
Si $F(s)=L${$f(t)$}$(s)$ decimos que $f(t)$ es la transformada de Laplace inversa de $F(s)$. La denotamos:

### $L^{-1}${$F(s)$}$(t)=f(t)$ 

#### Teorema: 
La transformada inversa de Laplace es una transformación lineal, esto es: 

### $L^{-1}${$\alpha F(s)+\beta G(s)$}$(t)=\alpha L^{-1}${$F(s)$}$(t)+\beta L^{-1}${$G(s)$}$(t)$



| Transformada de Laplace              | Transformada inversa de laplace                   |
| ------------------------------------ | ------------------------------------------------- |
| $L${1}$(s)=\frac{1}{s}$              | $L^{-1}${$\frac{1}{s}$}$(t)=1$                    |
| $L${$t^n$}$(s)=\frac{n!}{s^{n+1}}$   | $L^{-1}${$\frac{1}{s^{n+1}}$}$(t)=\frac{t^n}{n!}$ |
| $L${$e^{kt}$}$(s)=\frac{1}{s-k}$     | $L${$e^{kt}$}$(s)=\frac{1}{s-k}$                  |
| $L${$sin(kt)$}$(s)= \frac{s}{s²+k²}$ | $L${$sin(kt)$}$(s)= \frac{s}{s²+k²}$              |
| $L${$cos(kt)$}$(s)=\frac{s}{s²+k²}$  | $L${$sin(kt)$}$(s)= \frac{s}{s²+k²}$              |
(cambiar ultimas tres de $L^{-1}$)


### Ejemplos: 

$L^{-1}${$\frac{1}{s⁵}$}$(t)=\frac{1}{4!}L^{-1}${$\frac{4!}{s⁵}$}$(t)=\frac{1}{4!}t⁴$ 

$L^{-1}${$\frac{1}{(s²-1)(s²+1)}$}$(t)$

usando fraciones parciales: 

$\frac{1}{(s²-1)(s²+1)}=\frac{A}{s-1}+\frac{B}{s+1}+\frac{Cs+D}{s²+1}$

$=\frac{A(s+1)(s²+1)+B(s-1)(s²+1)+(Cs+D)(s-1)(s+1)}{(s²-1)(s²+1)}$ 

$\Rightarrow{1}=A(s+1)(s²+1)+B(s-1)(s²+1)+(Cs+D)(s-1)(s+1)$ 

$\Rightarrow A=\frac{1}{4};B=-\frac{1}{4};C=0;D=-\frac{1}{2}$ 

entonces, $\frac{1}{(s²-1)(s²+1)}=\frac{1}{4}\frac{1}{s-1}-\frac{1}{4}\frac{1}{s+1}-\frac{1}{2}\frac{1}{s²+1}$ 

finalkmente:

### $L^{-1}${$\frac{1}{(s²-1)(s²+1)}$}$(t)=\frac{1}{4}L^{-1}${$\frac{1}{s-1}$}$(t)-\frac{1}{4}L^{-1}${$frac{1}{s+1}$}$(t)-\frac{1}{2}L^{-1}${$\frac{1}{s²+1}$}$(t)=\frac{1}{4}e^{t}-\frac{1}{4}e{-t}-\frac{1}{2}sin(t)$


## $I$) Primer teorema de traslación:

### $L${$a^tf(t)$}$(s)=F(s-a)$ 

### $\Rightarrow L^{-1}${$F(s-a)$}$(t)=e^{at}f(t)$ 

## $II$) Segundo teorema de traslación:

### $L${$f(t-a)\mu(t-a)$}$(s)=e^{-as}F(s)$ 

### $\Rightarrow L^{-1}${$e^{-as}F(s)$}$(t)=f(t-a)\mu(t-a)$ 



#### Ejemplo:
Calcule $L^{-1}${$\frac{1}{s-4}e^{-2s}$}$(t)$ 

$=f(t-2)\mu(t-2)$ donde $f(t)=L^{-1}${$\frac{1}{s-4}$}$(t)=e^{4t}$ 

entonces: 

$L^{-1}${$\frac{1}{s-4}e^{-2s}$}$(t)=e^{4(t-2)}\mu(t-2)$ 



# Derivada de la transformada de la Laplace

#### Teorema:
SI $F(s)=L${$f(t)$}$(s)$, entonces:
$L\{t^{n}f(t)\}(s)=(-1)^{n}\frac{d^n}{ds^n}(F(s))$ 

En particular:

- $L\{tf(t)\}(s)=-\frac{dF}{ds}$
- $L\{t²f(t)\}(s)=\frac{d²F}{ds²}$

#### Ejemplo: Calcule $L\{tsin(t)\}(s)$ 

sea $f(t)=sin(t)$ entonces:

$$F(s)=L\{f(t)\}(s)=L\{sin(t)\}(s)=\frac{1}{s²+1}$$
luego:
$$L\{tsin(t)\}(s)=-\frac{d}{ds}(F(s))=-\frac{d}{ds}(\frac{1}{s²+1})=-(-\frac{2s}{(s²+1)²})=\frac{2s}{(s²+1)²}$$

### Ejemplo: Calcule $L^{-1}\{ln(\frac{s²+2}{s²+9})\}(t)$ 

#### Solución: note que $F(s)=ln(\frac{s²+2}{s²+9})=ln(s²+2)-ln(s²+9)$ 

luego, $f(t)=L^{-1}\{ln(\frac{s^2+2}{s²+9})\}(t)$ que lo necesitamos determinar, entonces, recordando que:
$$L\{t^{n}f(t)\}(s)=(-1)^{n}\frac{d^{n}F}{ds^n}$$
entonces:

$t^{n}f(t)=(-1)^{n}L^{-1}\{F^{(n)(s)}\}(t)$ 

de donde podemos determinar $f(t)$. En nuestro caso:

#### $F'(s)=\frac{2s}{s²+2}-\frac{2s}{s^2+9}$ 
#### $\Rightarrow tf(t)=-L^{-1}\{F'(s)\}(t)=-L^{-1}\{\frac{2s}{s²+2}\}(t)+L^{-1}\{\frac{2s}{s²+9}\}(t)$ 
#### $=2[-cos(\sqrt(2)t)+cos(3t)]$ 

entonces:
$$f(t)=\frac{2}{t}[cos(3t)-cos(\sqrt{2}t)]$$





### Ejercicio: Resuelva la ecuación $y''+3y'+2y=12e^{4t}$ si $y(0)=1$; $y'(0)=0$ usando Laplace.


### Respuesta:
Aplicando laplace a la ecuación:
$$\Rightarrow L\{y''\}(s)-3L\{y'\}(s)+2L\{y\}(s)=12L\{e^{4t}\}(s)(*)$$
Sea $Y(s)=L\{f(t)\}(s)$ :
- $L\{y''\}(s)=s²Y(s)-sy(0)-y'(0)=s²Y(s)-s$ 
- $L\{y'\}(s)=sY(s)-y(0)=sY(s)-1$ 
de $(*)$ se tiene:

$$s²y(s)-s-(sY(s)-1)+2Y(s)=12\frac{1}{s-4}$$

##### $\Rightarrow s²Y(s)-s-3sY(s)+3+2Y(s)=\frac{12}{s-4}$ 
##### $\Rightarrow Y(s)=(s^2-3s+2)-s+3=\frac{1}{s-4}$
##### $\Rightarrow Y(s)(s²-3s+2)=\frac{12}{s-4}+s-3=\frac{s²-7s+24}{s-4}$ 

##### $\Rightarrow Y(s)=\frac{12}{s-4}+s-3=\frac{s²-7s+24}{(s-4)(s²-3s+2)}=\frac{s²-7s+24}{(s-4)(s-2)(s-1)}$ 

aplicando fracciones parciales:

##### $\Rightarrow A(s-2)(s-1)+B(s-4)(s-1)+C(s-2)(s-4)=s²-7s+24$ 

de esto, sacamos que:
- $A=2$ 
- $B=-7$
- $C=6$ 
entonces:
$$\frac{s²-7s+24}{(s-4)(s-2)(s-1)}=Y(s)=\frac{2}{s-4}-\frac{7}{s-2}+\frac{6}{s-1}/L^{-1}$$

#### $\Rightarrow y(t)=2L^{-1}\{\frac{1}{s-4}\}(t)-7L^{-1}\{\frac{1}{s-2}\}(t)+6L^{-1}\{\frac{1}{s-1}\}(t)$ 

##### finalmente: $y(t)=2e^{4t}-7e^{2t}+6e^{t}$ 


### Ejercicio propuesto: 
Resolver el p.v.i:
$$y''+y'+y=(t-1)\mu(t-1);y(0)=0;y'(0)=1$$


# Producto convolución

#### Definición: 
Sea $f$ y $g$ funciones continuas por tramo en $[0,+\infty[$. Se define el producto convolución de $f$ y $g$, que anotamos $f*g$, como:
$$(f*g)(t)=\int_{0}^{*}f(t-\tau)g(\tau)d\tau$$
##### OBS: $(f*g)(t)=(g*f)(t)$, basta hacer el cambio de variable $\tau=t-u$ 

#### Teorema:
Sean $f$ y $g$ dos funciones continuas por tramos $[0,+\infty[$, y de orden exponencial $\alpha$. Entonces:
$$L\{f*g\}(s)=F(s)G(s)$$ donde $F(s)=L\{f(t)\}(s);G(s)=L\{g(t)\}(s)$ 

### "Forma reciproca del teorema anterior":
$$L^{-1}\{F(s)\cdot G(s)\}(t)=(f*g)(t)$$
donde $F(s)=L\{f(t)\}(s);G(s)=L\{g(t)\}(s)$ 

