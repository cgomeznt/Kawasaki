.. _prueba-estator-alternador:

=====
Prueba del Estator (Alternador) Kawasaki KLR650 (2013)  
=====

.. contents::  
   :depth: 3  
   :local:  

-----
**Herramientas Requeridas**  
-----

* Multímetro digital (con función Ω y AC Volt)  
* Destornillador de punta plana  
* Manual Kawasaki KLR650 2013 (valores de referencia)  

-----
**Preparación**  
-----

1. **Desconecte**:  
   - Terminal negativo de la batería.  
   - Conector de 3 cables del regulador/rectificador (ubicado cerca de la batería).  

2. **Acceso al Estator**:  
   - Retire la tapa plástica izquierda del motor.  
   - Localice el conector del estator (3 cables amarillos gruesos).  

-----
**Pruebas del Estator**  
-----

.. list-table:: Valores Esperados  
   :widths: 30 30  
   :header-rows: 1  

   * - **Parámetro**  
     - **Valor Normal**  
   * - Resistencia entre fases  
     - 0.1Ω - 0.5Ω  
   * - Voltaje AC (a 5,000 RPM)  
     - 50V - 80V por fase  

-----
**Procedimiento Paso a Paso**  
-----

Prueba 1: Resistencia entre Fases  
--------------------------------  

1. Configure el multímetro en **Ω (200Ω escala)**.  
2. Mida entre cada par de cables amarillos (A-B, A-C, B-C):  

   .. code-block:: none  

      Amarillo A ────┐  
      Amarillo B ────┼──► Multímetro  
      Amarillo C ────┘  

3. **Resultados**:  
   - Si la resistencia es **∞Ω**: Bobina abierta (reemplazar estator).  
   - Si es **<0.1Ω**: Cortocircuito interno.  

.. note::  
   La resistencia debe ser **similar en las 3 mediciones** (máx. 10% de variación).  

Prueba 2: Cortocircuito a Tierra  
--------------------------------  

1. Configure el multímetro en **Ω (2kΩ escala)**.  
2. Conecte una punta a **cualquier cable amarillo** y la otra al **chasis del motor**.  

.. danger::  
   Si el multímetro marca **<1MΩ**, hay fuga a tierra (estator dañado).  

Prueba 3: Voltaje AC de Salida  
------------------------------  

1. Configure el multímetro en **AC Volt (200V escala)**.  
2. Arranque el motor y mida entre cada par de cables (A-B, A-C, B-C) a **5,000 RPM**.  

.. image:: /path/to/estator_voltage_test.png  
   :width: 300  
   :align: center  

**Interpretación**:  
- Si el voltaje es **<50V por fase**: Estator defectuoso.  
- Si hay **desbalance >15%** entre fases: Bobina dañada.  

-----
**Síntomas de Fallo**  
-----

* **Batería no carga**: Aunque el regulador esté OK.  
* **Sobrecalentamiento**: Olor a quemado cerca del estator.  
* **Luces muy tenues**: Incluso con motor a altas RPM.  

-----
**Diagrama de Conexiones**  
-----

.. code-block:: none  

   Estator (3 fases)       Regulador/Rectificador  
   ┌──────────────┐        ┌───────────────────┐  
   │  Amarillo A  ├────────┤ Amarillo 1        │  
   │  Amarillo B  ├────────┤ Amarillo 2        │  
   │  Amarillo C  ├────────┤ Amarillo 3        │  
   └──────────────┘        └───────────────────┘  

-----
**Consejos Clave**  
-----

1. **Temperatura**: El estator funciona caliente, pero si quema el aislamiento es falla segura.  
2. **Inspección Visual**: Busque cables derretidos o manchas oscuras en las bobinas.  
3. **Reemplazo**: Use sólo estator OEM (ref: Kawasaki 21037-0451 para KLR650 2013).  


¿Cómo confirmar el diagnóstico?
Si todas las pruebas fallan: Estator dañado (reemplazar).

Si solo falla Prueba 2: Aislante dañado (fuga a tierra).

Si solo falla Prueba 3: Bobinas débiles (pérdida de eficiencia).

¿Necesitas el procedimiento para desmontar el estator o más detalles sobre las especificaciones eléctricas? ¡Avísame para complementar la información!

PD: Para motores con alta kilometraja, se recomienda esta prueba cada 20,000 km.
