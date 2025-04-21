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
