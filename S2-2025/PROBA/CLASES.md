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

#### $P(X...)=$ {P x=1; 1-P=q x=0}


### Possiar : Eventos que se repiten cada cuanto tiempo independientemente  (Taza promedio de repetición: $P_0:(\lambda))$ 

### Binomial: Repetir n veces experimentos independientes, bernally con p fija. 

# $P$(Obtener 2 exitos) = $\binom{3}{2}p²q¹=3$ 


# $P(X=k)=\binom{n}{k}p^{k}q^{n-k}$ 


## Propiedades de la esperanza: 

# 1. $E(ax+b)=aE(x)+b$ 
# 2. $E(x+y)=E(x)+E(y)$ 
# 3. Si $x$ e $y$ son independientes:

# $E(xy)=E(x)E(y)$ 


## Propiedades Variante:

# 1.$Var(ax)=a²Var(x)$ 
# 2. $Var(x+b)=Var(x)$ 
# 3. Si $x$ e $y$ son independientes: 

# $Var(x+-y)=Var(x)+-Var(y)$ 


































 


