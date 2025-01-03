# Áreas entre curvas

Ahora vamos a usar la integral definida para calcular áreas limitadas por las gráficas de 2 funciones. Sean $f$ y $g$ 2 funciones continuas en el intervalo $[a, b]$ con la condición $f(x) \geq g(x)$ en $[a, b]$:

![](https://calculo21.com/wp-content/uploads/2019/12/6.1_2.png)

El área del rectangulo diferencial es:

**Altura**

$$
f(x_i) - g(x_i)
$$

$$
x_i \in [x_{i-1}, x_i]
$$

**Grosor**

$$
\Delta x = \frac{b - a}{n}
$$

Por tanto:

$$
A = lim_{n \to \infty} \sum_{i = 1}^{n} f(x_i) - g(x_i)*\Delta x
$$

El **área A** de la región limitada por las curvas $y = f(x)$ y $y = g(x)$, y las rectas $x = a$, $x = b$, donde $f$, $g$ son funciones continuas y $f(x) \geq g(x)$, para todo $x \in [a, b]$, está dada por:

$$
A = \int_{a}^{b}{[f(x) - g(x)]}dx
$$
