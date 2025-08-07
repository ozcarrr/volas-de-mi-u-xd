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

     # $P^n = n!/(n-k)!$ 
     
     entonces, $P(ROLES)=40!/(40-3)!$


     Pero, si el orden no importara, se tiene lo siguiente:

     ## $C^n=n!/k!(n-k)!$  
     
     donde n es el total de elementos y k la cantidad de combinaciones en n elementos
     entonces $P(ROL SIN ORDEN)=40!/3!(40-3)!$ 