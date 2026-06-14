# PET Center — Metodologías Ágiles

> **Propósito de este documento:** Definir y justificar la metodología ágil que utilizaremos para gestionar el desarrollo del proyecto PET Center. Elegir una metodología adecuada nos permite organizar el trabajo en ciclos cortos, priorizar funcionalidades según su valor y adaptarnos a los cambios sin perder el rumbo del proyecto.

---

## 1. Metodología Elegida: Scrum + Kanban (Scrumban)

Para el desarrollo de PET Center, adoptamos una **combinación de Scrum y Kanban**, conocida como **Scrumban**. Esta decisión no es arbitraria: responde a las características particulares de nuestro proyecto (equipo pequeño, plazo fijo de 8 semanas, requisitos definidos pero con espacio para ajustes).

### 1.1 ¿Por qué Scrumban y no Scrum o Kanban puros?

| Metodología | Ventajas | Limitaciones para nuestro proyecto |
|-------------|----------|-----------------------------------|
| **Scrum puro** | Roles definidos, sprints fijos, ceremonias estructuradas | ❌ Requiere dedicación exclusiva del equipo. Las ceremonias (daily, retrospectiva, planning) pueden ser excesivas para un equipo de 2 personas. |
| **Kanban puro** | Flujo continuo, flexible, sin sprints | ❌ Al no tener iteraciones fijas, es difícil alinear entregas con los hitos académicos del cuatrimestre. |
| **Scrumban** | Toma lo mejor de ambos: sprints de Scrum + visualización y límites de trabajo de Kanban | ✅ Ideal para equipos pequeños con plazos fijos pero que necesitan flexibilidad en el día a día. |

> **Justificación:** Elegimos Scrumban porque nuestro equipo es de solo 2 personas. Las ceremonias completas de Scrum (daily de 15 minutos, sprint planning de 2 horas, retrospectiva) consumirían un tiempo valioso que podemos dedicar al desarrollo. En cambio, con Scrumban mantenemos la estructura de sprints para cumplir con los hitos académicos, pero usamos un tablero Kanban para visualizar el trabajo y limitar las tareas en progreso, evitando la sobrecarga del equipo.

---

## 2. Características de nuestra implementación Scrumban

### 2.1 Roles

| Rol | Responsable | Responsabilidades |
|-----|-------------|-------------------|
| **Equipo de Desarrollo** | Gustavo Oliva y Carelis Fagundez | Diseñar, codificar, probar y documentar. Ambos compartimos la responsabilidad del producto. |
| **Product Owner** | Gustavo Oliva | Definir prioridades, validar que las funcionalidades cumplan con los requisitos, mantener la visión del producto. |
| **Facilitador** | Carelis Fagundez | Organizar las reuniones, mantener el tablero actualizado, asegurar que el equipo tenga lo necesario para trabajar. |

> **Nota:** En un equipo de 2 personas, los roles se superponen. No tenemos un Scrum Master dedicado porque el equipo es autogestionado. La clave es que ambos sepamos quién lidera cada aspecto para evitar conflictos.

### 2.2 Ciclo de trabajo (Sprints)

Trabajaremos en **sprints de 2 semanas** de duración. Esta decisión se basa en:

- **Plazo total:** 8 semanas → 4 sprints completos.
- **Hitos académicos:** Cada 2 semanas podemos presentar avances concretos.
- **Capacidad del equipo:** 2 personas pueden completar funcionalidades significativas en 2 semanas sin agotarse.

| Sprint | Semanas | Tareas incluidas |
|--------|---------|------------------|
| Sprint 1 | 1 y 2 | T01 a T07: Objetivo SMART, stakeholders, metodología ágil, requerimientos, arquitectura, entorno de desarrollo, tablero Trello |
| Sprint 2 | 3 y 4 | T08 a T17: Registro y autenticación, perfiles de cliente y proveedor, búsqueda por categorías, vista de proveedor, valoraciones, promociones |
| Sprint 3 | 5 y 6 | T18 a T29: Registro de mascotas, edición de perfil, filtro por ubicación, reserva de turnos, disponibilidad, cancelación, gestión de reservas del proveedor, calificaciones, pruebas de rendimiento y seguridad |
| Sprint 4 | 7 y 8 | T30 a T40: Panel de administración, gestión de usuarios, estadísticas, pruebas de disponibilidad, usabilidad y compatibilidad, integración frontend-backend, pruebas integrales, corrección de errores, documentación final y despliegue |

### 2.3 Tablero Kanban

Utilizaremos un tablero con las siguientes columnas:

| Columna | Descripción | Límite de tareas |
|---------|-------------|------------------|
| **Pendiente** | Tareas identificadas pero no iniciadas | Sin límite |
| **En progreso** | Tareas que se están desarrollando actualmente | Máximo 2 tareas por persona (total 4) |
| **En revisión** | Tareas terminadas que esperan validación del otro miembro | Máximo 2 |
| **Terminado** | Tareas completadas y validadas | Sin límite |

> **Justificación del límite:** Con 2 personas, tener más de 2 tareas por persona en progreso significa que ninguna se termina. El límite de 4 tareas totales nos obliga a terminar antes de empezar algo nuevo, reduciendo el trabajo a medio hacer.

### 2.4 Ceremonias (adaptadas para equipo pequeño)

| Ceremonia | Frecuencia | Duración | ¿Qué hacemos? |
|-----------|------------|----------|---------------|
| **Planificación del sprint** | Cada 2 semanas | 30 minutos | Definir qué tareas del backlog entran al sprint y quién las hace |
| **Sincronización rápida** | 2 veces por semana | 10 minutos | Contarnos en qué estamos trabajando, si tenemos bloqueos, qué sigue |
| **Revisión del sprint** | Cada 2 semanas | 20 minutos | Mostrar lo que se completó, validar que cumple con lo esperado |
| **Retrospectiva** | Cada 4 semanas | 15 minutos | Analizar qué funcionó bien y qué podemos mejorar |

> **Nota:** Redujimos las ceremonias al mínimo necesario. En un equipo de 2, una daily de 15 minutos todos los días es excesiva. Con 2 sincronizaciones semanales de 10 minutos es suficiente para mantenernos alineados.

---

## 3. Artefactos que utilizaremos

### 3.1 Product Backlog

Lista priorizada de todas las funcionalidades que necesita PET Center. Se mantiene en este repositorio de GitHub, en la carpeta de documentación.

**Criterios de priorización:**
1. **Valor para el usuario:** Lo que los clientes y proveedores necesitan primero.
2. **Dependencias técnicas:** No podemos construir B si A no está terminado.
3. **Complejidad:** Funcionalidades simples primero para generar momentum.

### 3.2 Sprint Backlog

Subconjunto del Product Backlog que seleccionamos para cada sprint. Se representa visualmente en el tablero Kanban.

### 3.3 Tablero Kanban (físico o digital)

Usaremos GitHub Projects como tablero digital, ya que está integrado con nuestro repositorio y no requiere herramientas adicionales.

### 3.4 Ajuste de la Metodología de Trabajo
**Situación detectada**

Durante el Sprint 3, el equipo observó que las funcionalidades relacionadas con la gestión de reservas (HU-13, HU-14 y HU-16) presentaban una complejidad mayor a la estimada inicialmente debido a las dependencias entre módulos y la necesidad de coordinar distintas funcionalidades del sistema.

**Riesgo identificado**

La existencia de varias tareas simultáneamente en estado "En Progreso" dificultaba la finalización de historias de usuario completas dentro del sprint, aumentando el riesgo de retrasos y generando trabajo parcialmente terminado.

**Ajuste metodológico aplicado**

Como medida preventiva, el equipo decidió priorizar la finalización de tareas antes de iniciar nuevas actividades, limitando temporalmente la cantidad de tareas simultáneas en desarrollo durante el Sprint 3.

Asimismo, se incorporó una reunión adicional de sincronización semanal con el objetivo de identificar bloqueos y dependencias de manera temprana.

**Beneficios esperados**
- Mayor foco en las funcionalidades críticas.
- Reducción de tareas parcialmente completadas.
- Mejor seguimiento del avance real del sprint.
- Disminución del riesgo de retrasos.
- Mejor coordinación entre los integrantes del equipo.

**Resultado esperado**

La adaptación propuesta permite mantener los principios ágiles de mejora continua y flexibilidad, ajustando el proceso de trabajo para responder de manera efectiva a las necesidades del proyecto sin afectar los objetivos definidos para cada sprint.

---

## 4. Control de Versiones

| Versión | Fecha | Cambios realizados | Autor |
|---------|-------|--------------------|-------|
| 1.0.0 | 13-06-2026 | Creación inicial del documento con definición de Scrumban y justificación | Equipo PET Center |
| 1.1.0 | 13-06-2026 | Actualización de la sección 2.2 con tareas concretas de cada sprint según el Product Backlog y el tablero Trello | Equipo PET Center |
| 1.2.0 | 14-06-2026 | Incorporación de la sección 3.4 Ajuste de la Metodología de Trabajo para mejorar el seguimiento y control de tareas durante el Sprint 3 | Equipo PET Center |
