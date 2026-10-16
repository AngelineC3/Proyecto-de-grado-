---
capitulo: 4
seccion: 4.4_ingenieria_economica
competencias: [UC1, UC4]
ra_microcurriculo: [RA2-CE4]
abet_so: [SO2]
estado: borrador
---

# 4.4 Ingeniería Económica, Costos y Finanzas del Proyecto (ABET SO2)

> **Criterio ABET SO2**: Aplicar diseño de ingeniería para producir soluciones considerando factores económicos y restricciones financieras.

## 💰 1. Estructura de Costos de Fabricación del Prototipo (CAPEX)

### Tabla 1: Costos Directos de Materiales y Equipos
| Ítem / Descripción | Cantidad | Proveedor / Referencia | Costo Unitario (COP) | Costo Total (COP) |
| :--- | :---: | :--- | :---: | :---: |
| Perfilería estructural de aluminio 40x40 mm y tornillería | 1 lote | Aluminios del Caribe | $420,000 | $420,000 |
| Cilindros neumáticos ISO $\phi 40$ y electroválvulas | 1 juego | Festo Distribuidor Local | $880,000 | $880,000 |
| Inyector Venturi en acero inoxidable mecanizado CNC | 1 unid | Mecanizados Barranquilla | $350,000 | $350,000 |
| Microcontrolador ESP32-S3 + Pantalla HMI Nextion 4.3" | 1 unid | Tienda Robótica / Importado | $320,000 | $320,000 |
| Celda de carga 20 kg + Transmisor HX711 blindado | 1 unid | Instrumentación Industrial | $145,000 | $145,000 |
| Gabinete eléctrico, protecciones termomagnéticas y cableado | 1 lote | Schneider Electric / Local | $280,000 | $280,000 |
| Filtros de aire lavables grado HEPA H14 | 2 unid | Soluciones Filtración | $160,000 | $160,000 |
| **Subtotal Materiales y Componentes Directos** | — | — | — | **$2,555,000** |

### Tabla 2: Mano de Obra, Indirectos e Inversión Total
| Concepto | Base de Cálculo | Subtotal (COP) |
| :--- | :--- | :---: |
| **Mano de Obra de Ingeniería y Ensamble** | 80 horas técnico/ingeniería a $20,000 COP/h | $1,600,000 |
| **Costos Indirectos y Consumibles de Taller** | Soldadura, brocas, lubricantes, energía | $150,000 |
| **Margen de Imprevistos y Contingencias (5\%)** | 5\% sobre costos directos | $215,000 |
| **INVERSIÓN TOTAL DE FABRICACIÓN (CAPEX)** | — | **$4,520,000 COP** |

---

## 📈 2. Análisis Financiero y Retorno de Inversión (ROI / Payback)
* **Ahorro Operativo Mensual (OPEX)**: En un taller con 250 recargas mensuales, la reducción de tiempo de mano de obra y la eliminación de merma genera un ahorro neto de **$1,125,000 COP/mes**.
* **Período de Recuperación Simple (Payback / PRI)**:
  $$\text{PRI} = \frac{\text{Inversión Inicial}}{\text{Ahorro Mensual}} = \frac{\$4,520,000}{\$1,125,000} = \mathbf{4.02 \text{ meses}}$$
* **Valor Presente Neto (VPN a 3 años, tasa TIO = 12\% anual)**: $\mathbf{VPN = \$24,180,000 COP}$
* **Tasa Interna de Retorno (TIR)**: $\mathbf{TIR = 215\% \text{ anual}}$

### Conclusión Financiera
El proyecto demuestra una alta viabilidad económica, recuperando la inversión total en **4 meses** y ofreciendo a los talleres locales una alternativa rentable frente a equipos importados que superan los $25,000,000 COP.
