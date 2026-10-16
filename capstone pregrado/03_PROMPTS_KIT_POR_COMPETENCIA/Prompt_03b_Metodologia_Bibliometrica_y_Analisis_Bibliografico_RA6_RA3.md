# 🎯 Prompt 03b: Metodología de Bibliometría y Análisis Bibliográfico y de Referencias
**Competencias IUB**: `UC1-EC1`, `UC3-EC1`
**Resultados de Aprendizaje**: `RA6 (CA1, CA2, CA3)`, `RA3 (CE1)` | **ABET EAC**: `SO7`, `SO4`
**Capítulo Destino en LaTeX**: `\chapter{Estado del Arte y Estándares de Ingeniería}` — sección previa a §2.2 en `plantilla_iub.tex`
**Prerrequisito de**: [`Prompt_03_Estado_del_Arte_Patentes_Normas_y_SO7_RA6_RA3.md`](./Prompt_03_Estado_del_Arte_Patentes_Normas_y_SO7_RA6_RA3.md) — ejecuta este prompt **antes** de seleccionar las 3-5 fuentes finales de Prompt 03, para documentar cómo llegaste a ellas.

---

## 📥 Información que el Estudiante DEBE Proporcionar

```text
[DATOS DE BÚSQUEDA BIBLIOGRÁFICA]
- Pregunta / Objetivo de la revisión: [Ej. ¿Qué mecanismos de dosificación por venturi se han reportado para sistemas portátiles de extinción PQS?]
- Bases de Datos Consultadas: [Ej. Scopus, IEEE Xplore, ScienceDirect, Google Patents]
- Ecuación(es) de Búsqueda Booleana por base de datos:
  1. [Scopus]: [Ej. TITLE-ABS-KEY("venturi" AND "dry powder" AND "fire extinguisher")]
  2. [IEEE Xplore]: [Ej. ...]
- Filtros aplicados: [Rango de años, tipo de documento (article, conference paper, patent), idioma]
- Resultado bruto de la búsqueda (n.º de documentos por base de datos): [Ej. Scopus: 48, IEEE: 12]
- Criterios de Inclusión: [Ej. Trata explícitamente el mecanismo de dosificación; publicado 2015-2026; texto completo disponible]
- Criterios de Exclusión: [Ej. No es ingeniería mecatrónica; duplicado entre bases; solo resumen disponible]
- N.º de documentos tras cribado por título/resumen: [Ej. 22]
- N.º de documentos finales tras lectura completa: [Ej. 9]
- Gestor de Referencias Utilizado: [Zotero / Mendeley / JabRef] y archivo `.bib` asociado en `05_ENTORNO_LATEX_IUB/referencias.bib`
```

---

## 🤖 Prompt para Copiar y Pegar en la IA

```markdown
Actúa como Especialista en Bibliometría y Revisión Sistemática de Literatura para el Capstone de Ingeniería Mecatrónica IUB.
Con base en los [DATOS DE BÚSQUEDA BIBLIOGRÁFICA] suministrados:

1. **Protocolo de Búsqueda (§2.1a)**:
   - Redacta la metodología de búsqueda siguiendo un enfoque tipo PRISMA simplificado: pregunta de revisión, bases de datos, ecuaciones booleanas exactas por base, filtros y rango temporal.
   - No inventes cifras de resultados: usa únicamente los números que el estudiante reportó; si falta un dato, márcalo como `[DATO_PENDIENTE_DE_BUSQUEDA]`.

2. **Diagrama de Flujo de Selección Documental (§2.1b)**:
   - Genera un diagrama de flujo (identificación → cribado → elegibilidad → inclusión) con los conteos reales proporcionados, en formato Mermaid para el Markdown.
   - Para el LaTeX, represéntalo como una tabla `tablaCentrada`/`tabularx` de dos columnas (Etapa → Resultado): `plantilla_iub.tex` no carga el paquete `tikz`, así que un diagrama TikZ no compilará sin agregar esa dependencia; usa `\includegraphics` solo si el estudiante exporta el diagrama como imagen.

3. **Análisis Bibliométrico Descriptivo (§2.1c)**:
   - A partir de los documentos finalmente incluidos, construye una tabla con: `Año`, `Autor(es)`, `Fuente/Revista`, `País/Institución`, `Metodología`, `Hallazgo relevante para este proyecto`.
   - Identifica la distribución temporal de publicaciones (tendencia creciente/decreciente) y los autores/instituciones con mayor recurrencia.
   - Si el estudiante aporta un export de VOSviewer/Bibliometrix (co-ocurrencia de palabras clave o co-autoría), interpreta el mapa: clústeres temáticos principales y su relación con el problema de diseño.

4. **Síntesis Crítica y Brecha de Investigación (§2.1d)**:
   - Redacta un párrafo de síntesis que conecte los hallazgos bibliométricos con la brecha de diseño que este proyecto capstone busca cerrar. Evita afirmaciones subjetivas; fundamenta cada frase en los conteos y hallazgos reales.

5. **Gestión de Referencias**:
   - Verifica que cada documento incluido tenga una entrada BibTeX correspondiente en `05_ENTORNO_LATEX_IUB/referencias.bib`; señala cuáles faltan.
   - Genera las llamadas `\cite{...}` correctas para insertarlas en el texto de §2.2 (Prompt 03).

6. **Formato de Salida**:
   - Guarda el contenido en Markdown en `capstone/cap2_estado_del_arte/00_metodologia_bibliometrica.md`.
   - Entrega el código LaTeX estructurado para insertarlo como sección previa a §2.2 en `plantilla_iub.tex`, incluyendo la tabla en `tabularx` y el diagrama de flujo.
   - No redactes aún la síntesis cualitativa de soluciones existentes: eso lo hace `Prompt_03`. Este prompt solo entrega la metodología y el análisis bibliométrico de las fuentes ya filtradas.

7. **Reglas de compatibilidad LaTeX (validadas contra `plantilla_iub.tex`)**:
   - Usa únicamente macros definidas en `proyecto-grado.sty`: `tablaCentrada`, `tablaEncabezado`, `tablaHeader`. No uses `\fuenteTablaProyecto`, `\captionTablaProyecto` ni `\graficoProyecto`: son macros locales que algunos estudiantes (p. ej. el ejemplo de extintores) definen en su propio preámbulo, pero no existen en la plantilla en blanco.
   - Para el tamaño de fuente de la tabla usa `\small` (o ninguno). Para el pie de tabla usa `\captionof{table}{...}` seguido de `\label{...}` (el paquete `caption` ya está cargado por `proyecto-grado.sty`), no un wrapper personalizado.
   - En encabezados o celdas con palabras compuestas por `/` (p. ej. "País/Institución"), usa `\slash` en vez de `/` literal: en columnas angostas en negrita, `/` no permite salto de línea y puede desbordar el margen (`Overfull \hbox`).
   - En celdas de columnas angostas usa el marcador corto `[PENDIENTE]` en vez de `[DATO_PENDIENTE_DE_BUSQUEDA]` completo (reserva la forma larga para el Markdown/prosa); el texto completo es una cadena sin espacios que no se puede partir y desborda columnas de `tabularx` menores a ~0.15\textwidth.
```
