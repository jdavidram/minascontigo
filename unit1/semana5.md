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
