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
