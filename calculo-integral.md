![Minas Contigo](./img//header.png)

> [!NOTE]
>
> Notas opensource de Cálculo Integral

---

# Cálculo integral

## Capítulo 1: Integrales

- [Cálculo integral](#cálculo-integral)
  - [Capítulo 1: Integrales](#capítulo-1-integrales)
  - [Capítulo 2: Aplicaciones de la integración](#capítulo-2-aplicaciones-de-la-integración)
  - [Capítulo 3: Sucesiones y series infinitas](#capítulo-3-sucesiones-y-series-infinitas)
- [Notación Sigma](#notación-sigma)
  - [Propiedades de la sumatoria](#propiedades-de-la-sumatoria)
  - [Algunas fórmulas para sumatorias](#algunas-fórmulas-para-sumatorias)
- [El problema del área](#el-problema-del-área)
- [El problema de la distancia](#el-problema-de-la-distancia)
- [Integral definida](#integral-definida)
  - [Propiedades de la integral definida](#propiedades-de-la-integral-definida)
- [Antiderivada](#antiderivada)
  - [Integral indefinida](#integral-indefinida)
    - [Tabla de integrales fundamentales](#tabla-de-integrales-fundamentales)
- [Movimiento rectilíneo](#movimiento-rectilíneo)
- [Teorema Fundamental del Cálculo](#teorema-fundamental-del-cálculo)
  - [¿Cómo evaluar integrales definidas?](#cómo-evaluar-integrales-definidas)
  - [¿Cómo construir antiderivadas?](#cómo-construir-antiderivadas)
  - [La derivación y la integración como procesos inversos](#la-derivación-y-la-integración-como-procesos-inversos)
- [Teorema del cambio neto](#teorema-del-cambio-neto)
- [Regla de Sustitución](#regla-de-sustitución)
  - [El método de sustitución en integrales indefinidas](#el-método-de-sustitución-en-integrales-indefinidas)
  - [El método de sustitución en integrales definidas](#el-método-de-sustitución-en-integrales-definidas)
- [Técnica de Integración por Partes](#técnica-de-integración-por-partes)
- [Sustitución Trigonométrica](#sustitución-trigonométrica)
  - [Caso 1](#caso-1)
  - [Caso 2](#caso-2)
  - [Caso 3](#caso-3)
- [Integración por fracciones parciales](#integración-por-fracciones-parciales)
  - [Método de fracciones parciales](#método-de-fracciones-parciales)
    - [Caso 1: El denominador $Q(x)$ es producto de factores lineales distintos](#caso-1-el-denominador-qx-es-producto-de-factores-lineales-distintos)
  - [Caso 2: $Q(x)$ es producto de factores lineales, algunos de los cuales se repiten.](#caso-2-qx-es-producto-de-factores-lineales-algunos-de-los-cuales-se-repiten)
  - [Caso 3: $Q(x)$ contiene factores cuadráticos irreducibles, de los cuales ninguno se repite.](#caso-3-qx-contiene-factores-cuadráticos-irreducibles-de-los-cuales-ninguno-se-repite)
  - [Caso 4: $Q(x)$ contiene factores cuadráticos irreducibles repetidos.](#caso-4-qx-contiene-factores-cuadráticos-irreducibles-repetidos)
- [Integrales impropias](#integrales-impropias)
  - [Intervalos infinitos](#intervalos-infinitos)
  - [Integrandos con discontinuidad infinita](#integrandos-con-discontinuidad-infinita)
- [Pruebas de comparación para integrales impropias](#pruebas-de-comparación-para-integrales-impropias)
- [Áreas entre curvas](#áreas-entre-curvas)
- [Volúmenes](#volúmenes)
  - [Volúmenes mediante discos](#volúmenes-mediante-discos)
  - [Volúmenes mediante arandelas](#volúmenes-mediante-arandelas)
  - [Volúmenes mediante cascarones cilíndricos](#volúmenes-mediante-cascarones-cilíndricos)
- [Trabajo](#trabajo)
  - [Ley de Hooke](#ley-de-hooke)
  - [Ascensores](#ascensores)
  - [Vaciado de tanques](#vaciado-de-tanques)
- [Momentos y centros de masa](#momentos-y-centros-de-masa)
- [Curvas definidas por medio de ecuaciones paramétricas](#curvas-definidas-por-medio-de-ecuaciones-paramétricas)
- [Cálculo con curvas paramétricas](#cálculo-con-curvas-paramétricas)
  - [Tangentes](#tangentes)
  - [Área en paramétricas](#área-en-paramétricas)
  - [Longitud de arco](#longitud-de-arco)
- [Coordenadas polares](#coordenadas-polares)
- [Áreas en coordenadas polares](#áreas-en-coordenadas-polares)
- [Longitud de arco en polares](#longitud-de-arco-en-polares)
- [Sucesiones](#sucesiones)
  - [Leyes de los límites para sucesiones](#leyes-de-los-límites-para-sucesiones)
  - [Teorema de estricción para sucesiones](#teorema-de-estricción-para-sucesiones)
- [Sucesiones monotonas](#sucesiones-monotonas)
- [Sucesiones recursivas](#sucesiones-recursivas)
- [Series](#series)
  - [Álgebra de series](#álgebra-de-series)
- [Tipos de series](#tipos-de-series)
  - [Serie geométrica](#serie-geométrica)
  - [Serie telescópica](#serie-telescópica)
  - [Series P](#series-p)
- [Pruebas de divergencia](#pruebas-de-divergencia)
  - [Prueba de la divergencia](#prueba-de-la-divergencia)
  - [Prueba de la integral](#prueba-de-la-integral)
  - [Prueba por comparación](#prueba-por-comparación)
  - [Prueba por comparación en el límite](#prueba-por-comparación-en-el-límite)
  - [Prueba de la serie alternante (Criterio de Leibniz)](#prueba-de-la-serie-alternante-criterio-de-leibniz)
    - [Estimación de la suma de una serie alternante](#estimación-de-la-suma-de-una-serie-alternante)
  - [Prueba de la razón y de la raiz](#prueba-de-la-razón-y-de-la-raiz)
  - [Convergencia absoluta](#convergencia-absoluta)
- [Series de potencias](#series-de-potencias)
  - [Radio e intervalos de convergencia](#radio-e-intervalos-de-convergencia)
  - [Representación de funciones como series de potencias](#representación-de-funciones-como-series-de-potencias)
  - [Derivación e integración de series de potencias](#derivación-e-integración-de-series-de-potencias)
  - [Series de Taylor y Maclaurin](#series-de-taylor-y-maclaurin)
    - [Teorema de los coeficientes de Taylor](#teorema-de-los-coeficientes-de-taylor)
    - [Series importantes de Maclaurin y sus radios de convergencia](#series-importantes-de-maclaurin-y-sus-radios-de-convergencia)
  - [Aproximación de funciones por polinomios](#aproximación-de-funciones-por-polinomios)

## Capítulo 2: Aplicaciones de la integración

* [Áreas entre curvas](#áreas-entre-curvas)

* [Volúmenes](#volúmenes)

    * [Volúmenes mediante discos](#volúmenes-mediante-discos)

    * [Volúmenes mediante arandelas](#volúmenes-mediante-arandelas)

    * [Volúmenes mediante cascarones cilíndricos](#volúmenes-mediante-cascarones-cilíndricos)

* [Trabajo](#trabajo)

    * [Ley de Hooke](#ley-de-hooke)

    * [Ascensores](#ascensores)

    * [Vaciado de tanques](#vaciado-de-tanques)

* [Momentos y centros de masa](#momentos-y-centros-de-masa)

* [Curvas definidas por medio de ecuaciones paramétricas](#curvas-definidas-por-medio-de-ecuaciones-paramétricas)

* [Cálculo con curvas paramétricas](#cálculo-con-curvas-paramétricas)

    * [Tangentes](#tangentes)

    * [Área en paramétricas](#área-en-paramétricas)

    * [Longitud de arco](#longitud-de-arco)

* [Coordenadas polares](#coordenadas-polares)

* [Áreas en coordenadas polares](#áreas-en-coordenadas-polares)

* [Longitud de arco en polares](#longitud-de-arco-en-polares)

## Capítulo 3: Sucesiones y series infinitas

* [Sucesiones](#sucesiones)

    * [Leyes de los límites para sucesiones](#leyes-de-los-límites-para-sucesiones)

    * [Teorema de estricción para sucesiones](#teorema-de-estricción-para-sucesiones)

* [Sucesiones monotonas](#sucesiones-monotonas)

* [Sucesiones recursivas](#sucesiones-recursivas)

* [Series](#series)

    * [Álgebra de series](#álgebra-de-series)

* [Tipos de series](#tipos-de-series)

    * [Serie geométrica](#serie-geométrica)

    * [Serie telescópica](#serie-telescópica)

    * [Series P](#series-p)

* [Pruebas de divergencia](#pruebas-de-divergencia)

    * [Prueba de la divergencia](#prueba-de-la-divergencia)

    * [Prueba de la integral](#prueba-de-la-integral)

    * [Prueba por comparación](#prueba-por-comparación)

    * [Prueba por comparación en el límite](#prueba-por-comparación-en-el-límite)

    * [Prueba de la serie alternante (Criterio de Leibniz)](#prueba-de-la-serie-alternante-(criterio-de-leibniz))

    * [Prueba de la razón y de la raiz](#prueba-de-la-razón-y-de-la-raiz)

    * [Convergencia absoluta](#convergencia-absoluta)

* [Series de potencias](#series-de-potencias)

    * [Radio e intervalos de convergencia](#radio-e-intervalos-de-convergencia)

    * [Representación de funciones como series de potencias](#representación-de-funciones-como-series-de-potencias)

    * [Derivación e integración de series de potencias](#derivación-e-integración-de-series-de-potencias)

    * [Series de Taylor y Maclaurin](#series-de-taylor-y-maclaurin)

    * [Aproximación de funciones por polinomios](#aproximación-de-funciones-por-polinomios)

---

<table border=1>
  <thead>
    <th>
      <img src="https://minas.medellin.unal.edu.co/images/Programa-Minas-Contigo/Logo-Minas-Contigo.png" width="320px" height="270px" />
    </th>
    <th>
      <h1>Integrales</h1>
    </th>
  </thead>
</table>

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

## Propiedades de la sumatoria

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

# Integral definida

Si *f* es una función continua definida para $x \in [a, b]$. Dividimos el intervalo *[a, b]* en *n* subintervalos de tamaño $\Delta x = \frac{b-a}{n}$ y elegimos los puntos $x_{i}^{*} \in [x_{i-1}, x_{i}]$. Entonces **la integral definida de f, desde a hasta b**, es:

$$
\int_{a}^{b} f(x)dx = \lim_{n \to \infty} \sum_{i=1}^{n} f(x_{i}^{*})*\Delta x
$$

Si el límite existe, decimos que $f$ es **integrable sobre [a, b]**.

* En $\int_{a}^{b} f(x)dx$ la función $f$ es llamada **integrando** y los números $a, b$ son los **límites de integración**.
* La integral definida es un número real y no depende de la variable que usemos.
* No importa que valores toman los puntos de muestra $x_{i}^{*}$: Pueden ser $x_{i-1}$ o $x_i$ o un punto arbitrario en cada subintervalo.
* Si $f \geq 0$ en [a, b], entonces $\int_{a}^{b} f(x)dx$ = **área bajo f**.
* Sólo se pide que $f$ sea continua y puede ser positiva o negativa. Si $f$ toma tanto valores positivos como negativos, entonces la integral se puede interpretar como un **área neta**.

$$
\int_{a}^{b} f(x)dx = (área \ sobre \ el \ eje \ x) - (área \ debajo \ del \ eje \ x)
$$

* A la suma $\sum_{i=1}^{n} f(x_{i}^{*})*\Delta x$ se le denomina **suma de Riemann de f**.

## Propiedades de la integral definida

Sean $f$ y $g$ integrables sobre [a, b] y c $\in \mathbb{R}$.

$$
\int_{a}^{b} c*f(x)dx = c*\int_{a}^{b} f(x)dx
$$

$$
\int_{a}^{b} cdx = c*(b-a)
$$

$$
\int_{a}^{a} f(x)dx = 0
$$

$$
\int_{a}^{b} [f(x) \pm g(x)]dx = \int_{a}^{b} f(x)dx \pm \int_{a}^{b} g(x)dx
$$

$$
\int_{a}^{b} f(x)dx = \int_{a}^{c} f(x)dx + \int_{c}^{b} f(x)dx
$$

$$
\int_{a}^{b} f(x)dx = -\int_{b}^{a} f(x)dx
$$

> **Nota:** $\frac{b-a}{n} = -\frac{a-b}{n} = -\Delta x$

* Si $0 \leq f(x)$ en [a, b], entonces $0 \leq \int_{a}^{b} f(x)dx$.

* Si $g(x) \leq f(x)$ en [a, b], entonces $\int_{a}^{b} g(x)dx \leq \int_{a}^{b} f(x)dx$.

* Si $m \leq f(x) \leq M$ en [a, b], entonces:

$$
m*(b-a) \leq \int_{a}^{b} f(x)dx \leq M*(b-a)
$$

> **Nota:** $M = max_{x \in [a, b]} \ f(x)$ y $m = min_{x \in [a, b]} \ f(x)$.

# Antiderivada

Una función $F$ se dice que es una **antiderivada** (o una **primitiva**) de una función $f$ sobre un intervalo $I$ si:

$$
F'(x) = f(x) \ para \ todo \ x \in I
$$

Si $F$ es una antiderivada de $f$ sobre $I$, entonces la antiderivada más general de $f$ sobre $I$ es $F(x) + C$, donde $C \in \mathbb{R}$ es una constante arbitraria.

## Integral indefinida

> $\int f(x)dx = F(x) + C$ significa que $F'(x) = f(x)$.

### Tabla de integrales fundamentales

$$
\int x^{r}dx = \frac{x^{r+1}}{r+1} +C \ (r \neq -1)
$$

$$
\int k*dx = k*x +C
$$

$$
\int \frac{1}{x}dx = ln|x| +C
$$

$$
\int e^{x}dx = e^{x} +C
$$

$$
\int cos(x)dx = sin(x) +C
$$

$$
\int sin(x)dx = -cos(x) +C
$$

$$
\int sec^{2}(x)dx = tan(x) +C
$$

$$
\int sec(x)*tan(x)dx = sec(x) +C
$$

$$
\int csc^{2}(x)dx = -cot(x) +C
$$

$$
\int csc(x)*cot(x)dx = -csc(x) +C
$$

$$
\int \frac{1}{\sqrt{1 - x^2}}dx = sin^{-1}(x) +C
$$

$$
\int \frac{-1}{\sqrt{1 - x^2}}dx = cos^{-1}(x) +C
$$

$$
\int \frac{1}{1 + x^2}dx = tan^{-1}(x) +C
$$

# Movimiento rectilíneo

La antiderivación es en particular útil al analizar el movimiento de un objeto que se mueve en línea recta. Se sabe del **Cálculo Diferencial** que si $s(t)$ es la función posición, la velocidad es $v(t) = s'(t)$. Esto significa que $s(t)$ es una antiderivada de $v(t)$. De forma análoga, la función aceleración es $a(t) = v'(t)$, de modo que la velocidad es una antiderivada de la aceleración.

# Teorema Fundamental del Cálculo

El **Teorema Fundamental del Cálculo** recibe de manera apropiada este nombre porque establece una conexión entre las 2 ramas del cálculo: **El cálculo diferencial** y el **cálculo integral**. Usando la relación inversa entre la integral y la derivada que afirma el teorema, Newton y Leibniz desarrollaron un método sistemático que nos permite calcular con gran facilidad áreas, distancias e integrales definidas, sin tener que evaluarlas como límite de sumas.

## ¿Cómo evaluar integrales definidas?

Sean $f$ una función continua en $[a, b]$ y $F(x)$ una antiderivada de $f(x)$ en $[a, b]$. Entonces

$$
\int_{a}^{b} f(x)dx = [F(x)]_{a}^{b} = F(b) - F(a)
$$

## ¿Cómo construir antiderivadas?

Si $f$ es continua en $[a, b]$, entonces la función

$$
F(x) := \int_{a}^{x} f(t)dt
$$

es continua en $[a, b]$ y derivable en (a, b) y su derivada es

$$
F'(x) = \frac{d}{dx} \int_{a}^{x} f(t)dt = f(x)
$$

> **Nota:** Si a la definición anterior del TFC le sumamos la regla de la cadena, obtenemos de manera más general lo siguiente:
> 
> Si se tiene $G(x) = \int_{a(x)}^{b(x)} f(t)dt$
> 
> Entonces $G'(x) = f(b(x))*b'(x) - f(a(x))*a'(x)$

## La derivación y la integración como procesos inversos

**TFC1:** Si usted inicia con $f(x)$ continua y, luego, forma la integral $\int_{a}^{x} f(t)dt$, puede recuperar la función original derivando:

$$
f(x) \to_{\int} \int_{a}^{x} f(t)dt \to_{dx} \frac{d}{dx} \int_{a}^{x} f(t)dt = f(x)
$$

**TFC2:** Si usted deriva primero y, luego, integra, también puede recuperar $f(x)$ [*Excepto, en una constante $f(a)$*]:

$$
f(x) \to_{dx} f'(x) \to_{\int} \int_{a}^{x} f'(t)dt = f(x) - f(a)
$$

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

---

<table border=1>
  <thead>
    <th>
      <img src="https://minas.medellin.unal.edu.co/images/Programa-Minas-Contigo/Logo-Minas-Contigo.png" width="320px" height="270px" />
    </th>
    <th>
      <h1>Aplicaciones de la integración</h1>
    </th>
  </thead>
</table>

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

# Volúmenes

Sea $A(x)$ el área de la sección transversal para cada punto $x \in [a, b]$. Definimos el **volumen** del sólido $S$ por:

$$
V(S) = \int_{a}^{b}{A(x)}dx
$$

## Volúmenes mediante discos

$$
A(x) = \pi*R^2(x)
$$

## Volúmenes mediante arandelas

![](https://i.ytimg.com/vi/J0eyio8uAoA/maxresdefault.jpg)

$$
A(x) = \pi*(R^2(x) - r^2(x))
$$

## Volúmenes mediante cascarones cilíndricos

$$
V(S) = 2\pi*\int_{a}^{b}{d(x)*f(x)}dx
$$

* **Distancia al eje de giro**: $d(x)$

* **Altura del cilindro**: $f(x)$

# Trabajo

Para el estudio de este tema recordemos antes algunas unidades de medida para cantidades fisicas.

<table>
<thead>
<th>Cantidad (símbolo)</th>
<th>Internacional</th>
<th>Ingles</th>
</thead>
<tbody>
<tr>
<th>Longitud (L)</th>
<td><strong>Metros</strong>: m</td>
<td>pies (ft) = 0.3048 m</td>
</tr>
<tr>
<th>Masa (m)</th>
<td><strong>Kilogramo</strong>: kg</td>
<td>slug = 14.5939 kg</td>
</tr>
<tr>
<th>Tiempo (t)</th>
<td colspan="2" style="text-align: center"><strong>Segundo</strong>: s</td>
</tr>
<tr>
<th>Fuerza (F)</th>
<td><strong>Newton</strong>: N</td>
<td>libras (lb) = 4.44822 N</td>
</tr>
<tr>
<th>Trabajo (W)</th>
<td><strong>Joule</strong>: J</td>
<td>Libras-pie (lb-ft) = 1.356 J</td>
</tr>
</tbody>
</table>

* Segunda Ley de movimiento de Newton: $F = m*a = m*v'(t)$

* Gravedad: $g = 9.8*\frac{m}{s^{2}} = 32.2*\frac{ft}{s^{2}}$

* Densidad del agua: $\rho = \frac{m}{v} = 1000*\frac{kg}{m^{3}} = 1.94*\frac{slug}{ft^{3}}$

* Peso específico del agua: $\gamma = \rho * g = 9800 * \frac{N}{m^{3}} = 62.4 * \frac{lb}{ft^{3}}$

> **Nota:** Al trabajar este tipo de problemas debemos expresar todas las cantidades físicas en las mismas unidades.

Se define el trabajo como la cantidad de fuerza necesaria para mover un objeto una cierta distancia. Cuando se trabaja con una fuerza constante, se define el trabajo (W) como

$$
W_{Trabajo} = F_{Fuerza}*L_{Distancia}
$$

Para el caso en que la Fuerza y la distancia se definan como funciones, el trabajo resultante se define como una integral.

## Ley de Hooke

La **fuerza** requerida para mantener un resorte estirado *x* unidades mas allá de su longitud natural es proporcional a *x*:

$$
F(x) = k*x
$$

Donde $k > 0$ es **la constante elastica** del resorte.

Por lo tanto para calcular el trabajo de mover un resorte desde a hasta b (con respecto a la posición natural), se define la integral de la siguiente forma:

$$
F = F(x) = k*x
$$

$$
L = dx
$$

$$
dW = F * L = k * x * dx
$$

$$
\int{W}dW =  \int_{a}^{b}{k*x}dx
$$

## Ascensores

$$
F = g*(m + ((L_{total} - y)*\rho_{L}))
$$

$$
L = dy
$$

$$
dW = F * L = g * (m + ((L_{total} - y) * \rho_{L}))dy
$$

$$
\int{W}dW =  \int_{a}^{b}{g*(m + ((L_{total} - y)*\rho_{L}))}dy
$$

> **Ejercicio:** Calcula el trabajo que tiene que hacer un motor para mover un elevador desde el primer piso al quinto piso a 30 metros del primero. Ten en cuenta que la cabina sola pesa 200kg, que en el primer piso se subió un hombre de 70kg y que en cada piso se sube otro del mismo peso.

## Vaciado de tanques

$$
F = \gamma*dV
$$

$$
L = (y_{f} - y)
$$

$$
dW = F * L = (y_{f} - y) * \gamma * dv
$$

$$
\int{W}dW =  \int_{a}^{b}{(y_{f} - y)*\gamma}dV
$$

> **Ejercicio:** Te estas tomando una michelada en la playa a 30°C, en un vaso con altura de 10cm y un diametro de 7cm; además, te dieron un pitillo de 15cm para beber. Calcula el trabajo de tomarte la michelada asumiendo que el vaso esta lleno hasta el borde.

> **Ejercicio:** Te fuiste a San Andres de vacaciones y te sirvieron un coco loco, asumiendo que el coco es una esfera perfecta de diametro de 20cm, que esta lleno hasta 3/4 de la altura completa y que tienes un pitillo de 30cm, ¿Cual es el trabajo de tomarte el coco loco?

> **Ejercicio:** Trabajas en un equipo de la ONU que desarrolla viviendas rurales en zonas inundadas, la estrategia que escogieron para el diseño de las viviendas son los palafitos; sin embargo, ahora se enfrentan al problema de subir agua desde la laguna en la que están hasta la vivienda, para ello necesitan poner unas bombas en las viviendas pero tienes que calcular el trabajo que tiene que hacer la bomba para escoger la mejor. Ten en cuenta que la poseta dentro de la vivienda tiene forma de prisma rectangular con base de 2X2 metros cuadrados y altura de 1,5 metros; además, por eficiencia de la bomba, esta poseta se tiene que llenar desde arriba.

# Momentos y centros de masa

La **masa** del rectángulo $R_{i}$ está dad por $m(R_{i}) = densidad*área(R_{i}) = \rho*[f(\bar{x_{i}}) - g(\bar{x_{i}})]*\Delta x$

El **momento** del rectángulo $R_{i}$ respecto al eje $y$ es $m(R_{i})$ por la distancia de $C_{i}$ al eje y; es decir, $M_{y}(R_{i}) = m(R_{i})*\bar{x_{i}}$

Definimos el **momento** de R **respecto al eje y** por

$$
M_{y} = \lim_{n \to \infty} \sum_{i=1}^{n} M_{y}(R_{i}) = \int_{a}^{b}{\rho x*(f(x) - g(x))}dx
$$

De manera análoga, se justifica que el **momento** de R **respecto al eje x** es

$$
M_{x} = \int_{a}^{b}{\frac{1}{2}*\rho*(f^{2}(x) - g^{2}(x))}dx
$$

Sean A el área y $m = \rho*A$ la masa de R. El **centroide** $(\bar{x}, \bar{y})$ de R se define por

$$
\bar{x} = \frac{M_{y}}{m} = \frac{1}{A}*\int_{a}^{b}{x*(f(x) - g(x))}dx
$$

$$
\bar{y} = \frac{M_{x}}{m} = \frac{1}{2A}*\int_{a}^{b}{f^{2}(x) - g^{2}(x)}dx
$$

# Curvas definidas por medio de ecuaciones paramétricas

Si $f$ y $g$ son funciones continuas definidas sobre un intervalo común *I*, entonces $x = f(t)$, $y = g(t)$ se denominan **ecuaciones paramétricas** y $t$ recibe el nombre de **paraámetro**. La curva plana

$$
C = \{(f(t), g(t)) | t \in I\} \subseteq \mathbb{R}
$$

Se denomina **curva paramétrica**.

Cuando $I = [a, b]$, decimos que la curva tiene punto inicial $(f(a), g(a))$ y punto final $(f(b), g(b))$.

# Cálculo con curvas paramétricas

## Tangentes

Una curva paramétrica $x = f(t)$, $y = g(t)$ es **diferenciable** en t si f y g son diferenciables en t. Usando la regla de la cadena, si las 3 derivadas existen y $\frac{dx}{dt} \neq 0$, entonces

$$
\frac{dy}{dx} = \frac{dy / dt}{dx / dt} = \frac{y'(t)}{x'(t)}
$$

La anterior fórmula nos da un criterio que es útil para trazar curvas paramétricas.

> **Tangentes**
>
> * Si $\frac{dy}{dt} = 0$ en $t_0$ y $\frac{dx}{dt} \neq 0$ en $t_0$, entonces la curva tiene una tangente horizontal en $y(t_0)$.
>
> * Si $\frac{dx}{dt} = 0$ en $t_1$ y $\frac{dy}{dt} \neq 0$ en $t_1$, entonces la curva tiene una tangente vertical en $x(t_1)$.
>
> * Cuando $\frac{dy}{dt} = \frac{dx}{dt} = 0$ en un punto, no se puede extraer una conclusión inmediata acerca de la recta tangente.

Como sabemos también es muy útil considerar la segunda derivada para determinar concavidad:

Si f, g son continuamente derivables y $\frac{dy}{dt} \neq 0$, entonces

$$
\frac{d^{2}y}{dx^{2}} = \frac{dy' / dt}{dx / dt}
$$

donde $y' = \frac{dy}{dx}$

## Área en paramétricas

Si tenemos una curva con ecuaciones paramétricas:

$$
x = f(t), \ y = g(t), \ \alpha \leq t \leq \beta
$$

entonces podemos calcular el área usando la regla de sustitución para integrales definidas:

> **Fórmula paramétrica para área**
>
> $A = \int_{a}^{b} ydx = \int_{\alpha}^{\beta} g(t)f'(t)dt$
>
> $A = \int_{a}^{b} xdy = \int_{\alpha}^{\beta} f(t)g'(t)dt$
>
> **Nota** Al calcular el área, el orden en los límites de integración depende del sentido en el cual se recorre la curva.

## Longitud de arco

Si tenemos una curva con ecuaciones paramétricas:

$$
x = f(t), \ y = g(t), \ \alpha \leq t \leq \beta
$$

Decimos que $C$ es **suave** si $f'$ y $g'$ son continuas y no simultaneamente iguales a 0 en $t \in [\alpha, \beta]$. Intuitivamente, significa que $C$ es una curva continua sin picos, ni esquinas.

Ahora, si $C$ es una curva suave, que se recorre sólo una vez cuando $t$ aumenta de $\alpha$ a $\beta$, se define la **longitud de arco** de C por:

$$
L = \int_{\alpha}^{\beta} \sqrt{(\frac{dx}{dt})^{2} + (\frac{dy}{dt})^{2}} dt
$$

En el caso particular en que $y = f(x)$, $a \leq x \leq b$, podemos parametrizar la curva por $x = x, \ y= f(x)$. Es decir, tomamos la variable independiente $x$ como parámetro. Así:

$$
L = \int_{a}^{b} \sqrt{1 + (\frac{dy}{dx})^{2}} dx
$$

De manera análoga, si $x = g(y)$, $c \leq y \leq d$, tenemos

$$
L = \int_{a}^{b} \sqrt{(\frac{dx}{dy})^{2} + 1} dy
$$

# Coordenadas polares

El **sistema coordenado polar**, introducido por Newton, proporciona descripciones y ecuaciones más simples para cierto tipo de curvas y regiones en el plano.

> **Conexión entre coordenadas polares y cartesianas**
>
> * Si el punto $P \in \mathbb{R}^{2}$ tiene coordenadas polares $(r, \theta)$, entonces sus coordenadas cartesianas se obtienen mediante:
>
> $$x = rcos(\theta) \\ y = rsin(\theta)$$
>
> * Si el punto $P \in \mathbb{R}^{2}$ tiene coordenadas cartesianas $(x, y)$, entonces sus coordenadas polares se obtienen mediante:
>
> $$r^{2} = x^{2} + y^{2} \\ tan(\theta) = \frac{y}{x}; \ x \neq 0$$

# Áreas en coordenadas polares

El **área** de la región $R$ acotada por la curva $r = f(\theta)$ entre las rectas $\theta = \alpha$ y $\theta = \beta$ es

$$
A = \int_{\alpha}^{\beta} \frac{1}{2}*[f(\theta)]^{2} d\theta = \frac{1}{2}*\int_{\alpha}^{\beta} r^{2}(\theta) d\theta
$$

Ahora, consideremos 2 curvas $r = f(\theta)$ y $r = g(\theta)$. Si $f, g$ son continuas en $[\alpha, \beta]$ y $f(\theta) \geq g(\theta)$ para todo $\theta \in [\alpha, \beta]$, entonces el **área** entre $f$ y $g$ es:

$$
A = \frac{1}{2}*\int_{\alpha}^{\beta} ([f(\theta)]^{2} - [g(\theta)]^{2}) d\theta
$$

# Longitud de arco en polares

Dada una curva polar $r = f(\theta)$ podemos considerar la parametrización

$$
x = rcos(\theta) = f(\theta)*cos(\theta) \\ y = rsin(\theta) = f(\theta)*sin(\theta) \\ \alpha \leq \theta \leq \beta
$$

lo cual da lugar a la **fórmula polar para longitud de arco**:

$$
L = \int_{\alpha}^{\beta} \sqrt{(\frac{dx}{d\theta})^{2} + (\frac{dy}{d\theta})^{2}} d\theta = \int_{\alpha}^{\beta} \sqrt{r^{2} + (\frac{dr}{d\theta})^{2}} d\theta
$$

---

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

![Minas Contigo - Facultad de Minas - UNAL](./img/footer.png)
