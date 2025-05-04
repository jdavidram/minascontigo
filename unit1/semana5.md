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
