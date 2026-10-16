# 📄 Entorno Oficial LaTeX — Capstone IUB

Esta carpeta contiene los archivos oficiales para la compilación y entrega final de tu documento de grado en formato PDF.

---

## 🚀 Cómo Compilar tu Documento

### Opción A: En Overleaf (Recomendado)
1. Comprime todos los archivos de esta carpeta (`plantilla_iub.tex`, `proyecto-grado.sty`, `referencias.bib` y la carpeta `logos/`) en un archivo `.zip`.
2. Ve a [overleaf.com](https://www.overleaf.com) y selecciona **"New Project" ➔ "Upload Project"**.
3. Sube el `.zip`.
4. En el menú de Overleaf, asegúrate de que el compilador esté configurado en **pdfLaTeX** o **XeLaTeX** con TeX Live actual.
5. Haz clic en **Recompile**.

### Opción B: En Distribución Local (VS Code + LaTeX Workshop / TeXstudio)
1. Abre `plantilla_iub.tex` en tu editor.
2. Compila con `pdflatex` ➔ `bibtex` ➔ `pdflatex` ➔ `pdflatex`.

---

## 📂 Archivos en esta Carpeta
* `plantilla_iub.tex`: Documento maestro con las secciones, tablas de contenido, resúmenes y capítulos.
* `proyecto-grado.sty`: Paquete de macros, tipografía, márgenes y entornos institucionales de la IUB.
* `referencias.bib`: Base de datos de citas bibliográficas BibTeX.
* `logos/`: Escudos y logotipos institucionales oficiales.
