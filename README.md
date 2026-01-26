# # Tarea (a+b) · Cloud: niveles y funciones (DAW 1º)

## 🅰️ Tarea A — Niveles de cloud (IaaS/PaaS/SaaS)
Crea una tabla con 10 servicios reales. Incluye enlace oficial y justifica responsabilidades.

| Servicio                         | Proveedor             | Nivel (IaaS/PaaS/SaaS) | Enlace oficial                                                                                                   | ¿Qué gestiona el proveedor?                                                                      | ¿Qué gestiona el equipo/usuario?                                     |
| -------------------------------- | --------------------- | ---------------------- | ---------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------- |
| AWS EC2                          | Amazon Web Services   | **IaaS**               | [https://aws.amazon.com/ec2/](https://aws.amazon.com/ec2/)                                                       | Infraestructura física, red, virtualización y hardware subyacente.                               | Sistema operativo, configuración de VMs, aplicaciones y datos.       |
| Google Compute Engine            | Google Cloud Platform | **IaaS**               | [https://cloud.google.com/compute](https://cloud.google.com/compute)                                             | Servidores virtuales, redes y almacenamiento.                                                    | OS, aplicaciones, seguridad y datos.                                 |
| Microsoft Azure Virtual Machines | Microsoft Azure       | **IaaS**               | [https://azure.microsoft.com/services/virtual-machines/](https://azure.microsoft.com/services/virtual-machines/) | Hardware, red, almacenamiento y virtualización.                                                  | Administración de OS, software, configuración y datos.               |
| Heroku                           | Salesforce (PaaS)     | **PaaS**               | [https://www.heroku.com/](https://www.heroku.com/)                                                               | Infraestructura, plataforma de ejecución, runtime y herramientas de despliegue. ([Wikipedia][1]) | Código de la app, configuración específica de la aplicación y datos. |
| Google App Engine                | Google Cloud Platform | **PaaS**               | [https://cloud.google.com/appengine](https://cloud.google.com/appengine)                                         | Plataforma de host, runtime, escalado automático.                                                | Código de la aplicación, configuración, datos y lógica de negocio.   |
| Azure App Service                | Microsoft Azure       | **PaaS**               | [https://azure.microsoft.com/services/app-service/](https://azure.microsoft.com/services/app-service/)           | Hosting de aplicaciones, escalado, runtime y middleware.                                         | Código, datos y configuración específica de apps.                    |
| Google Workspace                 | Google                | **SaaS**               | [https://workspace.google.com/](https://workspace.google.com/)                                                   | Aplicaciones completas (correo, docs, calendario), mantenimiento y actualizaciones.              | Gestión de usuarios, configuración de permisos y datos de usuarios.  |
| Microsoft 365                    | Microsoft             | **SaaS**               | [https://www.microsoft.com/microsoft-365](https://www.microsoft.com/microsoft-365)                               | Software completo (Word, Excel, Outlook), actualizaciones y seguridad del servicio.              | Usuarios, datos, configuración de seguridad de la organización.      |
| Salesforce CRM                   | Salesforce            | **SaaS**               | [https://www.salesforce.com/](https://www.salesforce.com/)                                                       | Plataforma de CRM completa, mantenimiento, disponibilidad y seguridad.                           | Personalización de campos, procesos de negocio y datos.              |
| Dropbox                          | Dropbox, Inc.         | **SaaS**               | [https://www.dropbox.com/](https://www.dropbox.com/)                                                             | Aplicación de almacenamiento y sincronización, infraestructura de back-end.                      | Contenido de usuario, organización de archivos y permisos.           |

[1]: https://es.wikipedia.org/wiki/Heroku?utm_source=chatgpt.com "Heroku"


## 🅱️ Tarea B — Funciones principales de cloud (arquitectura)
Incluye un diagrama (ASCII/Mermaid/imagen) y una explicación breve.


### Diagrama
(Pega aquí el diagrama)
flowchart TD
    A[Usuario/Cliente] -->|Solicita servicio| B[Cloud Provider]
    
    B --> C[Computación (IaaS/PaaS)]
    B --> D[Almacenamiento (Storage)]
    B --> E[Redes (Networking)]
    B --> F[Seguridad y Gestión (IAM, Monitoring)]
    
    C --> G[Ejecuta Aplicaciones/VMs]
    D --> H[Guarda datos, Backups]
    E --> I[Conexiones seguras y balanceo de carga]
    F --> J[Control de acceso y auditoría]


### Explicación (8–12 líneas)
(Describe el flujo front → API → BBDD/storage y dónde entra la cloud)
Este diagrama representa cómo un usuario interactúa con un proveedor de servicios en la nube:

El usuario solicita un servicio (ej. ejecutar una app o guardar datos).

El proveedor de cloud ofrece funciones principales:

Computación: máquinas virtuales, contenedores o plataformas de desarrollo (IaaS/PaaS).

Almacenamiento: bases de datos, archivos, backups.

Redes: conexiones, balanceo de carga y entrega de contenido.

Seguridad y gestión: control de accesos, monitoreo y auditoría.

Cada función permite que la nube ejecute aplicaciones, guarde datos, mantenga conexiones seguras y gestione usuarios y recursos.

Este diagrama muestra cómo un usuario interactúa con un proveedor de servicios en la nube.
El usuario accede desde el front-end (web o app) y envía una solicitud.
La petición viaja a través de una API, que gestiona la lógica y valida accesos.
La capa cloud ejecuta la aplicación usando servicios de computación (IaaS o PaaS).
Si es necesario, la API consulta o guarda información en bases de datos o almacenamiento en la nube.
Los servicios de red permiten la comunicación segura y el balanceo de carga.
La seguridad y gestión controlan identidades, permisos y monitoreo.
Finalmente, la respuesta vuelve al front-end y se muestra al usuario.

### Mapeo de funciones cloud a componentes (mínimo 3)

- Procesamiento → Servidores cloud / máquinas virtuales / contenedores
- Ejecución → Aplicaciones backend / servicios PaaS / funciones serverless
- Almacenamiento → Bases de datos en la nube / almacenamiento de objetos
- Intercambio → APIs, redes virtuales y balanceadores de carga

## 📚 Fuentes (enlaces oficiales)
(Enlaces oficiales usados en la tabla A y en la B)

- AWS – Cloud Computing Overview: https://aws.amazon.com/what-is-cloud-computing/
- Microsoft Azure – Cloud Concepts: https://learn.microsoft.com/azure/cloud-adoption-framework
- Google Cloud – Cloud Architecture: https://cloud.google.com/learn/what-is-cloud-computing
