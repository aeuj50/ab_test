# Proyecto de A/B Testing: Efectividad de un Nuevo Botón de Compra

## Introducción
Este proyecto se centra en evaluar la efectividad de un nuevo diseño de botón de compra para una tienda en línea mediante una prueba A/B. La versión experimental del botón (circular con un carrito de compras) fue comparada con la versión de control (rectangular con texto "BUY NOW") para determinar si la nueva versión incrementa significativamente la tasa de clics.

---

## Planteamiento del Problema
La empresa busca incrementar la participación del usuario, medida en clics, mediante un cambio en la interfaz de usuario (UX). Se establecieron las siguientes hipótesis:

- **Hipótesis Nula (\(H_0\))**: No hay diferencia significativa en la tasa de clics entre el grupo experimental y el de control.
- **Hipótesis Alternativa (\(H_1\))**: Hay una diferencia significativa en la tasa de clics entre los grupos.

---

## Metodología
1. **Definición de Parámetros**:
   - Poder de la prueba: 80%.
   - Nivel de significancia: 5%.
   - Efecto mínimo detectable (MDE): 10%.

2. **Carga y Exploración de Datos**:
   - **Variables clave**:
     - `user_id`: Identificador único del usuario.
     - `click`: Binaria, indica si el usuario hizo clic (1) o no (0).
     - `group`: Categoría, indica el grupo (control o experimental).
   - Tamaño de muestra total: 20,000 registros.

3. **Validación de Supuestos**:
   - **Normalidad**: Confirmada mediante el Teorema del Límite Central (tamaño de muestra grande).
   - **Independencia**: Garantizada por el diseño experimental (aleatorización y separación de grupos).
   - **Datos binarios**: Confirmado (valores 0 y 1 en la columna `click`).

4. **Prueba Estadística**:
   - Se utilizó una prueba paramétrica Z de dos muestras para comparar proporciones.
   - Estadístico Z calculado: \(-59.44\). Cae en la región de rechazo de la hipótesis nula.
   - Valor \(p\): \(0.0\) (menor a \(0.05\), nivel de significancia).

5. **Intervalo de Confianza**:
   - \(95\%\) IC: \([39.9\%, 42.6\%]\).
   - El intervalo está completamente por encima de \(0\), lo que confirma una mayor tasa de clics para el grupo experimental.

---

## Resultados
1. **Diferencia estadísticamente significativa**:
   - La prueba Z mostró que el grupo experimental tiene una tasa de clics significativamente mayor que el grupo de control.

2. **Significancia práctica**:
   - La diferencia validada excede el MDE del \(10\%\), demostrando relevancia práctica para la empresa.

3. **Efectividad del botón experimental**:
   - Tasa de clic promedio:
     - Grupo experimental: \(61.16\%\).
     - Grupo de control: \(19.89\%\).

---

## Recomendaciones
1. **Implementar el nuevo diseño del botón**:
   - La versión experimental ha demostrado ser más efectiva en captar clics.

2. **Monitorear resultados tras la implementación**:
   - Evaluar el impacto en métricas secundarias, como el número total de compras y el valor promedio de los pedidos.

3. **Explorar mejoras adicionales**:
   - Considerar combinaciones adicionales de diseño (colores, animaciones, ubicación).

4. **Ampliar el análisis**:
   - Extender el estudio a otras métricas clave para optimizar la experiencia del usuario.


---

## Autor
**Andrés Ulloa Jaramillo**

