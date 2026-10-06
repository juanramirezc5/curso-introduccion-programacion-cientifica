# Retroalimentación — Taller evaluativo 01

**Estudiante:** Juan Manuel Ramírez Ciro · **Taller:** Taller evaluativo 01 — Python y estructuras de datos
**Fecha límite:** 2026-10-06 23:59 · **Versión revisada:** commit `e588609`

Excelente trabajo: el código de los nueve ejercicios es correcto y limpio.

## Nota

| Criterio | Puntos |
|---|---|
| Variables, tipos y operadores (Ej. 1 a 4) | 20 / 20 |
| Condicionales y clasificación (Ej. 5) | 15 / 15 |
| Bucles, acumuladores y control de flujo (Ej. 6 a 8) | 30 / 30 |
| Estructuras de datos nativas (Ej. 9) | 15 / 15 |
| Ejecución sin errores | 10 / 10 |
| Documentación en celdas de texto | 2 / 5 |
| Entrega correcta | 2 / 5 |
| **Total** | **94 / 100** |
| **Nota (0–5)** | **4.70** |

Este taller aporta **14.1 %** de los 15 % del momento evaluativo.

## 1. Variables, tipos y operadores (20 / 20)
**Lo que hizo bien:**
- Las siete variables del Ejercicio 1 tienen el tipo exacto y los verificó con `type()`.
- La conversión y los tres errores del Ejercicio 2 salen de operadores, no de valores escritos a mano.
- El Ejercicio 3 usa solo `//` y `%`; el Ejercicio 4 usa `and` y `not` sin ningún `if`.

## 2. Condicionales y clasificación (15 / 15)
**Lo que hizo bien:**
- La cadena `if` / `elif` / `else` va de menor a mayor umbral, cubre las cuatro categorías y da "Dañina para grupos sensibles" para 41.8.

## 3. Bucles, acumuladores y control de flujo (30 / 30)
**Lo que hizo bien:**
- Ejercicio 6: descarta los dos -999.0 con `continue` antes de acumular; quedan 10 lecturas y el promedio es 22.55.
- Ejercicio 7: máximo 58.3, mínimo 7.5, y la desviación con dos recorridos, sin `max()`, `min()` ni `sum()`.
- Ejercicio 8: el `while` actualiza `concentracion` dentro del bloque y termina (10 horas).

## 4. Estructuras de datos nativas (15 / 15)
**Lo que hizo bien:**
- Accede a cada dato por su clave, desempaqueta las coordenadas en `latitud` y `longitud` y usa `get` con "no disponible", sin errores.

## 5. Ejecución sin errores (10 / 10)
**Lo que hizo bien:**
- El notebook corre completo desde cero y la celda de verificación imprime el mensaje final.

## 6. Documentación en celdas de texto (2 / 5)
**Lo lograda:** los nombres de variables son claros y en `snake_case`.
**Lo que puede mejorar:**
- Las celdas previas a cada ejercicio solo dicen "EJERCICIO 1", "EJERCICIO 2", etc. No explican qué hace cada ejercicio. Cada una debe describir brevemente el problema y lo que se calcula.

## 7. Entrega correcta (2 / 5)
**Lo que hizo bien:** el notebook está en la carpeta `ejercicios/` de `main` y se entregó a tiempo.
**Lo que puede mejorar:**
- No siguió la convención de nombre: el archivo se llama `taller_evaluativo_01_calidad_del_aire.ipynb` y debía llamarse exactamente `taller-evaluativo-01-calidad-del-aire.ipynb` (con guiones, no guiones bajos).

## ¿El notebook funciona?
Sí. Corre completo sin errores, la celda de verificación imprime "Verificación completada sin errores." y los resultados coinciden con los esperados.

## Para el próximo taller
- Escriba en cada celda de texto una o dos frases que expliquen qué hace el ejercicio.
- Revise el nombre exacto del archivo antes de subirlo.
- Mantenga la práctica de calcular los resultados con operadores y bucles.
