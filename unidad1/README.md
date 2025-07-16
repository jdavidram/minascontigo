<table border=1>
  <thead>
    <th>
      <img src="https://minas.medellin.unal.edu.co/images/Programa-Minas-Contigo/Logo-Minas-Contigo.png" width="320px" height="270px" />
    </th>
    <th>
      <h1>Integrales</h1>
    </th>
  </thead>
</table>

# Notación Sigma

El **Operador sumatoria** nos permite escribir la suma de varios números $a_m, ..., a_n$ $(m \leq n)$ en la forma compacta

$$
\sum_{i=m}^{n} a_i = a_m + a_{m+1} + ... + a_{n-1} + a_{n}
$$

Por definición

> Indica terminar en $i = n$
> 
> La letra $\sum$ significa suma
> 
> Indica iniciar en $i = m$

## Propiedades de la sumatoria

$$
\sum_{i=1}^{n} c = n*c
$$

$$
\sum_{i=1}^{n} c*a_i = c*\sum_{i=1}^{n} a_i
$$

$$
\sum_{i=1}^{n} (a_i \pm b_i) = \sum_{i=1}^{n} a_i \pm \sum_{i=1}^{n} b_i
$$

## Algunas fórmulas para sumatorias

$$
\sum_{i=1}^{n} i = \frac{n*(n+1)}{2}
$$

$$
\sum_{i=1}^{n} i^2 = \frac{n*(n+1)*(2n+1)}{6} = \frac{n^3}{3} + \frac{n^2}{2} + \frac{n}{6}
$$

$$
\sum_{i=1}^{n} i^3 = (\frac{n*(n+1)}{2})^2 = \frac{n^4}{4} + \frac{n^3}{2} + \frac{n^2}{4}
$$

# El problema del área

Queremos resolver **el problema del área bajo la curva** $y = f(x)$, $x \in [a, b]$: Hallar el área de la región limitada por la gráfica de una función continua *f*, donde $f(x) \geq 0$, las rectas verticales $x = a$, $x = b$ y el eje *x*:

$$
\Delta x = \frac{b-a}{n}
\\
x_i = a + i*\Delta x
\\
x_{i-1} = a + (i-1)*\Delta x
$$

Luego, la aproximación del área por la derecha es:

$$
R_n = \sum_{i=1}^{n} f(x_i)*\Delta x
$$

y por la izquierda es:

$$
L_n = \sum_{i=1}^{n} f(x_{i-1})*\Delta x
$$

Por tanto, se define el **área bajo la curva** *f* por

$$
A = \lim_{n \to \infty} R_n = \lim_{n \to \infty} L_n = \lim_{n \to \infty} \sum_{i = 1}^{n} f(x_{i}^{*})*\Delta x
$$

# El problema de la distancia

Supongamos que se quiere calcular la distancia recorrida por un objeto móvil. Sabemos que si la velocidad es constante, entonces:

$$
velocidad = \frac{distancia \ recorrida}{tiempo \ transcurrido} \rArr d = v*t
$$

Pero, ¿Qué pasa si la velocidad varía durante el recorrido; es decir, $v = v(t)$?

En general, si $v(t) \geq 0$ es la velocidad en un instante *t*, definimos la **distancia recorrida** como:

$$
d = \lim_{n \to \infty} \sum_{i=1}^{n} v(t_i)*\Delta t
$$

# Integral definida

Si *f* es una función continua definida para $x \in [a, b]$. Dividimos el intervalo *[a, b]* en *n* subintervalos de tamaño $\Delta x = \frac{b-a}{n}$ y elegimos los puntos $x_{i}^{*} \in [x_{i-1}, x_{i}]$. Entonces **la integral definida de f, desde a hasta b**, es:

$$
\int_{a}^{b} f(x)dx = \lim_{n \to \infty} \sum_{i=1}^{n} f(x_{i}^{*})*\Delta x
$$

Si el límite existe, decimos que $f$ es **integrable sobre [a, b]**.

* En $\int_{a}^{b} f(x)dx$ la función $f$ es llamada **integrando** y los números $a, b$ son los **límites de integración**.
* La integral definida es un número real y no depende de la variable que usemos.
* No importa que valores toman los puntos de muestra $x_{i}^{*}$: Pueden ser $x_{i-1}$ o $x_i$ o un punto arbitrario en cada subintervalo.
* Si $f \geq 0$ en [a, b], entonces $\int_{a}^{b} f(x)dx$ = **área bajo f**.
* Sólo se pide que $f$ sea continua y puede ser positiva o negativa. Si $f$ toma tanto valores positivos como negativos, entonces la integral se puede interpretar como un **área neta**.

$$
\int_{a}^{b} f(x)dx = (área \ sobre \ el \ eje \ x) - (área \ debajo \ del \ eje \ x)
$$

* A la suma $\sum_{i=1}^{n} f(x_{i}^{*})*\Delta x$ se le denomina **suma de Riemann de f**.

## Propiedades de la integral definida

Sean $f$ y $g$ integrables sobre [a, b] y c $\in \mathbb{R}$.

$$
\int_{a}^{b} c*f(x)dx = c*\int_{a}^{b} f(x)dx
$$

$$
\int_{a}^{b} cdx = c*(b-a)
$$

$$
\int_{a}^{a} f(x)dx = 0
$$

$$
\int_{a}^{b} [f(x) \pm g(x)]dx = \int_{a}^{b} f(x)dx \pm \int_{a}^{b} g(x)dx
$$

$$
\int_{a}^{b} f(x)dx = \int_{a}^{c} f(x)dx + \int_{c}^{b} f(x)dx
$$

$$
\int_{a}^{b} f(x)dx = -\int_{b}^{a} f(x)dx
$$

> **Nota:** $\frac{b-a}{n} = -\frac{a-b}{n} = -\Delta x$

* Si $0 \leq f(x)$ en [a, b], entonces $0 \leq \int_{a}^{b} f(x)dx$.

* Si $g(x) \leq f(x)$ en [a, b], entonces $\int_{a}^{b} g(x)dx \leq \int_{a}^{b} f(x)dx$.

* Si $m \leq f(x) \leq M$ en [a, b], entonces:

$$
m*(b-a) \leq \int_{a}^{b} f(x)dx \leq M*(b-a)
$$

> **Nota:** $M = max_{x \in [a, b]} \ f(x)$ y $m = min_{x \in [a, b]} \ f(x)$.

# Antiderivada

Una función $F$ se dice que es una **antiderivada** (o una **primitiva**) de una función $f$ sobre un intervalo $I$ si:

$$
F'(x) = f(x) \ para \ todo \ x \in I
$$

Si $F$ es una antiderivada de $f$ sobre $I$, entonces la antiderivada más general de $f$ sobre $I$ es $F(x) + C$, donde $C \in \mathbb{R}$ es una constante arbitraria.

## Integral indefinida

> $\int f(x)dx = F(x) + C$ significa que $F'(x) = f(x)$.

### Tabla de integrales fundamentales

$$
\int x^{r}dx = \frac{x^{r+1}}{r+1} +C \ (r \neq -1)
$$

$$
\int k*dx = k*x +C
$$

$$
\int \frac{1}{x}dx = ln|x| +C
$$

$$
\int e^{x}dx = e^{x} +C
$$

$$
\int cos(x)dx = sin(x) +C
$$

$$
\int sin(x)dx = -cos(x) +C
$$

$$
\int sec^{2}(x)dx = tan(x) +C
$$

$$
\int sec(x)*tan(x)dx = sec(x) +C
$$

$$
\int csc^{2}(x)dx = -cot(x) +C
$$

$$
\int csc(x)*cot(x)dx = -csc(x) +C
$$

$$
\int \frac{1}{\sqrt{1 - x^2}}dx = sin^{-1}(x) +C
$$

$$
\int \frac{-1}{\sqrt{1 - x^2}}dx = cos^{-1}(x) +C
$$

$$
\int \frac{1}{1 + x^2}dx = tan^{-1}(x) +C
$$

# Movimiento rectilíneo

La antiderivación es en particular útil al analizar el movimiento de un objeto que se mueve en línea recta. Se sabe del **Cálculo Diferencial** que si $s(t)$ es la función posición, la velocidad es $v(t) = s'(t)$. Esto significa que $s(t)$ es una antiderivada de $v(t)$. De forma análoga, la función aceleración es $a(t) = v'(t)$, de modo que la velocidad es una antiderivada de la aceleración.

# Teorema Fundamental del Cálculo

El **Teorema Fundamental del Cálculo** recibe de manera apropiada este nombre porque establece una conexión entre las 2 ramas del cálculo: **El cálculo diferencial** y el **cálculo integral**. Usando la relación inversa entre la integral y la derivada que afirma el teorema, Newton y Leibniz desarrollaron un método sistemático que nos permite calcular con gran facilidad áreas, distancias e integrales definidas, sin tener que evaluarlas como límite de sumas.

## ¿Cómo evaluar integrales definidas?

Sean $f$ una función continua en $[a, b]$ y $F(x)$ una antiderivada de $f(x)$ en $[a, b]$. Entonces

$$
\int_{a}^{b} f(x)dx = [F(x)]_{a}^{b} = F(b) - F(a)
$$

## ¿Cómo construir antiderivadas?

Si $f$ es continua en $[a, b]$, entonces la función

$$
F(x) := \int_{a}^{x} f(t)dt
$$

es continua en $[a, b]$ y derivable en (a, b) y su derivada es

$$
F'(x) = \frac{d}{dx} \int_{a}^{x} f(t)dt = f(x)
$$

> **Nota:** Si a la definición anterior del TFC le sumamos la regla de la cadena, obtenemos de manera más general lo siguiente:
> 
> Si se tiene $G(x) = \int_{a(x)}^{b(x)} f(t)dt$
> 
> Entonces $G'(x) = f(b(x))*b'(x) - f(a(x))*a'(x)$

## La derivación y la integración como procesos inversos

**TFC1:** Si usted inicia con $f(x)$ continua y, luego, forma la integral $\int_{a}^{x} f(t)dt$, puede recuperar la función original derivando:

$$
f(x) \to_{\int} \int_{a}^{x} f(t)dt \to_{dx} \frac{d}{dx} \int_{a}^{x} f(t)dt = f(x)
$$

**TFC2:** Si usted deriva primero y, luego, integra, también puede recuperar $f(x)$ [*Excepto, en una constante $f(a)$*]:

$$
f(x) \to_{dx} f'(x) \to_{\int} \int_{a}^{x} f'(t)dt = f(x) - f(a)
$$

# Teorema del cambio neto

> La integral de una razón de cambio es el cambio neto (o total):
> 
> $\int_{a}^{b}{Q'(x)}dx = Q(b) - Q(a)$

* Si un objeto se mueve a lo largo de una línea recta con función posición $y(t)$, su velocidad es $v(t) = y'(t)$. De modo que **el desplazamiento** de la particula desde $t_1$ hasta $t_2$ es:

$$
\int_{t_1}^{t_2}{v(t)}dt = y(t_2) - y(t_1)
$$

* Si se desea conocer **la rapidez** simplemente habría que integrar el valor absoluto de la velocidad:

$$
\int_{t_1}^{t_2}{|v(t)|}dt
$$

* Si un objeto, a lo largo de su movimiento presenta variaciones en su velocidad; puede significar que está presentando una aceleración, lo cual se mide como el cambio de la velocidad por el tiempo, osea $v'(t) = a(t)$; por lo que si se integra la aceleración se obtiene el cambio neto en la velocidad:

$$
\int_{t_1}^{t_2}{a(t)}dt = v(t_2) - v(t_1)
$$

* Si $Q(t) = V'(t)$ es el **caudal** (de entrada o de salida) de un tanque con un fluido en el instante $t$. Por tanto la variación en el volumen entre el tiempo $t_1$ y $t_2$ es:

$$
\int_{t_1}^{t_2}{Q(t)}dt = V(t_2) - V(t_1)
$$

* Si $C(x)$ es el costo de producir $x$ unidades de un artículo, **el costo marginal** es la derivada $C'(x)$. De está manera, el incremento del costo de producción al pasar de $x_1$ a $x_2$ unidades es:

$$
\int_{x_1}^{x_2}{C'(x)}dx = C(x_2) - C(x_1)
$$

* Si $m(x)$ es la masa de una varilla, medida desde un extremo hasta un punto $x$, **la densidad lineal** es $\rho(x) = m'(x)$, osea el cambio de la masa con respecto a la longitud de la varilla. Ahora, si se quiere obtener la masa de la varilla entre los puntos $x_1$ y $x_2$ se realiza la siguiente integral:

$$
\int_{x_1}^{x_2}{\rho(x)}dx = m(x_2) - m(x_1)
$$

# Regla de Sustitución

La Regla de Sustitución es el proceso inverso a **la derivada de la cadena**.

$$
\frac{dF(G(x))}{dx} = f(G(x))*g(x)
$$

$$
\int{f(G(x))*g(x)}dx = F(G(x)) + C
$$

## El método de sustitución en integrales indefinidas

Para evaluar $\int{f(G(x))*g(x)}dx$

1. Sustituya $u = G(x)$ y $du = g(x)dx$, para reescribir la integral de la siguiente forma: $\int{f(u)}du$

2. Integra con respecto a $u$: $\int{f(u)}du = F(u) + C$

3. Reemplace $u$ por $G(x)$: $F(u) + C = F(G(x)) + C$

## El método de sustitución en integrales definidas

**Método 1**: Evalúa primero la integral indefinida y despues de volver en la sustitución, aplique el teorema de evaluación.

**Método 2**: Cambie los límites de integración cuando se cambie la variable:

$$
\int_{a}^{b}{f(G(x))*g(x)}dx = \int_{G(a)}^{G(b)}{f(u)}du
$$

# Técnica de Integración por Partes

La Técnica de Integración por Partes es el proceso inverso a **la derivada del producto**.

$$
\frac{dF(x)*G(x)}{dx} = F(x)*g(x) + f(x)*G(x)
$$

$$
\int{\frac{dF(x)*G(x)}{dx}}dx = \int{F(x)*g(x) + f(x)*G(x)}dx
$$

$$
F(x)*G(x) = \int{F(x)*g(x)}dx + \int{f(x)*G(x)}dx
$$

$$
\int{F(x)*g(x)}dx = F(x)*G(x) - \int{f(x)*G(x)}dx
$$

# Sustitución Trigonométrica

## Caso 1

* Expresión

$$
\sqrt{a^2 - x^2}
$$

* Sustitución

$$
x = a*sin(\theta)
$$

$$
-\frac{\pi}{2} \leq \theta \leq \frac{\pi}{2}
$$

* Diferencial

$$
dx = a*cos(\theta)d\theta
$$

* Identidad

$$
1 - sin^2{\theta} = cos^2{\theta}
$$

## Caso 2

* Expresión

$$
\sqrt{a^2 + x^2}
$$

* Sustitución

$$
x = a*tan(\theta)
$$

$$
-\frac{\pi}{2} \leq \theta \leq \frac{\pi}{2}
$$

* Diferencial

$$
dx = a*sec^2{\theta}d\theta
$$

* Identidad

$$
1 + tan^2{\theta} = sec^2{\theta}
$$

## Caso 3

* Expresión

$$
\sqrt{x^2 - a^2}
$$

* Sustitución

$$
x = a*sec(\theta)
$$

$$
0 \leq \theta < \frac{\pi}{2} \cup \pi \leq \theta < \frac{3*\pi}{2}
$$

* Diferencial

$$
dx = a*tan(\theta)*sec(\theta)d\theta
$$

* Identidad

$$
sec^2{\theta} - 1 = tan^2{\theta}
$$

# Integración por fracciones parciales

> **Nota**: Este método se puede aplicar si $f(x) = \frac{P(x)}{Q(x)}$ es una **fracción propia** (el grado del numerador P es menor que el grado del denominador Q). Si la fracción es impropia, se debe realizar el paso preliminar de dividir $P$ por $Q$.

## Método de fracciones parciales

Para evaluar $\int{\frac{P(x)}{Q(x)}}dx$

1. Factorice $Q(x)$ tanto como sea posible en factores lineales y/o factores cuadráticos irreducibles.

2. Descomponga la fracción propia como una suma de *fracciones parciales* de la forma:

$$
\frac{A}{ax+b}
$$

$$
\frac{Ax + B}{ax^2 + bx + c}
$$

3. Halle las constantes A, B,... usando el hecho de que la suma de estas fracciones tiene que ser igual a $\frac{P(x)}{Q(x)}$

4. Integre de acuerdo a cada caso.

### Caso 1: El denominador $Q(x)$ es producto de factores lineales distintos

$$
\frac{3x^2 + 7x - 2}{x^3 - x}
$$

$$
\frac{A}{x} + \frac{B}{x-1} + \frac{C}{x+1}
$$

$$
A = 2 \ B = 4 \ C = -3
$$

## Caso 2: $Q(x)$ es producto de factores lineales, algunos de los cuales se repiten.

$$
\frac{4x^2 + 2x + 3}{(4-x)*(x+1)^2}
$$

$$
\frac{A}{x-4} + \frac{B}{x+1} + \frac{C}{(x+1)^2}
$$

$$
A = 3 \ B = 1 \ C = -1
$$

> **Nota**
> 
> * Un factor cuadrático $ax^2 + bx + c$ se dice que es irreducible si $b^2 - 4ac < 0$. (Es decir, si su discriminante es negativo)
> 
> * Todo polinomio se factoriza como producto de factores lineales y cuadráticos irreducibles.
> 
> * En algunos casos es útil saber que:
> 
> $\int{\frac{1}{x^2 + a^2}}dx = \frac{1}{a}*tan^{-1}\frac{x}{a} + C$

## Caso 3: $Q(x)$ contiene factores cuadráticos irreducibles, de los cuales ninguno se repite.

$$
\frac{x^3 - x + 6}{x^3 + 4x}
$$

$$
\frac{x*(x^2 + 4) - 5x + 6}{x*(x^2 + 4)} = \frac{x*(x^2 + 4)}{x*(x^2 + 4)} + \frac{-5x + 6}{x*(x^2 + 4)}
$$

$$
1 + \frac{-5x + 6}{x*(x^2 + 4)}
$$

$$
1 + \frac{A}{x} + \frac{Bx + C}{x^2 + 4}
$$

$$
A = \frac{3}{2} \ B = -\frac{3}{2} \ C = -5
$$

## Caso 4: $Q(x)$ contiene factores cuadráticos irreducibles repetidos.

$$
\frac{-x^3 + 2x^2 - x + 1}{x*(x^2 + 1)^2}
$$

$$
\frac{A}{x} + \frac{Bx + C}{x^2 + 1} + \frac{Dx + E}{(x^2 + 1)^2}
$$

$$
A = 1 \ B = -1 \ C = -1 \ D = 1 \ E = 0
$$

# Integrales impropias

En el caso de que el intervalo de integración sea infinito o en el caso que $f(x)$ tenga una discontinuidad infinita en $(a, b)$, se denomina una **integral impropia**.

## Intervalos infinitos

Decimos que las **integrales impropias**

$$
\int_{a}^{\infty} f(x)dx = \lim_{t \to \infty} \int_{a}^{t} f(x)dx
$$

$$
\int_{-\infty}^{b} f(x)dx = \lim_{t \to -\infty} \int_{t}^{b} f(x)dx
$$

son **convergentes**, si los límites existen y son finitos. En caso contrario, decimos que son **divergentes**.

Además, decimos que

$$
\int_{-\infty}^{\infty} f(x)dx = \int_{-\infty}^{a} f(x)dx + \int_{a}^{\infty} f(x)dx
$$

es **convergente**, si ambas integrales convergen. En caso contrario, decimos que es **divergente**.

> **Integrales p**: ¿Para qué valores de $p$ la integral $\int_{1}^{\infty} \frac{dx}{x^{p}}$ es convergente?
> 
> $\int_{1}^{\infty} \frac{dx}{x^{p}}$
> 
> **Converge** a $\frac{1}{p-1}$, si $p > 1$
> 
> **Diverge** si $p \leq 1$

## Integrandos con discontinuidad infinita

Si $f$ es continua en $[a,b)$ y es discontinua en $x=b$, definimos

$$
\int_{a}^{b} f(x)dx = \lim_{t \to b^{-}} \int_{a}^{t} f(x)dx
$$

Similarmente, si $f$ es continua en $(a,b]$ y es discontinua en $x=a$, definimos

$$
\int_{a}^{b} f(x)dx = \lim_{t \to a^{+}} \int_{t}^{b} f(x)dx
$$

En ambos casos, decimos que la integral impropia **converge** si existe el límite y que **diverge** en caso contrario.

Si la discontinuidad infinita ocurre en $c$, con $a < c < b$ y tanto $\int_{a}^{c} f(x)dx$ como $\int_{c}^{b} f(x)dx$ son convergentes, se define:

$$
\int_{a}^{b} f(x)dx = \int_{a}^{c} f(x)dx + \int_{c}^{b} f(x)dx
$$

> **Nota**: En adelante, siempre que se encuentre el símbolo $\int_{a}^{b} f(x)dx$ se debe verificar si la función es continua o no en $[a, b]$ para decidir si hay que evaluar una integral definida ordinaria ó una integral impropia con una discontinuidad infinita en $[a, b]$.

# Pruebas de comparación para integrales impropias

Algunas veces no es posible calcular el valor exacto de una integral impropia. Sin embargo, es posible determinar si converge o no al compararla con otra integral impropia conocida ó más fácil de calcular.

Supongamos que $f$ y $g$ son continuas con $0 \leq g(x) \leq f(x)$, para todo $x \geq a$.

* Si $\int_{a}^{\infty} f(x)dx$ converge, entonces $\int_{a}^{\infty} g(x)dx$ también converge.

* Si $\int_{a}^{\infty} g(x)dx$ diverge, entonces $\int_{a}^{\infty} f(x)dx$ también diverge.

