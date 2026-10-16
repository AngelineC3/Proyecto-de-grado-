---
capitulo: 5
seccion: 5.2_5.3_limitaciones_y_recomendaciones
competencias: [UC1, UC2, UC4]
ra_microcurriculo: [RA7-CA2]
abet_so: [SO3]
estado: borrador
---

# 5.2 Limitaciones de la Solución y 5.3 Recomendaciones para Trabajos Futuros

## 5.2 Limitaciones de la Solución Real
1. **Sensibilidad a Perturbaciones por Flujo de Aire Externo**: Durante las pruebas se identificó que corrientes de aire directas sobre el soporte del extintor introducían fluctuaciones de hasta $\pm 5\text{ g}$ en la celda de carga antes del filtrado digital.
2. **Compatibilidad Geométrica de Cilindros**: El mecanismo de acople rápido actual está dimensionado exclusivamente para cuellos de extintor de 2 a 3 pulgadas de diámetro exterior.
3. **Presión Mínima de Entrada Requerida**: Para lograr la tasa de succión nominal del inyector Venturi se requiere una presión de red estable mínima de $5.5\text{ bar}$.

---

## 5.3 Recomendaciones para Trabajos Futuros
1. **Integración de Visión Artificial (IA - YOLOv8)**: Implementar una cámara para el reconocimiento automático del código QR, año de fabricación y tara del extintor, precargando los parámetros de recarga sin intervención del usuario.
2. **Celda de Carga Hermética IP67 con Encapsulado Antivibratorio**: Incorporar una celda de carga con aislamiento mecánico completo para eliminar la necesidad de filtrado por software.
3. **Conectividad IoT en la Nube**: Desarrollar un módulo de telemetría MQTT para registrar cada ciclo de recarga en una base de datos institucional en la nube para auditoría y trazabilidad de calidad.
4. **Mecanismo de Mordaza Universal Autoajustable**: Diseñar un acople autocentrante con diafragma de nitrilo para admitir cualquier diámetro de cilindro sin cambio de herramental.
