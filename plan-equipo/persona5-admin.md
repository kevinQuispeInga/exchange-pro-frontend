# Persona 5 — Admin, Perfil, Notificaciones

## Branch

`feature/admin` ← Persona 5

## Dependencia

Persona 1 debe haber subido el proyecto a github

## Tareas

1. Clonar ambos repos

2. Crear tu branch `feature/admin`

## Tus archivos

### Backend

```
Controllers/
├── AdminController.cs
├── PerfilController.cs
├── NotificacionesController.cs
└── ReporteController.cs

Core/
├── Services/
│   └── AdminService.cs
├── Interfaces/
│   ├── IAdminService.cs
│   └── INotificacionesRepository.cs
└── DTOs/
    ├── PerfilResponseDTO.cs
    └── ActualizarPerfilDTO.cs
```

### Frontend

```
src/
├── pages/
│   ├── AdminDashboardPage.vue
│   ├── AdminReportesPage.vue
│   ├── AdminDisputasPage.vue
│   ├── AdminFeedbackPage.vue
│   ├── PerfilPage.vue
│   └── NotificacionesPage.vue
└── services/
    ├── perfilService.js
    ├── adminService.js
    └── notificacionesService.js
```
