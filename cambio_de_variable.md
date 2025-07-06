### Problema 1
$\displaystyle \int \sqrt{25-x^2}(-2x) dx$

**Solución:**

Sea $u = 25 - x^2$

Entonces $du = -2x dx$

Sustituyendo:
$$\int \sqrt{25-x^2}(-2x) dx = \int \sqrt{u} du = \int u^{1/2} du$$

$$= \frac{u^{3/2}}{3/2} + C = \frac{2u^{3/2}}{3} + C$$

Regresando a la variable original:
$$= \frac{2(25-x^2)^{3/2}}{3} + C$$

---

### Problema 2
$\displaystyle \int x^3(x^4+3)^2 dx$

**Solución:**

Sea $u = x^4 + 3$

Entonces $du = 4x^3 dx$, por lo que $x^3 dx = \frac{1}{4} du$

Sustituyendo:
$$\int x^3(x^4+3)^2 dx = \int (x^4+3)^2 \cdot x^3 dx = \int u^2 \cdot \frac{1}{4} du$$

$$= \frac{1}{4} \int u^2 du = \frac{1}{4} \cdot \frac{u^3}{3} + C = \frac{u^3}{12} + C$$

Regresando a la variable original:
$$= \frac{(x^4+3)^3}{12} + C$$

---

### Problema 3
$\displaystyle \int x^2(2x^3-1) dx$

**Solución:**

Expandiendo primero:
$$\int x^2(2x^3-1) dx = \int (2x^5 - x^2) dx$$

$$= \int 2x^5 dx - \int x^2 dx = 2 \cdot \frac{x^6}{6} - \frac{x^3}{3} + C$$

$$= \frac{x^6}{3} - \frac{x^3}{3} + C = \frac{x^3(x^3-1)}{3} + C$$

**Alternativa por cambio de variable:**

Sea $u = 2x^3 - 1$

Entonces $du = 6x^2 dx$, por lo que $x^2 dx = \frac{1}{6} du$

$$\int x^2(2x^3-1) dx = \int u \cdot \frac{1}{6} du = \frac{1}{6} \int u du = \frac{u^2}{12} + C$$

$$= \frac{(2x^3-1)^2}{12} + C$$

---

### Problema 4
$\displaystyle \int t\sqrt{t^2+2} dt$

**Solución:**

Sea $u = t^2 + 2$

Entonces $du = 2t dt$, por lo que $t dt = \frac{1}{2} du$

Sustituyendo:
$$\int t\sqrt{t^2+2} dt = \int \sqrt{u} \cdot \frac{1}{2} du = \frac{1}{2} \int u^{1/2} du$$

$$= \frac{1}{2} \cdot \frac{u^{3/2}}{3/2} + C = \frac{1}{2} \cdot \frac{2u^{3/2}}{3} + C = \frac{u^{3/2}}{3} + C$$

Regresando a la variable original:
$$= \frac{(t^2+2)^{3/2}}{3} + C$$

---

### Problema 5
$\displaystyle \int \frac{7x}{(1-x^2)^3} dx$

**Solución:**

Sea $u = 1 - x^2$

Entonces $du = -2x dx$, por lo que $x dx = -\frac{1}{2} du$

Sustituyendo:
$$\int \frac{7x}{(1-x^2)^3} dx = \int \frac{7}{u^3} \cdot \left(-\frac{1}{2}\right) du = -\frac{7}{2} \int u^{-3} du$$

$$= -\frac{7}{2} \cdot \frac{u^{-2}}{-2} + C = \frac{7u^{-2}}{4} + C = \frac{7}{4u^2} + C$$

Regresando a la variable original:
$$= \frac{7}{4(1-x^2)^2} + C$$

---

### Problema 6
$\displaystyle \int \frac{x}{\sqrt{1-x^2}} dx$

**Solución:**

Sea $u = 1 - x^2$

Entonces $du = -2x dx$, por lo que $x dx = -\frac{1}{2} du$

Sustituyendo:
$$\int \frac{x}{\sqrt{1-x^2}} dx = \int \frac{1}{\sqrt{u}} \cdot \left(-\frac{1}{2}\right) du = -\frac{1}{2} \int u^{-1/2} du$$

$$= -\frac{1}{2} \cdot \frac{u^{1/2}}{1/2} + C = -\frac{1}{2} \cdot 2u^{1/2} + C = -u^{1/2} + C$$

Regresando a la variable original:
$$= -\sqrt{1-x^2} + C$$

---

<!-- ## Resumen de la Técnica

El **cambio de variable** (sustitución) es útil cuando:

1. **Identificamos una función compuesta** $f(g(x))$ donde $g'(x)$ también aparece en el integrando
2. **Hacemos la sustitución** $u = g(x)$, entonces $du = g'(x) dx$
3. **Transformamos** toda la integral en términos de $u$
4. **Integramos** respecto a $u$
5. **Sustituimos de vuelta** $u = g(x)$ para obtener el resultado final

### Patrones Comunes

- Si vemos $(ax + b)^n$ y su derivada $a$, usar $u = ax + b$
- Si vemos $\sqrt{f(x)}$ y $f'(x)$, usar $u = f(x)$
- Si vemos $\frac{f'(x)}{f(x)}$, la integral es $\ln|f(x)| + C$
- Si vemos $f'(x) \cdot [f(x)]^n$, usar $u = f(x)$ -->