# 🎯 Prompt 07: Protocolo de Pruebas, Validación Experimental y Estadística
**Competencias IUB**: `UC2-EC3`, `UC4-EC3`  
**Resultados de Aprendizaje**: `RA5 (CA1, CA2, CA3)` | **ABET EAC**: `SO6` (Experimentación, análisis de datos y juicio de ingeniería)  
**Capítulo Destino en LaTeX**: `\chapter{Resultados}` -> `\section{Implementación y validación experimental}` (§4.3 en `plantilla_iub.tex`)

---

## 📥 Información que el Estudiante DEBE Proporcionar

```text
[DATOS EXPERIMENTALES Y DE PRUEBAS REALES]
- Descripción del Banco de Pruebas / Montaje Físico: [Ej. Montaje del prototipo en el taller de mecatrónica con línea de aire comprimido a 6 bar, balanza patrón calibrada OHAUS de 0.1 g de resolución y cronómetro digital]
- Variable Evaluada 1: [Ej. Masa de polvo dosificada (Objetivo: 4.54 kg / 10 lbs, Tolerancia máxima permitida: ± 2%)]
  * Datos Medidos en 10 Ensayos (kg): [4.53, 4.55, 4.52, 4.54, 4.56, 4.53, 4.54, 4.55, 4.53, 4.54]
- Variable Evaluada 2: [Ej. Tiempo de ciclo de recarga completo (Objetivo: < 180 segundos)]
  * Datos Medidos en 10 Ensayos (s): [142, 138, 145, 140, 139, 144, 141, 137, 143, 140]
- Fallas o Comportamientos Anómalos Observados: [Ej. En el ensayo 3 se observó ligera oscilación en la lectura por vibración del compresor, mitigada con filtro digital de promedio móvil]
```

---

## 🤖 Prompt para Copiar y Pegar en la IA

```markdown
Actúa como Ingeniero de Ensayos y Analista Estadístico de Datos Experimentales (ABET SO6) para el Capstone IUB. 
Con base en los [DATOS EXPERIMENTALES Y DE PRUEBAS REALES] suministrados:

1. **Protocolo y Diseño Experimental (§4.3.1)**:
   - Describe el procedimiento estandarizado de pruebas:
     * Condiciones ambientales y de operación (presión, voltaje, temperatura).
     * Instrumentación utilizada con marca, modelo, rango de medición e incertidumbre instrumental.
     * Definición de variables: Independientes, Dependientes y Variables de Control.
     * Secuencia paso a paso del ensayo para garantizar repetibilidad.

2. **Procesamiento de Datos y Análisis Estadístico Riguroso (§4.3.2 - ABET SO6)**:
   - Calcula para cada conjunto de datos experimentales:
     * Media muestral ($\bar{x}$).
     * Desviación estándar muestral ($s$).
     * Varianza ($s^2$) y Coeficiente de Variación ($CV = \frac{s}{\bar{x}} \times 100\%$).
     * Error relativo porcentual frente al valor objetivo o nominal.
     * Intervalo de confianza al 95\%: $\bar{x} \pm t_{\alpha/2, n-1} \frac{s}{\sqrt{n}}$.
   - Presenta los resultados en una tabla estadística consolidada.

3. **Matriz de Validación: Requerimientos vs Resultados Experimentales (§4.3.3)**:
   - Construye una tabla comparativa con columnas:
     * `Requerimiento de Diseño (§1.6)` | `Valor Meta Requerido` | `Valor Experimental Medido (Media ± s)` | `Error / Desviación` | `Estado (CUMPLE / NO CUMPLE)` | `Juicio Técnico de Ingeniería`.

4. **Discusión de Resultados y Curvas de Comportamiento (§4.3.4)**:
   - Redacta el análisis crítico explicando la física detrás de las variaciones observadas y cómo se optimizó el sistema.

5. **Formato de Salida**:
   - Guarda el borrador en Markdown en `capstone/cap4_resultados/4.3_pruebas/`.
   - Genera el código LaTeX correspondiente para `plantilla_iub.tex` utilizando tablas en `tabularx` y ecuaciones estadísticas debidamente referenciadas.
```
