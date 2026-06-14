# PET Center - Product Backlog

> **Proposito de este documento:** ✅ Listar y priorizar todas las funcionalidades que debe tener el sistema PET Center.

---

## 1. Criterios de Priorizacion

| Prioridad | Criterio |
|-----------|----------|
| 🔴 **Alta** | Funcionalidad indispensable para el MVP. |
| 🟡 **Media** | Funcionalidad importante que mejora la experiencia. |
| 🟢 **Baja** | Funcionalidad deseable que agrega valor. |

---

## 2. Metodo de Estimacion: Puntos de Historia (Fibonacci)

Para estimar el esfuerzo de cada item del backlog, utilizamos la **escala Fibonacci** (1, 2, 3, 5, 8, 13).

| Puntos | Significado | Ejemplo |
|--------|-------------|---------|
| **1** | Tarea muy simple, pocos minutos | Configurar entorno |
| **2** | Tarea simple, media jornada | Formulario de login |
| **3** | Tarea media, una jornada | Registro con validacion |
| **5** | Tarea compleja, varios dias | Reserva con disponibilidad |
| **8** | Tarea muy compleja, requiere coordinacion | Integracion frontend-backend |
| **13** | Tarea epica, abarca varios componentes | Pruebas integrales |

> **Impacto:** Conocer los puntos de historia permite calcular la velocidad del equipo y ajustar expectativas.

---

## 3. Criterios de Asignacion de Miembros

Cada item del backlog se asigna al miembro del equipo segun su rol y especialidad:

| Miembro | Rol | Tipo de tareas asignadas |
|---------|-----|--------------------------|
| **Gustavo Oliva** | Product Owner | Documentacion, frontend (busqueda, perfiles, valoraciones), administracion, integracion, despliegue |
| **Carelis Fagundez** | Facilitador | Backend, base de datos, autenticacion, registro, reservas, pruebas tecnicas, configuracion de entorno |
| **Ambos** | Equipo de Desarrollo | Tareas que requieren coordinacion: definicion de objetivos, metodologia, pruebas integrales, correccion de errores |

> **Nota:** La asignacion no es rigida. Ambos miembros pueden colaborar en cualquier tarea segun la carga de trabajo del sprint. Esta columna indica el **responsable principal** de cada item.

---

## 4. Product Backlog

| ID | Funcionalidad | Prioridad | Est. | Asignado a | Depende de | Sprint |
|----|--------------|-----------|:----:|------------|------------|--------|
| PB-01 | Definir objetivo SMART | Alta | 1 | Gustavo, Carelis | - | Sprint 1 |
| PB-02 | Identificar stakeholders | Alta | 1 | Gustavo, Carelis | - | Sprint 1 |
| PB-03 | Definir metodologia agil | Alta | 2 | Gustavo, Carelis | - | Sprint 1 |
| PB-04 | Relevar requerimientos | Alta | 3 | Gustavo, Carelis | PB-02 | Sprint 1 |
| PB-05 | Disenar arquitectura | Alta | 3 | Gustavo | PB-04 | Sprint 1 |
| PB-06 | Configurar entorno | Alta | 1 | Carelis | - | Sprint 1 |
| PB-07 | Crear tablero Trello | Media | 2 | Gustavo | PB-03 | Sprint 1 |
| PB-08 | HU-01: Registro de usuarios | Alta | 5 | Carelis | PB-06 | Sprint 2 |
| PB-09 | HU-02: Inicio de sesion | Alta | 3 | Carelis | PB-08 | Sprint 2 |
| PB-10 | HU-03: Recuperar contrasenia | Media | 3 | Carelis | PB-09 | Sprint 2 |
| PB-11 | HU-04: Registro de proveedores | Alta | 3 | Carelis | PB-08 | Sprint 2 |
| PB-12 | HU-05: Perfil de cliente | Media | 3 | Gustavo | PB-08 | Sprint 2 |
| PB-13 | HU-06: Perfil de proveedor | Alta | 5 | Gustavo | PB-11 | Sprint 2 |
| PB-14 | HU-09: Busqueda por categorias | Alta | 5 | Gustavo | PB-13 | Sprint 2 |
| PB-15 | HU-10: Ver perfil de proveedor | Alta | 3 | Gustavo | PB-13 | Sprint 2 |
| PB-16 | HU-19: Ver valoraciones | Alta | 2 | Gustavo | PB-15 | Sprint 2 |
| PB-17 | HU-12: Promociones destacadas | Baja | 2 | Gustavo | PB-14 | Sprint 2 |
| PB-18 | HU-07: Registrar mascotas | Media | 3 | Carelis | PB-12 | Sprint 3 |
| PB-19 | HU-08: Editar perfil | Media | 2 | Carelis | PB-12 | Sprint 3 |
| PB-20 | HU-13: Reservar turno | Alta | 8 | Gustavo | PB-15 | Sprint 3 |
| PB-21 | HU-14: Ver disponibilidad | Alta | 5 | Gustavo | PB-20 | Sprint 3 |
| PB-22 | HU-15: Cancelar reserva | Media | 3 | Gustavo | PB-20 | Sprint 3 |
| PB-23 | HU-16: Ver reservas (proveedor) | Alta | 5 | Carelis | PB-20 | Sprint 3 |
| PB-24 | HU-17: Confirmar/rechazar reserva | Media | 3 | Carelis | PB-23 | Sprint 3 |
| PB-25 | HU-18: Calificar servicio | Media | 3 | Carelis | PB-20 | Sprint 3 |
| PB-26 | HU-20: Ver valoraciones (proveedor) | Baja | 2 | Carelis | PB-25 | Sprint 3 |
| PB-27 | RNF-02: Pruebas de rendimiento | Alta | 5 | Gustavo | PB-20 | Sprint 3 |
| PB-28 | HU-21: Aprobar/rechazar proveedores | Alta | 5 | Gustavo | PB-11 | Sprint 4 |
| PB-29 | HU-22: Gestionar usuarios | Media | 3 | Gustavo | PB-28 | Sprint 4 |
| PB-30 | HU-23: Estadisticas de uso | Baja | 5 | Gustavo | PB-28 | Sprint 4 |
| PB-31 | RNF-01: Pruebas de disponibilidad | Alta | 3 | Carelis | PB-27 | Sprint 4 |
| PB-32 | RNF-04: Pruebas de usabilidad | Media | 3 | Carelis | PB-20 | Sprint 4 |
| PB-33 | RNF-05: Pruebas de compatibilidad | Media | 2 | Carelis | PB-06 | Sprint 4 |
| PB-34 | Integracion frontend-backend | Alta | 8 | Gustavo, Carelis | PB-20, PB-27 | Sprint 4 |
| PB-35 | Pruebas integrales | Alta | 8 | Gustavo, Carelis | PB-34 | Sprint 4 |
| PB-36 | Correccion de errores | Alta | 5 | Gustavo, Carelis | PB-35 | Sprint 4 |
| PB-37 | Documentacion final | Alta | 3 | Gustavo, Carelis | PB-01 a PB-07 | Sprint 4 |
| PB-38 | Despliegue en produccion | Alta | 5 | Gustavo | PB-36 | Sprint 4 |

---

## 5. Resumen del Backlog

| Metrica | Valor |
|---------|-------|
| Total de items | 38 |
| Alta prioridad | 22 |
| Media prioridad | 12 |
| Baja prioridad | 4 |
| Sprint 1 | 7 items (PB-01 a PB-07) |
| Sprint 2 | 10 items (PB-08 a PB-17) |
| Sprint 3 | 10 items (PB-18 a PB-27) |
| Sprint 4 | 11 items (PB-28 a PB-38) |
| **Total puntos de historia** | **146** |
| **Promedio por sprint** | **36.5 puntos** |
| Items asignados a Gustavo | 17 |
| Items asignados a Carelis | 12 |
| Items asignados a Ambos | 9 |

---

## 6. Relacion con otros documentos

| Documento | Relacion |
|-----------|----------|
| 01_SMART_documentacion.md | El backlog responde a las metricas del objetivo SMART |
| 02_STAKEHOLDERS_documentacion.md | Las funcionalidades cubren expectativas de stakeholders |
| 03_METODOLOGIAS_AGILES_documentacion.md | El backlog se gestiona con Scrumban |
| 04_ANALISIS_DE_REQUERIMIENTOS_documentacion.md | Cada PB corresponde a una HU o RNF |
| 05_TABLERO_descripcion.md | Las tarjetas de Trello corresponden 1 a 1 con los PB |

---

## 7. Control de Versiones

| Version | Fecha | Cambios realizados | Autor |
|---------|-------|--------------------|-------|
| 1.0.0 | 13-06-2026 | Creacion inicial con 40 items priorizados | Equipo PET Center |
| 1.1.0 | 13-06-2026 | Eliminados PB-20 y PB-29 originales. Reordenados IDs (38 items). Agregada columna de estimacion Fibonacci. Impacto: 146 puntos totales, ~36.5 por sprint. | Equipo PET Center |
| 1.2.0 | 13-06-2026 | Agregada columna de asignacion de miembros con responsables de cada item. Agregada seccion 3 con criterios de asignacion segun rol (Product Owner y Facilitador). Impacto: cada miembro conoce sus responsabilidades principales y se facilita el seguimiento en Trello. | Equipo PET Center |