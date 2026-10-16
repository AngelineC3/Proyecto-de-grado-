# 🎯 Prompt 03: Estado del Arte, Patentes, Normas y Autoformación SO7
**Competencias IUB**: `UC1-EC1`, `UC3-EC1`  
**Resultados de Aprendizaje**: `RA6 (CA1, CA2, CA3)`, `RA3 (CE1)` | **ABET EAC**: `SO7`, `SO4`  
**Capítulo Destino en LaTeX**: `\chapter{Estado del Arte y Estándares de Ingeniería}` (Capítulo 2 en `plantilla_iub.tex`)
**Ver también**: si aún no documentaste cómo seleccionaste tus fuentes, ejecuta antes [`Prompt_03b_Metodologia_Bibliometrica_y_Analisis_Bibliografico_RA6_RA3.md`](./Prompt_03b_Metodologia_Bibliometrica_y_Analisis_Bibliografico_RA6_RA3.md).

---

## 📥 Información que el Estudiante DEBE Proporcionar

```text
[FUENTES BIBLIOGRÁFICAS Y TECNOLÓGICAS]
- Artículos Científicos Clave (3 a 5 papers en tu carpeta raw/papers/):
  1. [Autor, Año, Título, Aporte técnico o método analizado]
  2. [Autor, Año, Título, Aporte técnico o método analizado]
  3. [Autor, Año, Título, Aporte técnico o método analizado]
- Patentes o Soluciones Comerciales (2 a 3 patentes en raw/):
  1. [Número de Patente / Fabricante, País, Mecanismo utilizado, Ventaja/Desventaja]
  2. [Número de Patente / Fabricante, País, Mecanismo utilizado, Ventaja/Desventaja]
- Normativa Técnica Identificada (en raw/normas_tecnicas/):
  * [Ej. ISO 12100 Seguridad de maquinaria, NFPA 10 Extintores portátiles, IEC 60204 Seguridad eléctrica, NTC 2885]
- Nuevo Conocimiento Adquirido de Forma Autónoma (Requisito ABET SO7):
  * [Tecnología / Software / Algoritmo que tuviste que estudiar por tu cuenta sin haberlo visto en clase previa, ej. Algoritmo YOLOv8, Simulación de fluidos en OpenFOAM, Protocolo Modbus TCP en microcontrolador ESP32]
  * [Cómo lo aprendiste: documentación oficial, cursos, papers, experimentos preliminares]
  * [Cómo se aplica directamente en tu diseño]
```

---

## 🤖 Prompt para Copiar y Pegar en la IA

```markdown
Actúa como Curador Científico y Evaluador ABET SO7 para el Capstone IUB. 
Con base en las [FUENTES BIBLIOGRÁFICAS Y TECNOLÓGICAS] suministradas:

1. **Introducción breve del Capítulo (§2.1)**:
   - Redacta un párrafo que introduzca el enfoque de la revisión tecnológica.

2. **Revisión de Soluciones Existentes y Patentes (§2.2)**:
   - Sintetiza las soluciones comerciales y patentes, destacando sus principios de operación, ventajas mecánicas/electrónicas y brechas no resueltas.

3. **Adquisición de Nuevo Conocimiento - Evidencia ABET SO7 (§2.3)**:
   - Redacta una subsección explícita que demuestre la competencia de autoformación:
     * Nombre de la tecnología/conocimiento adquirido de forma independiente.
     * Metodología de aprendizaje autónomo utilizada (revisión de manuales, experimentación preliminar).
     * Aplicación directa e impacto técnico en el desarrollo del proyecto.

4. **Estándares y Normativa Técnica Aplicable (§2.4 - ABET SO4)**:
   - Construye una tabla con las normas técnicas (ISO, IEEE, IEC, ASME, NTC) indicando: Código de norma, Título, Entidad emisora, y Cláusula / Requisito específico que se cumple en este diseño.

5. **Comparación Crítica Multicriterio (§2.5)**:
   - Genera una matriz de decisión multicriterio ponderada (con escala de 1 a 5) que compare:
     * Alternativa Comercial / Patente A.
     * Alternativa Comercial / Patente B.
     * Solución Propuesta en este Proyecto Capstone.
     * Criterios: Costo, Precisión/Tolerancia, Tiempo de ciclo, Seguridad del operador, Complejidad de mantenimiento.
   - Redacta el análisis cualitativo justificando la superioridad técnica y económica de la propuesta.

6. **Conclusión del Capítulo (§2.6)**:
   - Cierre sintético que resuma la oportunidad de diseño fundamentada en la literatura.

7. **Formato de Salida**:
   - Guarda el contenido en Markdown en `capstone/cap2_estado_del_arte/`.
   - Entrega el código LaTeX estructurado para `plantilla_iub.tex` incluyendo las citas en formato `\cite{...}` y la matriz comparativa en `tabularx`.
```
