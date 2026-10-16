---
capitulo: 4
seccion: 4.1_modelado_fisico_matematico_y_simulacion
competencias: [UC1-EC3, UC3-EC2]
ra_microcurriculo: [RA1-CE3]
abet_so: [SO1]
estado: borrador
---

# 4.1 Modelado Físico-Matemático y Simulación Numérica (ABET SO1)

> **Criterio ABET SO1**: Aplicar conocimientos de matemáticas, ciencias e ingeniería para resolver problemas complejos de ingeniería.

## 4.1.1 Deducción de Ecuaciones Gobernantes
<!-- Presenta el marco teórico matemático analítico -->
El comportamiento del sistema está gobernado por las siguientes ecuaciones fundamentales:

1. **Conservación de Masa y Cantidad de Movimiento**:
   $$\dot{m} = \rho \cdot A \cdot v = \text{constante}$$

2. **Ecuación de Bernoulli Modificada (con pérdidas)**:
   $$P_1 + \frac{1}{2}\rho v_1^2 + \rho g z_1 = P_2 + \frac{1}{2}\rho v_2^2 + \rho g z_2 + \Delta P_{\text{fricción}}$$

3. **Criterio de Falla de Von Mises (Esfuerzo Equivalente)**:
   $$\sigma_v = \sqrt{\frac{1}{2} \left[ (\sigma_1 - \sigma_2)^2 + (\sigma_2 - \sigma_3)^2 + (\sigma_3 - \sigma_1)^2 \right]}$$

### Tabla de Nomenclatura y Parámetros del Modelo
| Símbolo | Parámetro Físico | Valor Numérico | Unidades SI |
| :---: | :--- | :---: | :---: |
| $\rho$ | Densidad del fluido / material | [Valor] | $\text{kg/m}^3$ |
| $P_1$ | Presión de suministro de aire | [Valor] | $\text{Pa}$ |
| $A$ | Área transversal de paso | [Valor] | $\text{m}^2$ |
| $S_y$ | Límite de fluencia del material | [Valor] | $\text{MPa}$ |

---

## 4.1.2 Parámetros y Configuración de Simulación Numérica
* **Software utilizado**: [SolidWorks Simulation / ANSYS Fluent / MATLAB Simulink]
* **Tipo de Análisis**: [Estático lineal / CFD multifásico / Dinámica transitoria]
* **Propiedades del Mallado**: [Número de nodos, tamaño de elemento, calidad ortogonal]
* **Condiciones de Frontera**: [Cargas aplicadas, presiones de entrada/salida, apoyos fijos]

---

## 4.1.3 Validación Teórica: Analítico vs Simulado
| Variable Física Evaluada | Valor Analítico Calculado | Valor Obtenido en Simulación | Error Relativo (\%) | Factor de Seguridad (FOS) |
| :--- | :---: | :---: | :---: | :---: |
| **Esfuerzo Máximo ($\sigma_{\text{max}}$)** | [Valor] MPa | [Valor] MPa | [Error]\% | **[FOS]** (Meta: $\ge 2.5$) |
| **Caída de Presión ($\Delta P$)** | [Valor] bar | [Valor] bar | [Error]\% | — |
