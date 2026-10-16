# 🎯 Prompt 02: Alcances, Limitaciones y Requerimientos de Diseño
**Competencias IUB**: `UC1-EC1`, `UC2-EC1`  
**Resultados de Aprendizaje**: `RA1 (CE1)`, `RA2 (CE1, CE2)` | **ABET EAC**: `SO2`  
**Capítulo Destino en LaTeX**: `\chapter{Introducción}` (§1.4, §1.5, §1.6 en `plantilla_iub.tex`)

---

## 📥 Información que el Estudiante DEBE Proporcionar

```text
[DETALLES DE ALCANCE Y REQUERIMIENTOS]
- Frontera del Proyecto (Hasta dónde llega): [Ej. Diseño completo, simulación y construcción de un prototipo funcional a escala 1:1 para cilindros de 10 a 20 lbs]
- Qué NO cubre el proyecto: [Ej. No incluye certificación formal RETIE/UL, ni fabricación en serie industrial]
- Capacidades Funcionales Clave: [Ej. Capacidad de dosificación de 2 a 10 kg con resolución de 5 g, presión de trabajo de 6 bar]
- Restricciones Físicas y Ambientales: [Ej. Espacio máximo de 1.2 m x 0.8 m x 1.8 m, alimentación eléctrica monofásica 110/220 VAC, temperatura operativa 15 a 40 °C]
- Restricciones Económicas y Normativas: [Ej. Presupuesto límite de fabricación del prototipo de $4,500,000 COP, cumplimiento de norma NFPA 10 y NTC 2885]
```

---

## 🤖 Prompt para Copiar y Pegar en la IA

```markdown
Actúa como Ingeniero de Requisitos y Asesor de Diseño de Capstone IUB. 
Con base en los [DETALLES DE ALCANCE Y REQUERIMIENTOS] proporcionados:

1. **Alcances (§1.4)**:
   - Redacta de 4 a 6 viñetas precisas que delimiten exactamente las metas técnicas tangibles (entregables de ingeniería, modelos, prototipo y pruebas).

2. **Limitaciones (§1.5)**:
   - Redacta de 3 a 5 viñetas que establezcan los límites técnicos, operacionales y contextuales que no son cubiertos por el proyecto, justificando el motivo técnico de la exclusión.

3. **Requerimientos de Diseño (§1.6 - ABET SO2)**:
   - Estructura una tabla técnica exhaustiva dividida en:
     * **Requerimientos Funcionales (RF)**: Qué debe hacer el sistema (con métricas numéricas obligatorias: tolerancias, velocidades, flujos, presiones).
     * **Requerimientos No Funcionales (RNF)**: Seguridad, usabilidad, mantenibilidad, fiabilidad.
     * **Restricciones de Ingeniería Real**:
       - Económicas (presupuesto tope de fabricación).
       - Ambientales y de Salud (emisiones, ruido, ergonomía).
       - Normativas y Estándares (normas aplicables).
       - Fabricabilidad (materiales y procesos disponibles localmente).
       - Espacio y Alimentación energética.

4. **Formato de Salida**:
   - Genera el contenido en Markdown para la bóveda (`capstone/cap1_introduccion/04_alcances_y_limitaciones.md` y `05_requerimientos_diseno.md`).
   - Genera la tabla en sintaxis LaTeX utilizando el entorno `\begin{tablaCentrada}\begin{tabularx}{\textwidth}{...}` con columnas: `Código`, `Tipo`, `Descripción del Requerimiento`, `Valor / Métrica Objetivo`, `Restricción Asociada`.
```
