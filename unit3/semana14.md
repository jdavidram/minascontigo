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
