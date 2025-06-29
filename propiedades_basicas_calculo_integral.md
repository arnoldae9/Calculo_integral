# Propiedades Básicas del Cálculo Integral

Las propiedades básicas de la integral definida son reglas fundamentales que permiten simplificar y manipular integrales de manera eficiente.

## Propiedades Principales

### Linealidad de la Integral

La integral es un operador lineal, lo que significa que se puede factorizar constantes y separar sumas:

- $\int_a^b k \cdot f(x)dx = k \cdot \int_a^b f(x)dx$ (donde $k$ es una constante)
- $\int_a^b [f(x) + g(x)]dx = \int_a^b f(x)dx + \int_a^b g(x)dx$

**Ejemplos:**
- $\int_0^2 3x^2 dx = 3 \cdot \int_0^2 x^2 dx = 3 \cdot \left[\frac{x^3}{3}\right]_0^2 = 3 \cdot \left(\frac{8}{3}\right) = 8$
- $\int_1^3 (2x + 5)dx = \int_1^3 2x dx + \int_1^3 5 dx = 2 \cdot \int_1^3 x dx + 5 \cdot \int_1^3 1 dx = 2 \cdot \left[\frac{x^2}{2}\right]_1^3 + 5 \cdot [x]_1^3 = 2 \cdot \left(\frac{9}{2} - \frac{1}{2}\right) + 5 \cdot (3-1) = 8 + 10 = 18$

### Propiedad de Inversión de Límites

Cuando se intercambian los límites de integración, la integral cambia de signo:

- $\int_a^b f(x)dx = -\int_b^a f(x)dx$

**Ejemplo:**
- $\int_1^4 x dx = \left[\frac{x^2}{2}\right]_1^4 = 8 - \frac{1}{2} = \frac{15}{2}$
- $\int_4^1 x dx = -\int_1^4 x dx = -\frac{15}{2}$

### Integral con Límites Iguales

Cuando los límites superior e inferior son iguales, la integral vale cero:

- $\int_a^a f(x)dx = 0$

**Ejemplo:**
- $\int_3^3 (x^2 + 2x + 1)dx = 0$

### Aditividad Respecto al Dominio

Se puede dividir el intervalo de integración:

- $\int_a^c f(x)dx = \int_a^b f(x)dx + \int_b^c f(x)dx$ (donde $a \leq b \leq c$)

**Ejemplo:**
- $\int_0^4 x^2 dx = \int_0^2 x^2 dx + \int_2^4 x^2 dx$
- $\int_0^4 x^2 dx = \left[\frac{x^3}{3}\right]_0^4 = \frac{64}{3}$
- $\int_0^2 x^2 dx = \left[\frac{x^3}{3}\right]_0^2 = \frac{8}{3}$
- $\int_2^4 x^2 dx = \left[\frac{x^3}{3}\right]_2^4 = \frac{64}{3} - \frac{8}{3} = \frac{56}{3}$
- Verificación: $\frac{8}{3} + \frac{56}{3} = \frac{64}{3}$

## Propiedades de Comparación

### Monotonía

Si $f(x) \leq g(x)$ en $[a,b]$, entonces:

- $\int_a^b f(x)dx \leq \int_a^b g(x)dx$

**Ejemplo:**
- Si $f(x) = x$ y $g(x) = x^2$ en $[2,3]$, entonces $x \leq x^2$ en este intervalo
- $\int_2^3 x dx = \left[\frac{x^2}{2}\right]_2^3 = \frac{9}{2} - 2 = \frac{5}{2}$
- $\int_2^3 x^2 dx = \left[\frac{x^3}{3}\right]_2^3 = 9 - \frac{8}{3} = \frac{19}{3}$
- Como $\frac{5}{2} = \frac{7.5}{3} < \frac{19}{3}$, se cumple la propiedad

### Valor Absoluto

La integral del valor absoluto es mayor o igual al valor absoluto de la integral:

- $\left|\int_a^b f(x)dx\right| \leq \int_a^b |f(x)|dx$

**Ejemplo:**
- Sea $f(x) = x$ en $[-1,1]$
- $\int_{-1}^1 x dx = \left[\frac{x^2}{2}\right]_{-1}^1 = \frac{1}{2} - \frac{1}{2} = 0$
- $\left|\int_{-1}^1 x dx\right| = |0| = 0$
- $\int_{-1}^1 |x| dx = \int_{-1}^0 (-x) dx + \int_0^1 x dx = \left[-\frac{x^2}{2}\right]_{-1}^0 + \left[\frac{x^2}{2}\right]_0^1 = \frac{1}{2} + \frac{1}{2} = 1$
- Se verifica que $0 \leq 1$

## Ejemplos de Integrales Básicas

### Integrales de Polinomios

**Fórmula general:**
- $\int x^n dx = \frac{x^{n+1}}{n+1} + C$ (para $n \neq -1$)

**Ejemplo:**
- $\int_0^3 (2x^3 - 5x^2 + 3x - 1) dx = \left[\frac{x^4}{2} - \frac{5x^3}{3} + \frac{3x^2}{2} - x\right]_0^3 = \frac{81}{2} - 45 + \frac{27}{2} - 3 = \frac{81}{2} - 48 + \frac{27}{2} = \frac{108}{2} - 48 = 54 - 48 = 6$

### Integrales Trigonométricas

#### Seno y Coseno

**Fórmulas:**
- $\int \sin(x) dx = -\cos(x) + C$
- $\int \cos(x) dx = \sin(x) + C$

**Ejemplos:**
- $\int_0^{\pi/2} \sin(x) dx = [-\cos(x)]_0^{\pi/2} = -\cos(\pi/2) - (-\cos(0)) = 0 - (-1) = 1$
- $\int_0^{\pi/4} \cos(x) dx = [\sin(x)]_0^{\pi/4} = \sin(\pi/4) - \sin(0) = \frac{\sqrt{2}}{2} - 0 = \frac{\sqrt{2}}{2}$

#### Secante al Cuadrado

**Fórmula:**
- $\int \sec^2(x) dx = \tan(x) + C$

**Ejemplo:**
- $\int_0^{\pi/4} \sec^2(x) dx = [\tan(x)]_0^{\pi/4} = \tan(\pi/4) - \tan(0) = 1 - 0 = 1$

#### Secante por Tangente

**Fórmula:**
- $\int \sec(x)\tan(x) dx = \sec(x) + C$

**Ejemplo:**
- $\int_0^{\pi/4} \sec(x)\tan(x) dx = [\sec(x)]_0^{\pi/4} = \sec(\pi/4) - \sec(0) = \sqrt{2} - 1$

### Integral de 1/x

**Fórmula:**
- $\int \frac{1}{x} dx = \ln|x| + C$

**Ejemplos:**
- $\int_1^e \frac{1}{x} dx = [\ln|x|]_1^e = \ln(e) - \ln(1) = 1 - 0 = 1$
- $\int_2^4 \frac{3}{x} dx = 3 \cdot \int_2^4 \frac{1}{x} dx = 3 \cdot [\ln|x|]_2^4 = 3 \cdot (\ln(4) - \ln(2)) = 3 \cdot \ln(2) = 3\ln(2)$

## Ejemplo Combinado

Utilizando varias propiedades y tipos de funciones:

$\int_0^{\pi/2} \left(x^2 + 2\sin(x) - 3\cos(x) + \frac{4}{x}\right) dx$

**Nota:** Esta integral no se puede evaluar directamente en $[0,\pi/2]$ debido a $\frac{4}{x}$ en $x=0$. Para fines ilustrativos, evaluemos en $[1,\pi/2]$:

$\int_1^{\pi/2} \left(x^2 + 2\sin(x) - 3\cos(x) + \frac{4}{x}\right) dx$

Aplicando linealidad:
$$= \int_1^{\pi/2} x^2 dx + 2\int_1^{\pi/2} \sin(x) dx - 3\int_1^{\pi/2} \cos(x) dx + 4\int_1^{\pi/2} \frac{1}{x} dx$$

$$= \left[\frac{x^3}{3}\right]_1^{\pi/2} + 2[-\cos(x)]_1^{\pi/2} - 3[\sin(x)]_1^{\pi/2} + 4[\ln|x|]_1^{\pi/2}$$

$$= \left(\frac{\pi^3}{24} - \frac{1}{3}\right) + 2(0 - (-\cos(1))) - 3(1 - \sin(1)) + 4(\ln(\pi/2) - \ln(1))$$

$$= \frac{\pi^3}{24} - \frac{1}{3} + 2\cos(1) - 3 + 3\sin(1) + 4\ln(\pi/2)$$

## Aplicaciones Prácticas

Estas propiedades son fundamentales para resolver integrales complejas, ya que permiten descomponer problemas difíciles en partes más manejables. Permiten separar una función complicada en suma de funciones más simples, factorizar constantes para simplificar cálculos, y cambiar los límites de integración según convenga para el problema específico.

El dominio de estas propiedades básicas y las integrales fundamentales es esencial antes de avanzar a técnicas más sofisticadas como integración por partes o sustitución trigonométrica.

## Resumen de Fórmulas Principales
<center>

| Función          | Integral Indefinida       |
| ---------------- | ------------------------- |
| $x^n$            | $\frac{x^{n+1}}{n+1} + C$ |
| $\frac{1}{x}$    | $\ln\|x\| + C$            |
| $\sin(x)$        | $-\cos(x) + C$            |
| $\cos(x)$        | $\sin(x) + C$             |
| $\sec^2(x)$      | $\tan(x) + C$             |
| $\sec(x)\tan(x)$ | $\sec(x) + C$             |
</center>