---
capitulo: 5
seccion: 5.1_conclusiones_cuantitativas
competencias: [UC1 a UC4]
ra_microcurriculo: [RA5-CA4, RA7-CA1]
abet_so: [SO3]
estado: borrador
---

# 5.1 Conclusiones Técnicas Cuantitativas (1 a 1 con Objetivos Específicos)

> **Regla de Oro Institucional**: Cada conclusión debe responder de manera numérica y directa a uno de los objetivos específicos formulados en el Capítulo 1.

1. **Frente al Objetivo 1 (Modelado y Simulación)**:  
   Se formuló y validó el modelo fluidodinámico y estructural del sistema, determinando un esfuerzo máximo de Von Mises de $68.4\text{ MPa}$ en la estructura de soporte bajo carga de $50\text{ kg}$, lo que arrojó un **Factor de Seguridad de 3.65** frente al límite de fluencia del acero A36 ($250\text{ MPa}$), garantizando integridad estructural ante sobrecargas accidentales.

2. **Frente al Objetivo 2 (Diseño Detallado y AMFE)**:  
   Se diseñó e integró la arquitectura mecatrónica de 4 subsistemas, seleccionando componentes comerciales con márgenes de seguridad superiores al $100\%$. La aplicación de la matriz AMFE permitió mitigar 4 modos de falla críticos, reduciendo el Número de Prioridad de Riesgo (NPR) promedio de $160.5$ a **$18.25$** mediante enclavamientos por software y hardware.

3. **Frente al Objetivo 3 (Implementación del Prototipo)**:  
   Se construyó un prototipo funcional a escala 1:1 con un costo total de fabricación de **$\$4,520,000\text{ COP}$**, integrando un inyector Venturi en acero inoxidable, celda de carga de $20\text{ kg}$, microcontrolador ESP32-S3 y pantalla HMI táctil con tiempos de respuesta en visualización menores a $50\text{ ms}$.

4. **Frente al Objetivo 4 (Validación Experimental y Evaluación Económica)**:  
   La validación experimental sobre $10$ ensayos demostró un error de repetibilidad en masa de **$\pm 0.207\%$** (error máximo de $+16\text{ g}$ en $4.54\text{ kg}$), cumpliendo holgadamente el requerimiento de diseño ($\le \pm 1.0\%$) y reduciendo el tiempo de ciclo a **$141.35 \pm 2.41\text{ s}$** ($72\%$ de mejora). La evaluación financiera demostró un retorno de inversión en **$4.02\text{ meses}$** con un VPN a 3 años de $\$24,180,000\text{ COP}$.
