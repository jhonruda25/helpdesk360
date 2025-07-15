# HelpDesk360

**HelpDesk360** es una plataforma web de gestión de incidencias tipo Help Desk. Permite a los usuarios reportar problemas técnicos y al equipo de soporte asignarlos, resolverlos y dar seguimiento. Pensada para empresas que necesitan organizar y centralizar sus solicitudes de soporte técnico.

---

## 🚀 Características principales

- Registro y autenticación de usuarios (JWT)
- Creación y seguimiento de tickets de soporte
- Asignación de técnicos a cada ticket
- Panel administrativo con métricas de soporte
- Sistema de comentarios por ticket
- Arquitectura basada en microservicios
- Contenedores Docker para despliegue local o en la nube
- Pruebas unitarias en frontend y backend
- Planificación ágil con metodología SCRUM

---

## 🧠 Tecnologías utilizadas

| Área         | Tecnología               |
|--------------|---------------------------|
| Frontend     | React + Tailwind CSS      |
| Backend      | Java + Spring Boot        |
| Base de datos| PostgreSQL                |
| Autenticación| JWT                       |
| Contenedores | Docker + Docker Compose   |
| Testing      | JUnit (backend), Jest (frontend) |
| CI/CD        | GitHub Actions (opcional) |
| Gestión Ágil | Trello o Jira             |

---

## 🏗️ Estructura del repositorio

```
helpdesk360/
│
├── backend/                 # Microservicios en Spring Boot
├── frontend/                # Aplicación React
├── docker-compose.yml       # Orquestación local de servicios
├── docs/
│   └── requerimientos.md    # Documentación funcional y técnica
└── README.md
```

---

## 📦 Instalación rápida

> Requiere tener Docker y Docker Compose instalados.

```bash
git clone https://github.com/tu_usuario/helpdesk360.git
cd helpdesk360
docker-compose up --build
```

El frontend estará disponible en: `http://localhost:3000`  
El backend en: `http://localhost:8080`

---

## 📅 Planificación (SCRUM)

Plan de desarrollo dividido en 4 sprints de 1 semana cada uno:

| Sprint | Objetivo                             |
|--------|--------------------------------------|
| 1      | Login, registro, UI base             |
| 2      | Gestión de tickets y asignación      |
| 3      | Comentarios, métricas y dashboard    |
| 4      | Pruebas, mejoras, documentación final|

---

## 👤 Roles del sistema

- **Usuario final:** Crea y revisa tickets.
- **Técnico:** Atiende tickets asignados.
- **Administrador:** Gestiona usuarios y ve estadísticas.

---

## 📌 Estado del proyecto

- [x] Definición funcional
- [ ] Backend - Microservicio de usuarios
- [ ] Backend - Microservicio de tickets
- [ ] Frontend - Interfaz básica
- [ ] Autenticación JWT
- [ ] Pruebas unitarias
- [ ] Dockerización

---

## ✍️ Autor

Desarrollado por Jhonrueda25 como proyecto demostrativo para procesos de selección y mejora continua en desarrollo de software.
