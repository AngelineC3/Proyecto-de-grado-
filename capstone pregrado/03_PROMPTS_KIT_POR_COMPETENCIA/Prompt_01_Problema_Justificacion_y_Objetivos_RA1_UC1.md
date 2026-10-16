# 🎯 Prompt 01: Planteamiento del Problema, Justificación y Objetivos
**Competencias IUB**: `UC1-EC1`, `UC1-EC2`, `UC4-EC1`  
**Resultados de Aprendizaje**: `RA1 (CE1, CE2)`, `RA2 (CE1)` | **ABET EAC**: `SO1`, `SO2`  
**Capítulo Destino en LaTeX**: `\chapter{Introducción}` (§1.1, §1.2, §1.3 en `plantilla_iub.tex`)

---

## 📥 Información que el Estudiante DEBE Proporcionar

Copia este bloque, completa los datos entre corchetes y pégalo en tu IA junto con el prompt:

```text
[DATOS DEL PROYECTO]
- Título Preliminar: [Ej. Sistema Automatizado de Recarga de Extintores PQS]
- Sector Industrial / Entorno de Aplicación: [Ej. Industria de seguridad contra incendios en Barranquilla]
- Problema Actual / Fallo de Ingeniería: [Ej. El llenado manual genera exposición a polvo tóxico, variabilidad de masa ±15% y tiempos de ciclo de 12 minutos]
- Consecuencias de no resolverlo: [Ej. Riesgos de salud ocupacional, multas normativas, baja productividad]
- Solución Propuesta a Nivel Conceptual: [Ej. Máquina mecatrónica de dosificación por vacío/venturi con pesaje continuo y control PLC]
- Beneficiarios Directos: [Ej. Operarios de recarga, empresas certificadoras]
- Impactos Previstos: 
  * Técnico: [Ej. Reducción de variabilidad a < ±1%]
  * Económico: [Ej. Disminución del 60% en tiempo de ciclo]
  * Social/Ambiental: [Ej. Cero dispersión de partículas al aire mediante filtros HEPA]
```

---

## 🤖 Prompt para Copiar y Pegar en la IA

```markdown
Actúa como Asesor Metodológico y de Ingeniería para el Proyecto Capstone en la IUB. 
Con base en los [DATOS DEL PROYECTO] que te he proporcionado:

1. **Planteamiento del Problema (§1.1)**:
   - Redacta la descripción del problema en 3 párrafos técnicos impersonales (pasado/presente formal):
     * Párrafo 1: Contexto industrial y necesidad operativa real.
     * Párrafo 2: Brecha tecnológica y síntomas cuantitativos del fallo actual.
     * Párrafo 3: Formulación de la pregunta problema y sistematización del problema (3 sub-preguntas técnicas clave según el Microcurrículo IMD09).

2. **Justificación (§1.2)**:
   - Redacta las siguientes cuatro subsecciones con lenguaje formal de ingeniería:
     * 1.2.1 Importancia del problema (lo que está en juego).
     * 1.2.2 Beneficios esperados (técnicos, operativos y productivos).
     * 1.2.3 Relevancia académica o investigativa (articulación con el perfil del Ingeniero Mecatrónico IUB).
     * 1.2.4 Impacto social, económico o ambiental (considerando seguridad laboral y sostenibilidad).

3. **Objetivos (§1.3)**:
   - **Objetivo General**: Redacta 1 sola oración que inicie con un verbo en infinitivo de nivel taxonómico alto (diseñar, implementar, desarrollar, optimizar) que integre la solución, el mecanismo y el beneficio final.
   - **Objetivos Específicos**: Redacta exactamente 3 o 4 objetivos específicos ordenados cronológicamente:
     * Obj. 1: Diagnóstico / Levantamiento de requerimientos y modelado.
     * Obj. 2: Diseño detallado de subsistemas (mecánico, electrónico, control, software).
     * Obj. 3: Implementación / Prototipado y banco de pruebas.
     * Obj. 4: Validación experimental y evaluación técnico-económica.

4. **Formato de Salida**:
   - Entrega primero el contenido en Markdown limpio para guardar en mi bóveda (`capstone/cap1_introduccion/`).
   - Entrega luego el bloque de código en LaTeX listo para insertar en `plantilla_iub.tex` utilizando las secciones y entornos oficiales.
```
