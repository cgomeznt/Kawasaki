.. _mantenimiento-periodico:

=====
Mantenimiento Periódico
=====

.. contents:: Tabla de Contenidos
   :depth: 3
   :local:

-----
Tabla de Mantenimiento Periódico
-----

.. list-table:: Frecuencia de Inspección (lo que ocurra primero)
   :widths: 20 15 15 15 15 15 15 15
   :header-rows: 1

   * - **Inspección**
     - **Cada**
     - **1,000 km**
     - **6,000 km**
     - **12,000 km**
     - **18,000 km**
     - **24,000 km**
     - **36,000 km**
   * - Sistema de Combustible
     - Año
     - ✓
     - ✓
     - ✓
     - ✓
     - ✓
     - ✓
   * - Limpieza filtro de aire
     - 
     - 
     - ✓
     - ✓
     - ✓
     - ✓
     - ✓
   * - Sistema de Refrigeración
     - Año
     - ✓
     - ✓
     - ✓
     - ✓
     - ✓
     - ✓

-----
Tabla de Reemplazo de Partes
-----

.. list-table:: Partes de Reemplazo Periódico
   :widths: 30 20 20 20 20
   :header-rows: 1

   * - **Componente**
     - **Cada 1,000 km**
     - **Cada 12,000 km**
     - **Cada 24,000 km**
     - **Cada 36,000 km**
   * - Aceite del motor
     - ✓
     - ✓
     - ✓
     - ✓
   * - Filtro de aceite
     - 
     - ✓
     - ✓
     - ✓
   * - Bujías
     - 
     - 
     - ✓
     - 
   * - Líquido de frenos
     - 
     - 
     - ✓
     - 

-----
Torques Específicos
-----

.. list-table:: Torques para Mantenimiento
   :widths: 40 20 20 20
   :header-rows: 1

   * - **Componente**
     - **N·m**
     - **kgf·m**
     - **ft·lb**
   * - Tornillos del carburador
     - 2.0
     - 0.20
     - 18 in·lb
   * - Tuerca del eje trasero
     - 98
     - 10
     - 72
   * - Pernos de culata
     - 65
     - 6.6
     - 48

-----
Procedimientos Clave
-----

Ajuste de la Holgura del Acelerador
----------------------------------

.. warning::
   Verifique el estado de los cables antes del ajuste.

1. Gire el manillar a ambos lados para verificar que no hay resistencia.
2. Ajuste la holgura a **2-3 mm** usando los tornillos reguladores.

Cambio de Aceite
----------------

.. list-table:: Especificaciones de Aceite
   :widths: 30 30
   :header-rows: 1

   * - **Tipo**
     - **Cantidad**
   * - SAE 10W-40 API SL
     - 2.5 litros

1. Caliente el motor 3 minutos.
2. Retire el tornillo de drenaje con la moto en posición vertical.
3. Reemplace el filtro y la arandela.

-----
Inspección de Frenos
-----

+-----------------------------+-----------------------+
| **Componente**              | **Estándar**          |
+-----------------------------+-----------------------+
| Espesor de pastillas del.   | > 1.0 mm             |
+-----------------------------+-----------------------+
| Nivel líquido de frenos     | Entre marcas MIN/MAX  |
+-----------------------------+-----------------------+

.. note::
   Use sólo líquido DOT4 y evite derrames sobre piezas pintadas.

-----
Ajuste de Válvulas
-----

.. list-table:: Holguras de Válvulas
   :widths: 30 30
   :header-rows: 1

   * - **Válvula**
     - **Holgura (frío)**
   * - Admisión
     - 0.10 - 0.20 mm
   * - Escape
     - 0.15 - 0.25 mm

Procedimiento:
1. Gire el cigüeñal hasta alinear la marca "T".
2. Mida con galga de espesores.
3. Ajuste cambiando las láminas calibradoras.

-----
Lubricación de Partes
-----

* **Pivotes**: Usar grasa NLGI #2
* **Cables**: Lubricar con aceite penetrante
* **Cadena**: Lubricar cada 500 km con lubricante específico

-----
Tabla de Presión de Neumáticos
-----

.. list-table:: Presiones Recomendadas (en frío)
   :widths: 30 30 30
   :header-rows: 1

   * - **Posición**
     - **Solo conductor**
     - **Con pasajero**
   * - Delantero
     - 1.5 kgf/cm² (21 psi)
     - 1.5 kgf/cm² (21 psi)
   * - Trasero
     - 1.5 kgf/cm² (21 psi)
     - 2.0 kgf/cm² (28 psi)


.. _diagnostico-regulador-rectificador:

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
¿Cómo interpretar los resultados?
Si todas las pruebas son OK: El problema podría estar en el alternador o cableado.

Si falla 1+ pruebas: Reemplace el regulador/rectificador.

¿Necesitas el procedimiento para probar el alternador (bobinas del estator)? ¡Déjame saber y lo desarrollo en RST!

PD: Para mayor precisión, compare siempre con los valores del manual específico de su modelo.
