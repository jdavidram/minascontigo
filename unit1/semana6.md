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
