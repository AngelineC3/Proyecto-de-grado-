# 🎯 Prompt 05: Modelado Físico-Matemático y Simulación Numérica
**Competencias IUB**: `UC1-EC3`, `UC3-EC2`  
**Resultados de Aprendizaje**: `RA1 (CE3)` | **ABET EAC**: `SO1` (Matemáticas, ciencias e ingeniería para problemas complejos)  
**Capítulo Destino en LaTeX**: `\chapter{Resultados}` -> `\section{Modelado físico-matemático y simulación}` (§4.1 en `plantilla_iub.tex`)

---

## 📥 Información que el Estudiante DEBE Proporcionar

```text
[DATOS DE MODELADO Y SIMULACIÓN]
- Fenómeno Físico / Mecanismo Principal a Modelar: [Ej. Dinámica de flujo en inyector Venturi y esfuerzo en estructura de soporte de tolva de 50 kg]
- Leyes Físicas y Principios Aplicados: [Ej. Ecuación de Bernoulli, Conservación de Masa, Ecuaciones de Navier-Stokes, Criterio de Falla de Von Mises]
- Variables de Entrada, Parámetros y Constantes: [Ej. Presión de entrada P1 = 6 bar, Densidad del polvo rho = 1100 kg/m3, Diámetro garganta d2 = 8 mm, Material acero estructural A36 con Sy = 250 MPa]
- Software de Simulación Utilizado: [Ej. ANSYS Fluent para CFD, SolidWorks Simulation para FEA, MATLAB/Simulink para lazo de control]
- Resultados Numéricos Obtenidos de la Simulación: [Ej. Caída de presión calculada deltaP = 1.8 bar, Esfuerzo máximo de Von Mises = 68.4 MPa, Factor de Seguridad = 3.65]
```

---

## 🤖 Prompt para Copiar y Pegar en la IA

```markdown
Actúa como Ingeniero de Modelado Físico-Matemático y Simulación Avanzada (ABET SO1) para el Capstone IUB. 
Con base en los [DATOS DE MODELADO Y SIMULACIÓN] suministrados:

1. **Deducción de Ecuaciones Gobernantes (§4.1.1)**:
   - Presenta el marco teórico matemático formal:
     * Diagrama de cuerpo libre / Esquema del dominio físico con variables acotadas.
     * Deducción paso a paso de las ecuaciones analíticas gobernantes (dinámicas, cinemáticas, fluidodinámicas, térmicas o de optimización).
     * Tabla con la nomenclatura completa: Símbolo, Descripción, Unidades del Sistema Internacional (SI) y Valor numérico asignado.

2. **Parámetros de Simulación y Condiciones de Frontera (§4.1.2)**:
   - Documenta los parámetros del modelo computacional:
     * Tipo de mallado (número de elementos, tamaño de elemento, calidad ortogonal).
     * Condiciones de borde / frontera aplicadas (restricciones, cargas, presiones, temperaturas).
     * Propiedades mecánicas/físicas de los materiales seleccionados.

3. **Análisis de Resultados de Simulación y Validación Teórica (§4.1.3)**:
   - Compara los resultados calculados analíticamente vs los resultados obtenidos en la simulación numérica.
   - Calcula el porcentaje de error relativo: $\text{Error (\%)} = \frac{|V_{\text{analítico}} - V_{\text{simulado}}|}{V_{\text{analítico}}} \times 100\%$.
   - Concluye con el Factor de Seguridad (FOS) o margen de estabilidad del sistema, justificando la validez del dimensionamiento.

4. **Formato de Salida**:
   - Guarda el borrador en Markdown en `capstone/cap4_resultados/4.1_modelado/modelado_ecuaciones_y_simulaciones.md`.
   - Entrega el código LaTeX completo con todas las ecuaciones en entornos `\begin{equation} ... \label{eq:...} \end{equation}`, referencias cruzadas `\eqref{eq:...}` y tablas descriptivas en `tabularx`.
```
