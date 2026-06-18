# PET Center — Tablero de Seguimiento (Trello)

> **Propósito de este documento:** ✅ Documentar el proceso de creación del tablero en Trello para el seguimiento del proyecto PET Center. Primero se realizó un análisis completo de todas las tareas identificadas en los documentos anteriores (SMART, stakeholders, metodologías ágiles y análisis de requerimientos) y luego se volcaron en un borrador estructurado. Este borrador sirve como guía para armar el tablero en Trello, asegurando que ninguna tarea quede fuera y que el equipo tenga visibilidad completa del avance.

---

## 1. Configuración del Tablero en Trello

### 1.1 Creación del tablero

| Elemento | Valor |
|----------|-------|
| **Nombre del tablero** | PET Center — Proyecto |
| **Visibilidad** | Público |
| **Miembros del equipo** | Gustavo Oliva, Carelis Fagundez |
| **Invitado externo** | sergiod.medina@davinci.edu.ar |

### 1.2 Listas del tablero

El tablero se organiza en las siguientes listas, basadas en la metodología Scrumban definida en el documento `03_METODOLOGIAS_AGILES_documentacion.md`:

| # | Nombre de la lista | Propósito |
|---|-------------------|-----------|
| 1 | **Pendiente** | Tareas identificadas pero no asignadas a ningún sprint |
| 2 | **Sprint 1 — Análisis y Diseño** | Tareas de las semanas 1 y 2 |
| 3 | **Sprint 2 — Frontend** | Tareas de las semanas 3 y 4 |
| 4 | **Sprint 3 — Backend** | Tareas de las semanas 5 y 6 |
| 5 | **Sprint 4 — Integración y Despliegue** | Tareas de las semanas 7 y 8 |
| 6 | **En progreso** | Tareas que se están desarrollando actualmente (límite: 4) |
| 7 | **En revisión** | Tareas terminadas que esperan validación del otro miembro |
| 8 | **Terminado** | Tareas completadas y validadas |

> **Nota:** Las listas de sprints (2 a 5) funcionan como el Sprint Backlog. Al iniciar cada sprint, movemos las tarjetas correspondientes desde "Pendiente" a la lista del sprint activo, y de ahí a "En progreso" cuando comenzamos a trabajar en ellas.

---

## 2. Tarjetas del Tablero

A continuación, se detalla cada tarjeta con su título, descripción, miembros asignados, etiqueta de prioridad y lista de origen.

---

### 2.1 Sprint 1 — Análisis y Diseño (Semanas 1 y 2)

| # | Título | Descripción | Miembros | Prioridad |
|---|--------|-------------|----------|-----------|
| T01 | Definir objetivo SMART del proyecto | Redactar el objetivo general del proyecto siguiendo la metodología SMART. Incluir métricas medibles y plazos. | Gustavo, Carelis | 🔴 Alta |
| T02 | Identificar stakeholders | Realizar un análisis de interesados, identificar al menos 3 stakeholders clave y definir estrategias de comunicación. | Gustavo, Carelis | 🔴 Alta |
| T03 | Definir metodología ágil | Elegir y justificar la metodología ágil a utilizar (Scrumban). Definir roles, sprints, ceremonias y artefactos. | Gustavo, Carelis | 🔴 Alta |
| T04 | Relevar y documentar requerimientos | Identificar Historias de Usuario (HU) y Requerimientos No Funcionales (RNF) a partir del documento base y los stakeholders. | Gustavo, Carelis | 🔴 Alta |
| T05 | Diseñar arquitectura del sistema | Definir la arquitectura en capas (MVC), componentes, tecnologías y diagrama de despliegue. | Gustavo | 🔴 Alta |
| T06 | Configurar entorno de desarrollo | Instalar y configurar Python, Flask, Tailwind CSS, Git y entorno virtual. | Carelis | 🔴 Alta |
| T07 | Crear tablero en Trello | Armar el tablero de seguimiento con listas, tarjetas, miembros y configurar visibilidad pública. | Gustavo | 🟡 Media |

---

### 2.2 Sprint 2 — Frontend (Semanas 3 y 4)

| # | Título | Descripción | Miembros | Prioridad |
|---|--------|-------------|----------|-----------|
| T08 | HU-01: Registro de usuarios | Implementar formulario de registro con correo y contraseña. Validar datos y guardar en base de datos. | Carelis | 🔴 Alta |
| T09 | HU-02: Inicio de sesión | Implementar formulario de login con validación de credenciales y redirección según rol. | Carelis | 🔴 Alta |
| T10 | HU-03: Recuperación de contraseña | Implementar flujo de recuperación de contraseña (solicitud, enlace, cambio). | Carelis | 🟡 Media |
| T11 | HU-04: Registro de proveedores | Extender el registro para incluir perfil de proveedor con datos del negocio. | Carelis | 🔴 Alta |
| T12 | HU-05: Perfil de cliente | Crear vista de perfil de cliente con datos personales y listado de mascotas. | Gustavo | 🟡 Media |
| T13 | HU-06: Perfil de proveedor | Crear vista de perfil de proveedor con datos del negocio, horarios y servicios ofrecidos. | Gustavo | 🔴 Alta |
| T14 | HU-09: Búsqueda por categorías | Implementar filtros de búsqueda por categorías: veterinaria, servicios, tienda. | Gustavo | 🔴 Alta |
| T15 | HU-10: Ver perfil de proveedor | Vista detallada del proveedor con servicios, valoraciones y ubicación. | Gustavo | 🔴 Alta |
| T16 | HU-19: Ver valoraciones | Mostrar valoraciones y comentarios de otros usuarios en el perfil del proveedor. | Gustavo | 🔴 Alta |
| T17 | HU-12: Promociones destacadas | Sección visual con ofertas y promociones de los proveedores. | Gustavo | 🟢 Baja |

---

### 2.3 Sprint 3 — Backend (Semanas 5 y 6)

| # | Título | Descripción | Miembros | Prioridad |
|---|--------|-------------|----------|-----------|
| T18 | HU-07: Registrar mascotas | Formulario para registrar mascotas con nombre, raza y edad. Asociar al cliente. | Carelis | 🟡 Media |
| T19 | HU-08: Editar perfil | Permitir al usuario editar sus datos personales y de mascotas. | Carelis | 🟡 Media |
| T20 | HU-11: Filtrar por ubicación | Agregar filtro geográfico para buscar proveedores cercanos. | Gustavo | 🟡 Media |
| T21 | HU-13: Reservar turno | Implementar flujo completo de reserva: seleccionar servicio, fecha, horario y confirmar. | Gustavo | 🔴 Alta |
| T22 | HU-14: Ver disponibilidad | Mostrar calendario con horarios disponibles del proveedor en tiempo real. | Gustavo | 🔴 Alta |
| T23 | HU-15: Cancelar reserva | Permitir al cliente cancelar una reserva existente. | Gustavo | 🟡 Media |
| T24 | HU-16: Ver reservas (proveedor) | Panel para que el proveedor vea sus reservas confirmadas. | Carelis | 🔴 Alta |
| T25 | HU-17: Confirmar/rechazar reserva | Permitir al proveedor aceptar o rechazar solicitudes de reserva. | Carelis | 🟡 Media |
| T26 | HU-18: Calificar servicio | Formulario para que el cliente califique y comente el servicio recibido. | Carelis | 🟡 Media |
| T27 | HU-20: Ver valoraciones (proveedor) | Panel para que el proveedor vea sus calificaciones recibidas. | Carelis | 🟢 Baja |
| T28 | RNF-02: Pruebas de rendimiento | Verificar que el sistema soporta 50 reservas simultáneas sin degradación. | Gustavo | 🔴 Alta |
| T29 | RNF-03: Seguridad | Implementar encriptación de contraseñas y validación de sesiones. | Carelis | 🔴 Alta |

---

### 2.4 Sprint 4 — Integración y Despliegue (Semanas 7 y 8)

| # | Título | Descripción | Miembros | Prioridad |
|---|--------|-------------|----------|-----------|
| T30 | HU-21: Aprobar/rechazar proveedores | Panel de administración para gestionar proveedores. | Gustavo | 🔴 Alta |
| T31 | HU-22: Gestionar usuarios | Panel para suspender o eliminar usuarios desde administración. | Gustavo | 🟡 Media |
| T32 | HU-23: Estadísticas de uso | Panel con reportes y estadísticas del sistema. | Gustavo | 🟢 Baja |
| T33 | RNF-01: Pruebas de disponibilidad | Verificar uptime del sistema en horario comercial. | Carelis | 🔴 Alta |
| T34 | RNF-04: Pruebas de usabilidad | Realizar pruebas con usuarios para verificar que una reserva se completa en menos de 3 minutos. | Carelis | 🟡 Media |
| T35 | RNF-05: Pruebas de compatibilidad | Verificar funcionamiento en Chrome, Firefox y Edge. | Carelis | 🟡 Media |
| T36 | Integración frontend-backend | Conectar todas las vistas del frontend con la API REST del backend. | Gustavo, Carelis | 🔴 Alta |
| T37 | Pruebas integrales del sistema | Probar todos los flujos completos: registro → búsqueda → reserva → valoración. | Gustavo, Carelis | 🔴 Alta |
| T38 | Corrección de errores | Revisar y corregir bugs encontrados durante las pruebas. | Gustavo, Carelis | 🔴 Alta |
| T39 | Documentación final | Completar y revisar toda la documentación del proyecto. | Gustavo, Carelis | 🔴 Alta |
| T40 | Despliegue en producción | Publicar la plataforma en un servidor accesible. | Gustavo | 🔴 Alta |

---

## 3. Etiquetas de Prioridad

Se utilizarán las siguientes etiquetas de color en Trello para identificar la prioridad de cada tarjeta:

| Etiqueta | Color | Significado | Cantidad de tarjetas |
|----------|-------|-------------|----------------------|
| 🔴 Alta | Rojo | Imprescindible para el MVP. Sin esto, el proyecto no cumple los requisitos mínimos. | 22 |
| 🟡 Media | Amarillo | Importante pero no bloqueante. Mejora la experiencia del usuario. | 14 |
| 🟢 Baja | Verde | Deseable. Se implementa si el tiempo lo permite. | 4 |

---

## 4. Enlace del Tablero

> **Enlace público del tablero:**  [ https://trello.com/invite/b/6a2e970877d8772ab68cb8ef/ATTI3de9cf2ddf90cbe5a3d3d5077d95a2a95BF9912A/pet-center ]


---

## 5. Control de Versiones

| Versión |   Fecha    | Cambios realizados | Autor |
|---------|------------|--------------------|-------|
| 1.0.0   | 13-06-2026 | Creación inicial del documento con descripción completa del tablero Trello | Equipo PET Center |
| 1.1.0   | 18-06-2026 | Incorporación del enlace público del tablero |Equipo PET Center|

