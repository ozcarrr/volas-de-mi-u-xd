


![[Pasted image 20251019191658.png]]

# Tarea 1 Ecuaciones Diferenciales

## S2-2025
## Docente: Juan Rossel
## Sección: 2
## Integrantes:

- Sebastian Herrera
- Benjamín Pinto
- Oscar Pichuman


## 1)
### a) Encuentre las trayectorias ortogonales de todas las parábolas con vértice en el origen y  foco sobre el eje $x$. Haga un bosquejo de las gráficas.

Notamos que la forma canonica de una parabola con dichas condiciones esta dada por:
$$y²=4px=cx$$
donde $c=4p$. 

entonces, para obtener la pendiente de esta curva, diferenciamos:
$$\Rightarrow 2y\frac{dy}{dx}=c$$ sustituyendo $c$ en la ecuación original: 
$$\Rightarrow y^2=2y\frac{dy}{dx}x\Rightarrow\frac{dy}{dx}=\frac{y}{2x}=m_f$$
donde $m_f$ es la pendiente de la curva de la familia (1), entonces, por calcular la pendiente de la curva de la familia(2), $m_g$:
$$\Rightarrow m_g\cdot{m_f}=-1\Rightarrow m_g=-\frac{2x}{y}$$
entonces, la edo de la familia $g$ queda:

$$\frac{dy}{dx}=-\frac{2x}{y}\Rightarrow ydy=-2xdx\Rightarrow\frac{y²}{2}=-x^2+k\Rightarrow y²+2x^2=k$$
entonces, $g:y²+\frac{x²}{\frac{1}{2}}=k$ es una familia de elipses cuyas rectas tangente son perpendiculares a las rectas tangentes de la familia de  parábolas $f:y^2=cx$ cuando interceptan.


![[Screenshot from 2025-10-19 19-12-01.png]]
### b) Encuentre las trayectorias ortogonales de todas las hipérbolas equilateras de centro del origen de coordenadas.

tomando a $f$ como nuestra hipérbola, tomamos la forma canónica de hipérbolas equilateras con centro en el origen:
$$x^2-y²=c$$
diferenciando:
$$2x-2y\frac{dy}{dx}=0\Rightarrow m_f=\frac{dy}{dx}=\frac{x}{y}$$
entonces, calculando $m_g$:
$$m_f\cdot m_g=-1\Rightarrow m_g=-\frac{y}{x}$$
La ecuación diferencial de $g$ queda como una de variables separables:
$$\frac{dy}{dx}=-\frac{y}{x}\Rightarrow \frac{dy}{y}=-\frac{dx}{x}\Rightarrow ln|y|=-ln|x|+k\Rightarrow y=\frac{k}{x}$$
entonces, las trayectorias ortogonales quedan como $f:x²-y²=C$ y $g:y=\frac{k}{x}$.

### c) Encuentre las trayectorias ortogonales de la familia de elipses con centro el origen de cordenadas vertices sobre los puntos $(1,0)$ y $(-1,0)$.

La familia de elipses con las condiciones dadas esta dada por la ecuación:
$$x²+\frac{y²}{b²}=x²+\frac{y²}{c}=1$$
Diferenciando la ecuación:
$$2x+\frac{2y}{c}\cdot\frac{dy}{dx}=0\Rightarrow\frac{dy}{dx}=-\frac{cx}{y}$$
luego, de la primera ecuación, obtenemos $c=\frac{y²}{1-x²}$, entonces:
$$m_f=\frac{dy}{dx}=-(\frac{y²}{1-x²})\frac{x}{y}=-\frac{xy}{1-x²}$$
entonces, calculando $m_g$:
$$m_g\cdot{m_f}=-1\Rightarrow m_g=\frac{1-x²}{xy}$$
entonces, la edo de $g$ queda como una de variables separables:
$$m_g=\frac{dy}{dx}=\frac{1-x²}{xy}\Rightarrow ydy=\frac{1-x²}{x}dx\Rightarrow\frac{y²}{2}=ln|x|-\frac{x²}{2}+k$$
finalmente, multiplicamos por 2:
$$\Rightarrow y²+x²-2ln|x|=k$$
entonces, las trayectorias ortogonales quedan de la forma $f:x²+\frac{y²}{c}=1$ y $g:y^2+x²-2ln|x|=k$.



### d) Si el angulo que forman las familias de curvas no es recto, pero sí fijo, las trayectorias son llamadas isogonales. Encuentre una familia de trayectorias isogonales corten a la familia de circunferencias $x² + y^2 = r^2;(r > 0)$ con un ́angulo de $\frac{\pi}{4}$ radianes.


Tomando a $f$ como la familia de circulos, diferenciamos:
$$\Rightarrow 2x+2y\frac{dy}{dx}=0\Rightarrow\frac{dy}{dx}=m_f=-\frac{x}{y}$$
luego, sea $\alpha=\frac{\pi}{4}$ el angulo que se forma entre ambas trayectorias:
$$\Rightarrow tan(\alpha)=1=\frac{m_g-m_f}{1+m_gm_f}\Rightarrow m_g=\frac{y-x}{y+x}$$
entonces, la edo queda de la forma:

##### $m_g=\frac{dy}{dx}=\frac{y-x}{y+x}$ 

Sea $y=vx\Rightarrow\frac{dy}{dx}=v+x\frac{dv}{dx}$, entonces:

##### $v+x\frac{dv}{dx}=\frac{vx-x}{vx+x};x\not=0\Rightarrow x\frac{dv}{dx}=-\frac{v²+1}{v+1}$ que es una EDO de variables separadas, entonces:
$$\frac{v+1}{v²+1}dv=-\frac{dx}{x}\Rightarrow(\frac{v}{v²+1}+\frac{1}{v²+1})dv=-\frac{dx}{x}$$
integrando:
$$\Rightarrow\frac{1}{2}ln(v²+1)+arctan(v)+k=ln(x)$$
multiplicando por $2$ y devolviendo a $x$:
$$\Rightarrow ln(1+(\frac{y}{x})²)+2arctan(\frac{y}{x})=-2ln(x)+k$$
entonces: 
$$\Rightarrow g:ln(x²+y²)+2arctan(\frac{y}{x})=k$$
finalmente, las trayectorias isogonales quedan de las formas $f:x²+y²=r²$ y $g:ln(x²+y²)+2arctan(\frac{y}{x})=k$ 


## 2) 


### a) 

#### 1. Solución de equilibrio: Valor constante que es solución de una ecuación diferencial

#### 2. Atractor: Es una solución de equilibrio que, cuando la variable independiente de la EDO empieza a tender al $+\infty$, las soluciones empiezan a acercarce a dicha solución.
#### 3. Repulsor: Es una solución de equilibrio que, cuando la variable independiente de la EDO empieza a tender al $+\infty$, las soluciones empiezan a alejarse a dicha solución.

### b) 

#### 1. $\frac{dy}{dx}=-(y-1)$ es una edo con con un atractor.

Pues, hay equilibrio unico en $y=1$ y si $x\to\infty$, las soluciones de $y>1$ o $y<1$ convergen a $y=1$ 

#### 2. $\frac{dy}{dx}=y-1$ es una edo con un repulsor.

Pues, hay equilibrio unico en $y=1$ y si $x\to\infty$, las soluciones de $y>1$ o $y<1$ divergen o se alejan de  a $y=1$ 


