# 🎯 Prompt 06: Diseño Detallado, Selección de Componentes, AMFE y Ética
**Competencias IUB**: `UC1`, `UC2-EC2`, `UC3-EC3`, `UC4-EC2, EC3`  
**Resultados de Aprendizaje**: `RA2 (CE1-CE4)`, `RA3 (CE1)` | **ABET EAC**: `SO2`, `SO4` (Diseño bajo restricciones reales y ética)  
**Capítulo Destino en LaTeX**: `\chapter{Resultados}` -> `\section{Ingeniería de diseño detallado}` (§4.2 en `plantilla_iub.tex`)

---

## 📥 Información que el Estudiante DEBE Proporcionar

```text
[DATOS DE DISEÑO DETALLADO Y COMPONENTES]
- Arquitectura General del Sistema: [Ej. Diagrama de bloques que conecta Fuente 24VDC -> PLC S7-1200 / ESP32 -> Driver neumático -> Cilindros de sujeción -> Celda de carga 20kg con transmisor HX711 -> Interfaz HMI Nextion]
- Subsistema Mecánico: [Materiales seleccionados, mecanismos de transmisión, actuadores neumáticos Festo]
- Subsistema Eléctrico/Electrónico: [Sensores, acondicionamiento de señal, protecciones eléctricas termomagnéticas, relés de seguridad]
- Subsistema de Control y Software/IA: [Lógica de estados, lazo PID de llenado, algoritmo de detección de fugas]
- Modos de Falla Potenciales Identificados:
  1. [Falla: Fuga de presión en acople. Efecto: Llenado incompleto y emisión de polvo. Causa: Desgaste de empaque O-ring]
  2. [Falla: Descalibración de celda de carga. Efecto: Error de masa > 5%. Causa: Vibración mecánica continua]
  3. [Falla: Parada de emergencia manual presionada. Efecto: Despresurización segura sin expulsión de polvo]
- Medidas de Seguridad y Factores Ambientales: [Uso de paro de emergencia categoría 3 ISO 13849, filtros lavables grado HEPA H14, ergonomía según norma OSHA]
```

---

## 🤖 Prompt para Copiar y Pegar en la IA

```markdown
Actúa como Ingeniero de Integración Mecatrónica y Auditor de Seguridad y Ética (ABET SO2 + SO4) para el Capstone IUB. 
Con base en los [DATOS DE DISEÑO DETALLADO Y COMPONENTES] suministrados:

1. **Arquitectura del Sistema y Desglose por Subsistemas (§4.2.1)**:
   - Presenta la descripción técnica y diagramas de flujo de señales/energía para cada uno de los subsistemas:
     * Subsistema Mecánico y Estructural.
     * Subsistema Neumático / Hidráulico / Actuación.
     * Subsistema Eléctrico, Instrumentación y Sensórica.
     * Subsistema de Control, Lógica de Automatización y Software/IA.

2. **Selección Técnica Justificada de Componentes Críticos (§4.2.2)**:
   - Construye una tabla con la justificación ingenieril de los componentes seleccionados:
     * Componente, Fabricante / Modelo, Parámetro de Diseño Requerido, Capacidad Nominal Seleccionada, y Justificación Técnica del Margen de Seguridad.

3. **Planos y Documentación Técnica (§4.2.3)**:
   - Redacta el resumen de planos mecánicos normalizados y diagramas esquemáticos eléctricos/neumáticos que se adjuntan en los Anexos institucionales.

4. **Matriz AMFE / FMEA y Responsabilidad Ética y Ambiental (§4.2.4 - ABET SO4)**:
   - **Matriz AMFE**: Construye una tabla formal con columnas: `Subsistema`, `Modo de Falla Potencial`, `Efecto de la Falla`, `Causa Potencial`, `Severidad (S, 1-10)`, `Ocurrencia (O, 1-10)`, `Detección (D, 1-10)`, `Número de Prioridad de Riesgo (NPR = S x O x D)`, y `Acción Preventiva / Correctiva Implementada`.
   - **Impactos Globales, Sociales, Ambientales y de Seguridad**: Redacta 3 párrafos analizando los impactos éticos, la protección de la salud del operario y la gestión ambiental del ciclo de vida del equipo.

5. **Formato de Salida**:
   - Guarda el borrador en Markdown en `capstone/cap4_resultados/4.2_diseno/`.
   - Genera el código LaTeX correspondiente listo para compilar en `plantilla_iub.tex` utilizando tablas en `tabularx`.
```
