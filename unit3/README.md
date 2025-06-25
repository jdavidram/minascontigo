# Sucesiones

Intuitivamente, una **sucesión** es una lista ordenada de numeros donde $a_{n}$ se denomina el *n-ésimo* término de la sucesión. Por ejemplo:

$$
\{ a_{1}, a_{2}, a_{3}, a_{4}, ..., a_{n} \}
$$

Como trabajaremos exclusivamente con sucesiones infinitas, cada término $a_{n}$ tendrá un sucesor $a_{n+1}$.

> La **sucesión** $\{ a_{1}, a_{2}, a_{3}, a_{4}, ..., a_{n}, ... \}$ también se denota por $\{ a_{n} \}_{n = 0}^{\infty}$ o $\{ a_{n} \}$ o $a_{n}$; $n \ge 0$.

Una sucesión $\{ a_{n} \}$ tiene **límite** L, y escribimos

$$
\lim_{n \to \infty}{a_{n}} = L
\\
a_{n} \to_{n \to \infty} L
$$

Si podemos hacer que los términos $a_{n}$ se aproximen a *L* tanto como queramos al tomar *n* muy grande. Si $\lim_{n \to \infty}{a_{n}}$ existe, se dice que la sucesión **converge** (o es **convergente**). De lo contrario, se dice que **diverge** (o es **divergente**).

Sea $f: [1, \infty) \to \mathbb{R}$ una función tal que $f(n) = a_{n}$, para todo $n \ge 1$.

Si $\lim_{x \to \infty}{f(x)} = L$, entonces $\lim_{n \to \infty}{a_{n}} = L$.

Gráficamente,

![Grafica de f(x)]()

> [!NOTE]
>
> Sea $p \in \mathbb{R}$ fijo
>
> $$\lim_{n \to \infty} \frac{1}{n^{p}} = \lim_{x \to \infty} \frac{1}{x^{p}} = L$$
>
> * Si $p > 0 \Rightarrow L = 0$ y $\{ \frac{1}{n^{p}} \}$ converge a 0
>
> * Si $p < 0 \Rightarrow L = \infty$ y $\{ \frac{1}{n^{p}} \}$ diverge

## Leyes de los límites para sucesiones

Si $\{ a_{n} \}$ y $\{ b_{n} \}$ son sucesiones convergentes y c una constante, entonces:

* $\lim_{n \to \infty} (a_{n} \pm b_{n}) = \lim_{n \to \infty} a_{n} \pm \lim_{n \to \infty} b_{n}$

* $\lim_{n \to \infty} a_{n}*b_{n} = \lim_{n \to \infty} a_{n}*\lim_{n \to \infty} b_{n}$

* $\lim_{n \to \infty} ca_{n} = c*\lim_{n \to \infty} a_{n}$

* $\lim_{n \to \infty} \frac{a_{n}}{b_{n}} = \frac{\lim_{n \to \infty} a_{n}}{\lim_{n \to \infty} b_{n}}, \ si \ \lim_{n \to \infty} b_{n} \neq 0$

## Teorema de estricción para sucesiones

Si

$$
a_{n} \leq b_{n} \leq c_{n}, \ \forall n \geq n_{0}
$$

y

$$
\lim_{n \to \infty} a_{n} = L = \lim_{n \to \infty} c_{n}
$$

entonces

$$
\lim_{n \to \infty} b_{n} = L
$$

Usando el teorema de estricción se justifica el siguiente resultado:

Si $\lim_{n \to \infty} |a_{n}| = 0$, entonces $\lim_{n \to \infty} a_{n} = 0$.

Si $\lim_{n \to \infty} a_{n} = L$ y $f$ es una función continua en $a = L$, entonces

$$
\lim_{n \to \infty} f(a_{n}) = f(\lim_{n \to \infty} a_{n}) = f(L)
$$

> [!TIP]
>
> La sucesión $\{ r^{n} \}$ es convergente si $-1 < r \leq 1$ y divergente para todos los otros valores de r. De hecho, teniendo en cuenta lo siguiente:
>
> $$\lim_{n \to \infty} r^{n} = L$$
>
> * Si $|r| < 1$, entonces $L = 0$
>
> * Si $r = 1$, entonces $L = 1$

# Sucesiones monotonas

Decimos que una sucesión $\{ a_{n} \}$ es

* **Creciente** si $a_{n} < a_{n+1}, \ \forall n \geq 1$

* **Decreciente** Si $a_{n} > a_{n+1}, \ \forall n \geq 1$

* **Monótona** Si es siempre creciente o siempre decreciente

**Nota** También puede ocurrir que una sucesión sea monótona solo a partir de cierto $n$: $\{ 1, \frac{1}{2}, \frac{1}{3}, 2, 3, 4, 5, ... \}$ crece a partir de $n = 4$.

Una forma recomendable para determinar si una sucesión es monótona es usar el siguiente método: Simplificar $\frac{a_{n}}{a_{n+1}}$ y luego

* Es **creciente** si $\frac{a_{n}}{a_{n+1}} < 1 \Rightarrow a_{n} < a_{n+1}$

* Es **decreciente** si $\frac{a_{n}}{a_{n+1}} > 1 \Rightarrow a_{n} > a_{n+1}$

* Es **constante** si $\frac{a_{n}}{a_{n+1}} = 1 \Rightarrow a_{n} = a_{n+1}$

* Es **no concluyente** si $\frac{a_{n}}{a_{n+1}}$ varia entre ser creciente y decreciente

A veces cuando el anterior método no permite concluir, se puede definir una función derivable $f$ tal que $f(n) = a_{n}$. Basta mirar el signo de su primera derivada: Si $f$ crece, $a_{n}$ crece  si $f$ decrece, $a_{n}$ decrece.

# Sucesiones recursivas

Cuando se sabe que una sucesión $\{ a_{n} \}$ recursiva es convergente, se puede calcular su límite $L$ usando la siguiente propiedad:

$$
L = \lim_{n \to \infty} a_{n} = \lim_{n \to \infty} a_{n+1}
$$


