# Propiedades Básicas del Cálculo Integral

Las propiedades básicas de la integral definida son reglas fundamentales que permiten simplificar y manipular integrales de manera eficiente.

## Propiedades Principales

### Linealidad de la Integral

La integral es un operador lineal, lo que significa que se puede factorizar constantes y separar sumas:

- $\displaystyle\int_{a}^{b} k·f(x)dx = k·\int_{a}^{b} f(x)dx$ (donde k es una constante)
- $\displaystyle\int_{a}^{b} [f(x) + g(x)]dx = \int_{a}^{b} f(x)dx + \int_{a}^{b} g(x)dx$

**Ejemplos:**
- $\displaystyle\int_{0}^{2} 3x^2 dx = 3\int_{0}^{2} x^2 dx = 3\left[\dfrac{x^3}{3}\right]₀² = 3(8/3) = 8$
- \int[1,3] (2x + 5)dx = \int[1,3] 2x dx + \int[1,3] 5 dx = 2·\int[1,3] x dx + 5·\int[1,3] 1 dx = 2·[x²/2]₁³ + 5·[x]₁³ = 2·(9/2 - 1/2) + 5·(3-1) = 8 + 10 = 18

### Propiedad de Inversión de Límites

Cuando se intercambian los límites de integración, la integral cambia de signo:

- \int_{a}^{b} f(x)dx = -\int[b,a] f(x)dx

**Ejemplo:**
- \int[1,4] x dx = [x²/2]₁⁴ = 8 - 1/2 = 15/2
- \int[4,1] x dx = -\int[1,4] x dx = -15/2

### Integral con Límites Iguales

Cuando los límites superior e inferior son iguales, la integral vale cero:

- \int[a,a] f(x)dx = 0

**Ejemplo:**
- \int[3,3] (x² + 2x + 1)dx = 0

### Aditividad Respecto al Dominio

Se puede dividir el intervalo de integración:

- \int[a,c] f(x)dx = \int_{a}^{b} f(x)dx + \int[b,c] f(x)dx (donde a ≤ b ≤ c)

**Ejemplo:**
- \int[0,4] x² dx = \int_{0}^{2} x² dx + \int[2,4] x² dx
- \int[0,4] x² dx = [x³/3]₀⁴ = 64/3
- \int_{0}^{2} x² dx = [x³/3]₀² = 8/3
- \int[2,4] x² dx = [x³/3]₂⁴ = 64/3 - 8/3 = 56/3
- Verificación: 8/3 + 56/3 = 64/3 ✓

## Propiedades de Comparación

### Monotonía

Si f(x) ≤ g(x) en _{a}^{b}, entonces:

- \int_{a}^{b} f(x)dx ≤ \int_{a}^{b} g(x)dx

**Ejemplo:**
- Si f(x) = x y g(x) = x² en [2,3], entonces x ≤ x² en este intervalo
- \int[2,3] x dx = [x²/2]₂³ = 9/2 - 2 = 5/2
- \int[2,3] x² dx = [x³/3]₂³ = 9 - 8/3 = 19/3
- Como 5/2 = 7.5/3 < 19/3, se cumple la propiedad

### Valor Absoluto

La integral del valor absoluto es mayor o igual al valor absoluto de la integral:

- |\int_{a}^{b} f(x)dx| ≤ \int_{a}^{b} |f(x)|dx

**Ejemplo:**
- Sea f(x) = x en [-1,1]
- \int[-1,1] x dx = [x²/2]₋₁¹ = 1/2 - 1/2 = 0
- |\int[-1,1] x dx| = |0| = 0
- \int[-1,1] |x| dx = \int[-1,0] (-x) dx + \int[0,1] x dx = [-x²/2]₋₁⁰ + [x²/2]₀¹ = 1/2 + 1/2 = 1
- Se verifica que 0 ≤ 1

## Ejemplos de Integrales Básicas

### Integrales de Polinomios

**Fórmula general:**
- \int xⁿ dx = xⁿ⁺¹/(n+1) + C (para n ≠ -1)

**Ejemplo:**
- \int[0,3] (2x³ - 5x² + 3x - 1) dx = [x⁴/2 - 5x³/3 + 3x²/2 - x]₀³ = 81/2 - 45 + 27/2 - 3 = 81/2 - 48 + 27/2 = 108/2 - 48 = 54 - 48 = 6

### Integrales Trigonométricas

#### Seno y Coseno

**Fórmulas:**
- \int sen(x) dx = -cos(x) + C
- \int cos(x) dx = sen(x) + C

**Ejemplos:**
- \int[0,π/2] sen(x) dx = [-cos(x)]₀^(π/2) = -cos(π/2) - (-cos(0)) = 0 - (-1) = 1
- \int[0,π/4] cos(x) dx = [sen(x)]₀^(π/4) = sen(π/4) - sen(0) = √2/2 - 0 = √2/2

#### Secante al Cuadrado

**Fórmula:**
- \int sec²(x) dx = tan(x) + C

**Ejemplo:**
- \int[0,π/4] sec²(x) dx = [tan(x)]₀^(π/4) = tan(π/4) - tan(0) = 1 - 0 = 1

#### Secante por Tangente

**Fórmula:**
- \int sec(x)tan(x) dx = sec(x) + C

**Ejemplo:**
- \int[0,π/4] sec(x)tan(x) dx = [sec(x)]₀^(π/4) = sec(π/4) - sec(0) = √2 - 1

### Integral de 1/x

**Fórmula:**
- \int (1/x) dx = ln|x| + C

**Ejemplos:**
- \int[1,e] (1/x) dx = [ln|x|]₁ᵉ = ln(e) - ln(1) = 1 - 0 = 1
- \int[2,4] (3/x) dx = 3·\int[2,4] (1/x) dx = 3·[ln|x|]₂⁴ = 3·(ln(4) - ln(2)) = 3·ln(2) = 3ln(2)

## Ejemplo Combinado

Utilizando varias propiedades y tipos de funciones:

\int[0,π/2] (x² + 2sen(x) - 3cos(x) + 4/x) dx

**Nota:** Esta integral no se puede evaluar directamente en [0,π/2] debido a 4/x en x=0. Para fines ilustrativos, evaluemos en [1,π/2]:

\int[1,π/2] (x² + 2sen(x) - 3cos(x) + 4/x) dx

Aplicando linealidad:
= \int[1,π/2] x² dx + 2\int[1,π/2] sen(x) dx - 3\int[1,π/2] cos(x) dx + 4\int[1,π/2] (1/x) dx
= [x³/3]₁^(π/2) + 2[-cos(x)]₁^(π/2) - 3[sen(x)]₁^(π/2) + 4[ln|x|]₁^(π/2)
= (π³/24 - 1/3) + 2(0 - (-cos(1))) - 3(1 - sen(1)) + 4(ln(π/2) - ln(1))
= π³/24 - 1/3 + 2cos(1) - 3 + 3sen(1) + 4ln(π/2)

## Aplicaciones Prácticas

Estas propiedades son fundamentales para resolver integrales complejas, ya que permiten descomponer problemas difíciles en partes más manejables. Permiten separar una función complicada en suma de funciones más simples, factorizar constantes para simplificar cálculos, y cambiar los límites de integración según convenga para el problema específico.

El dominio de estas propiedades básicas y las integrales fundamentales es esencial antes de avanzar a técnicas más sofisticadas como integración por partes o sustitución trigonométrica.

## Resumen de Fórmulas Principales

| Función      | Integral Indefinida |
| ------------ | ------------------- |
| xⁿ           | xⁿ⁺¹/(n+1) + C      |
| 1/x          | ln\|x\| + C         |
| sen(x)       | -cos(x) + C         |
| cos(x)       | sen(x) + C          |
| sec²(x)      | tan(x) + C          |
| sec(x)tan(x) | sec(x) + C          |