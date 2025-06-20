# Pruebas de divergencia

> **Nota**
>
> Si $\sum a_{n}$ es convergente, entonces $\lim_{n \to \infty} a_{n} = 0$
>
> En general no se cumple el recíproco. Es decir, si $\lim_{n \to \infty} a_{n} = 0$, **NO** puedo concluir que $\sum a_{n}$ sea convergente.

## Prueba de la divergencia

Si

$$
\lim_{n \to \infty} a_{n} \neq 0 \ o \ \nexists
$$

entonces $\sum a_{n}$ diverge.

## Prueba de la integral

Sean $f: [1, \infty) \to \mathbb{R}^{+}$ una función continua, positiva y decreciente y $a_{n} = f(n)$, $\forall n$.

$$
\int_{1}^{\infty} f(x) dx \ converge => \sum_{n=1}^{\infty} a_{n} \ converge
$$

$$
\int_{1}^{\infty} f(x) dx \ diverge => \sum_{n=1}^{\infty} a_{n} \ diverge
$$

## Prueba por comparación

Suponga que $0 < a_{n} \leq b_{n}$, $\forall n$.

* Si $\sum b_{n} \ converge => \sum a_{n} converge$

* Si $\sum a_{n} \ diverge => \sum b_{n} diverge$

## Prueba por comparación en el límite

Sean $a_{n}$, $b_{n}$ positivos.

1. $\lim_{n \to \infty} \frac{a_{n}}{b_{n}} > 0$

$$
\sum_{n=1}^{\infty} b_{n} \ converge \leftrightarrow \sum_{n=1}^{\infty} a_{n} \ converge \\
\sum_{n=1}^{\infty} b_{n} \ diverge \leftrightarrow \sum_{n=1}^{\infty} a_{n} \ diverge
$$

2. $\lim_{n \to \infty} \frac{a_{n}}{b_{n}} = 0$

$$
\sum_{n=1}^{\infty} b_{n} \ converge => \sum_{n=1}^{\infty} a_{n} \ converge
$$

3. $\lim_{n \to \infty} \frac{a_{n}}{b_{n}} = \infty$

$$
\sum_{n=1}^{\infty} b_{n} \ diverge => \sum_{n=1}^{\infty} a_{n} \ diverge
$$

## Prueba de la serie alternante (Criterio de Leibniz)

Si la serie alternante $\sum_{n=1}^{\infty} (-1)^{n+1} * b_{n}$, $b_{n} > 0$, satisface:

1. $b_{n+1} \leq b_{n}$, para toda $n$ (NO creciente)
2. $\lim\limits_{n \to \infty} b_{n} = 0$

Entonces la serie es convergente.

> **Nota:**
> 
> * En la condición *1* sólo se requiere que la sucesión sea NO creciente a partir de un cierto *n*.
> * Si la condición *2* No se cumple, entonces se sigue que $\lim\limits_{n \to \infty} a_{n}$ NO existe. Por **la prueba de la divergencia**, la serie alternante diverge.

### Estimación de la suma de una serie alternante

El error involucrado, usando la *n-ésima* suma parcial $s_{n}$ como aproximación a la suma total $s$ de una serie alternante, es el residuo $R_{n} = s - s_{n}$. El siguiente teorema nos dice que dicho error es menor que el primer termino que se deja de sumar.

**Teorema**

Si $\sum_{n=1}^{\infty} (-1)^{n+1} * b_{n}$ es convergente y $s = \sum_{n=1}^{\infty} (-1)^{n+1} * b_{n}$, entonces:

$$
|R_{n}| = |s - s_{n}| \leq b_{n+1}
$$

**Ejemplo:** Estime la suma de la serie $\sum_{n=1}^{\infty} \frac{(-1)^{n+1}}{n^{4}}$ aproximada a 2 cifras decimales.

Observemos que la serie converge ya que:

$$
\frac{b_{n}}{b_{n+1}} = (\frac{n+1}{n})^{4} > 1
$$

y

$$
\lim\limits_{n \to \infty} b_{n} = \lim\limits_{n \to \infty} \frac{1}{n^{4}} = 0
$$

Ahora, escribimos algunos términos de la serie para tener una idea de cuántos debemos usar en la aproximación.

$$
s = \frac{1}{1^{4}} - \frac{1}{2^{4}} + \frac{1}{3^{4}} - \frac{1}{4^{4}} + \frac{1}{5^{4}} - ...
$$

$$
1 - \frac{1}{16} + \frac{1}{81} - \frac{1}{256} + \frac{1}{3125} - ...
$$

Observar que $b_{4} = \frac{1}{256} < \frac{1}{200} = 0.005$. Entonces por el teorema $|R_{3}| = |s - s_{3}| \leq b_{4}$, es decir, si estimamos $s$ por $s_{3}$ el error no afecta la segunda cifra decimal. Luego, una estimación para *s* aproximada a 2 cifras decimales es $s_{3} \approx 0.9498$

## Prueba de la razón y de la raiz

Sea $\lim\limits_{n \to \infty} |\frac{a_{n+1}}{a_{n}}| = L$ ó $\lim\limits_{n \to \infty} |a_{n}|^{\frac{1}{n}} = L$

* $L < 1 => \sum_{n=1}^{\infty} a_{n}$ es absolutamente convergente

* $L > 1$ ó $L = \infty => \sum_{n=1}^{\infty} a_{n}$ es divergente

* Si $L = 1$, entonces la prueba NO es concluyente.

## Convergencia absoluta

Dada cualquier serie $\sum a_{n}$ se puede considerar la serie

$$
\sum |a_{n}| = |a_{1}| + |a_{2}| + |a_{3}| + ... + |a_{n}| + ...
$$

cuyos términos son los valores absolutos de los términos de la serie original.

> Una serie $\sum a_{n}$ se dice que es
> 
> * **Absolutamente convergente** si la serie de valores absolutos $\sum |a_{n}|$ es convergente.
> * **Condicionalmente convergente** si es convergente, pero NO absolutamente convergente.

> **Nota:** Si $a_{n} > 0$, entonces $\sum a_{n} = \sum |a_{n}|$. Luego, la convergencia absoluta es lo mismo que la convergencia usual en este caso.
