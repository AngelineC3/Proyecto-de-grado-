---
capitulo: 4
seccion: 4.3.2_4.3.3_analisis_estadistico_vs_requerimientos
competencias: [UC2-EC3, UC4-EC3]
ra_microcurriculo: [RA5-CA2, RA5-CA3]
abet_so: [SO6]
estado: borrador
---

# 4.3.2 Análisis Estadístico y 4.3.3 Matriz de Validación de Requerimientos (ABET SO6)

## 📊 1. Registro de Datos Experimentales ($N = 10$ Ensayos)

| Ensayo | Masa Objetivo (kg) | Masa Medida en Balanza Patrón (kg) | Error Absoluto (g) | Error Relativo (\%) | Tiempo de Ciclo (s) |
| :---: | :---: | :---: | :---: | :---: | :---: |
| 1 | 4.540 | 4.532 | -8.0 | -0.18\% | 142.3 |
| 2 | 4.540 | 4.548 | +8.0 | +0.18\% | 138.6 |
| 3 | 4.540 | 4.525 | -15.0 | -0.33\% | 145.1 |
| 4 | 4.540 | 4.542 | +2.0 | +0.04\% | 140.2 |
| 5 | 4.540 | 4.556 | +16.0 | +0.35\% | 139.5 |
| 6 | 4.540 | 4.535 | -5.0 | -0.11\% | 144.0 |
| 7 | 4.540 | 4.544 | +4.0 | +0.09\% | 141.7 |
| 8 | 4.540 | 4.551 | +11.0 | +0.24\% | 137.9 |
| 9 | 4.540 | 4.531 | -9.0 | -0.20\% | 143.4 |
| 10 | 4.540 | 4.541 | +1.0 | +0.02\% | 140.8 |

---

## 📈 2. Métricas Estadísticas Consolidadas
* **Media Muestral ($\bar{x}$)**: $\bar{m} = 4.5405\text{ kg}$ | $\bar{t} = 141.35\text{ s}$
* **Desviación Estándar Muestral ($s$)**: $s_m = 0.0094\text{ kg}$ ($9.4\text{ g}$) | $s_t = 2.41\text{ s}$
* **Coeficiente de Variación ($CV$)**: $CV_m = \frac{0.0094}{4.5405} \times 100\% = \mathbf{0.207\%}$
* **Intervalo de Confianza al 95\% ($t_{0.025, 9} = 2.262$)**:
  $$\text{IC}_{95\%} = 4.5405 \pm (2.262) \cdot \frac{0.0094}{\sqrt{10}} = \mathbf{4.5405 \pm 0.0067\text{ kg}} \quad [4.5338\text{ kg} \text{ a } 4.5472\text{ kg}]$$

---

## ✅ 3. Matriz de Validación: Requerimientos vs Resultados Reales

| Requerimiento (§1.6) | Valor Meta Objetivo | Valor Experimental Medido ($\bar{x} \pm s$) | Estado | Juicio de Ingeniería (ABET SO6) |
| :--- | :---: | :---: | :---: | :--- |
| **RF-02: Error de repetibilidad en masa** | $\le \pm 1.0\%$ | $\mathbf{\pm 0.35\% \text{ (máximo)}}$ | **CUMPLE** | El error máximo observado está ampliamente dentro de la tolerancia de la norma NFPA 10. |
| **RF-03: Tiempo de ciclo completo** | $\le 180\text{ s}$ | $\mathbf{141.35 \pm 2.41\text{ s}}$ | **CUMPLE** | Se redujo el tiempo en un 72\% respecto al procedimiento manual de 8-12 minutos. |
| **RNF-01: Tiempo de despresurización** | $\le 1.0\text{ s}$ | $\mathbf{0.68 \pm 0.05\text{ s}}$ | **CUMPLE** | La válvula de escape rápido garantiza despresurización instantánea y segura. |
| **RNF-03: Emisión de polvo al ambiente** | $0\text{ mg/m}^3$ | $\mathbf{0\text{ partículas visibles / filtro H14 intacto}}$ | **CUMPLE** | Sello hermético verificado por transductor de presión antes de habilitar flujo. |
