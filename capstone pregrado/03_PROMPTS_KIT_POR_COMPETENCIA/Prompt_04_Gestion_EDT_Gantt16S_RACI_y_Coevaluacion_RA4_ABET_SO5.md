# 🎯 Prompt 04: Gestión del Proyecto, EDT, Gantt 16S y Matriz RACI
**Competencias IUB**: `UC1`, `UC2`, `UC4`  
**Resultados de Aprendizaje**: `RA4 (CA1, CA2, CA3, CA4)` | **ABET EAC**: `SO5` (Trabajo en equipo y liderazgo)  
**Capítulo Destino en LaTeX**: `\chapter{Gestión del Proyecto}` (Capítulo 3 en `plantilla_iub.tex`)

---

## 📥 Información que el Estudiante DEBE Proporcionar

```text
[DATOS DE GESTIÓN Y EQUIPO]
- Integrantes del Equipo:
  * Estudiante 1: [Nombre completo y rol principal, ej. Líder mecánico y simulación FEA]
  * Estudiante 2: [Nombre completo y rol principal, ej. Líder de control, electrónica y software]
- Metodología de Ingeniería: [Ej. Ciclo en V, Diseño Mecatrónico VDI 2206, Metodología Ágil Scrum]
- Fases Principales del Proyecto: [Ej. 1. Conceptualización, 2. Modelado y CAD, 3. Adquisición y Manufactura, 4. Integración y Pruebas, 5. Análisis y Documentación]
- Fechas de Inicio y Finalización: [Semana 1 a Semana 16]
- Recursos y Presupuesto Global Estimado: [Ej. $4,500,000 COP]
```

---

## 🤖 Prompt para Copiar y Pegar en la IA

```markdown
Actúa como Director de Proyectos de Ingeniería y Evaluador ABET SO5 para el Capstone IUB. 
Con base en los [DATOS DE GESTIÓN Y EQUIPO] suministrados:

1. **Metodología (§3.1)**:
   - Describe el enfoque metodológico de ingeniería aplicado (ej. VDI 2206 / Ciclo en V) detallando cada fase y entregables asociados.
   - Genera un diagrama de flujo en sintaxis Mermaid (`graph TD`) que muestre la secuencia de fases e iteraciones del proyecto.

2. **Planificación Detallada (§3.2 - ABET SO5)**:
   - **Estructura de Desglose del Trabajo (EDT / WBS)**: Diseña una jerarquía de 4 niveles (1. Proyecto Capstone -> 2. Fases -> 3. Paquetes de trabajo -> 4. Tareas específicas con código WBS 1.1.1, etc.).
   - **Cronograma de 16 Semanas**: Construye una tabla detallada con: Código WBS, Actividad, Semana de inicio, Semana de fin, Predecesoras, e Hito de entrega.
   - **Gestión de Riesgos del Proyecto**: Tabla con 4 riesgos técnicos/operativos identificando: Riesgo, Probabilidad (1-5), Impacto (1-5), Severidad, y Estrategia de Mitigación.

3. **Distribución de Funciones y Coevaluación (§3.3 - ABET SO5)**:
   - **Matriz RACI**: Construye una tabla que cruce las tareas principales de la WBS con los integrantes del equipo asignando: **R** (Responsable), **A** (Aprobador), **C** (Consultado), **I** (Informado).
   - **Matriz de Coevaluación de Equipo**: Formato cuantitativo de evaluación entre pares (criterios: asistencia, calidad técnica de entregables, cumplimiento de plazos, comunicación y resolución de conflictos) que evidencie el funcionamiento colaborativo del equipo.

4. **Formato de Salida**:
   - Guarda el contenido en Markdown en `capstone/cap3_gestion_proyecto/`.
   - Entrega el código LaTeX listo para insertar en `plantilla_iub.tex` utilizando tablas en `tabularx`.
```
