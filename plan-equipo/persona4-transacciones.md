# Persona 4 — Transacciones, Disputas, Feedback

## Branch

`feature/transacciones` ← Persona 4

## Dependencia

Persona 1 (auth) y Persona 3 (ofertas) deben haber subido el proyecto a github

## Tareas

1. Clonar ambos repos

2. Crear tu branch `feature/transacciones`

**Nota importante**: Las transacciones las **crea** Persona 3 (OfertaController). Tú solo las consultas, muestras y actualizas estado.

## Tus archivos

### Backend

```
Controllers/
├── TransaccionController.cs
├── DisputaController.cs
├── FeedbackController.cs
└── CalificacionController.cs

Infrastructure/Repositories/
└── TransaccionRepository.cs

Core/
├── Interfaces/
│   ├── ITransaccionRepository.cs
│   ├── IDisputaRepository.cs
│   ├── IFeedbackRepository.cs
│   └── ICalificacionRepository.cs
└── DTOs/
    ├── TransaccionResponseDTO.cs
    ├── TransaccionDetalleDTO.cs
    ├── CrearDisputaDTO.cs
    └── FeedbackDTO.cs
```

### Frontend

```
src/
├── pages/
│   ├── TransaccionesPage.vue
│   ├── TransaccionDetallePage.vue
│   ├── DisputasPage.vue
│   └── UserFeedbackPage.vue
└── services/
    ├── transaccionService.js
    ├── disputaService.js
    └── feedbackService.js
```
