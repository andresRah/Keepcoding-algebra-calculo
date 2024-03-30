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

---

## Ejercicio 3: Regresión Lineal - Mínimos Cuadrados

Este ejercicio evaluará tu habilidad para implementar el método de mínimos cuadrados para la regresión lineal en Python.

### Objetivos:
- Utilizar Python y Pandas para cargar y manipular datos.
- Comprender y aplicar los principios matemáticos detrás del método de mínimos cuadrados.

### Descripción del Problema:
Utilizando el conjunto de datos de precios de viviendas de Kaggle, desarrollarás un modelo de regresión que prediga el precio de una vivienda basado en su superficie habitable.

### Datos:
- El conjunto de datos de precios de viviendas de Kaggle (Kaggle's House Prices Dataset).

### Metodología:

Implementaremos la solución matricial del **método de mínimos cuadrados** para este problema de regresión. Los coeficientes \( w_{LS} \) se expresan como un vector y se calculan utilizando la matriz de entrada \( X \) y el vector de salida \( y \).

---

## Ejercicio 4: Regresión Lineal - Descenso de Gradiente

Este ejercicio aborda el problema de la regresión lineal utilizando el enfoque del Descenso de Gradiente, proporcionando una alternativa al método de los mínimos cuadrados.

### Objetivos:
- Comprender y aplicar los principios matemáticos detrás del Descenso de Gradiente.

### Descripción del Problema:
El objetivo es predecir el precio de las viviendas utilizando sus superficies habitables, empleando el conjunto de datos de precios de viviendas de Kaggle y el algoritmo del Descenso de Gradiente para ajustar el modelo de regresión.

### Datos:
- [Conjunto de datos de precios de viviendas de Kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)

### Conceptos Clave:

La función de pérdida que queremos minimizar es la Suma Residual de Cuadrados (RSS), definida como:

$$ RSS(w) = \frac{1}{2}\sum_{n=1}^{N}[y_n-f(x_n)]^2 $$

Donde:
- \( y_n \) son los valores reales.
- \( f(x_n) \) son las predicciones del modelo, expresadas como \( w_0 + \sum_{d=1}^{D}w_dx_{nd} \).

El objetivo es minimizar \( RSS(w) \) ajustando los parámetros del modelo \( w \), donde \( w_0 \) es el término de intercepción y \( w_d \) son los coeficientes de las características.

El gradiente de \( RSS(w) \), necesario para el Descenso de Gradiente, se calcula como:

$$ \nabla RSS(w) = X^T(Xw^t - y) $$

La actualización de los pesos en cada iteración del Descenso de Gradiente se realiza según la siguiente regla:

$$ w^{t+1} = w^t - \eta * \nabla RSS(w) $$

Donde \( \eta \) es la tasa de aprendizaje, un hiperparámetro que controla el tamaño del paso en cada iteración.

### Implementación:

Para implementar el Descenso de Gradiente en este contexto, se seguirán los siguientes pasos:
1. Inicializar los parámetros \( w \) aleatoriamente o con algún criterio específico.
2. Calcular el gradiente de \( RSS(w) \) usando la expresión dada.
3. Actualizar los parámetros \( w \) utilizando la regla de actualización.
4. Repetir los pasos 2 y 3 por un número definido de iteraciones o hasta que el cambio en \( RSS(w) \) sea menor que un umbral predefinido.

---



