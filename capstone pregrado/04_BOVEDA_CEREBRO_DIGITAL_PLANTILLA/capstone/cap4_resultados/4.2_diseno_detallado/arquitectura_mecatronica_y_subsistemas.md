---
capitulo: 4
seccion: 4.2.1_arquitectura_mecatronica
competencias: [UC1, UC2-EC2, UC3-EC3, UC4-EC2]
ra_microcurriculo: [RA2-CE3]
abet_so: [SO2]
estado: borrador
---

# 4.2.1 Arquitectura Mecatrónica y Desglose de Subsistemas (ABET SO2)

## 🖧 Diagrama de Bloques Funcional de la Solución

```mermaid
graph LR
    subgraph Potencia & Alimentacion
        P1[Red 110 VAC] --> P2[Fuente Switching 24VDC / 10A]
        P3[Compresor 6 bar] --> P4[Unidad FRL + Regulador]
    end

    subgraph Control & Procesamiento
        C1[Microcontrolador / PLC ESP32 / S7-1200]
        HMI[Pantalla Tactil HMI Nextion] <--> C1
    end

    subgraph Sensórica
        S1[Celda de Carga 20kg + HX711] --> C1
        S2[Transductor de Presión 0-10 bar] --> C1
        S3[Sensores Magnéticos de Posición] --> C1
    end

    subgraph Actuadores
        C1 --> A1[Electroválvulas Neumáticas 5/2]
        A1 --> A2[Cilindros de Sujeción y Válvula Venturi]
    end
```

## ⚙️ Descripción de Subsistemas
1. **Subsistema Mecánico y Estructural**: Chasis en perfilería de aluminio estructural 40x40 mm con cerramiento en acrílico transparente para contención de partículas.
2. **Subsistema Neumático**: Circuito de actuación con electroválvulas monoestables y biestables, válvula de escape rápido y sistema de eyección Venturi.
3. **Subsistema Eléctrico y Electrónico**: Cuadro eléctrico con protecciones termomagnéticas, parada de emergencia categoría 3 y aislamiento galvánico de señales analógicas.
4. **Subsistema de Control y Software/IA**: Máquina de estados finitos programada en C++/Structured Text, con lazo de dosificación por pesaje continuo y filtrado digital de ruido.
