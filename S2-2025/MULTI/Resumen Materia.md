# Vectores $\vec{T};\vec{B};\vec{N}$ (Unitarios)
Sea $\vec{r}(t)$ una función vectorial, sus vector tangente es:

$\vec{T}(t)=\frac{\vec{r}'(t)}{||\vec{r}'(t)||}$ 

Su vector normal esta dado por:

$\vec{N}(t)=\frac{\vec{T}'(t)}{||\vec{T}'(t)||}$ 

Su vector Binormal esta dado por:

$\vec{B}=\vec{T}\times{\vec{N}}$

### Observaciones 

$\vec{T}=\vec{N}\times{\vec{B}}$ 
$\vec{N}=\vec{T}\times{\vec{B}}$ 
$\vec{B}=\vec{T}\times{\vec{N}}$ 

$\vec{T}\cdot\vec{T}=1$ 
$\vec{N}\cdot\vec{N}=1$ 
$\vec{B}\cdot\vec{B}=1$ 



# Longitud de arco 

Sea $\vec{r}(t)$ una función vectorial donde existe un $t_0\in{dom(r)}$, se define la longitud de arco de $\vec{r}$ relativa de $t_0$ hasta $t$ como:

$s(t)=\int_{t_0}^{t}||\vec{r}'(u)||du$ 

# Reparametrización respecto a longitud de arco

sea $s(t)$ la función longitud de arco de $\vec{r}$, se tiene:

$s=s(t)\Rightarrow{t=t(s)}$ , donde remplazamos $t(s)$ en nuestra función vectorial $\vec{r}$ , quedando una nueva función que llamaremos $\beta(t)$, donde $||\beta'(t)||=1$, entonces, $\beta(t)$ es una función parametrizada respecto a longitud de arco

### observación : 
Si $||\vec{r}'(t)||=1$, la función vectorial $\vec{r}(t)$ ya esta parametrizada respecto a longitud de curva


# Planos (Rectificante, normal y osculador)

### Plano Rectificante
Generado por los vectores $\vec{T}$ y $\vec{B}$ , por ende ortogonal al vector $\vec{N}$, entonces, la ecuación del plano rectificante a una función vectorial $\vec{r}(t)$ en un punto $(x_0,y_0,z_0)=\vec{r}(t_0);t_0\in{dom(f)}$ esta dada por:

$\vec{N}(t_0)\cdot(x-x_0,y-y_0,z-z_0)=0$ 

### Plano Normal 
Generado por los vectores $\vec{N}$ y $\vec{B}$, por ende ortogonal al vector $\vec{T}$, entonces, la ecuación del plano normal a una función vectorial $\vec{r}(t)$ en un punto $(x_0,y_0,z_0)=\vec{r}(t_0);t_0\in{dom(f)}$ esta dada por:

$\vec{T(t)}\cdot(x-x_0,y-y_0,z-z_0)=0$ 

### Plano osculador
Generado por los vectores $\vec{T}$ y $\vec{N}$, por ende ortogonal al vector $\vec{B}$, entonces, la ecuación del plano normal a una función vectorial $\vec{r}(t)$ en un punto $(x_0,y_0,z_0)=\vec{r}(t_0);t_0\in{dom(f)}$ esta dada por:

$\vec{B}(t)\cdot(x-x_0,y-y_0,z-z_0)=0$ 


# Curvatura y torsion

Sea $\vec{r}(t)$ una función vectorial, su curvatura y torsión estan dadas por:
### Curvatura

$k(t)=\frac{||\vec{r}'(t)\times\vec{r}''(t)||}{||\vec{r}'(t)||³}$ 

### Torsión
Mide el desvio de la curva respecto al plano osculador. 

$\tau(t)=\frac{(\vec{r}'(t)\vec{r}''(t))\cdot{\vec{r}'''(t)}}{||\vec{r}'(t)\times\vec{r}''(t)||}$ 


# Componentes tangencial y normal de la aceleración: 

### Tangencial : $a_T=\frac{r'(t)\cdot\vec{r}''(t)}{||\vec{r}'(t)||}$ 
### Normal : $a_N=\frac{||\vec{r}'(t)\times\vec{r}''(t)||}{||\vec{r}'(t)||}$ 


# Funciones de varias variables

## Conjuntos de nivel






