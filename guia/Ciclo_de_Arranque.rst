Ciclo de Arranque - Kawasaki KLR 650 (2013)
===========================================

Descripción paso a paso del proceso desde que se pulsa el botón de encendido hasta que el motor arranca.

1. Pre-chequeo del Sistema (Llave en "ON")
------------------------------------------

- **Acción**: Girar la llave a posición ``ON``.
- **Procesos**:
  - Cuadro de instrumentos se enciende (velocímetro, luces de advertencia).
  - Luz ``Check Engine`` (MIL) se enciende brevemente (si hay fallos, permanece encendida).
  - *Nota*: La KLR 650 2013 (carburada) **no activa bomba de combustible** (sistema por gravedad/vacío).

2. Verificación de Seguridades
------------------------------

- **Condiciones para arranque**:
  - Motor en ``punto muerto`` (sensor de neutro activado) **o**.
  - Palanca de ``embrague accionada`` (interruptor de embrague cerrado).
- **Si no se cumple**:
  - El motor de arranque **no gira** (protección anti-arranque en marcha).

3. Pulsar el Botón de Arranque
------------------------------

- **Flujo eléctrico**:
  1. Botón envía señal al ``relé de arranque (solenoide)``.
  2. Relé conecta la batería (12V) al ``motor de arranque`` (se escucha un "clic").
  3. Motor de arranque gira el cigüeñal mediante el ``piñón Bendix``.

4. Proceso de Combustión
------------------------

**Modelo Carburado (Típico 2013)**:

1. **Alimentación de combustible**:
   - El vacío del motor aspira gasolina desde el ``carburador``.
   - ``Choke (cebador)`` enriquece la mezcla si está en frío.
2. **Encendido**:
   - ``Bobina de encendido`` genera chispa (señal del CDI/ECU).
   - Sincronización por ``sensor de posición del cigüeñal``.

**Modelo con Inyección (Poco común en 2013)**:

1. Bomba de combustible presuriza el sistema.
2. ``ECU`` controla inyectores basándose en:
   - ``Sensor TPS`` (posición del acelerador).
   - ``Sensor MAP/MAF`` (flujo de aire).

5. Arranque Exitoso
-------------------

- **Motor en marcha**:
  - Revoluciones altas en frío (~1500-2000 RPM) con ``choke``.
  - Estabilización en ralentí (~1200-1400 RPM) en caliente.

Fallas Comunes Durante el Arranque
---------------------------------

+------------------------+-----------------------------------------------+
| **Síntoma**            | **Causas Probables**                          |
+========================+===============================================+
| Motor de arranque no   | - Batería descargada.                         |
| gira                   | - Fusible/relé dañado.                        |
|                        | - Fallo en sensor de neutro/embrague.         |
+------------------------+-----------------------------------------------+
| Gira pero no arranca   | - Carburador obstruido.                       |
|                        | - Bujía sin chispa (bobina/cables dañados).   |
|                        | - Válvula de descompresión mal ajustada.      |
+------------------------+-----------------------------------------------+

Consejos para Arranque en Frío (Carburador)
-------------------------------------------

- Usar ``choke`` completamente al arrancar.
- Bombear suavemente el acelerador antes de encender.
- Esperar 30 segundos entre intentos si no arranca (evitar inundar el motor).
