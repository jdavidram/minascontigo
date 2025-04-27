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
