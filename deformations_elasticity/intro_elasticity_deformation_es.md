# Análisis Elástico Unidimensional en Biomecánica

## Conceptos Clave y Ecuaciones

### 1. Esfuerzo y Deformación

En sistemas biomecánicos como tendones, músculos y huesos, el esfuerzo (σ) se define como fuerza por unidad de área:

```
σ = N/A
```

donde:
- N es la fuerza 
- A es el área transversal

La deformación (ε) se define como la derivada del campo de desplazamiento:

```
ε = du/dx
```

### 2. Relación Elástica Esfuerzo-Deformación

Para tejidos biológicos en su rango elástico:

```
σ = Eε
```

donde:
- E es el módulo de Young
- Esta relación es válida para pequeñas deformaciones

### 3. Ecuación de Equilibrio

Para un medio continuo unidimensional:

```
d/dx(EA du/dx) + q = 0
```

donde:
- q es la carga distribuida
- EA es la rigidez axial

## Ejemplos Resueltos

### Ejemplo 1: Análisis de un Tendón

Un tendón con módulo de Young E y longitud ℓ está fijo en x = 0 y cargado con una fuerza F en x = ℓ. La sección transversal varía según:

```
A(x) = A₀e^(-βx)
```

**Solución:**

1. Campo de esfuerzos:
   - Por equilibrio: N(x) = F
   - Por lo tanto: σ(x) = F/A(x) = F/(A₀e^(-βx)) = (F/A₀)e^(βx)

2. Campo de desplazamientos:
   - De la ley de Hooke: du/dx = σ/E = (F/EA₀)e^(βx)
   - Integrando y aplicando u(0) = 0:
   - u(x) = (F/EA₀β)(e^(βx) - 1)

### Ejemplo 2: Complejo Músculo-Tendón

Análisis de una unidad músculo-tendón con:
- Músculo: longitud ℓ₁, E₁, A₁
- Tendón: longitud ℓ₂, E₂, A₂

**Solución:**

1. Fuerzas internas:
   - Por equilibrio, la fuerza es constante = F

2. Esfuerzos:
   - Músculo: σ₁ = F/A₁
   - Tendón: σ₂ = F/A₂

3. Desplazamientos:
   - En el punto B: u(B) = Fℓ₁/(E₁A₁)
   - En el punto C: u(C) = Fℓ₁/(E₁A₁) + Fℓ₂/(E₂A₂)

## Problemas Propuestos

### 1. Análisis del Tendón de Aquiles

Considere el tendón de Aquiles como una barra uniforme con:
- Longitud L = 12 cm
- Área transversal A = 60 mm²
- Módulo de Young E = 1.2 GPa

Si se aplica una fuerza de 2000 N durante el salto, calcular:
- a) El esfuerzo en el tendón
- b) El alargamiento total
- c) La energía de deformación almacenada

### 2. Compresión de la Columna Vertebral

Un modelo simplificado de un cuerpo vertebral puede representarse como un cilindro con:
- Altura h = 20 mm
- Diámetro D = 30 mm
- E = 10 GPa

Bajo posición normal de pie, experimenta una fuerza de compresión de 400 N. Calcular:
- a) El esfuerzo de compresión
- b) La reducción de altura
- c) ¿Qué sucede con la deformación si el módulo disminuye en un 20% (como en la osteoporosis)?

### 3. Extensión de Fibra Muscular

Un haz de fibras musculares de longitud 10 cm tiene una sección transversal variable descrita por:
```
A(x) = A₀(1 - 0.2x/L)
```
donde A₀ = 2 mm². Si E = 0.5 MPa y se aplica una fuerza de 5 N:
- a) Encontrar la distribución de esfuerzos a lo largo de la fibra
- b) Calcular el esfuerzo máximo
- c) Determinar el alargamiento total

*Nota: Considere las restricciones fisiológicas en sus soluciones y discuta si los valores calculados están dentro de los rangos biológicos normales.*