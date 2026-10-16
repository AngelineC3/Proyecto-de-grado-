---
capitulo: 4
seccion: 4.2.2_4.2.3_seleccion_componentes_y_planos
competencias: [UC1, UC2-EC2]
ra_microcurriculo: [RA2-CE3]
abet_so: [SO2]
estado: borrador
---

# 4.2.2 Selección de Componentes y 4.2.3 Planos de Ingeniería (ABET SO2)

## 📋 Matriz de Selección Técnica de Componentes Críticos

| Componente | Parámetro de Diseño Requerido | Componente Comercial Seleccionado | Capacidad Nominal de Catálogo | Margen de Seguridad / Justificación |
| :--- | :--- | :--- | :--- | :--- |
| **Cilindro Neumático de Sujeción** | Fuerza de apriete $F \ge 350\text{ N}$ a 6 bar | Cilindro ISO 15552 $\phi 40\text{ mm}$, carrera $100\text{ mm}$ | $F_{\text{teórica}} = 754\text{ N}$ | $FOS = 2.15$, asegura sujeción sin deslizamiento |
| **Celda de Carga** | Rango 0 a 10 kg con precisión $\le 5\text{ g}$ | Celda de carga tipo viga de aluminio | Capacidad 20 kg, no linealidad 0.02\% F.S. | Sobrecarga segura del 150\%, evita daño por impacto |
| **Fuente de Alimentación** | Consumo total pico $P = 78\text{ W}$ a 24VDC | Fuente Mean Well LRS-150-24 | 24VDC / 6.5A (156 W) | Sobredimensionada al 100\% para operación térmica fría |
| **Microcontrolador / PLC** | 12 E/S digitales, 2 ADC, bus I2C/SPI | Microcontrolador ESP32-S3 / PLC S7-1200 | 36 GPIOs, dual core 240 MHz | Capacidad de procesamiento y conectividad IoT |

---

## 📐 Planos de Ingeniería Normalizados (Anexos Oficiales)
* **Plano MEC-01**: Ensamble General Isométrico y Despiece de la Máquina.
* **Plano MEC-02**: Estructura de Soporte y Tolva de Dosificación.
* **Plano ELEC-01**: Esquema Unifilar y Distribución de Gabinete Eléctrico.
* **Plano NEUM-01**: Esquema Neumático de Potencia y Válvulas de Seguridad.
