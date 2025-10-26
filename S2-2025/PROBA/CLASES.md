## $P(A\cap{B})=P(A)P(B)$ 
## $P(A\cup{B})=P(A)+P(B)-P(A\cap{B})$ 

## Clase pasada:
- Prob. condicional $[P(A ∩ B) = P(A)P(B | A)]$
- Independencia $[P(A) = P(A | B)]   [P(A ∩ B)=P(A)P(B)]$


## Eventos mutuamente excluyentes:

A y B son mutuamente excluyentes si:

## $[P(A ∩ B) = 0]$

### ejemplo, se tira una moneda:

 [P(C y S EN 1)] = 0
pero, [P(C EN 1 y S EN 2) = P(C)P(S) = P(C en 1)P(S en 2 | C en 1)]




Regla General :
- Caso excluyente: Ocurre en UNA repetición del exp. aleatorio

- Independiente: Puede ocurrir en varias repeticiones del exp. aleatorio o al combinar distintos exp. aleatorios



Principo Aditivo:

- Si A y B son ==eventos mutuamente excluyentes==, la probabilidad de que ocurra al menos uno de ellos es: 

  $[P(A ∪ B) = P(A) + P(B)]$

- Si A y B son ==NO son eventos mutuamente excluyentes==, la propbabilidad que ocurra al menos uno de ellos es: 

  $[P(A ∪ B) = P(A) + P(B) - P(A ∩ B)]$
  
ejemplo : se tiran 2 dados,  A y B¿Cual es la probabilidad de que salga un 1 en A o 1 en B? :

dado que ambos eventos no son mutuamente excluyentes, se tiene:


$P(A1 ∪ B1)=P(A1)+P(B1)-P(A1∩B1)$



### Conteo:

- Ordenar  $n$ elementos: se tiene $n!$ formas de ordenarlos
  Ejemplo: 
     Curso de 40 personas, se necesitan 3 personas para 3 roles distintos, cual es la Combinatoria posible para cada rol, si se elige uno primero y una persona puede tener maximo un rol para cada rol? 

     $P(ROL 1)=40!$ 
     $P(ROL2)=39!$
     $P(ROL2)=38!$
     
     Entonces, si queremos encontrar todas las posibles combinaciones para esto, se tiene una permutación:

     ## $P^n = \frac{n!}{(n-k)!}$ 
     
     entonces, $P(ROLES)=40!/(40-3)!$


     Pero, si el orden no importara, se tiene lo siguiente:

     ## $C^n=n!/k!(n-k)!$  
     
     donde n es el total de elementos y k la cantidad de combinaciones en n elementos
     entonces $P(ROL SIN ORDEN)=\frac{40!}{3!(40-3)!}$ 


## Permutaciones (con orden) : $P_k^{n}=\frac{n!}{(n-k)!}$ 

## Combinaciones (sin orden): $C_k^{n}=\frac{n!}{k!(n-k)!}$ 

### Permutaciones circulares: $P^n=\frac{n!}{n}=(n-1)!$ 



## Ej: ¿De cuantas maneras se pueden ordenar las letras de la palabra 'Irarrazaval'

#### primero, al ser 11 palabras, la respuesta directa seria $11!$ 

#### Sin embargo, contando las letras repetidas (3 'r', 4 'a'), y ignoramos los casos repetidos, la respuesta seria :

## $P^n=\frac{11!}{3!4!}$ (Caso de permutación multinomial $P^n=\frac{n!}{k_1!,k_2!,...,k_j!}$ donde $j$ es la cantidad de factores repetidos y $k_1,k_2,...,k_j$ son la cantidad de dichos factores) 


### Ej: Se tiene n personas, 

### C (evento): Al menos dos personas estan de cumpleaños el mismo dia.


### ¿P(C)?

### Sabemos que $C^{c}$ : No hay dos personas de cumpleaños el mismo dia

####  Casos totales = $365^n$ 
#### Combinaciones = $365!$
#### Las probabilidades se verian como $\frac{365}{365}\frac{364}{365}\frac{363}{365}...\frac{365-n+1}{365}$, entonces: 

### entonces, $P(C^{C})=\frac{365!}{365^n(365-n)!}$ 

## Luego, $P(C)=1-\frac{365!}{365^n(365-n)!}$ 



### Calcular probabilidad de que en un grupo de n personas tenga el cumpleaños eel mismo dia que el mio:


### Calculando el complemento, vemos que, la probabilidad de que esto pase, si nos contamos a nosotros mismos con las n personas, se veria como $\frac{364}{365}\frac{364}{365}...\frac{364}{365}$, entonces :

## $P(A^{C})=(\frac{364}{365})^{n-1}$ 

## entonces, $P(A)=1-(\frac{364}{365})^{n-1}$ 



## CLASE NOSE OLA

### T. de Bayes : Como actualizar nuestras probabilidades a partir de información nueva.

### $P(A\cap{B})=P(A)P(B|A)=P(B\cap{A})=P(B)P(A|B)$ 

## Es decir: $P(B|A)=\frac{P(B)P(A|B)}{P(A)}$ ; (Comunmente, $P(A)$ puede ser dificil de encontrar)


## EJERCICIO CERTAMEN: 

### Tres maquinas A,B,C han producido respectivamente 200, 200, 100 piezas. Se sabe que la maquina A produce un 5% de piezas defectuosas, la maquina B un 6% y la C un 7%. Se selecciona una maquina al azar, y luego, una pieza al azar:

#### a) Calcular la probabilidad que la pieza seleccionada sea defectuosa

#### b) Sabiendo que la pieza seleccionada es defectuosa, calcule la probabilidad de que provenga de la maquina A.

#### c) Calcule la probabilidad que la pieza seleccionada sea NO defectuosa y provenga de la maquina C

#### d) Si se sabe que la pieza seleccionada es no defectuosa, calcule la probabilidad de que provenga de la maquina B.

# SEAN:

## $r=$ {Piezas producidas} (Espacio Muestral)
## $A=$ {$w\in{r}$;$w$ producida por $A$ }
## $B=$ {$w\in{r}$;$w$ producida por $B$ }

## $C=$ {$w\in{r}$;$w$ producida por $C$ }

## $D=$ {$w\in{r}$;$w$ es defectuosa  }

Donde A, B, C y D son eventos en el espacio muestral


### obs : A, B, C cuando son intersectados, dan vacio, pero cuando son unidos, dan el espacio muestral, esto se conoce como particiones.

### Entonces:

## $P(A)=\frac{2}{5}$ ; $P(B)=\frac{2}{5}$ ; $P(C)=\frac{1}{5}$ 

### Luego "la maquina A produce un 5% de piezas defectuosas, la maquina B un 6% y la C un 7%"esto quiere decir:

## $P(D|A)=0.05$ ; $P(D|B)=0.06$ ; $P(D|C)=0.07$ 


Entonces: 

## $P(D)=P(A)P(D|A)+P(B)P(D|B)+P(C)P(D|C)=0.058$ 
#### Con estos datos se sabe cual seria la probabilidad de una pieza no defectuosa, calculando $D^{C}$.

### Luego, para b) nos piden $P(A|D)$

### Por teorema de Bayes :

## $P(A|D)=\frac{P(B)P(D|A)}{P(D)}=\frac{0.4\cdot0.5}{0.058}$ 

### Luego, para c), nos piden $P(D^{C}\cap{C})=P(C)P(D^{C}|C)$

#### Como $P(C)=0.2$ y $P(D^{C}|C)=0.93$, entonces la respuesta es 0.186 o 18.6%


### Luego, para d), se pide $P(B|D ^{C})$ 

### Por teorema: $P(B|D^{C})=\frac{P(B)P(D^{C}|B)}{P(D^{C})}$, de a), sacamos $P(D^{C})=0.942$, entonces, $P(B|D^{C})=\frac{0.4\cdot{0.94}}{0.942}=0.399$ 


### Otra metodologia, es una muestra:


|     | TOTAL | $D$ | $D^{C}$ |
| --- | ----- | --- | ------- |
| A   | 200   | 10  | 190     |
| B   | 200   | 12  | 188     |
| C   | 100   | 7   | 193     |


### Imaginemos una enfermedad llamada "malturismo", sean:

## $\Omega$ = {Poblacion de Chile}
## $E$ = {$w\in{\Omega}$ ; $w$ padece malturismo}

## $P(E)$ = 1% 

## $+$ = {$w\in{\Omega}$ ; $w$ dio positivo}

## $-=+^{C}$ 


## $T$ = {$w\in{\Omega}$ ; $w$ dio positivo} (Test de Malturismo)

### EXAMEN:
- Sensibilidad: Prob. de que el examen de positivo sabiendo que tengo la enferemedad $P(T|E)$ = 90% 
- Especificidad: Prob. de que el examen de negativo sabeindo que no tengo la enfermedad $P(-|E^{C})$ = 91% 

¿Probabilidad de que una persona este enferma sabiendo que el examen dio positivo? 

### $P(E|+)$? 

#### pista: $P(+)=P(+\cap{E})+P(+\cap{E^{C}})$ 


# Versión Numerica
## Se tienen 1000 personas: 

|       | $E$ | $E^{C}$ |
| ----- | --- | ------- |
| +     | 9   | 89      |
| -     | 1   | 901     |
| total | 10  | 990     |
### entonces, $P(E|+) =\frac{9}{9+89}=\frac{9}{98}\approx{0.09}$ 


# Versión Teorema (de Bayes)

## $P(E|+)=\frac{P(E)P(+|E)}{P(+)}$ ; $P(+)$ siendo la probabilidad total

### $A_{i=1}$ (Partición de $\Omega$)

## -> $P(B)=\sum_{i}^{n}P(B\cap{A_i})=\sum_{i}^{n}P(A_i)P(B|A_i)$ 


### Luego, $P(E|+)=\frac{P(E)P(+|E)}{P(E)P(+|E)+P(E^{C})P(+|E^{C})}=\frac{0.01\cdot{0.9}}{0.01\cdot{0.9}+0.99\cdot{0.09}}\approx{0.0917}$ 


### Notación 'odds':

### Ej: $\frac{9}{10}$ = 9:1 , $\frac{91}{100}$ = 91:9




### Ejemplo caso anterior : 

### Sabemos que P(-|E) = 1:9 ; P(+|E)=9:1
### luego $P(+|E^{C})$ = 89:901 ; $P(-|E^{C})$ = 901:89

### Entonces : O(E|+)=$O(E)\frac{O(+|E)}{O(+|E^{C})}$ ; $O(E)=\frac{n de E}{n de E^{C}}$ 




## EJEMPLO:

### Dos productores de productos dentales, A genera pasta de dientes y B genera dentífricos.

#### Cada mes, el 60% de los consumidores de A se van a B, el resto se queda

#### Cada mes, el 50% de consimidores de B se van a A, el resto se queda

#### Al inicio A y B tienen el 50% del mercado cada una. 


## Matematicamente, esto se expresa como :

#### $a_n=0.4\cdot{ạ_{n-1}}+0.5\cdot{b_{n-1}}$ 
#### $b_n=0.6\cdot{a_{n-1}}+0.5\cdot{b_{b_{n-1}}}$ 

## El efecto se conoce como la cadena de markov.

# Variables aleatorias: 

### $f:\Omega -> R$ ; $f(a)=P(X=x)$ 

#### Si se tiran 2 dados de cuatro caras, sea A = {La suma de los dado es 6 o más}

### Tenemos que:  $P(x=6)=\frac{3}{16}$ 
### Pensemos en $P$ como una función de variables aleatorias, llamada 'Función de masa de probabilidad' :

### $P(x=2)=\frac{1}{16}$
### $P(x=3)=\frac{2}{16}$
### $P(x=4)=\frac{3}{16}$
### $P(x=5)=\frac{4}{16}$
### $P(x=6)=\frac{3}{16}$
### $P(x=7)=\frac{2}{16}$
### $P(x=8)=\frac{1}{16}$


### Condiciones: 
## $\sum_{x}{P(X=x)}=1$ 

## $P(X=x)\geq{0}$ 


# Axiomas de probabilidad :

### 1. $P(A)\geq{0}$
### 2. $P(\Omega)=1$

### 3. $U_i\cap{V}_j=\emptyset;\forall{i,j}$ distintos


### Función acumulada de probabilidad : $F(a)=P(X\leq{x})=\sum_{x_i\leq{x}}{P(x=x_i)}$ 

### La idea es que $F$ (funcion acumulada) acumula los valores, tendiendo a 1 (100%) mientras que la de masa solo da los valores respectivos al caso actual.



#### obs: El caso utilizado es disctreto, No continuo (Es decir $P=0$ -> imposibilidad de evento)

#### continuo : ($P=0$ NO implica imposibilidad de evento), en este caso, no podemos dener una función de masa de probabilidad, dado a que todas darian 0. 

### Para los casos continuos tendriamos "Función de densidad de probabilidad" ($P(a\leq{x}\leq{b})$ )(probabilidad de que el numero (o evento) este en cierto intervalo)




### entonces: 

## Discreto : 

### - $f(x)=P(X=x)=f_X(x)$  (Función de masa) (Función de cuantía)  
### - $F(x)=P(X\leq{x})$ (Función de probabilidad acumulada)

## Continuo:

### - $f(x)=P(a\leq{X}\leq{b})=\int_{a}^{b}{f(x)dx}$  (función de densidad de probabilidad)  donde $P(x=x_0)=0$ 

### - $F(x)=P(X\leq{x})=\int_{-\infty}^{x}{f(t)dt}$ (función de probabilidad acumulada)


### ejemplo modelo: 

## Se lanza una moneda, la probabilidad de sello (x=1) es 1-p y pa probabilidad de cara (x=0) es p: 

### $P(x=0)=1-p=q$ 
### $P(x=1)=p$ 

### Sea $z:$ n° de sellos en 100 lanzamientos 

### tenemos que $Z=\sum_{i=1}^{100}x_i$ 

### $P(z=n)=\binom{100}{n}p^n q^{100-n}$ (Distribución Binomial) 

### Ejemplo continua:
- Tirar dardos 
- Decibelios de la voz del profe
- graduacion del lente de las personas
- Voltaje usado en la sala
- cuanta ram esta utilizando un pc cualquiera 
#### Condición: $f(x)\geq{0}$ y $\sum_{x}^{n}f(x)=1$ 

### Ejemplo Discreta:
- Dedos que tiene una persona
- Color del pelo de una persona
- C de gente q utiliza tablet o cuaderno
- C de computadores en los lab
- Profes mujeres en la facultad de ingeneria
#### Condición : $f(x)\geq{0}$ y $\int_{-\infty}^{\infty}{f(x)dx}=1$ 


### Esperanza: Promedio ponderado (se toma en cuenta la probabilidad de cada uno de los eventos), es decir :

### $E(x)=\mu=$ $\sum_{x}xP(X=x)$ (para prob. discreta)

### $E(x)=\mu=\int_{-\infty}^{\infty}{xP(X=x)dx}$ (Para prob. continua)


### Ej, se tienen los eventos 1, 2 y 3, la probabilidad de cada uno es 0,25 , 0,65 y 0,1 respectivamente, entonces, la esperanza es :

## $E(x)=1\cdot{0.25}+2\cdot{0.65}+3\cdot{0.1}=1.85$ 

#### Dispersión: Comparar la 'distancia' del dato con la esperanza 
#### Varianza: $E[(x-\mu)²]=Var(x)$


### Ejemplo caso anterior :

### $Var(x)=E[(x-1.85)²]$ , dado a que esto es muy complejo de calcular, entonces, notemos que: 

## sea $g(x)$ una función cualquiera, sabemos que:

### $E[g(x)]=\sum_{x}g(x)P(X=x)$ , luego, por demostración :

## $Var(x)=E[x²]-(E[x])²$ 

### luego, $Var(x)=E(x²)-E²(X)=E(X²) - 1.85²=3.75-1.85²=0.3275$ 

### Desvación estandar =$DE(x)=\sqrt{Var(x)}$ 


# Modelos discretos de probabilidad: 

## Bernouli 

#### X = {1: Exito ; 0: Fracaso}

#### $P(X=x)=$ $p$ si $x=1$ o $1-p=q$ si $x=0$ 


### Poisson : Eventos que se repiten cada cuanto tiempo independientemente  (Taza promedio de repetición: $P_0:(\lambda))$ 

### Binomial: Repetir n veces experimentos independientes, bernally con p fija. 

# $P$(Obtener 2 exitos) = $\binom{3}{2}p²q¹=3$ 


# $P(X=k)=\binom{n}{k}p^{k}q^{n-k}$ 

### Geometrica: Repetir n veces hasta el 1er exito

### Negativa: Repetir n veces hasta el exito numero k

## Propiedades de la esperanza: 

# 1. $E(ax+b)=aE(x)+b$ 
# 2. $E(x+y)=E(x)+E(y)$ 
# 3. Si $x$ e $y$ son independientes:

# $E(xy)=E(x)E(y)$ 

\
## Propiedades Variante:

# 1.$Var(ax)=a²Var(x)$ ; $a\in{R}$ 
# 2. $Var(x+b)=Var(x)$ ;$b\in{R}$ 
# 3. Si $x$ e $y$ son independientes: 

# $Var(x+-y)=Var(x)+-Var(y)$ 

# Control miercoles: Hasta varianza

### Ejercicio Binomial: se tiene una muestra aleatoria de 10 bicicletas en una fabrica cuya probbabilidad de generar una bicileta mala es 0.3. ¿Cual es la probabilidad de encontrar entre 2 y 4 bicis malas? 
### Sean X: C°de bicis malas ; n: muestra aleatoria ; 

### Se nota que $X~Bin(10;0.3)$ 

### entonces, nos piden $P(2\leq{X}\leq{4})=P(X=2)+P(X=3)+P(X=4)$ 
### Entonces, se aplica la formula para cada uno ($P(X=x)=\binom{n}{k}p^{k}q^{n-k})$

### en este caso, para $P(X=2)$ se tiene $k=2;n=10$ y $p=0.3$ y $q=1-p=0.7$ 

### resolviendo, queda $P(2\leq{X}\leq{4})=0.7$ 

### Geométrica: 'N° de fracasos hasta un exito' (Notación: $X~Geom(x)$):

# $P(X=n)=pq^{n-1}$ 
# $P(X\leq{n})=\sum_{i=1}^{n}pq^{i-1}=1-q^{n}$  
# $P(x\geq{n})=q^{n-1}$ 

# $E(X)=\frac{1}{p}$


### en el contexto del ejercicio anterior: 

### X: N° de bicis que se examinan hasta la 1° mala

### $x$ ~ $geom(0.3)$ 




### Binomial Negativa: 'N° intentos hasta exito k'



## Ejercicios control

### Se apuestan 3$ una ruleta europea tiene los siguientes huecos, si cae en el bloque apostado, se gana 3$:

### 18 Negras (N); 18 Rojas (R); 1 Verde (V)
### a) Calcule la esperanza y varianza de ganancia 
### $P(R)=P(N)=\frac{18}{37}$ 

#### Luego X = {3 : Ganar ; -3 Pierdo}

#### Ademas, $P(X=x)$ = $\frac{18}{37};x=3$ o $\frac{19}{37};x=-3$ 

### Luego; #$E(X)=3\cdot{\frac{18}{37}}+(-3)\cdot{\frac{19}{37}}=-\frac{3}{37}$   

### Luego, $Var(x)=E(x^{2})-(E(x))^{2}$ 

### $E(X^{2})=3²\frac{18}{37}+(-3)²\frac{19}{37}=9$ 
### $(E(X))²=(-\frac{3}{37})²=0.006$

### -> $Var(x)\approx{9}$ 



## b) Si apostamos 1$ , 1$ y 1$, separadamente, cual es la esperanza y varianza? 

### Sea $z= y_1+y_2+y_3\not=3y$ 

### $E(z)=E(y_1)+E(y_2)+E(y_3)=-\frac{1}{37}-\frac{1}{37}-\frac{1}{37}=-\frac{3}{37}$ 

### Sin embargo: 

## $Var(z)=Var(y_1)+Var(y_2)+Var(y_3)=1+1+1=3$ 


### 2. Sean A,B,C eventos en un espacio $\Omega$ tales que: 

### - La probabilidad de que pase al menos alguno de los eventos es 0.9 ($P(A\cup{B}\cup{C})=0.9)$ 
### - La suma de de las probabilidades de que pase cada uno es 1.3 ($P(A)+P(B)+P(C)=1.3$) 

### - La suma de probabilidad de que pasen dos de los eventos es 0.45 ($P(A\cap{B})+P(A\cap{C})+P(B\cap{C})-2P(A\cap{B}\cap{C})$ =0.45)

### a) Determine la probabilidad de que pasen los 3 eventos

### Por propiedades de conjunto:

# $P(A\cup{B}\cup{C})=P(A)+P(B)+P(C)-(P(A\cap{B})+P(A\cap{C})+P(B\cap{C}))+P(A\cap{B}\cap{C}))$ 
### Se sabe que $P(A\cup{B}\cup{C})=0.9$ ; $P(A)+P(B)P(C)=1.3$ 

### ; $P(A\cap{B})+P(A\cap{C})+P(B\cap{C})=0.45 + 2P(A\cap{B}\cap{C})$ 

### entonces :

### -> $0.9=1.3-(0.45+3P(A\cap{B}\cap{C}))$ -> $P(A\cap{B}\cap{C})=0.05$ 


## 3. Se tienen 3 urnas con las siguientes caracteristicas

### - La urna 1 tiene 1 bola roja y 2 bolas blancas
### - La urna 2 tiene un número desconocido tanto de bolas rojas como de bolas blancas
### - La urna 3 tiene 2 bolas rojas y 2 bolas blancas


### Se elige una urna y se extrae una bola. Se sabe que la prob. de que la urna 1 haya sido escogida, dado que se extrajo una bola roja es $\frac{2}{9}$ y que hay 10 bolas entre las $3$ urnas. 

## R: Sacar bola roja ; B: Sacar bola blanca ; 1,2,3 : Esocger urna 1,2,3

### se tiene que: 

## $P(1|R)=\frac{2}{9}$ 

### a) Muestre que la cantidad de bolas rojas y blancas en la urna 2 es 2 y 1, respectivamente. 

### Se sabe que $P(1)=P(2)=P(3)=\frac{1}{3}$, ademas $P(R|1)=\frac{1}{3}$, 
### $P(B|1)=\frac{2}{3}$ , $P(R|3)=P(B|3)=\frac{1}{2}$ 

### Luego, por bayes:

### $P(1|R)=\frac{P(1)P(R|1)}{P(R)}$ -> $P(R)=\frac{1}{2}$ 

### Entonces, usando los datos entrgados, usamos Probabilidad total para calcular $P(R)$ y demostrar que son equivalentes

### 

### b) $P(2|R)=\frac{P(2)P(R|2)}{P(R)}=\frac{4}{9}$ dado que conocemos todos los datos 


## 3. Un restaurante con una estrella Michelin (un certificado de categoría a   nivel mundial) tiene un menú de 7 tiempos: 1 bebestible, 2 entradas, 2 fondos y 2   postres. Estos ítemes tienen que elegirse desde el menú del restaurant, el cual cuenta   con 4 bebestibles, 6 entradas, 7 fondos y 5 postres. ¿De cu ́antas maneras se pueden  colocar los 7 ́ıtemes del menú sobre la mesa de un cliente?

### $B$ ; $E:\binom{6}{2}$ ; $F:\binom{7}{2}$ ; $P:\binom{5}{4}$ (todos divididos por $2$)

### Entonces: $C=\frac{\binom{6}{2}\binom{7}{2}\binom{5}{2}}{8}=12.600$ 


# Discretar: 

### Sea $p$ la probabilidad de que suceda un evento y $q=1-p$ :

### - Binomial 
#### $X$ ~ $Bin(n,p)$ 
#### $P(X=k)=\binom{n}{k}p^{k}q^{n-k}$ ; $E(X)=np$ , $V(x)=npq$ 
### - Geométrica (intentar n veces hasta el 1er exito)
#### $P(X=n)=pq^{n-1}$ ; $E(X)=\frac{1}{p}$ ;$Var(x)=\frac{q}{{p²}}$ 
### - Binomial Negativa :ooo (intentar n veces hasta el k-esimo exito)
#### $X$ ~ $NBin(k,p)$ 
#### $P(X=n)=\binom{n-1}{k-1}p^{k}q^{n-k}$ 
#### $E(X)=k\frac{1}{p}$ ; $Var(X)=k\frac{q}{p²}$ 

### Ejemplo: Se quieren completar 20 encuestas, la probabilidad de que se complete $1$ encuesta es $0.2$, Si se llama a 50 personas ¿Se llegaria a la meta? 

## X: C°de intentos para tener 20 exitos

### -> $X$ ~ $NBin(20;0.2)$ 
## -> $E(X)=20\frac{1}{0.2}=20\cdot{5}=100$ 
### Luego, si queremos saber la probabilidad de que se alcanze la meta en 50 llamadas: 

## -> $P(X=50)=\binom{49}{19}0.2^{20}\cdot{0.8^{30}}=0.0002447$  


### - Hipergeométrica:
#### Esta discreción asume que NO hay independecia (Como caja sin reposición)
## $P(X=k)=\frac{\binom{r}{k}\binom{N-r}{n-k}}{\binom{N}{n}}$ 
### Donde N : Tamaño total (Espacio Muestral), r: "exitos" dentro de N, n: Tamaño que tomo eventos de una vez

### Ejemplo: De 10 dulces, se tienen 4 frugeles, si solo podemos sacar 3, ¿Cual es la prob. de sacar 2 frugeles? 

### $P(X=2) = \frac{\binom{4}{2}\binom{6}{1}}{\binom{10}{3}}$ ; $X$ : Sacar 2 frugele :0
 
## $X$ ~ $Hip(10;4;3)$ 

## $\Rightarrow{P(X=x)}=\frac{\binom{r}{x}\binom{N-r}{n-x}}{\binom{N}{n}}$
donde, N es el total, r son los exitos iniciales y n es el 'tamaño' del grupo.

### Ejemplo: De 37 estudiantes, hay 5 mujeres, ¿Cual es la probabilidad de que, al sacar 3 estudiantes, 1 sea mujer?

#####  X: Numero de muejeres escogidas de un curso de 37 alumnos de los cuales 5 son mujeres y se seleccionan 3 estudiantes.

### $\Rightarrow{p(X=1)}=\frac{\binom{5}{1}\binom{32}{2}}{\binom{37}{3}}$
## $E(X)=r\frac{n}{N}$ 
### $V(X)=r\frac{n}{N}\frac{N-r}{N-1}$ 



# Proceso de Poisson:

### Sea $x(t);t\in{[0,+\infty[}$, se define como "El N°de 'cosas' que ocurren entre 0 y t"

-  Cada ocurrencia es independiente de la demas
- El promedio de ocurrencias es constante en el tiempo
- No pueden ocurrir dos eventos en un t
- $x(0)=0$

### Dist. de Poisson (discreta) :
Cuenta el numero de eventos en un intervalo
### Exponencial (continua):
Mide el tiempo entre eventos

### Notación: 

# $X$~$Poi( \lambda)$ 
donde $\lambda$ es el promedio de ocurrencias en un intervalo

# $P(X=x)=\frac{\lambda^x}{x!}e^{-\lambda}$ 

# $E(X)=\sum_{x=0}^{\infty}x\frac{\lambda^x}{x!}e^{-\lambda}=\lambda$ 
# $Var(X)=\lambda$ 


## Ejercicios de distribuciones de prob.

Llegan 120 botellas/hora, cada botella tiene un 0.02 de estar mala.
Se toma muestras de 50 botellas cada 30 min. 
#### a) ¿Cual es la probabilidad de encontrar exactamente 3 botellas malas? 

Note que, esta es una distribución binomial, entonces:
sea $X$: el numero de botellas malas en 50 botellas $\rightarrow$$x$~$Bin(50;0,02)$
entonces: 
#### $P(X=3)=\binom{50}{3}0.02³\cdot{0.98^{47}}$ 

### b) $P(x\leq{2})=0.9216$

### c) ¿Cual es el numero esperado y la desviación estandar de defectuosas en una muestra de 50? 

### $E(X)=50\cdot{0.02}=1$ 
### $\Rightarrow{V(x)}=50\cdot{0.02}\cdot{0.98}=0.98$ 
### $\Rightarrow{\sigma}=\sqrt{0.98}$ 

### d) Las botellas llegan a inspección a razon de $\lambda=120$ por hora ¿Cual es la probabilidad de que en 5 minutos lleguen al menos 12 botellas? 

$X$:Cantidad de botellas que lleguan en 5 min.
$X$~$Poi(\lambda_1)$ ; $\lambda_1=10$ 

$P(x\geq{12})=1-P(X<12)$ = $h

### Contexto: 
- Llegan 120 botellas por hora auna inspección
- Cada botella tiene 0.02 de prob de estar mala
- Control de calidad toma muestras de 50 botellas cada 30 minutos
### e) Las botellas se revisan una hasta encontrar la primera defectuosa ¿Cual es la probabilidad de que la primera defectuosa aparezca en la $7^{ma}$ inspección?

### Geometrica (buscamos primer exito): 
### $X$: N° de botellas revisadas hasta la $1^{ra}$ defectuosa. 

#### donde $P(X=7)=0.02\cdot{0.98⁶}\approx{0.0117}$ 


### f) ¿Cual es la probabilidad de que se necesiten al menos 15 inspecciones para hallar la primera defecutosa? 

### Misma variable y distribución, pero dado que pide 'al menos 15', nos piden por: 

### $P(X\geq{15})=\sum_{x=15}^{\infty}pq^{x-1}=0.02\sum_{x=14}^{\infty}0.98^{x}=\frac{0.02}{1-0.98}$ 
### o tambien $P(X\geq{15})=1-\sum_{x=1}^{14}pq^{x-1}=1-0.02\sum_{x=0}^{13}0.98^x=1-0.02\frac{1-0.98^{13}}{1-0.98}=0.76$
### g) El turno de control necesita encontrar 4 defectuosas para calibrar un equipo ¿Cuál es la probabilidad de que esto ocurra exactamente al revisar la botella numero 25? 

### $Y$: N° de botellas revisadas para encontrar 4 malas
### $Y$~$BinNeg(4;0.02)$ 
### $P(Y=25)=\binom{24}{3}\cdot{0.02⁴}\cdot{0.98^{21}}\approx{0.000212}$ 

### h) En un bloque de 40 inspecciones consecutivas ¿Cual es la probabilidad de identificar exactamente 6 defectuosas? 

### $X$:N° de botellas defectuosas en 40 insepcciones

#### $X$:~$Bin(40;0.02)$ $\Rightarrow{P(X=6)}=\binom{40}{6}0.02⁶\cdot{0.98^{34}}$ 

### i) En una hora, el promedio de defectos detectados por sensores en linea es 2.4 ¿Cual es la probabilidad de registrar cero defectos de sensor en la proxima hora? 

### $Z$ : N° de defectos detectados ; $Z$:~$Poi(2.4)$ 

### $\Rightarrow{P(Z=0)}=\frac{2.4⁰}{0!}e^{-2.4}\approx{0.091}$ 

### j) Durante un intervalo de 30 minutos, ¿Cual es la probabilidad de registrar al menos 4 defectos por sensor? 

### $Z_2$ : N° de defectos detectados en media hora ; $Z_2$~$Poi(1.2)$ 

### $\Rightarrow{P(Z_2\geq{4})}=1-P(Z_2<4)=1-P(Z_2\leq{3})=1-(\frac{1.2⁰}{0!}e^{-1.2}+\frac{1.2¹}{1!}e^{-1.2}+\frac{1.2²}{2!}e^{-1.2}+\frac{1.2³}{3!}e^{-1.2})\approx{0.91}$ 
### k) En una jornada de 8 horas: 

- ¿Cual es el número esperado de defectos resgistrados por sensor? 
- ¿Cual es la probabilidad de observar $\geq{25}$ defectos? 

### $Y_2$ : N° de defectos en 8 horas ; $Y_2$~$Poi(19.2)$ 

### $\Rightarrow{E[Y_2]}=2.4\cdot{8}$ 
### luego, $P(Y_2\geq{25})=\sum_{i=25}^{\infty}\frac{19.2^{i}}{i!}e^{-19.2}$ 

# Distribuciones continuas de probabilidad

### Distribución Uniforme 

![[Pasted image 20250922163808.png]]
$X$ ~ $Unif(a,b)$ (notación)
Probabilidad: $P(X)=\frac{1}{b-a}$ 
Esperanza : $E[X] = \int_{a}^{b}\frac{x}{b-a}dx=\frac{b-a}{2}$ 

### Distribución normal

![[Pasted image 20250922163847.png]]
$X$~$N(\mu,\sigma²)$ 
$Z=\frac{x-\mu}{\sigma}$ 
$P(X\geq{\mu})=P(X\leq{\mu})=0.5$ 
$P(X>x)=1-P(X\leq{x})=1-P(Z\leq{\frac{x-\mu}{\sigma}})$ 
$E[X]=Z\cdot{\frac{\sigma}{x}}=Z\cdot{\frac{\sigma}{\sqrt{n}}}$ 
donde $\mu$ es el promedio, $\sigma$ es la desviación estandar, $X$ es la var. aleatoria, $x$ es el numero dado en el problema, $Z$ es la distribución estandarizada y $n$ es la "muestra deseada"
 
Estandar: $Z$~$N(0,1)$ 

![[Pasted image 20250922164232.png]]

# 23/09
# Distribución exponencial 

Funciona como Poisson, pero en lugar de medir "cuantas veces paras algo en un intervalo de tiempo o espacio" mide =="cuanto tiempo o espacio pasa entre las ocurrencias de un modelo de Poisson"== 
- Como poisson, se distribuye en muestras de tasa fijas con ocurrencias independientes. 
- La probabilidad es mayor en valores cercanos a la esperanza

Sea $\tau$ la tasa de tiempo o espacio en el que ocurre algo:
Función Probabilidad: 
$$
P(X=k)=
\begin{cases}
\frac{1}{\tau}e^{-\frac{k}{\tau}},\\
0 ; c.o.c
\end{cases}
$$ 
Esperanza: $\tau$ 
Varianza: $\tau²$ 
Distribución: $\chi²$ donde $\chi^{2}_{k}=[N(0,1)]²+[N(0,1)]²+...+[N(0,1)]²$ hasta el $k$-esimo termino,
donde $k$ son los grados de libertad.
$E(\chi_{k}^{2})=k$ ; $Var_{\chi_{k}^{2}}=2k$ 

### Control: 
- Distribuciones (Binomial, Geometrica, Binomial negativa, Poisson)

### PRUEBA: 
- Probabilidad / Conjuntos
- Bayes
- Variable aleatoria discreta
- FUncion de masa
- Función de prob. acumulada
- Distribuciones 

# CLASE 30/09 

##### La estadística es la:
- Recolección
- Limpieza
- Analisis
- Interpretación
de datos


### CONCEPTOS

- Población: EL universo de nuestro experimento
- Muestrar: Parte de la población se divide en dos subconjuntos:
-Probabilistica: Escoger al azar
-Representativa: Proporciones de Subgrupos parecidas a la población

- Estadistica Descriptiva 
- Conjeturas (Analisis exploratorio de datos)
- Estadistica inferencial

# Ayudantia 01/10
### Frecuencias en datos discrestos (notación)

- $x_i$ : Dato (raw data)
- $f_i$: Frecuencia absoluta (Numero de veces que se repite el dato)
- $F_i$: Frecuencia acumulada (Suma de las $f_i$ hasta cierto dato)
- $h_i$: Frecuencia relativa ($\frac{f_i}{N}$ donde $N$ es el total de datos).
- $H_i$ : Frecuencia relativa acumulada (Suma de las $h_i$ hasta ese dato)

# Medidas de disperción (de datos)

 Definición: Una medida de disperción informa sobre que tan diferentes o similares son los datos entre si. 

### Rango: $x_{max}-x_{min}=R$ 

Se intepreta el "espacio" en el que se pueden mover los datos, aunque esta medida es muy relativa o subjetiva.

### Rango intercuartílico: $R_I=P_{75}-P_{25}=Q_3-Q_1$ 

Percentil: Se obtiene un dato $P_K$, desde cuyo dato se cuentan todos los datos hasta el dato minimo, considerando un K% de los tados. (tambien se puede ver como un intervalo $[x_{min},K]$). Cnsidere que el intervalo restante es el 100-K% de las observaciones ($]K,x_{max}]$).

El rango intercualticilo obtiene, en cierta manera, la distribución de los datos en el centro.

### Como calcular cualquier percentil 
Sea un percentil $P_K$ perteneciente a un intervalo $[L_i,L_n]$ siendo el intervalo numero $i$ en una muestra de datos, $N$ el numero de datos totales, $F_{i-1}$ la frcuencia acumulada del intervalo anterior y $f_i$ la frecuencia de el intervalo actual.

Usamos la siguiente formula:
$$P_K=L_i+\frac{\frac{KN}{100}-F_{i-1}}{f_i}\cdot A_i$$

### Varianza : $Var(x)=\frac{\sum_{i=1}^{n}(\bar{x}-x_i)²}{n}$ 
Mide la distancia entre cada dato y el promedio. 

### Desv. estandar : $\sigma=\sqrt{Var(x)}$ 


### Coeficiente de variación: $\frac{\sigma}{\bar{x}}=C.V$

Es una metrica independiente de que tan grandes o pequeños sean los datos 

### Error estandar (para medidas absolutas): $\sqrt{n}\cdot \sigma$ 
donde $n$ es el numero de experimentos y $\sigma$ es la desviación estandar de nuestra variable aleatoria

## Ley de los grandes números

##### Definición debil: $\lim_{h\to{\infty}}P_r(|\bar{x}-u|<\epsilon)=0$ ; $\forall{\epsilon}>0$ 

##### Definición Fuerte: $P_r(\lim_{h\to{\infty}}{|\bar{x_n}-u}|)=0$

En palabras, a medida que tomamos más muestras, la proporción experimental se acerca a la teórica casi con seguridad.

control miercoles:

distribución normal y exponencial
teorema del limite central
# Clase 16/10

### ¿Cuando usar distribución normal o TCL?
### Dist. normal
Si conocemos la desv. estandar (o varianza) y la media, usamos la dist normal:

Esto es $\frac{\bar x-\mu}{\frac{\sigma}{\sqrt{n}}}$~$N(0,1)$ 

### TCL (para una muestra)
Si conocemos la media, pero no la desv. estandar (o varianza) usamos teorema central del limite (tcl) en LA muestra:
Esto es: $\frac{\bar x-\mu}{\frac{s}{\sqrt{n}}}$~$t_{n-1}$ 


Parametros de población: $\mu$, $\sigma$ y $n$ (media, desv. estandar y la muestra aleatoria poblacional (o población total, respectivamente)
note que $s$ es la desv estandar de la muestra dada 
Normalmente son numeros fijos


### Ejercicios: 


#### Media muestral de sueldos

"enunciado"

en este caso, conocemos la desv. estandar y la media, por lo que usamos una distribución normal:

$\Rightarrow\frac{\bar{x}-2500}{\frac{600}{\sqrt{64}}}$~$N(0,1)$ 
luego, nos piden $P(\bar{x}<2350)$
entonces, usando la "estandarización": 

$\Rightarrow P(\bar{x}<2350)=P(\frac{\bar{x}-2500}{\frac{600}{\sqrt{64}}}-\frac{2350-2500}{\frac{600}{\sqrt{64}}})=P(\frac{\bar{x}-2500}{{75}}<-2)\approx{0.0228}$ (observando la tabla en canvas)

#### Gasto promedio familiar en el feriado del 21 de mayo

"enunciado"
"a"
"b"

##### a) $P(\bar{x}>263.000)$

en este caso, usamos $\frac{\bar{x}-250.000}{\frac{130.000}{\sqrt{150}}}=\frac{\bar{x}-250.000}{10.614}$~$t_{149}$ dado que $\mu=250.000;S=130.000;n=150$ 

entonces $P(\bar{x}>263.000)=P(\frac{\bar{x}-250.000}{10.614}>\frac{263.000-250.000}{10.614})=P(\frac{\bar{x}-250.000}{10.614}>1.22)\approx{0.1}$ 

##### b) $P(\frac{S²}{2}>41.65)=P(S²>83.3)$
$=P(\frac{(61-1)S^2}{20.000²}>\frac{(61-1)\cdot{83.3}}{20.000²})=P(\chi²_{60}>1.2\cdot{10⁵})\approx{1}$ 



### Distribución Muestral | Varianza muestral

#### $\frac{(n-1)S²}{\sigma²}=\frac{\sum_{1=1}^{n}(x_i-\bar{x})²}{\sigma²}$~$\chi_{n-1}$ 

$\chi_1,\chi_2,...,\chi_n$ vienen de una distribución normal



### DIst. Continuas:

- Normal
- $T_2$
- $\chi²$ 
- Exponencial
- General




## Ejercicios Dist. Continuas y muestrales


### Distribución del porcentaje compuesto en el combustible


Notamos que la variable aleatoria es $X$: Porcentaje de compuesto por galon

entonces, $X$~$N(33,9²)$ 

#### a) Se interpreta como $P(35\leq{X}\leq{40})$ 

como una variable aleatoria normal no puede integrarse, usamos $z=\frac{x-\mu}{\sigma};Z$~$N(0,1)$ 

entonces, podemos interpretar la probabilidad que buscamos como:

$$P(\frac{35-33}{9}\leq{z}\leq{\frac{40-33}{9}})\approx{P(0.22\leq{z}\leq{0.78})}$$
luego, note que $P(0.22\leq{z}\leq{0.78})=P(z\leq{0.78})-P(z<22)=0.7823-0.5871=0.1952$ 

#### b) Se intepreta como el valor que da el percentil 84.13

Sea $z_0$ el valor que "genera" el percentil 84.13%=0.8413
$$\Rightarrow P(z<z_0)=0.8413\Rightarrow z_0=1$$

luego, $\frac{x-33}{9}=1\Rightarrow x=42$ 

finalmente, el porcentaje de compuesto máximo que tiene el 84.13% de produccion de galones es de un 42% 


### Distribución del gasto de los consumidores en un mall

notamos que la variable aleatoria es:

$X$:Gasto un domingo en un mall (en miles de pesos) $\Rightarrow{X}$~$N(65,40²)$

#### a)

#### b) Nos piden $P(X>120)$ 

entonces, estandarizando usando $z=\frac{x-\mu}{\sigma}$:
$$\Rightarrow P(X>120)=P(z>\frac{120-65}{40})=P(z>1.38)=1-P(z\leq{1.38})=1-0.9162=0.0838$$
entonces, la probabilidad de que el gasto supere el monto dado es de un 8% aprox.

#### c) Se interpreta como el percentil 30 si se invierte el orden de los datos, es decir, el percentil 70 de los datos en orden común.

esto nos implica que $P(z<z_0)=0.7$, donde que $z_0=\frac{x_0-65}{40}$ y $x_o$ es el valor que "genera" al percentil 70 y $z_0$ es el valor estandarizado
$\Rightarrow z_0=0.52$
finalmente, de $\frac{x_0-65}{40}=0.52\Rightarrow{x_0=85.8}$ 

### Tiempo entre llamadas a una empresa de charcutería

Notamos que la variable aleatoria y su distribución son:
$X$:TIempo entre llamadas
$X$~$Exp(\lambda=10)$ 

#### a) Se intepreta como $P(X<5)$ 

$P(X<5)=\int_{0}^{5}\frac{1}{10}e^{-\frac{x}{10}}dx=1-e^{-\frac{1}{2}}\approx{0.39}$ 

entonvces, la probabilidad de que transcurran menos de 5 minutos antes de recibir la primera llamada es de un 40% aprox

#### b) Se intepreta como $P(X<k)=0.9$ 

entonces, $P(Z<k)=\int_{0}^{k}\frac{1}{10}e^{-\frac{x}{10}}dx=1-e^{-\frac{k}{10}}=0.9$ 

$\Rightarrow{k=-10ln(0.1)\approx{23.03}}$ 



### Variabilidad en el contenido de carne de hamburgesas




### Ventas diarias de un analgésico 

#### datos: 
- $\mu=367.800$ 
- $\sigma²=62.450^2$ 
- $n=30$ (tamaño de mi muestra)

sea $\bar{X_n}$ el promedio de mi muestra, nos piden por:
$$P(\bar{X_n}<350.000)$$
y por T.C.L, $\bar{X_n}$~$N(\mu,\frac{\sigma²}{n})$ 

entonces, estandarizando (dado a que sigue una dist. normal):
$$\Rightarrow Z_n=\frac{\bar{X}-\mu}{\frac{\sigma}{\sqrt{n}}}$$
donde $Z_n$~$N(0.1)$ 


luego, $P(\bar{X_n}<350.000)=P(Z_n<\frac{350.000-367.800}{\frac{62.450}{\sqrt{30}}})=P(Z_n<-1.56)\approx{0.0594}$ 




## Distribuciones muestrales ejercicios


### Variabilidad en el contenido de carne de hamburgesas


#### a) 
##### Datos poblacionales: 
- $\mu=114.29$ ; $Var=5.71²$ 
##### Datos de la muestra:
- $n=25$ ;$Var=11.43$ 

notamos que la muestra de tamaño 25 sigue una distribución muestral de la varianza:

es decir $\frac{(n-1)S²}{\sigma²}$~$\chi²_{n-1}$ 

entonces, nos pidne por $P(S²\geq{8.664})$ , que estandarizando, queda:
$$P(\frac{(n-1)S²}{\sigma²}\geq\frac{(n-1)8.664}{\sigma²})=P(\frac{24\cdot S²}{5.71}\geq\frac{24\cdot 8.664}{5.71})=P(\frac{24\cdot S²}{5.71}\geq36.4161)$$
Luego, mirando la tabla (viendo el grado de libertad (numero de muestras) $v$ y el numero que se quiere comparar $36.4161$ )
$$\Rightarrow P(\frac{24\cdot S²}{5.71}\geq36.4161)=0.05$$

#### b) 
El supuesto de normalidad es necesario porque sin esta, no se puede ocupar el teorema dado a que esta dado solo para variables aleatorias en una población que siguen una distribución normal.




### Probabilidad de éxito en contactos telefónicos


Sea $X$: Numero de llamadas exitosas
$\Rightarrow{X}$~$Binom(100,p)$ donde $p=0.45$ 

entonces, notemos que nos piden una proporcion de exitos, es decir, a todos los parametros, se les divide por el total de intentos (en este caso $N=100$)

nos piden por $P(\bar{p}\leq{0.48})$ , que estandarizando queda:
$$=P(\frac{\bar{p}-p}{\sqrt{\frac{pq}{N}}}\leq\frac{0.48-p}{\sqrt{\frac{pq}{N}}})$$
donde $\bar{p}$ es la probabilidad de la muestra y $p$ es la probabilidad e extio de la población
entonces:
$$P(\frac{\bar{p}-p}{\sqrt{\frac{pq}{N}}}\leq\frac{0.48-p}{\sqrt{\frac{pq}{N}}})\approx P(\frac{\bar{p}-0.45}{0.05}\leq{0.6})=0.7257$$

## Ejercicios de estimadores

#### COnceptos:
- Población (Parametro):$\theta$ 
- Muestra (Variable aleatoria): $\bar{\theta}$ 
- Error cuadratico medio ($E[(\theta-\bar{\theta²})]=Var(\bar{\theta})+E[\theta-\bar{\theta}]$) donde $E[\theta-\bar{\theta}]$ es un estimador sesgado y $Var(\bar\theta)$ es la eficiencia del estimador

" No existen errores que sean 0"





















 


