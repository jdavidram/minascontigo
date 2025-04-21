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

## Propiedades

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
