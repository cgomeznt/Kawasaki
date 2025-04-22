.. _prueba-bobina-encendido:

=====
Prueba de la Bobina de Encendido Kawasaki KLR650 (2013)  
=====

.. contents::  
   :depth: 3  
   :local:

-----
**Datos Técnicos de Referencia**  
-----

.. list-table:: Especificaciones Oficiales  
   :widths: 30 30  
   :header-rows: 1  

   * - **Parámetro**  
     - **Valor**  
   * - Resistencia Primaria  
     - 0.1Ω - 0.3Ω  
   * - Resistencia Secundaria  
     - 4.5kΩ - 6.5kΩ  
   * - Tensión de Trabajo  
     - 12V DC  

-----
**Herramientas Requeridas**  
-----

* Multímetro digital (precisión 1%)  
* Llave Torx T25 (para retirar bobina)  
* Guantes dieléctricos (opcional)  

-----
**Ubicación y Acceso**  
-----

1. **Posición**:  
   - Debajo del tanque de combustible  
   - Montada en chasis frontal del motor  

2. **Identificación**:  
   - Cables:  
     * Primario: Negro/Amarillo (+) y Verde (Tierra)  
     * Secundario: Cable grueso a bujía  

-----
**Procedimiento de Prueba**  
-----

Prueba 1: Resistencia del Devanado Primario  
-------------------------------------------

1. Desconectar terminales de la bobina  
2. Configurar multímetro en **Ω (200Ω escala)**  
3. Medir entre terminales **Negro/Amarillo (+) y Verde (-)**  

.. warning::  
   Valor fuera de 0.1Ω-0.3Ω indica:  
   * Cortocircuito (<0.1Ω)  
   * Apertura (>0.3Ω)  

Prueba 2: Resistencia del Devanado Secundario  
---------------------------------------------

1. Retirar cable de bujía  
2. Configurar multímetro en **kΩ (20k escala)**  
3. Medir entre:  
   * Terminal central (bujía)  
   * Terminal positivo (Negro/Amarillo)  

.. image:: /path/to/bobina_secundaria_test.png  
   :width: 200  
   :align: center  

**Criterio**:  
- 4.5kΩ-6.5kΩ → OK  
- ∞Ω → Bobina abierta  

Prueba 3: Aislamiento a Tierra  
------------------------------

1. Configurar multímetro en **MΩ (20M escala)**  
2. Medir entre:  
   * Cualquier terminal de bobina  
   * Chasis del motor  

.. danger::  
   Si la lectura es **<1MΩ**: Fuga de corriente (aislamiento dañado)  

-----
**Prueba Dinámica con Motor**  
-----

1. Conectar bujía de prueba (gap ajustado a 6mm)  
2. Arrancar motor y observar chispa:  

.. list-table:: Interpretación  
   :widths: 40 40  
   :header-rows: 1  

   * - **Chispa**  
     - **Diagnóstico**  
   * - Azul intenso  
     - Bobina OK  
   * - Amarilla/débil  
     - Fallo secundario  
   * - Ausente  
     - Fallo primario o CDI  

-----
**Tabla de Fallos Comunes**  
-----

+----------------------+---------------------+---------------------+  
| **Síntoma**         | **Causa Probable**  | **Solución**        |  
+======================+=====================+=====================+  
| Motor no arranca    | Apertura en primario| Reemplazar bobina   |  
+----------------------+---------------------+---------------------+  
| Aceleración pobre   | Resistencia alta    | Verificar conexiones|  
+----------------------+---------------------+---------------------+  
| Chispa intermitente | Fuga a tierra       | Aislar o reemplazar |  
+----------------------+---------------------+---------------------+  

-----
**Consejos de Mantenimiento**  
-----

1. **Conexiones**: Limpiar terminales con lija fina (#400)  
2. **Montaje**: Apretar tornillos a **8.8 N·m** (evitar vibraciones)  
3. **Sustitución**: Usar sólo bobina OEM (Ref. Kawasaki 21170-0754)  

.. note::  
   La vida útil típica es **50,000 km**. En climas húmedos, verificar mensualmente.  


Diagrama de Flujo de Diagnóstico:

¿Resistencia primaria OK?

├─ No → Reemplazar bobina

└─ Sí → Continuar


¿Resistencia secundaria OK?

├─ No → Reemplazar bobina

└─ Sí → Continuar


¿Chispa azul fuerte en prueba dinámica?

├─ No → Verificar CDI y cables

└─ Sí → Bobina funcional


¿Necesitas ampliar cómo probar el cable de bujía o el circuito de alimentación? ¡Dímelo para complementar la información!

PD: En modelos 2013+, la bobina es del tipo "stick coil" (integrada con tapa de bujía).
