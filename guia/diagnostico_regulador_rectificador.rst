.. _diagnostico_regulador_rectificador:

=====
Diagnóstico del Regulador/Rectificador  
Kawasaki KLR650 (2013)  
=====

.. contents::  
   :depth: 3  
   :local:  

-----
**Herramientas Requeridas**  
-----

* Multímetro digital  
* Manual de servicio Kawasaki KLR650 2013 (para valores de referencia)  
* Destornillador de punta plana  

-----
**Preparación**  
-----

1. **Condiciones**:  
   - Motor en **temperatura normal de operación** (después de 10 minutos de funcionamiento).  
   - Batería **cargada al 100%** (12.8V - 13.2V en reposo).  

2. **Desconecte**:  
   - Terminal negativo de la batería para evitar cortocircuitos.  

-----
**Pruebas Eléctricas**  
-----

.. list-table:: Valores Esperados (Referencia)  
   :widths: 30 30 30  
   :header-rows: 1  

   * - **Prueba**  
     - **Condición**  
     - **Valor Normal**  
   * - Voltaje de carga  
     - Motor a 5,000 RPM  
     - 13.5V - 15.0V  
   * - Resistencia (Diodos)  
     - Motor apagado  
     - 0.3Ω - 0.7Ω (polaridad directa)  
     - ∞Ω (polaridad inversa)  

-----
**Procedimiento Paso a Paso**  
-----

Prueba 1: Voltaje de Salida  
---------------------------  

1. Conecte el multímetro en **DC Volt (20V escala)**.  
2. Conecte:  
   - Cable **rojo** al terminal positivo (+) de la batería.  
   - Cable **negro** al terminal negativo (-).  
3. Arranque el motor y acelere hasta **5,000 RPM**.  

.. warning::  
   Si el voltaje supera **15.5V**, el regulador está **defectuoso** (sobrecarga).  
   Si es inferior a **13.5V**, hay falla en el rectificador o alternador.  

Prueba 2: Continuidad de Diodos  
-------------------------------  

1. Desconecte el conector de 3 cables del regulador/rectificador.  
2. Configure el multímetro en **Ω (resistencia)**.  

+------------------+---------------------+---------------------+  
| **Cable**        | **Prueba (+ a -)**  | **Resultado OK**    |  
+==================+=====================+=====================+  
| Amarillo 1       | Multímetro en Ω     | 0.3Ω - 0.7Ω         |  
+------------------+---------------------+---------------------+  
| Amarillo 2       | Invierta puntas     | ∞Ω (sin continuidad)|  
+------------------+---------------------+---------------------+  

.. note::  
   Repita para los 3 cables amarillos (fases del alternador).  

Prueba 3: Cortocircuito a Tierra  
--------------------------------  

1. Coloque una punta en **cable amarillo** y otra en **chasis**.  
2. Valor esperado: **∞Ω** (sin continuidad).  

.. danger::  
   Si hay continuidad (0Ω), el rectificador está **en corto** y debe reemplazarse.  

-----
**Síntomas de Fallo**  
-----

* **Batería sobrecargada**: Líquido electrolítico hirviendo.  
* **Batería descargada**: Motor no arranca después de pocos días.  
* **Luces intermitentes**: Exceso o falta de voltaje.  
* **Olor a quemado**: Sobrecalentamiento del regulador.  

-----
**Diagrama de Conexiones (Referencia)**  
-----

.. code-block:: none

   Alternador       Regulador/Rectificador       Batería  
   ┌─────┐            ┌──────────────┐          ┌─────┐  
   │ 3x  ├────────────►│ 3x Amarillo  ├─────────►│  +  │  
   │Amar │            │              │          │     │  
   └─────┘            └──────┬───────┘          └─────┘  
                             │  
                             ▼  
                           Chasis (Tierra)  

-----
**Notas Finales**  
-----

1. **Temperatura**: El regulador debe estar **caliente al tacto** (normal), pero no quemando.  
2. **Conexiones**: Verifique oxidación en terminales (limpíe con lija fina si es necesario).  
3. **Reemplazo**: Use **partes OEM Kawasaki** (ref: 21066-0004 para KLR650 2013).  

