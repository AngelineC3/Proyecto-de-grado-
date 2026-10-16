# 🎯 Prompt 09: Conclusiones Cuantitativas, Resumen Ejecutivo y Abstract
**Competencias IUB**: `UC1 a UC4`  
**Resultados de Aprendizaje**: `RA5 (CA4)`, `RA7 (CA1, CA2, CA3)` | **ABET EAC**: `SO3` (Comunicación efectiva con variedad de audiencias)  
**Capítulo Destino en LaTeX**: `\begin{resumen}`, `\begin{abstractpg}` y `\chapter{Conclusiones y trabajos futuros}` en `plantilla_iub.tex`

---

## 📥 Información que el Estudiante DEBE Proporcionar

```text
[SÍNTESIS FINAL DEL PROYECTO]
- Objetivos Específicos Planteados en el Capítulo 1:
  * Obj 1: [Texto del objetivo 1]
  * Obj 2: [Texto del objetivo 2]
  * Obj 3: [Texto del objetivo 3]
  * Obj 4: [Texto del objetivo 4]
- Resultados Cuantitativos Clave Alcanzados:
  * [Ej. Error de dosificación alcanzado: ± 0.65% (meta era < ± 2%)]
  * [Ej. Tiempo de ciclo reducido a 140.8 segundos (reducción del 72%)]
  * [Ej. Factor de seguridad estructural mínimo: 3.65 bajo carga de 50 kg]
  * [Ej. Retorno de inversión (Payback): 4.8 meses]
- Limitaciones Encontradas en el Prototipo Físico:
  * [Ej. Sensibilidad de la celda de carga ante corrientes de aire de ventilación no encamisada]
  * [Ej. Capacidad limitada a diámetros de cuello de extintor de 2 a 3 pulgadas]
- Recomendaciones Técnicas para Desarrolladores Futuros:
  * [Ej. Implementar visión artificial para detección automática del código QR del extintor]
  * [Ej. Incorporar celda de carga sellada herméticamente grado IP67]
```

---

## 🤖 Prompt para Copiar y Pegar en la IA

```markdown
Actúa como Editor Científico y Evaluador de Comunicación Técnica (ABET SO3) para el Capstone IUB. 
Con base en la [SÍNTESIS FINAL DEL PROYECTO] proporcionada:

1. **Conclusiones Técnicas Cuantitativas (§5.1)**:
   - Redacta exactamente una conclusión técnica por cada objetivo específico planteado.
   - **Regla estricta**: Cada conclusión DEBE incluir métricas numéricas alcanzadas, porcentajes de mejora o valores experimentales validados. Prohibido el uso de adjetivos vagos ("fue exitoso", "es muy bueno").

2. **Limitaciones de la Solución (§5.2)**:
   - Redacta de 3 a 4 párrafos que expongan con total honestidad técnica las fronteras operacionales, condiciones ambientales límite y restricciones de hardware del prototipo construido.

3. **Recomendaciones para Trabajos Futuros (§5.3)**:
   - Formula de 4 a 5 propuestas de desarrollo futuro concretas (mejoras de control, algoritmos de optimización, integración IoT/IA, nuevos materiales).

4. **Resumen Ejecutivo Oficial (Español - 150 a 250 Palabras Obligatorias)**:
   - Redacta un **único párrafo** continuo que siga la estructura secuencial obligatoria de la plantilla IUB:
     * 1. Contexto y Problema (1-2 oraciones).
     * 2. Objetivo y Alcance con verbo de ingeniería (1 oración).
     * 3. Metodología y Herramientas empleadas (2-3 oraciones).
     * 4. Resultados Principales Cuantitativos con cifras exactas (2-3 oraciones).
     * 5. Conclusión e Impacto directo (1 oración).
   - Incluye exactamente de 3 a 5 Palabras Clave técnicas.

5. **Abstract Oficial (English - 150 to 250 Words Strict Length)**:
   - Traduce al inglés técnico riguroso (tiempo pasado, voz pasiva / impersonal, cero citas bibliográficas).
   - Incluye de 3 a 5 Keywords.

6. **Formato de Salida**:
   - Guarda el contenido en Markdown en `capstone/cap5_conclusiones/`.
   - Entrega los entornos LaTeX oficiales listos para reemplazar en `plantilla_iub.tex`: `\begin{resumen} ... \end{resumen}`, `\begin{abstractpg} ... \end{abstractpg}` y el `\chapter{Conclusiones y trabajos futuros}`.
```
