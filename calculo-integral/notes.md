<!-- CAPITULO 2 -->

# Capitulo 2

## Volúmenes

Sea $A(x)$ el área de la sección transversal para cada punto $x \in \[a, b]$. Definimos el **volumen** del sólido $S$ por:

$$
V(S) = \int_{a}^{b}{A(x)}dx
$$

### Volúmenes mediante discos

$$
A(x) = \pi*R^2(x)
$$

### Volúmenes mediante arandelas

![](https://i.ytimg.com/vi/J0eyio8uAoA/maxresdefault.jpg)

$$
A(x) = \pi*(R^2(x) - r^2(x))
$$

### Volúmenes mediante cascarones cilíndricos

$$
V(S) = 2\pi*\int_{a}^{b}{d(x)*f(x)}dx
$$

* **Distancia al eje de giro**: $d(x)$
* **Altura del cilindro**: $f(x)$

## Trabajo

Para el estudio de este tema recordemos antes algunas unidades de medida para cantidades fisicas.

| Cantidad (símbolo) | Internacional     | Ingles                       |
| ------------------ | ----------------- | ---------------------------- |
| Longitud (L)       | **Metros**: m     | pies (ft) = 0.3048 m         |
| Masa (m)           | **Kilogramo**: kg | slug = 14.5939 kg            |
| Tiempo (t)         | **Segundo**: s    |                              |
| Fuerza (F)         | **Newton**: N     | libras (lb) = 4.44822 N      |
| Trabajo (W)        | **Joule**: J      | Libras-pie (lb-ft) = 1.356 J |

* Segunda Ley de movimiento de Newton: $F = m*a = m*\frac{dv}{dt}$
* Gravedad: $g = 9.8*\frac{m}{s^{2}} = 32.2*\frac{ft}{s^{2}}$
* Densidad del agua: $\rho = \frac{m}{v} = 1000*\frac{kg}{m^{3}} = 1.94*\frac{slug}{ft^{3}}$
* Peso específico del agua: $\gamma = \rho*g = 9800*\frac{N}{m^{3}} = 62.4*\frac{lb}{ft^{3}}$

> **Nota:** Al trabajar este tipo de problemas debemos expresar todas las cantidades físicas en las mismas unidades.

Se define el trabajo como la cantidad de fuerza necesaria para mover un objeto una cierta distancia. Cuando se trabaja con una fuerza constante, se define el trabajo (W) como

$$
W_{Trabajo} = F_{Fuerza}*L_{Distancia}
$$

Para el caso en que la Fuerza y la distancia se definan como funciones, el trabajo resultante se define como una integral.

### Ley de Hooke

La **fuerza** requerida para mantener un resorte estirado _x_ unidades mas allá de su longitud natural es proporcional a _x_:

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

### Ascensores

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

### Vaciado de tanques

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

## Momentos y centros de masa

La **masa** del rectángulo $R\_{i}$ está dad por $m(R_{i}) = densidad*area(R_{i}) = \rho*[f(\bar{x_{i}}) - g(\bar{x_{i}})]*\Delta x$

El **momento** del rectángulo $R\_{i}$ respecto al eje $y$ es $m(R_{i})$ por la distancia de $C_{i}$ al eje y; es decir, $M_{y}(R_{i}) = m(R_{i})*\bar{x_{i}}$

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

## Curvas definidas por medio de ecuaciones paramétricas

Si $f$ y $g$ son funciones continuas definidas sobre un intervalo común _I_, entonces $x = f(t)$, $y = g(t)$ se denominan **ecuaciones paramétricas** y $t$ recibe el nombre de **paraámetro**. La curva plana

$$
C = \{(f(t), g(t)) | t \in I\} \subseteq \mathbb{R}
$$

Se denomina **curva paramétrica**.

Cuando $I = [a, b]$, decimos que la curva tiene punto inicial $(f(a), g(a))$ y punto final $(f(b), g(b))$.

## Cálculo con curvas paramétricas

### Tangentes

Una curva paramétrica $x = f(t)$, $y = g(t)$ es **diferenciable** en t si f y g son diferenciables en t. Usando la regla de la cadena, si las 3 derivadas existen y $\frac{dx}{dt} \neq 0$, entonces

$$
\frac{dy}{dx} = \frac{dy / dt}{dx / dt} = \frac{y'(t)}{x'(t)}
$$

La anterior fórmula nos da un criterio que es útil para trazar curvas paramétricas.

> **Tangentes**
> 
> * Si $\frac{dy}{dt} = 0$ en $t\_0$ y $\frac{dx}{dt} \neq 0$ en $t\_0$, entonces la curva tiene una tangente horizontal en $y(t\_0)$.
> * Si $\frac{dx}{dt} = 0$ en $t\_1$ y $\frac{dy}{dt} \neq 0$ en $t\_1$, entonces la curva tiene una tangente vertical en $x(t\_1)$.
> * Cuando $\frac{dy}{dt} = \frac{dx}{dt} = 0$ en un punto, no se puede extraer una conclusión inmediata acerca de la recta tangente.

Como sabemos también es muy útil considerar la segunda derivada para determinar concavidad:

Si f, g son continuamente derivables y $\frac{dy}{dt} \neq 0$, entonces

$$
\frac{d^{2}y}{dx^{2}} = \frac{dy' / dt}{dx / dt}
$$

donde $y' = \frac{dy}{dx}$

### Área en paramétricas

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

### Longitud de arco

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

## Coordenadas polares

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

## Áreas en coordenadas polares

El **área** de la región $R$ acotada por la curva $r = f(\theta)$ entre las rectas $\theta = \alpha$ y $\theta = \beta$ es

$$
A = \int_{\alpha}^{\beta} \frac{1}{2}*[f(\theta)]^{2} d\theta = \frac{1}{2}*\int_{\alpha}^{\beta} r^{2}(\theta) d\theta
$$

Ahora, consideremos 2 curvas $r = f(\theta)$ y $r = g(\theta)$. Si $f, g$ son continuas en $[\alpha, \beta]$ y $f(\theta) \geq g(\theta)$ para todo $\theta \in [\alpha, \beta]$, entonces el **área** entre $f$ y $g$ es:

$$
A = \frac{1}{2}*\int_{\alpha}^{\beta} ([f(\theta)]^{2} - [g(\theta)]^{2}) d\theta
$$

## Longitud de arco en polares

Dada una curva polar $r = f(\theta)$ podemos considerar la parametrización

$$
x = rcos(\theta) = f(\theta)*cos(\theta) \\ y = rsin(\theta) = f(\theta)*sin(\theta) \\ \alpha \leq \theta \leq \beta
$$

lo cual da lugar a la **fórmula polar para longitud de arco**:

$$
L = \int_{\alpha}^{\beta} \sqrt{(\frac{dx}{d\theta})^{2} + (\frac{dy}{d\theta})^{2}} d\theta = \int_{\alpha}^{\beta} \sqrt{r^{2} + (\frac{dr}{d\theta})^{2}} d\theta
$$

***

---

<!-- CAPITULO 3 -->

# Capitulo 3

## Series

## Pruebas de divergencia

> **Nota**
> 
> Si $\sum a\_{n}$ es convergente, entonces $\lim\_{n \to \infty} a\_{n} = 0$
> 
> En general no se cumple el recíproco. Es decir, si $\lim\_{n \to \infty} a\_{n} = 0$, **NO** puedo concluir que $\sum a\_{n}$ sea convergente.

### Prueba de la divergencia

Si

$$
\lim_{n \to \infty} a_{n} \neq 0 \ o \ \nexists
$$

entonces $\sum a\_{n}$ diverge.

### Prueba de la integral

Sean $f: [1, \infty) \to \mathbb{R}^{+}$ una función continua, positiva y decreciente y $a\_{n} = f(n)$, $\forall n$.

$$
\int_{1}^{\infty} f(x) dx \ converge => \sum_{n=1}^{\infty} a_{n} \ converge
$$

$$
\int_{1}^{\infty} f(x) dx \ diverge => \sum_{n=1}^{\infty} a_{n} \ diverge
$$

### Prueba por comparación

Suponga que $0 < a\_{n} \leq b\_{n}$, $\forall n$.

* Si $\sum b\_{n} \ converge => \sum a\_{n} converge$
* Si $\sum a\_{n} \ diverge => \sum b\_{n} diverge$

### Prueba por comparación en el límite

Sean $a\_{n}$, $b\_{n}$ positivos.

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

### Prueba de la serie alternante (Criterio de Leibniz)

Si la serie alternante $\sum\_{n=1}^{\infty} (-1)^{n+1} * b\_{n}$, $b\_{n} > 0$, satisface:

1. $b\_{n+1} \leq b\_{n}$, para toda $n$ (NO creciente)
2. $\lim\limits\_{n \to \infty} b\_{n} = 0$

Entonces la serie es convergente.

> **Nota:**
> 
> * En la condición _1_ sólo se requiere que la sucesión sea NO creciente a partir de un cierto _n_.
> * Si la condición _2_ No se cumple, entonces se sigue que $\lim\limits\_{n \to \infty} a\_{n}$ NO existe. Por **la prueba de la divergencia**, la serie alternante diverge.

#### Estimación de la suma de una serie alternante

El error involucrado, usando la _n-ésima_ suma parcial $s\_{n}$ como aproximación a la suma total $s$ de una serie alternante, es el residuo $R\_{n} = s - s\_{n}$. El siguiente teorema nos dice que dicho error es menor que el primer termino que se deja de sumar.

**Teorema**

Si $\sum\_{n=1}^{\infty} (-1)^{n+1} * b\_{n}$ es convergente y $s = \sum\_{n=1}^{\infty} (-1)^{n+1} * b\_{n}$, entonces:

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

Observar que $b\_{4} = \frac{1}{256} < \frac{1}{200} = 0.005$. Entonces por el teorema $|R\_{3}| = |s - s\_{3}| \leq b\_{4}$, es decir, si estimamos $s$ por $s\_{3}$ el error no afecta la segunda cifra decimal. Luego, una estimación para _s_ aproximada a 2 cifras decimales es $s\_{3} \approx 0.9498$

### Prueba de la razón y de la raiz

Sea $\lim\limits_{n \to \infty} |\frac{a_{n+1}}{a_{n}}| = L$ ó $\lim\limits_{n \to \infty} |a_{n}|^{\frac{1}{n}} = L$

* $L < 1 => \sum\_{n=1}^{\infty} a\_{n}$ es absolutamente convergente
* $L > 1$ ó $L = \infty => \sum\_{n=1}^{\infty} a\_{n}$ es divergente
* Si $L = 1$, entonces la prueba NO es concluyente.

### Convergencia absoluta

Dada cualquier serie $\sum a\_{n}$ se puede considerar la serie

$$
\sum |a_{n}| = |a_{1}| + |a_{2}| + |a_{3}| + ... + |a_{n}| + ...
$$

cuyos términos son los valores absolutos de los términos de la serie original.

> Una serie $\sum a\_{n}$ se dice que es
> 
> * **Absolutamente convergente** si la serie de valores absolutos $\sum |a\_{n}|$ es convergente.
> * **Condicionalmente convergente** si es convergente, pero NO absolutamente convergente.

> **Nota:** Si $a\_{n} > 0$, entonces $\sum a\_{n} = \sum |a\_{n}|$. Luego, la convergencia absoluta es lo mismo que la convergencia usual en este caso.

## Series de potencias

Una **serie de potencias** es una serie de la forma

$$
\sum_{n=0}^{\infty} c_{n}*x^{n} = c_{0} + c_{1}x + c_{2}x^{2} + ...
$$

Donde $x$ es una variable y los $c\_{n}$ son constantes llamados **coeficientes** de la serie.

Una serie de potencias puede converger para ciertos valores de $x$ y diverger para otros. La suma de una serie de potencias, cuando converge, es una función

$$
f(x) = c_{0} + c_{1}x + c_{2}x^{2} + ...
$$

Cuyo dominio es el conjunto de todas las $x$ para las cuales la serie converge.

Por ejemplo, con $c\_{n} = 1$ para todo $n$, nos queda la **serie geométrica**

$$
\sum_{n=0}^{\infty} x^{n} = 1 + x + x^{2} + ...
$$

La cual vimos que converge si $|x| < 1$ y diverge si $|x| \geq 1$. Ademas,

> **Serie geométrica**
> 
> $f(x) = \frac{1}{1-x} = \sum\_{n=0}^{\infty} x^{n}$
> 
> $|x| < 1$

De forma más general, una serie de la forma

$$
\sum_{n=0}^{\infty} c_{n}(x-a)^{n} = c_{0} + c_{1}(x-a) + c_{2}(x-a)^{2} + ...
$$

Se denomina **serie de potencias centrada en a**.

### Radio e intervalos de convergencia

Para una serie de potencias dada $\sum\_{n=0}^{\infty} c\_{n}(x-a)^{n}$ hay solo 3 posibilidades:

* La serie solo converge cuando $x=a$, osea $R=0$
* La serie converge para todo $x$, osea $R=\infty$
* Existe un número positivo R tal que la serie
  * Converge, si $|x-a| < R$
  * Diverge, si $|x-a| > R$

A este $R$ se le llama **radio de convergencia** de la serie de potencias.

El **intervalo de convergencia** de una serie de potencias consta de todos los valores de $x$ para los cuales la serie converge.

* Cuando $R=0$, definimos el intervalo como $I={ a }$
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
> Intervalo = ${ 2 }$

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

### Representación de funciones como series de potencias

Decimos que la función $f(x) = \frac{1}{1-x}$, $|x| < 1$, tiene la representación en series de potencias

$$
\frac{1}{1-x} = \sum_{n=0}^{\infty} x^{n}
$$

en el intervalo $(-1, 1)$.

### Derivación e integración de series de potencias

Como la suma de una serie de potencias es una función, entonces nos gustaría poder diferenciar e integrar series de potencias. El siguiente teorema nos dice que podemos diferenciar e integrar cada uno de los términos de la serie, justo como se haría con un polinomio, allí donde ella converge. Esto se denomina **derivación e integración término a término**.

**Teorema:** Si la serie de potencias $\sum c\_{n}(x-a)^{n}$ tiene radio de convergencia R, la función $f$ definida por:

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
> * El invervalo de convergencia si puede cambiar en los extremos. Luego, siempre debemos analizarlos por aparte.

### Series de Taylor y Maclaurin

El objetivo de esta clase es tratar de responder las siguientes preguntas:

* ¿Qué funciones se pueden representar como series de potencias?
* Si una función se puede representar en series de potencias. ¿Cómo se puede hallar dicha representación?

Respondamos la segunda pregunta. Supongamos que $f(x)$ se representa mediante la serie de potencias

$$
f(x) = c_{0} + c_{1}(x-a) + c_{2}(x-a)^{2} + ...
$$

con $|x-a| < R$.

Hallemos los **coeficientes** $c\_{n}$ en términos de $f$. Primero, observamos que si sustituimos $x=a$ en la función anterior, se obtiene

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

#### Teorema de los coeficientes de Taylor

Si $f$ tiene una representación en forma de serie de potencias centrada en a:

$$
f(x) = \sum_{n=0}^{\infty} c_{n}(x-a)^{n} \\ |x-a| < R
$$

Entonces los coeficientes de la serie están dados por

$$
c_{n} = frac{f^{(n)}(a)}{n!}
$$

Si sustituimos la fórmula para $c\_{n}$ de nuevo en la serie, obtenemos **la serie de Taylor de $f$ centrada en $a \in \mathbb{R}$**:

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

Al tratar de probar que $\lim\limits\_{n\to\infty} R\_{n}(x) = 0$ para la serie de potencias de una cierta $f$ generalmente se emplea el siguiente resultado:

**Desigualdad de Taylor**: Si

$$
|f^{(n+1)(x)}| \leq M
$$

para $|x-a| < R$, entonces el residuos $R\_{n}(x)$ satisface la desigualdad

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

#### Series importantes de Maclaurin y sus radios de convergencia

**$R=\infty$**

* $e^{x} = \sum_{n=0}^{\infty} \frac{x^{n}}{n!}$
* $cos(x) = \sum_{n=0}^{\infty} (-1)^{n} \frac{x^{2n}}{(2n)!}$
* $sin(x) = \sum_{n=0}^{\infty} (-1)^{n} \frac{x^{2n+1}}{(2n+1)!}$

**$R=1$**

* $\frac{1}{1-x} = \sum\_{n=0}^{\infty} x^{n}$
* $ln(1+x) = \sum_{n=0}^{\infty} (-1)^{n-1} \frac{x^{n}}{n}$
* $tan^{-1}(x) = \sum_{n=0}^{\infty} (-1)^{n} \frac{x^{2n+1}}{2n+1}$

### Aproximación de funciones por polinomios

Podemos usar un polinomio de Taylor de grado $n$, $T\_{n}(x)$, para aproximar una función $f$ la cual se puede representar como una serie de Taylor centrada en a, digamos

$$
f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!} (x-a)^{n}
$$

Para $|x-a| < R$, en donde R es el radio de convergencia de la serie. Puesto que en este caso $f(x) = \lim\limits\_{n\to\infty} T\_{n}(x)$, entonces decimos que $f(x) \approx T\_{n}(x)$. Si queremos saber que tan buena es esta aproximación debemos analizar el tamaño del residuo

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
2. Use la desigualdad de Taylor para estimar la precisión de la aproximación $f(x) \approx T\_{3}(x)$ cuando $0.5 \leq x \leq 1.5$.

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

La aproximación en _Solución 1_, para $0.5 \leq x \leq 1.5$, tiene una precisión de una cifra decimal.    
