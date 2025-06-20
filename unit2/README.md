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

