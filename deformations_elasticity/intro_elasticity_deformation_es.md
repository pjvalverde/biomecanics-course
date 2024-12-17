
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

1. **Tensión (\(\sigma\))**  
   La tensión es la fuerza por unidad de área en la sección transversal:  

   ```math
   \sigma = \frac{N}{A}
   ```  
   Donde:  
   - \(N\): Fuerza axial (N).  
   - \(A\): Área de la sección transversal (m²).

2. **Deformación unitaria (\(\varepsilon\))**  
   Es el cambio relativo en la longitud del cuerpo:  

   ```math
   \varepsilon = \frac{\Delta L}{L_0}
   ```  
   Donde:  
   - \(\Delta L\): Cambio de longitud (m).  
   - \(L_0\): Longitud original (m).

3. **Ley de Hooke**  
   En la región elástica, tensión y deformación son proporcionales:  

   ```math
   \sigma = E \cdot \varepsilon
   ```  
   Donde \(E\) es el **módulo de Young** (Pa), que mide la rigidez del material.

   La deformación unitaria también puede expresarse como la **derivada del desplazamiento**:  

   ```math
   \varepsilon = \frac{du}{dx}
   ```

---

## **Sección 3: Ecuación de Equilibrio**

La ecuación de equilibrio para un cuerpo extenso sometido a cargas axiales es:  

```math
\frac{d}{dx} \left( EA \frac{du}{dx} \right) + q = 0
```  
Donde:  
- \(E\): Módulo de Young (Pa).  
- \(A\): Área de la sección transversal.  
- \(q\): Fuerza distribuida por unidad de longitud (N/m).

La solución de esta ecuación proporciona:  
- El **campo de desplazamiento** $u(x)$
- La **deformación**: $\varepsilon = \frac{du}{dx}$. 
- La **tensión**: $\sigma = E \cdot \varepsilon$.

---

## **Sección 4: Ejemplo de Aplicación**

### **Ejemplo 1: Barra homogénea sin carga distribuida**  
**Problema**: Una barra de longitud \(L\), módulo de Young \(E\), y sección constante \(A\) está fijada en \(x = 0\) y sometida a una fuerza \(F\) en \(x = L\).  

**Solución**:

1. **Ecuación de equilibrio**:  

   ```math
   \frac{d}{dx} \left( EA \frac{du}{dx} \right) = 0
   ```  
   Integrando una vez:  

   ```math
   EA \frac{du}{dx} = C_1
   ```  
2. **Integrando nuevamente**:  

   ```math
   u(x) = \frac{C_1}{EA}x + C_2
   ```  
3. **Aplicando condiciones de frontera**:  
   - $u(0) = 0$ $\implies$ $C_2 = 0$.
   - En $x = L$, $EA \frac{du}{dx} = F \implies C_1 = F$.

   Solución final:  

   ```math
   u(x) = \frac{F}{EA}x
   ```  
4. **Deformación**:  

   ```math
   \varepsilon = \frac{du}{dx} = \frac{F}{EA}
   ```  
5. **Tensión**:  

   ```math
   \sigma = E \cdot \varepsilon = \frac{F}{A}
   ```

---

## **Sección 5: Ejercicios Propuestos**

1. Una barra con **módulo de Young \(E\)** y longitud \(L\) está sometida a una carga distribuida \(q(x) = \alpha e^{\beta x}\). Determina:  
   - El desplazamiento \(u(x)\).  
   - La tensión \(\sigma(x)\).

2. Un tendón con módulo \(E\) y sección constante \(A\) está fijado en un extremo y sometido a una fuerza \(F\). Calcula:  
   - La deformación.  
   - El desplazamiento en función de su longitud.

3. Modela un **músculo-tendón** como un sistema de dos barras:  
   - Músculo: longitud \(L_1\), módulo \(E_1\), sección \(A_1\).  
   - Tendón: longitud \(L_2\), módulo \(E_2\), sección \(A_2\).

   Determina:  
   - El desplazamiento en el punto de unión.  
   - La tensión en cada barra.

4. Una barra suspendida bajo su propio peso tiene longitud \(L\), densidad \(\rho\) y sección \(A\). Determina:  
   - El alargamiento total debido a la gravedad.

5. Una sección del **fémur** se modela como un tubo hueco con:  
   - Diámetro externo \(D\), diámetro interno \(d\), longitud \(L\), y carga axial \(P\).  

   Determina:  
   - La tensión \(\sigma(x)\).  
   - El desplazamiento \(u(x)\).

---

## **Conclusión**

El estudio de **cuerpos extensos y deformaciones axiales** es fundamental en biomecánica para entender cómo responden estructuras como huesos, tendones y músculos ante fuerzas aplicadas. Resolver estas ecuaciones permite predecir el comportamiento de los tejidos bajo diversas condiciones de carga.

---