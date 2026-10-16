---
id: 202608301200
tipo: zettel
titulo: "Decisión de Diseño: Selección de Inyector Venturi vs Tornillo Sinfín"
tags: [decision-diseno, subsistema-mecanico, dosificacion]
estado: madura
enlaces: ["[[capstone/cap4_resultados/4.2_diseno_detallado/arquitectura_mecatronica_y_subsistemas]]"]
fuente: "Cálculos fluidodinámicos y pruebas de banco"
---

# Decisión de Diseño: Inyector Venturi vs Tornillo Sinfín

## 💡 Idea Central
Se seleccionó un sistema de eyección y transporte por efecto Venturi accionado por aire comprimido en lugar de un dosificador de tornillo sinfín motorizado.

## ⚙️ Contexto y Justificación Técnica
* El tornillo sinfín presenta fricción mecánica directa con el polvo PQS, generando atascamientos por aglomeración y desgaste acelerado de sellos mecánicos.
* El inyector Venturi no posee partes mecánicas móviles en contacto con el polvo químico, reduciendo el mantenimiento a cero y permitiendo una tasa de transferencia de $35\text{ g/s}$ a $6\text{ bar}$.

## 🔗 Conexiones
* [[capstone/cap4_resultados/4.1_modelado_y_simulacion/modelado_ecuaciones_y_simulaciones|Modelado de Presión en Garganta Venturi]]
* [[capstone/cap4_resultados/4.2_diseno_detallado/amfe_y_responsabilidad_etica_SO4|Modo de Falla por Desgaste de Sellos]]

## ❓ Preguntas Abiertas / Siguientes Pasos
* ¿Cuál es el diámetro óptimo de la boquilla inyectora para evitar turbulencias excesivas a presiones mayores a $7\text{ bar}$?
