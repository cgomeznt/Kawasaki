.. _prueba-cdi-klr650:

=====
Prueba del Módulo CDI Kawasaki KLR650 (2013)  
=====

.. contents::  
   :depth: 3  
   :local:

-----
**Herramientas Necesarias**
-----

* Multímetro digital (con función de continuidad y Ω)  
* Manual de servicio KLR650 2013 (para diagrama de pines)  
* Juego de destornilladores  
* Luz de prueba 12V (opcional)  

-----
**Ubicación del CDI**
-----

1. Bajo el asiento del piloto  
2. Conector rectangular de 6 pines (color blanco/negro)  
3. Identificación: **KHI Part# 21119-XXXX** (ver etiqueta)

-----
**Pruebas Básicas**
-----

Prueba 1: Alimentación y Tierra
-------------------------------

1. Desconecte el conector del CDI  
2. Encienda el interruptor de llave (ON)  

.. list-table:: Verificación de Voltaje  
   :widths: 30 30 30  
   :header-rows: 1  

   * - **Pin**  
     - **Color Cable**  
     - **Valor Esperado**  
   * - 1  
     - Rojo/Negro  
     - 12V DC (Batería)  
   * - 2  
     - Verde  
     - 0V (Tierra)  
   * - 6  
     - Negro/Amarillo  
     - 12V DC (Ignición ON)  

.. warning::  
   Si falta voltaje en pin 1 o 6: revisar fusibles (main 20A, ignición 10A)

Prueba 2: Señal del Sensor de Cigüeñal
--------------------------------------

1. Motor en punto muerto  
2. Medir entre pines 3 (Azul) y 4 (Blanco):  

   - Resistencia: **90Ω-110Ω** (a 20°C)  
   - Voltaje AC: **>0.5V** al arrancar  

.. image:: /path/to/cdi_pinout.png  
   :width: 250  
   :align: center  

Prueba 3: Salida a Bobina
-------------------------

1. Conectar luz de prueba entre:  
   - Pin 5 (Negro/Amarillo)  
   - Tierra del motor  

2. Al arrancar: **la luz debe parpadear**  

.. danger::  
   Si no hay parpadeo: CDI defectuoso  

-----
**Tabla de Diagnóstico**
-----

+----------------------+---------------------+---------------------+  
| **Síntoma**         | **Posible Causa**   | **Verificación**    |  
+======================+=====================+=====================+  
| No chispa           | Fallo alimentación  | Testear pin 1 y 6   |  
+----------------------+---------------------+---------------------+  
| Chispa intermitente | Mal contacto        | Inspeccionar pines  |  
+----------------------+---------------------+---------------------+  
| Motor no acelera    | Señal sensor dañada | Medir pines 3-4     |  
+----------------------+---------------------+---------------------+  

-----
**Procedimiento Avanzado**
-----

Prueba de Resistencia Interna
-----------------------------

1. Desconectar CDI completamente  
2. Medir entre:  

   .. list-table::  
      :widths: 40 30  
      :header-rows: 1  

      * - **Pines**  
        - **Valor Normal**  
      * - 2 (Tierra) y 5 (Salida)  
        - 1kΩ-3kΩ  
      * - 1 (Alim) y 6 (Ignición)  
        - ∞Ω (sin continuidad)  

-----
**Recomendaciones**
-----

1. **Prueba definitiva**: Sustituir por CDI conocido bueno  
2. **Conexiones**: Limpiar con contacto spray si hay oxidación  
3. **Códigos**: La KLR650 2013 no tiene sistema de error OBD  

.. note::  
   El CDI rara vez falla (sólo 2% de casos). Primero descartar:  
   - Bobina de encendido  
   - Sensor de cigüeñal  
   - Cableado dañado  


Diagrama de Flujo de Diagnóstico:

¿Hay 12V en pin 1 y 6?

├─ No → Revisar fusibles/cableado

└─ Sí → Continuar



¿Señal del sensor cigüeñal OK?

├─ No → Probar sensor

└─ Sí → Continuar



¿Salida a bobina parpadea?

├─ No → CDI defectuoso

└─ Sí → Problema en bobina/cables de bujía



¿Necesitas ampliar la prueba del sensor de cigüeñal o bobina de encendido? ¡Dímelo y completo la información!


PD: En modelos 2013+, el "CDI" es realmente una unidad IC igniter (sin condensador descargable clásico).

