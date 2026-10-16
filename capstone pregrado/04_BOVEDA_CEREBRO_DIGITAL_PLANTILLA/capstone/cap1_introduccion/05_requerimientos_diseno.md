---
capitulo: 1
seccion: 1.6_requerimientos_de_diseno
competencias: [UC1-EC1, UC2-EC1]
ra_microcurriculo: [RA2-CE1, RA2-CE2]
abet_so: [SO2]
estado: borrador
---

# 1.6 Requerimientos de Diseño y Restricciones de Ingeniería (ABET SO2)

> **Criterio ABET SO2**: Los requerimientos deben formularse con variables físicas medibles (valores numéricos y tolerancias) bajo restricciones realistas de ingeniería.

## 📊 Matriz de Requerimientos del Sistema

| Código | Tipo | Descripción del Requerimiento | Valor Objetivo / Tolerancia | Restricción Asociada (Económica / Seguridad / Ambiental / Normativa) |
| :---: | :--- | :--- | :---: | :--- |
| **RF-01** | Funcional | Rango de dosificación / capacidad de carga | 2.0 a 10.0 kg | Operación estándar en talleres de mantenimiento |
| **RF-02** | Funcional | Error de repetibilidad en masa final | $\le \pm 1.0\%$ | Cumplimiento de norma técnica de calidad |
| **RF-03** | Funcional | Tiempo máximo de ciclo completo | $\le 180 \text{ s}$ | Eficiencia y productividad operativa |
| **RNF-01** | Seguridad | Mecanismo de despresurización de emergencia | $\le 1.0 \text{ s}$ | Seguridad del operario (ISO 13849-1) |
| **RNF-02** | Ergonomía | Altura de la estación de carga de cilindros | $900 \pm 50 \text{ mm}$ | Normas ergonómicas laborales OSHA |
| **RNF-03** | Ambiental | Emisión de partículas al aire circundante | $0 \text{ mg/m}^3$ (Filtro H14) | Salud ocupacional y protección ambiental |
| **REST-01**| Económica | Presupuesto máximo de manufactura del prototipo | $\le \$4,500,000 \text{ COP}$ | Viabilidad financiera y fondos disponibles |
| **REST-02**| Eléctrica | Suministro de energía disponible en planta | $110\text{ VAC} \pm 10\%, 60\text{ Hz}$ | Red eléctrica convencional sin subestación |
| **REST-03**| Neumática | Presión de suministro de aire comprimido | $6.0 \pm 0.5\text{ bar}$ | Compresor de taller convencional |
