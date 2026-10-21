# Retroalimentación — Taller evaluativo 02: Funciones y POO

**Estudiante:** Juan Manuel Ramírez Ciro · **Taller:** Taller evaluativo 02 — Funciones y POO
**Fecha límite:** 2026-10-21 00:00 · **Versión revisada:** commit `b62d4b3`

Excelente trabajo: el código funciona y todos los resultados coinciden con los esperados.

## Nota

| Criterio | Puntos |
|---|---|
| Funciones: parámetros, valores por defecto y retorno (Ej. 1 a 3) | 20 / 20 |
| `map`, `filter` y `lambda` (Ej. 4) | 10 / 10 |
| Clases, atributos y métodos (Ej. 5 y 7) | 15 / 15 |
| Encapsulamiento y validación (Ej. 6) | 15 / 15 |
| `__repr__` y `__str__` (Ej. 6 a 8) | 10 / 10 |
| Integración de funciones y clases (Ej. 8) | 10 / 10 |
| Ejecución sin errores | 10 / 10 |
| Documentación | 1 / 5 |
| Entrega correcta | 2 / 5 |
| **Total** | **93 / 100** |
| **Nota (0–5)** | **4.65** |

Este taller aporta **14.0 %** de los 15 % del momento evaluativo.

## 1. Funciones (20 / 20)
**Lo que hizo bien:**
- `calibrar_lectura` tiene los valores por defecto en la firma y usa `return`.
- `es_lectura_valida` clasifica bien -999.0, 600.0, 25.0 y 0.0.
- `promedio_valido` reutiliza `es_lectura_valida`, da 27.0 y devuelve `None` si no hay lecturas válidas.

## 2. `map`, `filter` y `lambda` (10 / 10)
**Lo que hizo bien:**
- Obtuvo 5 lecturas calibradas (de 11.5 a 61.9) y 2 excedencias, sin bucles `for`.

## 3. Clases, atributos y métodos (15 / 15)
**Lo que hizo bien:**
- `Lectura` guarda sus tres datos con valores por defecto y convierte bien de mg/m3 a ug/m3 (25.2).
- `Estacion` guarda objetos `Lectura` y `valores()` usa `a_microgramos()`.

## 4. Encapsulamiento y validación (15 / 15)
**Lo que hizo bien:**
- `Sensor` lanza `ValueError` con código vacío o pendiente menor o igual a cero, antes de guardar datos.
- `_pendiente` e `_intercepto` son internos y `calibrar` reutiliza `calibrar_lectura`.
- No dejó celdas de prueba que fallen.

## 5. `__repr__` y `__str__` (10 / 10)
**Lo que hizo bien:**
- Los textos de `Sensor`, `Estacion` e `InformeEstacion` coinciden exactamente con lo pedido.

## 6. Integración de funciones y clases (10 / 10)
**Lo que hizo bien:**
- `InformeEstacion` da 31.9 y "Moderada" reutilizando las funciones y el método `calibrar`.
- `categoria_pm25` usa una sola cadena `if` / `elif` / `else` y cubre las cuatro categorías.

## 7. Ejecución sin errores (10 / 10)
**Lo que hizo bien:**
- El notebook corre completo sin errores y la verificación imprime el mensaje final.

## 8. Documentación (1 / 5)
**Lo que hizo bien:**
- Cada ejercicio tiene una celda de texto previa que lo explica y los nombres siguen las convenciones.

**Lo que puede mejorar:**
- Ninguna función, clase ni método tiene docstring (la frase de una línea entre triples comillas al inicio). Era un requisito de todo el taller.

## 9. Entrega correcta (2 / 5)
**Lo que puede mejorar:**
- No siguió la estructura acordada: el nombre del archivo debe ser exactamente `taller-evaluativo-02-funciones-y-poo.ipynb` (con guiones). Usted lo subió como `taller_evaluativo_02_funciones_y_poo.ipynb` (con guiones bajos).
- Sí estaba en la carpeta `ejercicios/` y en la rama `main`, a tiempo.

## ¿El notebook funciona?
Sí. Corre completo sin errores, la celda de verificación imprime "Verificación completada sin errores." y los resultados coinciden con los esperados.

## Para el próximo taller
- Escriba un docstring de una línea en cada función, clase y método.
- Copie el nombre exacto del archivo que indica la guía, respetando los guiones.
- Antes de subir, revise la lista de requisitos de la guía uno por uno.
- Siga ejecutando "Reiniciar y ejecutar todas" antes de entregar, como lo hizo aquí.
