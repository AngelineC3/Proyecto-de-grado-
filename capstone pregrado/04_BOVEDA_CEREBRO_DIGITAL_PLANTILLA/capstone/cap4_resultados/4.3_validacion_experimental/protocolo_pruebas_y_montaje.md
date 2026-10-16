---
capitulo: 4
seccion: 4.3.1_protocolo_pruebas_y_montaje
competencias: [UC2-EC3, UC4-EC3]
ra_microcurriculo: [RA5-CA1, RA5-CA2]
abet_so: [SO6]
estado: borrador
---

# 4.3.1 Protocolo de Pruebas y Montaje Experimental (ABET SO6)

> **Criterio ABET SO6**: Desarrollar y conducir una experimentación apropiada, analizar e interpretar datos, y usar el juicio de ingeniería para sacar conclusiones.

## 🔬 Protocolo Experimental Estandarizado

### 1. Condiciones Ambientales e Instrumentación
* **Ubicación de Ensayos**: Laboratorio de Mecatrónica / Taller de Prototipado IUB.
* **Temperatura y Humedad**: $28 \pm 2\text{ }^\circ\text{C}$, $65 \pm 5\%\text{ HR}$.
* **Presión de Red Neumática**: $6.0 \pm 0.2\text{ bar}$ regulada.
* **Instrumentos de Medición Patrón**:
  * Balanza digital patrón calibrada OHAUS Ranger 3000 (Resolución: 0.1 g, Incertidumbre: $\pm 0.2\text{ g}$).
  * Manómetro digital de precisión Fluke 700G (Rango: 0-10 bar, Precisión: $\pm 0.05\%\text{ F.S.}$).
  * Cronómetro digital de precisión certificado (Resolución: 0.01 s).

### 2. Definición de Variables Experimentales
* **Variables Independientes**: Tipo de cilindro (10 lbs y 20 lbs), Presión de suministro (5.0, 6.0, 7.0 bar).
* **Variables Dependientes**: Masa final dosificada ($m_{\text{real}}$), Tiempo de ciclo de recarga ($t_{\text{ciclo}}$), Fuga de presión ($\Delta P$).
* **Variables de Control**: Temperatura ambiente, granulometría del polvo PQS estándar, diámetro de manguera de eyección.

### 3. Procedimiento Secuencial de Ensayo
1. Tarar y calibrar a cero la celda de carga del prototipo y la balanza patrón externa.
2. Posicionar el cilindro en la estación de recarga y activar el ciclo de sujeción neumática.
3. Iniciar secuencia automática en la HMI y registrar el tiempo de ciclo cronometrado.
4. Finalizado el llenado, despresurizar y retirar el cilindro para pesaje de control en la balanza patrón.
5. Repetir el procedimiento $N = 10$ veces consecutivas bajo idénticas condiciones.
