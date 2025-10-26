
# Certamen 1
# Propiedades de conjuntos

### 1. $P(\emptyset)=0$ 
### 2. $P(A^{C})=1-P(A)$
### 3.$P(A-B)=P(A\cap{B^{C}})$ 
### 4. $P(A\cup{B})=P(A)+P(B)-P(A\cap{B})$ 
### 5.$P(A\cup{B}\cup{C})=P(A)+P(B)+P(C)$
### $-P(A\cap{B})-P(A\cap{C})-P(B\cap{C})$
### $+2P(A\cap{B}\cap{C})$ 


# Probabildad condicional 

### $P(A|B) = \frac{P(A\cap{B})}{P(B)}$ (Probabilidad de A dado B)

### independecia: 

#### A y B son independientes si y solo si: 

### $P(A|B)=P(A)$ y $P(B|A)=P(B)$


# Teorema de bayes

### Considerando un espacio muestral $S$ con $(A_1,A_2,A_3)$ eventos colectivamente exauhtivos (si o si pasa uno de ellos) y $B$ es un evento en $S$: 

## $P(A_i|B)=\frac{P(A_i)P(B|A_i)}{P(B)}=\frac{P(A_i)P(B|A_i)}{\sum_{k=1}^{n}P(A_k)P(B|A_k)}$ 


### Donde $B=\sum_{k=1}^{n}P(A_k)P(B|A_k)$ (Probabilidad total de un evento)

# Permutación (El orden importa): 

### $P^{n}_k=\frac{n!}{(n-k)!}$ 

# Combinatoria (El orden no importa): 
### $C^{n}_{k}=\frac{n!}{k!(n-k)!}$ 
# Permutación circular: 
### $P^{n}=\frac{n!}{n}=(n-1)!$ 



# BERNOULLI: 

Funcion: $f_x(x)=p(X=x)=p^{x}(1-p)^{1-x};x=0...$ 
$p$ es la prob. de exito y $q$ el complemento de $p$ 
media = $p$ 
esperanza = $p$ 
varianza = $p(1-p)=pq$ 

"Evento binario, de un solo intento"
# Binomial: 

FUnción: $f_x(x)=p(X=x)=\binom{n}{x}p^{x}q^{n-x};x\in{[0...n]}$ ; $q=1-p$ 
Esperanza : $n\cdot{p}$ 
Varianza : $npq$ 
donde $n$ es la cantidad de intentos y $p$ la probabilidad de exito

"numero de exitos en n intentos independientes"
# Geometrica: 

Función : $P(X=k)=(1-p)^{(k-1)}\cdot{p}=p\cdot{q^{(k-1)}}$ 
donde $p$ es la prob. de exito
Media : 
Esperanza : $\frac{1}{p}$ 
Varianza: $\frac{(1-p)}{p²}=\frac{q}{p²}$ 
"Número de intentos hasta el primer exito (incluyendo el exito)"

# Binomial Negativa
Función: $P(X=k)=C^{k-1}_{r-1}p^rq^{(k-r)}$  
donde $r$ es el numero de exitos deseados y $p$ la prob. de exito.
Esperanza: $\frac{r}{p}$ 
Varianza: $\frac{rq}{p^2}$ 
"Número de intentos hasta el r-esimo exito (incluyendo el ultimo exito)"
# Hipergeometrica

"Número de existos al muestrear $n$ elementos sin remplazo de una población finita de tamaño $N$ que contiene $K$ exitos"

Función: $P(X=k)=\frac{C_{k}^{K}C_{n-k}^{N-K}}{C_{n}^{N}}$ 
Esperanza: $n\frac{K}{N}$ 
Varianza: $n\frac{K}{N}\frac{1-K}{N}\frac{(N-n)}{N-1}$ 

# Poisson 
Función: $P(X=k)=\frac{e^{-\lambda}\lambda^k}{k!}$ 
Esperanza: $\lambda$ 
Varianza: $\lambda$ 
"Numero de eventos raros que ocurren en un intervalo fijo de tiempo o espacio (con tasa promedio $\lambda$)"



# Certamen 2



## Distribución Exponencial

Sea $X$ la variable aleatoria y $\lambda$ la media de dicha variable: 

Notación: $X$~$exp(\lambda)$
Función probabilidad: $P(X=k)=\lambda e^{-\lambda k}$ ; $k\geq{0}$
Media: $\mu_X=frac{1}{\lambda}$
Varianza: $\sigma²=\frac{1}{\lambda²} \Rightarrow$ Varianza: $\sigma=\pm\frac{1}{\lambda}$ (dependiendo del contexto)

""
## Distribución Normal

Se utiliza en una variable aleatoria $X$ en una población, donde conocemos la media ($\mu$) y desviación estandar ($\sigma²$).

Notación: $X$~$N(\sigma²,\mu)$


La probabilidad de esta se obtiene a travez de una tabla que aproxima la probabilidad de nuestra variable aleatoria

## Teorema central del limite


## Distribuciones de tendencia central