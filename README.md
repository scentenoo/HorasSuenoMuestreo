# 😴 Estimación del promedio de horas de sueño en estudiantes de Ecuaciones Diferenciales

Proyecto del curso **Muestreo Estadístico (3006933)** — Universidad Nacional de Colombia, Sede Medellín — Semestre 2026-1.

**Docente:** Raúl Pérez
**Integrantes:** Gerson Bayona Aro · Samir Centeno

---

## 🎯 Objetivo

Estimar el promedio poblacional de horas de sueño por noche (μ) de los **1130 estudiantes** matriculados en Ecuaciones Diferenciales, mediante **Muestreo Aleatorio Simple (MAS) sin reemplazo**, con una confiabilidad del 95 % y un margen de error máximo admisible de 0,5 horas.

## 🧭 Diseño muestral

| Parámetro | Valor |
|---|---|
| Población (N) | 1130 estudiantes |
| Marco muestral | Listado oficial del coordinador de la asignatura |
| Diseño | MAS sin reemplazo (no se pudieron construir estratos: el marco no incluía grupo/horario) |
| Parámetro de interés | μ = horas de sueño promedio por noche |

## 🔢 Cálculo del tamaño de muestra

- Se calculó primero con un supuesto conservador de variabilidad (S = 1,5 h, regla rango/4) → **n = 34**.
- Se hizo un piloto de 9 respuestas efectivas que arrojó una variabilidad real menor (S ≈ 0,858 h), lo que hubiera permitido un n = 12.
- **Decisión final: se mantuvo n = 34** por criterio conservador (el piloto era una base pequeña para fijar S de forma definitiva) y porque la recolección ya estaba en marcha.

## 📊 Resultados principales

| Estimador | Valor |
|---|---|
| Media muestral (ȳ) | **5,62 horas por noche** |
| Varianza muestral (S²) | 0,713 |
| Error estándar | 0,1426 h |
| **IC 95 % para μ** | **[5,33 ; 5,91] horas** |
| Margen de error logrado | 0,29 h (mejor que el 0,5 h exigido) |
| Total poblacional estimado (τ) | ≈ 6347,9 horas/noche (IC 95%: [6020,1 ; 6675,8]) |

La precisión lograda superó la exigida: el margen de error real (0,29 h) fue menor al máximo admisible (0,5 h).

## 🔍 Análisis por dominios de interés

Se exploró la relación entre las horas de sueño y variables auxiliares (número de materias, horas de estudio autónomo, si trabaja, sexo, etc.):

- **Número de materias** y **horas de estudio autónomo** fueron los factores más asociados con menos horas de sueño (correlaciones negativas de ≈ -0,5 y -0,4).
- Estudiantes con 5-6 materias matriculadas duermen en promedio **1 hora menos** que quienes tienen 3-4 (4,75 h vs 5,88 h).
- Sentirse descansado correlaciona fuertemente (≈0,6) con dormir más, como es esperable.
- **Sexo** y **condición laboral** casi no explican diferencias en horas de sueño (correlaciones cercanas a 0).
- **Conclusión:** la carga académica pesa más que la condición laboral o el sexo al explicar cuánto duermen los estudiantes.

## 🛠️ Metodología de recolección

- Formulario digital (Google Forms) enviado a estudiantes sorteados aleatoriamente del marco muestral.
- Manejo de no-respuesta mediante reemplazo con nuevos sorteos.
- Limpieza de datos: respuestas en rango (ej. "4 a 5") codificadas a su punto medio; valores faltantes estructurales tratados como NA (no como no-respuesta).

## 📁 Contenido de este repositorio

- Presentación completa con la documentación del diseño, cálculo de tamaño de muestra, trabajo de campo, estimación y análisis por dominios.

## 🎓 Líneas de trabajo futuro

- Ampliar el estudio a otras asignaturas y semestres.
- Comparar subgrupos con muestras más grandes (sexo, programa, condición laboral).
- Usar escalas estandarizadas de calidad del sueño en vez de autodeclaración.
- Replicar el estudio en distintos semestres para evaluar estabilidad temporal.

---

*Universidad Nacional de Colombia — Sede Medellín · Departamento de Estadística*
