# Retroalimentación — Taller evaluativo 03 (NumPy)

**Estudiante:** Juan Manuel Ramírez Ciro · **Taller:** Taller evaluativo 03 — NumPy
**Fecha límite:** 2026-10-30 23:59 · **Versión revisada:** commit `1585b0f`

¡Muy buen trabajo! Casi todo el taller está correcto.

## Nota

| Criterio | Puntos |
|---|---|
| Creación y atributos de arreglos (Ej. 1) | 10 / 10 |
| Indexación y slicing (Ej. 2) | 10 / 10 |
| Máscaras booleanas (Ej. 3) | 15 / 15 |
| Vectorización y broadcasting (Ej. 4) | 15 / 15 |
| Estadística por eje y funciones universales (Ej. 5 y 6) | 20 / 20 |
| Integración (Ej. 7) | 6 / 10 |
| Ejecución sin errores | 10 / 10 |
| Documentación | 5 / 5 |
| Entrega correcta | 2 / 5 |
| **Total** | **93 / 100** |
| **Nota (0–5)** | **4.65** |

Este taller aporta **14.0 %** de los 15 % del momento evaluativo.

## 1. Creación y atributos de arreglos (10 / 10)
**Lo que hizo bien:** creó `lecturas_crudas` con `np.array` y una lista de listas, leyó forma, dimensiones, tamaño y tipo desde sus atributos, y creó `dias`, `pendientes` e `interceptos` correctamente.

## 2. Indexación y slicing (10 / 10)
**Lo que hizo bien:** cada resultado sale de una sola expresión, usó el índice negativo para `ultimo_primer` y el bloque tiene forma (3, 4).

## 3. Máscaras booleanas (15 / 15)
**Lo que hizo bien:** `es_util` une las dos comparaciones con `&` y paréntesis, quedan 5 lecturas útiles, 2 faltantes y el promedio es 27.0, sin bucles.

## 4. Vectorización y broadcasting (15 / 15)
**Lo que hizo bien:** convirtió pendientes e interceptos en columnas (5, 1), `calibradas` da los valores esperados, explicó bien en texto por qué fallaba la multiplicación y el promedio calibrado de SBC-A es 31.9.

## 5. Estadística por eje y funciones universales (20 / 20)
**Lo que hizo bien:** los promedios por sensor y por día, los máximos y la media sobre 35.4 coinciden con lo esperado. Usó `np.maximum`, `np.abs` y `np.round`, y `en_alerta` es una copia con 8 celdas mayores que 0, sin alterar `calibradas`.

## 6. Integración (6 / 10)
**Lo que hizo bien:** los cuatro conteos (9, 18, 7 y 1) salen de máscaras, suman 35 y `dia_pico` es 5.
**Lo que puede mejorar:**
- Las dos líneas de salida no coinciden con el texto pedido: faltan los signos "=" y los dos puntos, y hay una palabra mal escrita ("coon") en la segunda línea.
- `dia_pico` se obtiene comparando con el máximo, no con una máscara sobre `promedio_por_dia` como se pedía, aunque el resultado es correcto.
**Cómo corregirlo:**
- Reescriba los dos `print` copiando el texto exacto de la guía, con "Buena=", "Moderada=", etc., y "Día más contaminado: 5 con 43.0 ug/m3".
- Cree una máscara sobre `promedio_por_dia` (por ejemplo, que sea igual al máximo) y úsela para filtrar `dias`.

## 7. Ejecución sin errores (10 / 10)
**Lo que hizo bien:** el notebook corre completo sin errores y la celda de verificación imprime el mensaje final.

## 8. Documentación (5 / 5)
**Lo que hizo bien:** cada ejercicio tiene su celda de texto previa y los nombres de variables siguen `snake_case` sin tildes.

## 9. Entrega correcta (2 / 5)
**Lo que hizo bien:** el notebook está en la carpeta `ejercicios/` de la rama `main` y se ve en GitHub.
**Lo que puede mejorar:**
- No siguió la estructura acordada: el nombre del archivo es `taller_evaluativo_03_numpy.ipynb` (con guiones bajos) y debía ser `taller-evaluativo-03-numpy.ipynb`.
- La celda de título no incluye la fecha.
**Cómo corregirlo:**
- Cambie el nombre del archivo en `ejercicios/` a `taller-evaluativo-03-numpy.ipynb`.
- Agregue la fecha en la celda de texto inicial.

## ¿El notebook funciona?
Sí. Corre completo sin errores, la celda de verificación imprime "Verificación completada sin errores." y los resultados coinciden con los esperados.

## Para el próximo taller
- Copie los textos de salida exactamente como los pide la guía.
- Use los nombres de archivo exactos indicados en la entrega.
- Siga la forma de resolver que pide cada instrucción (por ejemplo, usar una máscara para filtrar).
- Incluya siempre el título, su nombre y la fecha en la primera celda.
