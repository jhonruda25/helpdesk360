# Documento de Requerimientos - HelpDesk360

---

## 1. Descripción General

**HelpDesk360** es una plataforma de gestión de solicitudes e incidencias técnicas (tipo Help Desk). Los usuarios podrán registrar problemas, los técnicos gestionarlos y los administradores visualizar métricas. El sistema busca optimizar los tiempos de respuesta, priorización de tickets y trazabilidad del soporte.

---

## 2. Objetivos del sistema

- Gestionar incidencias y requerimientos técnicos.
- Agilizar la asignación y resolución de tickets.
- Generar trazabilidad de cada solicitud.
- Permitir la supervisión del equipo técnico.
- Ofrecer métricas sobre el soporte entregado.

---

## 3. Alcance

✔️ Lo que incluye:
- Registro y login con JWT
- CRUD de tickets
- Asignación de técnicos
- Comentarios por ticket
- Panel de métricas
- Gestión de usuarios (admin)

❌ Lo que no incluye (por ahora):
- Integración con WhatsApp o chat en tiempo real
- Portal móvil nativo

---

## 4. Requerimientos Funcionales

| ID  | Requerimiento                                         |
|-----|--------------------------------------------------------|
| RF1 | El usuario debe poder registrarse y autenticarse      |
| RF2 | El usuario puede crear, ver y comentar sus tickets    |
| RF3 | El técnico debe ver tickets asignados y actualizarlos |
| RF4 | El administrador puede gestionar usuarios y técnicos  |
| RF5 | El sistema debe enviar métricas al panel admin        |
| RF6 | El sistema debe permitir comentarios por ticket       |

---

## 5. Requerimientos No Funcionales

| ID  | Requerimiento                                                |
|-----|---------------------------------------------------------------|
| RNF1| El sistema debe funcionar en navegadores modernos             |
| RNF2| El backend debe ser escalable con microservicios              |
| RNF3| Toda la comunicación debe usar HTTPS y JWT                    |
| RNF4| Debe ser dockerizado para entornos de prueba y producción     |
| RNF5| La interfaz debe responder en menos de 2 segundos             |

---

## 6. Reglas del negocio

- Un técnico no puede editar tickets que no le han sido asignados.
- Un ticket no puede cerrarse sin al menos un comentario de resolución.
- Los tickets deben tener estados: `pendiente`, `en progreso`, `resuelto`.

---

## 7. Usuarios del sistema

| Rol          | Permisos principales                                                  |
|--------------|-----------------------------------------------------------------------|
| Usuario      | Crear tickets, ver estado, comentar                                   |
| Técnico      | Ver tickets asignados, actualizar estado, comentar                    |
| Administrador| Ver todos los tickets, asignar técnicos, ver métricas, gestionar roles|

---

## 8. Diagramas (futuro)

📌 Se incluirán diagramas de:
- Caso de uso
- Flujo de navegación
- Arquitectura lógica (microservicios)

---

## 9. Supuestos

- Todos los usuarios tienen correo corporativo.
- Se usará PostgreSQL como base de datos principal.
- Se usará GitHub como repositorio central.
