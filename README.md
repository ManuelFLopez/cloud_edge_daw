# Tarea (C + D + E) — Edge, Fog, Mist y Cloud  
**DAW 1º**

---

# 🅲 Tarea C — Edge Computing y relación con Cloud

## Definición (3–5 líneas)

El **Edge Computing** es un modelo de computación donde el procesamiento de datos se realiza cerca de donde se generan, como sensores, dispositivos IoT o gateways locales. En lugar de enviar toda la información a la nube, parte del análisis se hace localmente. Esto reduce la latencia, el uso de red y mejora la velocidad de respuesta. Es clave en sistemas en tiempo real.

## Relación Edge ↔ Cloud (5–8 líneas)

Edge y Cloud trabajan de forma complementaria. El Edge procesa datos inmediatos y críticos cerca del dispositivo, permitiendo respuestas rápidas. La Cloud se encarga del almacenamiento masivo, análisis avanzado e inteligencia artificial. Normalmente, el Edge filtra y resume datos antes de enviarlos a la nube. Así se reduce el tráfico de red. La Cloud puede devolver modelos entrenados y configuraciones al Edge. Juntos forman una arquitectura eficiente y escalable.

## Ejemplo real

En vehículos autónomos, los sensores procesan datos en el Edge para reaccionar en milisegundos (frenar o girar). Después, los datos importantes se envían a la Cloud para mejorar los algoritmos de conducción del sistema completo.

## Fuentes oficiales (mín. 2)

- Microsoft Azure — Edge Computing  
  https://azure.microsoft.com/solutions/edge-computing/

- AWS — What is Edge Computing  
  https://aws.amazon.com/what-is/edge-computing/

---

# 🅳 Tarea D — Fog vs Mist (niveles y zonas de aplicación)

## Definición Fog (2–4 líneas)

El **Fog Computing** sitúa recursos de computación en nodos intermedios de la red, como routers avanzados o micro centros de datos locales. Reduce latencia respecto a la nube y coordina múltiples dispositivos Edge. Sirve como capa regional de procesamiento.

## Definición Mist (2–4 líneas)

El **Mist Computing** lleva el procesamiento al propio dispositivo o sensor. Ejecuta reglas simples y decisiones básicas directamente en el hardware. Minimiza completamente la dependencia de red para tareas pequeñas.

## Esquema de capas

[ Sensores / Dispositivos ]
          │
        MIST
 (procesamiento mínimo)
          │
        EDGE
 (gateway / dispositivo local)
          │
         FOG

## 🅴 Tarea E — Ventajas de la Cloud en sistemas conectados

1) **Ventaja: Escalabilidad**  
   **Explicación:** Permite aumentar o reducir recursos automáticamente según la demanda sin necesidad de infraestructura física adicional.  
   **Ejemplo:** Una plataforma IoT puede ampliar servidores durante picos de tráfico y reducirlos en horas de baja actividad, optimizando costes.

2) **Ventaja: Acceso global**  
   **Explicación:** Los servicios y datos están disponibles desde cualquier lugar con conexión a Internet, facilitando el trabajo remoto y la gestión distribuida.  
   **Ejemplo:** Un panel de control de dispositivos inteligentes se puede consultar desde cualquier ciudad o país.

3) **Ventaja: Alta capacidad de almacenamiento**  
   **Explicación:** Permite guardar grandes volúmenes de información sin necesidad de servidores locales.  
   **Ejemplo:** Históricos de sensores de una planta industrial que generan datos continuos durante años.

4) **Ventaja: Integración con Inteligencia Artificial y análisis de datos**  
   **Explicación:** La Cloud ofrece herramientas avanzadas de análisis y aprendizaje automático para optimizar procesos y predecir fallos.  
   **Ejemplo:** Un sistema de mantenimiento predictivo que analiza datos de máquinas conectadas para anticipar averías.

5) **Ventaja: Menor coste inicial y mantenimiento**  
   **Explicación:** No se requiere comprar ni mantener servidores físicos propios, reduciendo inversión y gastos operativos.  
   **Ejemplo:** Una startup puede desplegar su red de sensores y bases de datos directamente en la nube sin inversión en hardware.

**Fuente oficial (mín. 1):**  
- Google Cloud — What is Cloud Computing  
  https://cloud.google.com/learn/what-is-cloud-computing

## 📚 Fuentes (enlaces oficiales)

- Microsoft Azure — Edge Computing  
  https://azure.microsoft.com/solutions/edge-computing/  

- AWS — What is Edge Computing  
  https://aws.amazon.com/what-is/edge-computing/  

- Google Cloud — What is Cloud Computing  
  https://cloud.google.com/learn/what-is-cloud-computing

 (nodos intermedios)
          │
        CLOUD
 (data centers)
