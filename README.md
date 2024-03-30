# Keepcoding-algebra-calculo
Keepcoding Big Data Processing 

# Práctica Final: Big Data y Machine Learning

## Drawing

La práctica consiste en diversos ejercicios que abarcan conceptos y técnicas claves de Big Data y Machine Learning. Cada uno está diseñado para desafiarte y ayudarte a aplicar lo que has aprendido de manera práctica y efectiva.

### Ejercicio 1: Multiconjuntos

Este ejercicio prueba tu habilidad para resolver problemas utilizando vectores y fundamentos matemáticos de operaciones de conjuntos.

#### Objetivos:
- Utilizar Python para manejar estructuras de datos y librerías especializadas.
- Comprender y aplicar los fundamentos matemáticos detrás de las operaciones con multiconjuntos.

#### Descripción del Problema:
Deberás implementar las operaciones básicas de los multiconjuntos, tales como la inserción, eliminación, comparación y más, usando las estructuras de datos y librerías vistas en el curso.

#### Datos a tener en cuenta:
- Un **multiconjunto** es una colección de elementos donde se permiten repeticiones y cada elemento tiene una multiplicidad asociada.
- Operaciones como la cardinalidad, inserción, eliminación, comparación, pertenencia, subconjunto, unión, intersección y diferencia deben ser implementadas.

#### Ejemplo:
Para el multiconjunto `{a, a, b, b, b, c}`:
- **Cardinalidad**: La cantidad total de elementos contando multiplicidades, que es 6.
- **Inserción**: Agregar un nuevo elemento al multiconjunto.
- **Eliminación**: Remover un elemento del multiconjunto.
- **Comparación**: Determinar si dos multiconjuntos son iguales.
- **Pertenencia**: Verificar si un elemento está en el multiconjunto.
- **Subconjunto**: Chequear si todos los elementos de un multiconjunto están en otro.
- **Unión**: Combinar elementos de dos multiconjuntos sumando multiplicidades.
- **Intersección**: Encontrar elementos comunes con la menor multiplicidad.
- **Diferencia**: Restar los elementos de un multiconjunto de otro.

---

## Ejercicio 2: Descomposición en Valores Singulares (SVD)

Este ejercicio te reta a aplicar la Descomposición en Valores Singulares (SVD) para la compresión de imágenes. SVD es una técnica poderosa en la ciencia de datos, especialmente útil en el procesamiento de señales y la reducción de dimensionalidad.

### Objetivos:
- Usar Python para implementar SVD.
- Entender los principios matemáticos detrás de SVD y cómo puede ser utilizado para la compresión de datos.

### Descripción del Problema:
Deberás utilizar SVD para comprimir una imagen en blanco y negro, explorando cómo la reducción del número de valores singulares utilizados afecta la calidad de la imagen reconstruida.

### Datos a tener en cuenta:
- La SVD descompone una matriz en tres matrices: U, Σ (Sigma, una matriz diagonal con los valores singulares), y V^T.
- Los valores singulares en Σ representan la "importancia" de cada característica en los datos; valores más grandes significan características más importantes.
- Al descartar los valores singulares más pequeños (y sus vectores correspondientes), podemos aproximarnos a la matriz original con menos información, logrando así la compresión.

### Ejemplo:
Dada una imagen representada por una matriz \( A \), la descompones usando SVD:

\[ A = UΣV^T \]

Luego, seleccionas las \( k \) valores singulares más grandes para reconstruir una versión comprimida \( A_k \) de la imagen original:

\[ A_k = U_kΣ_kV_k^T \]

Donde \( U_k \), \( Σ_k \), y \( V_k^T \) son versiones reducidas de las matrices originales, conteniendo sólo las \( k \) columnas (para \( U \) y \( V^T \)) y \( k \) valores singulares (para \( Σ \)) más importantes.

Esta sección debería proporcionar instrucciones detalladas y ejemplos de cómo realizar la compresión de la imagen utilizando SVD en Python.

---


