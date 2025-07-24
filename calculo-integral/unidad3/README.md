<table border=1>
  <thead>
    <th>
      <img src="https://minas.medellin.unal.edu.co/images/Programa-Minas-Contigo/Logo-Minas-Contigo.png" width="320px" height="270px" />
    </th>
    <th>
      <h1>Sucesiones y series infinitas</h1>
    </th>
  </thead>
</table>

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

# Series de potencias

Una **serie de potencias** es una serie de la forma

$$
\sum_{n=0}^{\infty} c_{n}*x^{n} = c_{0} + c_{1}x + c_{2}x^{2} + ...
$$

Donde $x$ es una variable y los $c_{n}$ son constantes llamados **coeficientes** de la serie.

Una serie de potencias puede converger para ciertos valores de $x$ y diverger para otros. La suma de una serie de potencias, cuando converge, es una función

$$
f(x) = c_{0} + c_{1}x + c_{2}x^{2} + ...
$$

Cuyo dominio es el conjunto de todas las $x$ para las cuales la serie converge.

Por ejemplo, con $c_{n} = 1$ para todo $n$, nos queda la **serie geométrica**

$$
\sum_{n=0}^{\infty} x^{n} = 1 + x + x^{2} + ...
$$

La cual vimos que converge si $|x| < 1$ y diverge si $|x| \geq 1$. Ademas,

> **Serie geométrica**
> 
> $f(x) = \frac{1}{1-x} = \sum_{n=0}^{\infty} x^{n}$
> 
> $|x| < 1$

De forma más general, una serie de la forma

$$
\sum_{n=0}^{\infty} c_{n}(x-a)^{n} = c_{0} + c_{1}(x-a) + c_{2}(x-a)^{2} + ...
$$

Se denomina **serie de potencias centrada en a**.

## Radio e intervalos de convergencia

Para una serie de potencias dada $\sum_{n=0}^{\infty} c_{n}(x-a)^{n}$ hay solo 3 posibilidades:

* La serie solo converge cuando $x=a$, osea $R=0$
* La serie converge para todo $x$, osea $R=\infty$
* Existe un número positivo R tal que la serie
  * Converge, si $|x-a| < R$
  * Diverge, si $|x-a| > R$

A este $R$ se le llama **radio de convergencia** de la serie de potencias.

El **intervalo de convergencia** de una serie de potencias consta de todos los valores de $x$ para los cuales la serie converge.

* Cuando $R=0$, definimos el intervalo como $I=\{ a \}$
* Cuando $R=\infty$, el intervalo es $I = (-\infty, \infty) = \mathbb{R}$
* Cuando $R>0$, se deben analizar los extremos $x = a \pm R$ del intervalo abierto por separado. Luego, hay 4 posibilidades:
  * $(a-R, a+R)$
  * $[a-R, a+R]$
  * $[a-R, a+R)$
  * $(a-R, a+R]$

De los ejemplos anteriores podemos observar:

> $\sum x^{n}$
> 
> Centrada en $a=0$
> 
> Radio $R=1$
> 
> Intervalo = $(-1, 1)$

> $\sum (n+1)!(x-2)^{n}$
> 
> Centrada en $a=2$
> 
> Radio $R=0$
> 
> Intervalo = $\{ 2 \}$

> $\sum (-1)^{n} \frac{x^{n}}{\sqrt[3] x}$
> 
> Centrada en $a=0$
> 
> Radio $R=1$
> 
> Intervalo = $(-1, 1]$

> $\sum \frac{x^{n}}{n!}$
> 
> Centrada en $a=0$
> 
> Radio $R=\infty$
> 
> Intervalo = $(-\infty, \infty)$

## Representación de funciones como series de potencias

Decimos que la función $f(x) = \frac{1}{1-x}$, $|x| < 1$, tiene la representación en series de potencias

$$
\frac{1}{1-x} = \sum_{n=0}^{\infty} x^{n}
$$

en el intervalo $(-1, 1)$.

<!-- EJEMPLOS DE REPRESENTACIÓN DE OTRAS FUNCIONES COMO SERIES DE POTENCIAS (1/1+X^2) -->

## Derivación e integración de series de potencias

Como la suma de una serie de potencias es una función, entonces nos gustaría poder diferenciar e integrar series de potencias. El siguiente teorema nos dice que podemos diferenciar e integrar cada uno de los términos de la serie, justo como se haría con un polinomio, allí donde ella converge. Esto se denomina **derivación e integración término a término**.

**Teorema:** Si la serie de potencias $\sum c_{n}(x-a)^{n}$ tiene radio de convergencia R, la función $f$ definida por:

$$
f(x) = c_{0} + c_{1}(x-a) + c_{2}(x-a)^{2} + ... = \sum_{n=0}^{\infty} c_{n}(x-a)^{n}
$$

es diferenciable sobre el intervalo $(a-R, a+R)$, y

$$
f'(x) = \frac{d}{dx}[\sum_{n=0}^{\infty} c_{n}(x-a)^{n}] = \sum_{n=0}^{\infty} \frac{d}{dx}[c_{n}(x-a)^{n}] = \sum_{n=1}^{\infty} n*c_{n}(x-a)^{n-1}
$$

$$
\int f(x)dx = \int [\sum_{n=0}^{\infty} c_{n}(x-a)^{n}] dx = \sum_{n=0}^{\infty} \int c_{n}(x-a)^{n} dx = \sum_{n=0}^{\infty} \frac{c_{n}}{n+1} (x-a)^{n+1} +C
$$

En ambos casos, el radio de convergencia sigue siendo R.

> **Nota**
> 
> * Observar que al derivar la serie se pierde el primer término (por ser una constante), esto no pasa siempre.
> 
> * El invervalo de convergencia si puede cambiar en los extremos. Luego, siempre debemos analizarlos por aparte.

## Series de Taylor y Maclaurin

El objetivo de esta clase es tratar de responder las siguientes preguntas:

* ¿Qué funciones se pueden representar como series de potencias?
* Si una función se puede representar en series de potencias. ¿Cómo se puede hallar dicha representación?

Respondamos la segunda pregunta. Supongamos que $f(x)$ se representa mediante la serie de potencias

$$
f(x) = c_{0} + c_{1}(x-a) + c_{2}(x-a)^{2} + ...
$$

con $|x-a| < R$.

Hallemos los **coeficientes** $c_{n}$ en términos de $f$. Primero, observamos que si sustituimos $x=a$ en la función anterior, se obtiene

$$
f(a) = c_{0} \to f^{(0)}(a) = 0!c_{0}
$$

Por un teorema de la clase anterior podemos derivar término a término en la función. Luego, sustituimos $x=a$:

$$
f'(x) = c_{1} + 2c_{2}(x-a) + 3c_{3}(x-a)^{2} + ... \to f'(a) = c_{1} = 1!c_{1}
$$

Volvemos a derivar término a término y sustituimos $x=a$:

$$
f''(x) = 2c_{2} + 3*2c_{3}(x-a) + ... \to f''(a) = 2c_{2} = 2!c_{2}
$$

Iterando este procedimiento $n$ veces, es fácil ver que se obtiene

$$
f^{(n)}(a) = n!c_{n} \to c_{n} = frac{f^{(n)}(a)}{n!}
$$

Esto prueba el siguiente resultado.

### Teorema de los coeficientes de Taylor

Si $f$ tiene una representación en forma de serie de potencias centrada en a:

$$
f(x) = \sum_{n=0}^{\infty} c_{n}(x-a)^{n} \\ |x-a| < R
$$

Entonces los coeficientes de la serie están dados por

$$
c_{n} = frac{f^{(n)}(a)}{n!}
$$

Si sustituimos la fórmula para $c_{n}$ de nuevo en la serie, obtenemos **la serie de Taylor de $f$ centrada en $a \in \mathbb{R}$**:

$$
f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!} (x-a)^{n} = f(a) + \frac{f'(a)}{1!}(x-a) + \frac{f''(a)}{2!}(x-a)^{2} + \frac{f^{3}(a)}{3!}(x-a)^{3} + ...
$$

En el caso particular en que $a=0$, se denomina **la serie de Maclaurin de $f$**:

$$
f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(0)}{n!} (x)^{n} = f(0) + \frac{f'(0)}{1!}(x) + \frac{f''(0)}{2!}(x)^{2} + \frac{f^{3}(0)}{3!}(x)^{3} + ...
$$

> **Nota:**
> 
> Hemos probado que si $f$ se puede representar en una serie de potencias, entonces $f$ es igual a su serie de Taylor. Pero existen funciones que tienen derivadas de todos los ordenes, pero **no** son iguales a su serie de Taylor.

Sea

$$
\sum_{n=0}^{\infty} \frac{f^{n}(a)}{n!} = T_{n}(x) + R_{n}(x)
$$

Si se cumple que

$$
\lim\limits_{n \to \infty} R_{n}(x) = 0
$$

Para todo $|x-a| < R$, entonces $f$ es igual a la suma de su serie de Taylor en el intervalo $|x-a| < R$. Es decir,

$$
f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!} (x-a)^{n}
$$

en $|x-a| < R$.

Al tratar de probar que $\lim\limits_{n\to\infty} R_{n}(x) = 0$ para la serie de potencias de una cierta $f$ generalmente se emplea el siguiente resultado:

**Desigualdad de Taylor**: Si

$$
|f^{(n+1)(x)}| \leq M
$$

para $|x-a| < R$, entonces el residuos $R_{n}(x)$ satisface la desigualdad

$$
|R_{n}(x)| \leq \frac{M}{(n+1)!} |x-a|^{n+1}
$$

para $|x-a| < R$.

> **Nota:**
> 
> Al aplicar estos teoremas suele ser útil el siguiente límite:
> 
> $\lim\limits_{n\to\infty} \frac{|x|^{(n+1)}}{(n+1)!} = 0$
> 
> Para todo número $x \in \mathbb{R}$.

### Series importantes de Maclaurin y sus radios de convergencia

**$R=\infty$**

* $e^{x} = \sum_{n=0}^{\infty} \frac{x^{n}}{n!}$
* $cos(x) = \sum_{n=0}^{\infty} (-1)^{n} \frac{x^{2n}}{(2n)!}$
* $sin(x) = \sum_{n=0}^{\infty} (-1)^{n} \frac{x^{2n+1}}{(2n+1)!}$

**$R=1$**

* $\frac{1}{1-x} = \sum_{n=0}^{\infty} x^{n}$
* $ln(1+x) = \sum_{n=0}^{\infty} (-1)^{n-1} \frac{x^{n}}{n}$
* $tan^{-1}(x) = \sum_{n=0}^{\infty} (-1)^{n} \frac{x^{2n+1}}{2n+1}$

## Aproximación de funciones por polinomios

Podemos usar un polinomio de Taylor de grado $n$, $T_{n}(x)$, para aproximar una función $f$ la cual se puede representar como una serie de Taylor centrada en a, digamos

$$
f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!} (x-a)^{n}
$$

Para $|x-a| < R$, en donde R es el radio de convergencia de la serie. Puesto que en este caso $f(x) = \lim\limits_{n\to\infty} T_{n}(x)$, entonces decimos que $f(x) \approx T_{n}(x)$. Si queremos saber que tan buena es esta aproximación debemos analizar el tamaño del residuo

$$
|R_{n}(x)| = |f(x) - T_{n}(x)|
$$

Para estimar este valor usamos la desigualdad de Taylor que dice que si $|f^{(n+1)}(x)| \leq M$, entonces

$$
|R_{n}(x)| \leq \frac{M}{(n+1)!} |x-a|^{n+1}
$$

El siguiente ejemplo ilustra el método que se puede seguir para obtener dicha aproximación:

**Ejemplo**

1. Aproxime la función $f(x) = ln(1+2x)$ por medio de un polinomio de Taylor de grado 3 en $a = 1$.
2. Use la desigualdad de Taylor para estimar la precisión de la aproximación $f(x) \approx T_{3}(x)$ cuando $0.5 \leq x \leq 1.5$.

**Solución 1**

$$
f(x) = ln(1+2x) \to f(1) = ln(3)
$$

$$
f'(x) = \frac{2}{1+2x} \to f'(1) = \frac{2}{3}
$$

$$
f''(x) = -\frac{4}{(1+2x)^{2}} \to f''(1) = -\frac{4}{9}
$$

$$
f^{(3)}(x) = \frac{16}{(1+2x)^{3}} \to f^{(3)}(1) = \frac{16}{27}
$$

Entonces la aproximación deseada es

$$
ln(1+2x) \approx T_{3}(x) = f(1) + \frac{f'(1)}{1!}(x-1) + \frac{f''(1)}{2!}(x-1)^{2} + \frac{f^{(3)}(1)}{3!}(x-1)^{3}
$$

$$
T_{3}(x) = ln(3) + \frac{2}{3}(x-1) - \frac{4}{18}(x-1)^{2} + \frac{8}{81}(x-1)^{3}
$$

**Solución 2**

Por la desigualdad de Taylor con $n=3$ y $a=1$:

$$
|R_{3}(x)| \leq \frac{M}{4!} |x-1|^{4}
$$

Donde $|f^{(4)}(x)| \leq M$

En este caso, $f^{(4)}(x) = -\frac{96}{(1+2x)^{4}}$. Puesto $x \geq 0.5$, tenemos que $(1 + 2x)^{4} \geq (1 + 2(0.5))^{4} = 16$, de donde

$$
|f^{(4)}(x)| = \frac{96}{(1+2x)^{4}} \leq \frac{96}{16} = 6
$$

Así, podemos tomar $M=6$. Además, como $0.5 \leq x \leq 1.5$, entonces $-0.5 \leq x-1 \leq 0.5$; es decir, $|x-1| \leq 0.5$. Se sigue que

$$
|R_{3}(x)| \leq \frac{6}{24} (0.5)^{4} = \frac{1}{64} = 0.015625 \approx 0.016
$$

La aproximación en *Solución 1*, para $0.5 \leq x \leq 1.5$, tiene una precisión de una cifra decimal.

