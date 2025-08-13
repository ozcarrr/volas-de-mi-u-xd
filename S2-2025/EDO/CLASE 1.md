
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















 