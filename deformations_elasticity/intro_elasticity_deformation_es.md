
---

# **Cuerpos Extensos y Deformaciones Axiales en Biomecánica**


## **Sección 1: Introducción a las Deformaciones Axiales**

Un **cuerpo extenso** es aquel cuya longitud no puede despreciarse al analizar su deformación bajo una carga. Las **cargas axiales** son fuerzas aplicadas a lo largo del eje longitudinal del cuerpo, generando dos tipos de esfuerzos:

- **Tracción**: Alargamiento del cuerpo.
- **Compresión**: Acortamiento del cuerpo.

**Ejemplos en biomecánica**:
- **Huesos largos** (fémur, tibia).
- **Tendones y ligamentos** sometidos a tracción.
- **Músculos** bajo carga axial.

---

## **Sección 2: Tensión y Deformación**

1. **Tensión ($\sigma$)**  
   La tensión es la fuerza por unidad de área en la sección transversal:  
   $$
   \sigma = \frac{N}{A}
   $$  
   Donde:  
   - $N$: Fuerza axial (N).  
   - $A$: Área de la sección transversal (m²).

2. **Deformación unitaria ($\varepsilon$)**  
   Es el cambio relativo en la longitud del cuerpo:  
   $$
   \varepsilon = \frac{\Delta L}{L_0}
   $$  
   Donde:  
   - $\Delta L$ Cambio de longitud (m).  
   - $L_0$: Longitud original (m).

3. **Ley de Hooke**  
   En la región elástica, tensión y deformación son proporcionales:  
   $$
   \sigma = E \cdot \varepsilon
   $$
   Donde $E$ es el **módulo de Young** (Pa), que mide la rigidez del material.

   La deformación unitaria también puede expresarse como la **derivada del desplazamiento**:  
   $$
   \varepsilon = \frac{du}{dx}
   $$

---

## **Sección 3: Ecuación de Equilibrio**

La ecuación de equilibrio para un cuerpo extenso sometido a cargas axiales es:  
$$
\frac{d}{dx} \left( EA \frac{du}{dx} \right) + q = 0
$$  
Donde:  
- $E$: Módulo de Young (Pa).  
- $A$: Área de la sección transversal.  
- $q$: Fuerza distribuida por unidad de longitud (N/m).

La solución de esta ecuación proporciona:  
- El **campo de desplazamiento** $u(x)$
- La **deformación**: $\varepsilon = \frac{du}{dx}$  
- La **tensión**: $\sigma = E \cdot \varepsilon$

---

## **Sección 4: Ejemplo de Aplicación**

### **Ejemplo 1: Barra homogénea sin carga distribuida**  
**Problema**: Una barra de longitud $L$, módulo de Young $E$, y sección constante $A$ está fijada en $x = 0$ y sometida a una fuerza $F$ en $x = L$.  

**Solución**:

1. **Ecuación de equilibrio**:  
   $$
   \frac{d}{dx} \left( EA \frac{du}{dx} \right) = 0
   $$  
   Integrando una vez:  
   $$
   EA \frac{du}{dx} = C_1
   $$  
2. **Integrando nuevamente**:  
   $$
   u(x) = \frac{C_1}{EA}x + C_2
   $$
3. **Aplicando condiciones de frontera**:  
   - $u(0) = 0$ $\implies$ $C_2 = 0$.  
   - En $x = L$, $EA \frac{du}{dx} = F \implies C_1 = F$.

   Solución final:  
   $$
   u(x) = \frac{F}{EA}x
   $$
4. **Deformación**:  
   $$
   \varepsilon = \frac{du}{dx} = \frac{F}{EA}
   $$
5. **Tensión**:  
   $$
   \sigma = E \cdot \varepsilon = \frac{F}{A}
   $$

---


## Sección 5: **Ejercicios Resueltos: Deformación y Elasticidad en Biomecánica**



## **Ejercicio 1**

**Enunciado**:  
Un campo de desplazamiento está dado como:  
$ u(x) = ax^2 + bx + c $  
donde $a$, $b$ y $c$ son constantes. Determina el campo de deformación $\varepsilon(x)$.

**Solución**:  
La deformación unitaria se calcula como la derivada del desplazamiento respecto a $x$:  
$$
\varepsilon(x) = \frac{du}{dx}
$$  
Derivando la función dada:  
$$
u(x) = ax^2 + bx + c
$$  
$$
\frac{du}{dx} = 2ax + b
$$  
Por lo tanto, el campo de deformación es:  
$$
\varepsilon(x) = 2ax + b
$$  

---

## **Ejercicio 2**

**Enunciado**:  
Un campo de deformación está dado como:  
$$ \varepsilon(x) = ax^2 + bx + c $$  
donde $a$, $b$ y $c$ son constantes. Determina el campo de desplazamiento $u(x)$ si $u(0) = 0$.

**Solución**:  
La deformación unitaria está relacionada con el desplazamiento mediante:  
$$
\varepsilon(x) = \frac{du}{dx}
$$  
Integrando con respecto a $x$:  
$$
\frac{du}{dx} = ax^2 + bx + c
$$  
$$
u(x) = \int (ax^2 + bx + c) dx
$$  
La integral es:  
$$
u(x) = \frac{a}{3}x^3 + \frac{b}{2}x^2 + cx + C
$$  
Aplicando la condición de frontera $$u(0) = 0 $$
$$
u(0) = \frac{a}{3}(0)^3 + \frac{b}{2}(0)^2 + c(0) + C = 0 \implies C = 0
$$  
Por lo tanto, el campo de desplazamiento es:  
$$
u(x) = \frac{a}{3}x^3 + \frac{b}{2}x^2 + cx
$$  

---

## **Ejercicio 3**

**Enunciado**:  
Una barra con módulo de Young $E$ y longitud $L$ está sujeta a una fuerza $F$ en $x = L$. La sección transversal es:  
$$
A(x) = A_0 e^{-\beta x}
$$  
donde $A_0$ es el área en $x = 0$ y $beta$ es una constante positiva. Determina:  

1. El campo de tensión $\sigma(x)$.  
2. El campo de desplazamiento $u(x)$.

### **Solución**:

1. **Cálculo de la tensión \(\sigma(x)\):**  
   La tensión se define como:  
   $$
   \sigma(x) = \frac{F}{A(x)}
   $$  
   Sustituyendo $A(x)$:  
   $$
   \sigma(x) = \frac{F}{A_0 e^{-\beta x}}
   $$  
   Simplificando:  
   $$
   \sigma(x) = F \cdot \frac{e^{\beta x}}{A_0}
   $$  

2. **Cálculo del desplazamiento $u(x)$:**  
   La ecuación de equilibrio para la barra es:  
   $$
   \frac{d}{dx} \left( EA(x) \frac{du}{dx} \right) = 0
   $$  
   Integrando una vez:  
   $$
   EA(x) \frac{du}{dx} = C_1
   $$  
   Sustituyendo \(A(x) = A_0 e^{-\beta x}\):  
   $$
   E A_0 e^{-\beta x} \frac{du}{dx} = C_1
   $$  
   Despejando \(\frac{du}{dx}\):  
   $$
   \frac{du}{dx} = \frac{C_1}{E A_0} e^{\beta x}
   $$  
   Integrando nuevamente:  
   $$
   u(x) = \frac{C_1}{E A_0 \beta} e^{\beta x} + C_2
   $$  
   Aplicando las condiciones de frontera:  
   - En \(x = 0\), \(u(0) = 0\):  
     $$
     u(0) = \frac{C_1}{E A_0 \beta} e^{0} + C_2 = 0 \implies C_2 = -\frac{C_1}{E A_0 \beta}
     $$  
   - En \(x = L\), la fuerza \(F\) se aplica:  
     $$
     \sigma(L) = E \frac{du}{dx} \bigg|_{x=L}
     $$  
     De aquí, se obtiene $C_1 = F$.

   Finalmente, el campo de desplazamiento es:  
   $$
   u(x) = \frac{F}{E A_0 \beta} \left( e^{\beta x} - 1 \right)
   $$  

---

## **Ejercicio 4**

**Enunciado**:  
Una barra de módulo de Young \(E\), área \(A\) y longitud \(L\) está sometida a una carga distribuida $q(x) = \alpha e^{\beta x}$. Determina:  
1. El campo de tensión $\sigma(x)\$.  
2. El campo de desplazamiento $u(x)$.

**Solución**:  

1. **Ecuación de equilibrio**:  
   $$
   \frac{d}{dx} \left( EA \frac{du}{dx} \right) = -q(x)
   $$  
   Sustituyendo \(q(x) = \alpha e^{\beta x}\):  
   $$
   \frac{d}{dx} \left( EA \frac{du}{dx} \right) = -\alpha e^{\beta x}
   $$  
   Integrando una vez:  
   $$
   EA \frac{du}{dx} = -\frac{\alpha}{\beta} e^{\beta x} + C_1
   $$  
   Despejando \(\frac{du}{dx}\):  
   $$
   \frac{du}{dx} = -\frac{\alpha}{\beta EA} e^{\beta x} + \frac{C_1}{EA}
   $$  
2. **Integración del desplazamiento**:  
   $$
   u(x) = -\frac{\alpha}{\beta^2 EA} e^{\beta x} + \frac{C_1}{EA}x + C_2
   $$  
   Aplicando las condiciones de frontera:  
   - $u(0) = 0$:  
     $$
     u(0) = -\frac{\alpha}{\beta^2 EA} e^{0} + C_2 = 0 \implies C_2 = \frac{\alpha}{\beta^2 EA}
     $$  
   - En $x = L$, se impone la carga o se ajusta según el problema.

   El resultado final es:  
   $$
   u(x) = -\frac{\alpha}{\beta^2 EA} \left( e^{\beta x} - 1 \right) + \frac{C_1}{EA}x
   $$  

---

## **Sección 6: Ejercicios Propuestos**

1. Una barra con **módulo de Young $E$** y longitud $L$ está sometida a una carga distribuida $q(x) = \alpha e^{\beta x}$. Determina:  
   - El desplazamiento $u(x)$.  
   - La tensión $\sigma(x)$.

2. Un tendón con módulo $E$ y sección constante $A$ está fijado en un extremo y sometido a una fuerza $F$. Calcula:  
   - La deformación.  
   - El desplazamiento en función de su longitud.

3. Modela un **músculo-tendón** como un sistema de dos barras:  
   - Músculo: longitud $L_1$, módulo $E_1$, sección $A_1$.  
   - Tendón: longitud $L_2$, módulo $E_2$, sección $A_2$

   Determina:  
   - El desplazamiento en el punto de unión.  
   - La tensión en cada barra.

4. Una barra suspendida bajo su propio peso tiene longitud $L$, densidad $\rho$ y sección $A$. Determina:  
   - El alargamiento total debido a la gravedad.

5. Una sección del **fémur** se modela como un tubo hueco con:  
   - Diámetro externo $D$, diámetro interno $d$, longitud $L$, y carga axial $P$.  

   Determina:  
   - La tensión $\sigma(x)$.  
   - El desplazamiento $u(x)$.

---

## **Conclusión**

El estudio de **cuerpos extensos y deformaciones axiales** es fundamental en biomecánica para entender cómo responden estructuras como huesos, tendones y músculos ante fuerzas aplicadas. Resolver estas ecuaciones permite predecir el comportamiento de los tejidos bajo diversas condiciones de carga.

---
