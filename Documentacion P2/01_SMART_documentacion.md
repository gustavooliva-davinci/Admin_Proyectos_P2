# PET Center — Documentación del Proyecto

> **Propósito de este documento:** Definir de forma clara y medible hacia dónde se dirige el proyecto PET Center, estableciendo un objetivo general que sirva como brújula para todas las decisiones técnicas y de negocio. Elegimos la metodología **SMART** porque nos permite tener metas concretas y verificables, fundamentales para un proyecto con plazo acotado y recursos definidos como este.

---

## 1. Objetivo General del Proyecto (SMART)

A continuación, desglosamos el objetivo en sus cinco dimensiones SMART. Cada una incluye una justificación breve de por qué se definió de esa manera.

### 1.1 Específico (Specific)

**¿Qué vamos a hacer exactamente?**

Desarrollar una plataforma web llamada **PET Center** que conecte a dueños de mascotas con proveedores verificados de servicios: veterinarias, peluquerías, paseadores, cuidadores y tiendas de productos. La plataforma permitirá buscar servicios, reservar turnos, valorar experiencias y gestionar el historial de cada mascota.

> **Justificación:** Un objetivo específico elimina la ambigüedad. En lugar de decir "hacer una app para mascotas", definimos actores (dueños, proveedores), funcionalidades concretas (búsqueda, reserva, valoración) y el tipo de plataforma (web). Esto evita desviaciones durante el desarrollo.

### 1.2 Medible (Measurable)

**¿Cómo sabremos que lo logramos?**

| Indicador | Meta | ¿Por qué esta métrica? |
|-----------|------|------------------------|
| Usuarios registrados | 50 en el primer mes | Número realista para un lanzamiento inicial, nos permite validar la aceptación del producto |
| Proveedores verificados | 15 | Mínimo necesario para ofrecer variedad de servicios y categorías |
| Reservas gestionadas | 40 simultáneas sin degradación | Garantiza que la plataforma soporta la demanda esperada en etapa temprana |
| Valoraciones recibidas | 20 reseñas | Indica que los usuarios están usando activamente el sistema de feedback |
| Disponibilidad | 99.5% en horario comercial (08:00–22:00) | Estándar aceptable para un MVP sin comprometer la experiencia del usuario |

> **Justificación:** Sin métricas, un objetivo es solo una intención. Estas cinco métricas cubren adopción (usuarios), oferta (proveedores), rendimiento técnico (reservas), engagement (valoraciones) y confiabilidad (disponibilidad).

### 1.3 Alcanzable (Achievable)

**¿Tenemos los recursos y capacidades para lograrlo?**

- El equipo domina las tecnologías seleccionadas: HTML, CSS, JavaScript, Python y Flask.
- El plazo de 8 semanas es suficiente para un MVP con las funcionalidades esenciales.
- Todas las herramientas son open-source y sin costo de licencias (Tailwind CSS, Flask, SQLite).
- El alcance se limitó deliberadamente a lo esencial: registro, perfiles, búsqueda, reserva, valoraciones y panel admin básico.

> **Justificación:** Un objetivo ambicioso pero inalcanzable genera frustración. Preferimos un alcance realista que podamos entregar con calidad, y sobre esa base escalar en futuras iteraciones.

### 1.4 Relevante (Relevant)

**¿Este objetivo importa realmente?**

Sí, porque:
- **Problema real:** Hoy los servicios para mascotas se contratan por redes sociales o contactos informales, sin garantías ni historial.
- **Mercado en crecimiento:** La industria pet ha crecido sostenidamente; los dueños buscan cada vez más servicios profesionales.
- **Valor dual:** Beneficia tanto a dueños (seguridad, organización) como a proveedores (visibilidad, gestión de agenda).

> **Justificación:** Un proyecto solo tiene sentido si resuelve un problema real. Validamos que existe una necesidad concreta y que nuestra solución aporta valor genuino a ambos lados del mercado.

### 1.5 Temporal (Time-bound)

**¿Para cuándo estará listo?**

| Hito | Semana | Entregable |
|------|--------|------------|
| Análisis y diseño | 2 | Documentación de requerimientos y arquitectura |
| Prototipo frontend | 4 | Interfaz funcional con datos mock |
| Backend completo | 6 | API REST + base de datos operativa |
| Integración y pruebas | 7 | Sistema integrado y probado |
| Despliegue final | 8 | Plataforma en producción |

> **Justificación:** Sin fecha límite, los proyectos se dilatan. Dividir en hitos semanales nos permite hacer seguimiento objetivo y corregir desvíos a tiempo.

---

## 2. Declaración del Objetivo SMART

> **"Desarrollar la plataforma web PET Center para que dueños de mascotas puedan buscar, reservar y valorar servicios de proveedores verificados, alcanzando 15 proveedores registrados y gestionando 50 reservas simultáneas, en un plazo de 8 semanas, utilizando tecnologías web open-source."**


---

## 3. Control de Versiones

Llevar un registro de versiones nos permite saber qué cambió, cuándo y por qué. Es una práctica profesional que facilita la auditoría y la colaboración.

| Versión | Fecha | Cambios realizados | Autor |
|---------|-------|--------------------|-------|
| 1.0.0 | 12-06-2026 | Creación inicial del documento con objetivo SMART | Equipo PET Center |

---

*Documento elaborado para el Parcial I — Administración de Proyectos. Cualquier sugerencia o corrección es bienvenida para mejorar la calidad de esta documentación.*