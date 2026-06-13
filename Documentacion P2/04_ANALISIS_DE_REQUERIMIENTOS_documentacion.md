# PET Center — Análisis de Requerimientos

> **Propósito de este documento:** ✅ Identificar, describir y priorizar los requerimientos funcionales del sistema PET Center utilizando Historias de Usuario (HU). Este análisis traduce las necesidades de los stakeholders en funcionalidades concretas que el equipo de desarrollo deberá implementar durante los sprints.

---

## 1. Metodología de Relevamiento

Para obtener los requerimientos, utilizamos las siguientes fuentes:

- **Documento base del proyecto** (Animal Center App): funcionalidades principales mencionadas.
- **Análisis de stakeholders**: expectativas identificadas de clientes, proveedores y administrador.
- **Objetivo SMART**: las métricas definidas nos indican qué debe poder hacer el sistema.

A partir de estas fuentes, redactamos **Historias de Usuario (HU)** siguiendo el formato estándar:

> **Como** [rol] **quiero** [acción] **para** [beneficio].

---

## 2. Historias de Usuario

### 2.1 Módulo de Autenticación y Registro

| ID | Historia de Usuario | Prioridad | Sprint estimado |
|----|-------------------|-----------|-----------------|
| HU-01 | **Como** usuario **quiero** registrarme en la plataforma con mi correo y contraseña **para** acceder a los servicios de PET Center. | 🔴 Alta | Sprint 2 |
| HU-02 | **Como** usuario **quiero** iniciar sesión con mi correo y contraseña **para** acceder a mi perfil y funcionalidades. | 🔴 Alta | Sprint 2 |
| HU-03 | **Como** usuario **quiero** recuperar mi contraseña **para** poder acceder a mi cuenta si la olvido. | 🟡 Media | Sprint 2 |
| HU-04 | **Como** proveedor **quiero** registrarme con un perfil especial de proveedor **para** ofrecer mis servicios en la plataforma. | 🔴 Alta | Sprint 2 |

### 2.2 Módulo de Gestión de Perfiles

| ID | Historia de Usuario | Prioridad | Sprint estimado |
|----|-------------------|-----------|-----------------|
| HU-05 | **Como** cliente **quiero** completar mi perfil con datos personales y de mis mascotas **para** que los proveedores me conozcan. | 🟡 Media | Sprint 2 |
| HU-06 | **Como** proveedor **quiero** completar mi perfil con información de mi negocio, horarios y servicios **para** que los clientes puedan encontrarme. | 🔴 Alta | Sprint 2 |
| HU-07 | **Como** cliente **quiero** registrar una o más mascotas con nombre, raza y edad **para** gestionar sus servicios. | 🟡 Media | Sprint 3 |
| HU-08 | **Como** usuario **quiero** editar mi perfil **para** mantener mi información actualizada. | 🟡 Media | Sprint 3 |

### 2.3 Módulo de Búsqueda y Exploración

| ID | Historia de Usuario | Prioridad | Sprint estimado |
|----|-------------------|-----------|-----------------|
| HU-09 | **Como** cliente **quiero** buscar servicios por categoría (veterinaria, servicios, tienda) **para** encontrar lo que necesito rápidamente. | 🔴 Alta | Sprint 2 |
| HU-10 | **Como** cliente **quiero** ver el perfil de un proveedor con sus servicios, valoraciones y ubicación **para** decidir si contratarlo. | 🔴 Alta | Sprint 3 |
| HU-11 | **Como** cliente **quiero** filtrar proveedores por ubicación **para** encontrar servicios cerca de mi domicilio. | 🟡 Media | Sprint 3 |
| HU-12 | **Como** cliente **quiero** ver promociones y ofertas destacadas **para** aprovechar descuentos. | 🟢 Baja | Sprint 3 |

### 2.4 Módulo de Reservas

| ID | Historia de Usuario | Prioridad | Sprint estimado |
|----|-------------------|-----------|-----------------|
| HU-13 | **Como** cliente **quiero** seleccionar un servicio y elegir fecha y horario disponible **para** reservar un turno. | 🔴 Alta | Sprint 3 |
| HU-14 | **Como** cliente **quiero** ver la disponibilidad del proveedor en tiempo real **para** elegir un horario que me sirva. | 🔴 Alta | Sprint 3 |
| HU-15 | **Como** cliente **quiero** cancelar una reserva **para** liberar el turno si no puedo asistir. | 🟡 Media | Sprint 3 |
| HU-16 | **Como** proveedor **quiero** ver mis reservas confirmadas **para** organizar mi agenda de trabajo. | 🔴 Alta | Sprint 3 |
| HU-17 | **Como** proveedor **quiero** confirmar o rechazar una reserva **para** gestionar mi disponibilidad. | 🟡 Media | Sprint 3 |

### 2.5 Módulo de Valoraciones y Reputación

| ID | Historia de Usuario | Prioridad | Sprint estimado |
|----|-------------------|-----------|-----------------|
| HU-18 | **Como** cliente **quiero** calificar y comentar el servicio recibido **para** compartir mi experiencia con otros usuarios. | 🟡 Media | Sprint 4 |
| HU-19 | **Como** cliente **quiero** ver las valoraciones de otros usuarios sobre un proveedor **para** tomar una decisión informada. | 🔴 Alta | Sprint 3 |
| HU-20 | **Como** proveedor **quiero** ver mis valoraciones recibidas **para** conocer mi reputación en la plataforma. | 🟢 Baja | Sprint 4 |

### 2.6 Módulo de Administración

| ID | Historia de Usuario | Prioridad | Sprint estimado |
|----|-------------------|-----------|-----------------|
| HU-21 | **Como** administrador **quiero** aprobar o rechazar proveedores **para** garantizar la calidad de los servicios. | 🔴 Alta | Sprint 4 |
| HU-22 | **Como** administrador **quiero** gestionar usuarios (suspender, eliminar) **para** mantener el orden en la plataforma. | 🟡 Media | Sprint 4 |
| HU-23 | **Como** administrador **quiero** ver estadísticas de uso (usuarios, reservas, valoraciones) **para** tomar decisiones sobre la plataforma. | 🟢 Baja | Sprint 4 |

---

## 3. Requerimientos No Funcionales

Además de las funcionalidades, el sistema debe cumplir con los siguientes atributos de calidad:

| ID | Requerimiento | Descripción | Prioridad |
|----|--------------|-------------|-----------|
| RNF-01 | **Disponibilidad** | La plataforma debe estar operativa el 99.5% del tiempo en horario comercial (08:00 a 22:00). | 🔴 Alta |
| RNF-02 | **Rendimiento** | El sistema debe soportar al menos 50 reservas simultáneas sin degradación del tiempo de respuesta. | 🔴 Alta |
| RNF-03 | **Seguridad** | Las contraseñas deben almacenarse encriptadas. El acceso a datos sensibles debe requerir autenticación. | 🔴 Alta |
| RNF-04 | **Usabilidad** | La interfaz debe ser intuitiva, permitiendo a un usuario nuevo completar una reserva en menos de 3 minutos. | 🟡 Media |
| RNF-05 | **Compatibilidad** | La plataforma debe funcionar correctamente en los navegadores Chrome, Firefox y Edge en sus versiones actuales. | 🟡 Media |
| RNF-06 | **Escalabilidad** | La arquitectura debe permitir agregar nuevos módulos sin afectar los existentes. | 🟡 Media |

---

## 4. Matriz de Trazabilidad

A continuación, relacionamos las Historias de Usuario con los stakeholders que las originan y los sprints donde se implementarán.

| Stakeholder | HU relacionadas | Sprint |
|-------------|----------------|--------|
| Cliente (Dueño de mascota) 🟢 | HU-01, HU-02, HU-03, HU-05, HU-07, HU-08, HU-09, HU-10, HU-11, HU-12, HU-13, HU-14, HU-15, HU-18, HU-19 | Sprint 2, 3 y 4 |
| Proveedor 🟡 | HU-04, HU-06, HU-16, HU-17, HU-20 | Sprint 2, 3 y 4 |
| Administrador 🔴 | HU-21, HU-22, HU-23 | Sprint 4 |

---

## 5. Control de Versiones

| Versión | Fecha | Cambios realizados | Autor |
|---------|-------|--------------------|-------|
| 1.0.0 | 13-06-2026 | Creación inicial del documento con 23 HU y 6 RNF | Equipo PET Center |

---

*Documento elaborado para el Parcial I — Administración de Proyectos. Este análisis se actualizará a medida que se identifiquen nuevos requerimientos durante el desarrollo.*