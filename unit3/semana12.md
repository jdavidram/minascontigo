# Series

Sumando los términos de una sucesión $\{ a_{n} \}$ obtenemos una expresión de la forma

$$
a_1 + a_2 + a_3 + ... + a_{n} + ...
$$

la cual se denomina **serie** y se representa por

$$
\sum_{n = 1}^{\infty} a_{n}
$$

Consideremos las sumas parciales

$$
S_1 = a_1
\\
S_2 = a_1 + a_2
\\
S_3 = a_1 + a_2 + a_3
\\
S_{n} = a_1 + a_2 + a_3 + ... + a_{n} = \sum_{i=1}^{n} a_{i}
$$

las cuales forman en si una nueva sucesión $\{ S_{n} \}_{n=1}^{\infty}$ que puede ser o no convergente.

Si $\{ S_{n} \}$ converge a un límite $S \in \mathbb{R}$, decimos que la serie **converge** y su **suma** es S. En este caso, escribimos

$$
\sum_{n=1}^{\infty} a_{n} = \lim_{n \to \infty} \sum_{i=1}^{n} a_{i} = \lim_{n \to \infty} S_{n} = S \in \mathbb{R}
$$

Si la sucesión de sumas parciales o converge, decimos que la serie **diverge**.

## Álgebra de series

Si $\sum a_{n}$ y $\sum b_{n}$ son convergentes, entonces también lo son $\sum c*a_{n}$ y $\sum (a_{n} \pm b_{n})$. En este caso

$$
\sum c*a_{n} = c*\sum a_{n}
\\
\sum (a_{n} \pm b_{n}) = \sum a_{n} \pm \sum b_{n}
$$

# Tipos de series

## Serie geométrica

Dados $a \neq 0$ y $r \in \mathbb{R}$:

$$
a + ar + ar^2 + ar^3 + ... + ar^{n-1} + ... = \sum_{n=1}^{\infty} ar^{n-1}
$$

* **Converge** a $\frac{a}{1-r}$ si $|r| < 1$

* **Diverge** si $|r| \geq 1$

## Serie telescópica

Sea una serie como la siguiente

$$
\sum_{n=1}^{\infty} a_{n} - a_{n+1}
$$

notese que al realizar las sumas parciales de la seria obtenemos

$$
S_{n} = (a_1 - a_2) + (a_2 - a_3) + (a_3 - a_4) + ... + (a_{n} - a_{n+1})
$$

vea que hay varios terminos que se van cancelando a lo largo de la serie, dejando unicamente el primero $a_1$ y el último, el cual al evaluarlo cuando $n \to \infty$ quedaría de la siguiente manera

$$
\sum_{n=1}^{\infty} a_{n} - a_{n+1} = a_1 - \lim_{n \to \infty} a_{n+1}
$$

## Series P

La serie $\sum_{n=1}^{\infty} \frac{1}{n^{p}}$

* **Converge:**, si $p > 1$
* **Diverge:**, si $p \leq 1$

> Notese que cuando $p = 1$, la **serie p** se convierte en una **serie armonica**.
