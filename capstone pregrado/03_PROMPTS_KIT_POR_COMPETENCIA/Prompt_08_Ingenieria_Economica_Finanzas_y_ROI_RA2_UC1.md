# 🎯 Prompt 08: Ingeniería Económica, Presupuesto, Costos y ROI
**Competencias IUB**: `UC1`, `UC4`  
**Resultados de Aprendizaje**: `RA2 (CE4)` | **ABET EAC**: `SO2` (Consideraciones económicas y restricciones de costo)  
**Capítulo Destino en LaTeX**: `\chapter{Resultados}` -> `\section{Ingeniería económica y finanzas del proyecto}` (§4.4 en `plantilla_iub.tex`)

---

## 📥 Información que el Estudiante DEBE Proporcionar

```text
[DATOS ECONÓMICOS Y FINANCIEROS REALES]
- Moneda: [COP / USD]
- Costos de Materiales y Componentes Directos (Lista resumida con precios reales):
  * [Ej. Estructura y perfilería de aluminio: $450,000 COP]
  * [Ej. Actuadores neumáticos y electroválvulas: $850,000 COP]
  * [Ej. PLC / Microcontrolador y fuentes de poder: $620,000 COP]
  * [Ej. Celda de carga, display HMI y sensórica: $380,000 COP]
  * [Ej. Mecanizado en torno/fresadora y corte láser: $420,000 COP]
- Mano de Obra Estimada: [Ej. 120 horas de ingeniería/técnico a $25,000 COP/hora = $3,000,000 COP]
- Costos Indirectos y Margen de Contingencia (10%): [Ej. $272,000 COP]
- Ahorros o Beneficios Económicos Estimados para el Cliente/Empresa:
  * [Ej. Ahorro de $12,000 COP por extintor recargado gracias a menor merma de polvo y reducción de tiempo laboral de 12 min a 2.5 min]
  * [Ej. Volumen estimado de producción: 250 recargas/mes]
- Tasa de Descuento / Oportunidad (TIO): [Ej. 12% anual]
- Horizonte de Evaluación: [Ej. 3 a 5 años]
```

---

## 🤖 Prompt para Copiar y Pegar en la IA

```markdown
Actúa como Ingeniero de Costos y Evaluador de Proyectos Financieros (ABET SO2) para el Capstone IUB. 
Con base en los [DATOS ECONÓMICOS Y FINANCIEROS REALES] suministrados:

1. **Estructura de Costos del Prototipo / Sistema (§4.4.1)**:
   - Construye tablas detalladas en moneda local:
     * **Tabla 1: Costos Directos de Materiales y Equipos** (Ítem, Cantidad, Proveedor / Referencia, Costo Unitario, Costo Total).
     * **Tabla 2: Costos de Mano de Obra y Servicios de Manufactura** (Rol, Horas estimadas, Tarifa horaria, Subtotal).
     * **Tabla 3: Costos Indirectos, Consumibles y Contingencias (10%)**.
     * **Tabla Consolidada de Inversión Total del Proyecto (CAPEX)**.

2. **Costo Unitario de Fabricación y Escalamiento Industrial (§4.4.2)**:
   - Calcula el costo de fabricación por lote industrial (10-50 unidades), proyectando la reducción por compras a escala y optimización de tiempos de ensamble.

3. **Evaluación Financiera y Retorno de Inversión (§4.4.3)**:
   - Proyecta el flujo de caja neto mensual/anual considerando los ahorros operativos (OPEX) y el incremento de productividad.
   - Calcula:
     * **Período de Recuperación de la Inversión (Payback / PRI)** en meses: $\text{PRI} = \frac{\text{Inversión Inicial}}{\text{Ahorro Mensual Neto}}$.
     * **Valor Presente Neto (VPN / VAN)**: $\text{VAN} = \sum_{t=1}^n \frac{F_t}{(1+k)^t} - I_0$.
     * **Tasa Interna de Retorno (TIR)** y Relación Beneficio/Costo (B/C).
   - Redacta la conclusión económica justificando la viabilidad y atractivo del proyecto para la industria local.

4. **Formato de Salida**:
   - Guarda el borrador en Markdown en `capstone/cap4_resultados/4.4_finanzas/costos_capex_opex_y_retorno.md`.
   - Genera el código LaTeX correspondiente para `plantilla_iub.tex` utilizando tablas en `tabularx` con formato numérico monetario claro.
```
