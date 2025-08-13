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












