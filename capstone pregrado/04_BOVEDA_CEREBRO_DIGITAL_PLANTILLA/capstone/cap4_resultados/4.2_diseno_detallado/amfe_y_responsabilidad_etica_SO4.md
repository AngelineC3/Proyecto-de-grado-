---
capitulo: 4
seccion: 4.2.4_amfe_y_responsabilidad_etica
competencias: [UC1, UC2, UC4]
ra_microcurriculo: [RA3-CE1, RA2-CE4]
abet_so: [SO4]
estado: borrador
---

# 4.2.4 Análisis de Modos y Efectos de Falla (AMFE) y Responsabilidad Ética (ABET SO4)

> **Criterio ABET SO4**: Reconocer responsabilidades éticas y profesionales en situaciones de ingeniería, considerando impactos globales, económicos, ambientales y sociales.

## 🛠️ Matriz AMFE / FMEA de Seguridad y Operación
* **S (Severidad)**: 1 a 10 | **O (Ocurrencia)**: 1 a 10 | **D (Detección)**: 1 a 10 | **NPR (Número de Prioridad de Riesgo) = S x O x D**

| Subsistema | Modo de Falla Potencial | Efecto de la Falla | Causa Potencial | S | O | D | NPR Inicial | Acción Preventiva Implementada | S | O | D | NPR Final |
| :--- | :--- | :--- | :--- | :---: | :---: | :---: | :---: | :--- | :---: | :---: | :---: | :---: |
| **Neumático** | Fuga de presión en acople de recarga | Emisión de polvo particulado al ambiente | Desgaste o desalineación del empaque O-ring | 7 | 4 | 5 | **140** | Enclavamiento de presurización: solo activa si transductor confirma sello hermético | 7 | 1 | 2 | **14** |
| **Sensórica** | Descalibración de celda de carga | Error en la masa dosificada (> ±2%) | Vibración continua del compresor | 8 | 5 | 4 | **160** | Montaje sobre silentblocks antivibratorios y filtro digital paso bajo en firmware | 8 | 2 | 2 | **32** |
| **Control** | Bloqueo o cuelgue del microcontrolador | Actuador queda energizado indefinidamente | Ruido electromagnético en la línea | 9 | 3 | 6 | **162** | Activación de temporizador Watchdog por hardware y relé térmico redundante | 9 | 1 | 2 | **18** |
| **Operación** | Acceso del operario a zona móvil | Atrapamiento de extremidades | Apertura indebida de compuerta | 9 | 4 | 5 | **180** | Sensor de seguridad magnético en compuerta que corta energía a válvulas | 9 | 1 | 1 | **9** |

---

## 🌍 Matriz de Responsabilidad Ética, Ambiental y Social
* **Salud y Seguridad en el Trabajo**: Eliminación del 100% del contacto directo del operario con polvo químico mediante cabina presurizada y filtros de extracción H14.
* **Sostenibilidad y Ciclo de Vida**: Uso de materiales 100% reciclables (aluminio A36 y policarbonato), y minimización del desperdicio de materia prima por merma a menos del 0.5%.
* **Cumplimiento Ético**: Verificación rigurosa de que la máquina opera bajo estándares de no riesgo de sobrepresión accidental, incorporando válvula de alivio calibrada a 8 bar.
