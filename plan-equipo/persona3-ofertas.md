# Persona 3 — Ofertas P2P

## Branch

`feature/ofertas` ← Persona 3

## Dependencia

Persona 1 debe haber subido el proyecto a github

## Tareas

1. Clonar ambos repos

2. Crear tu branch `feature/ofertas`

3. Verificar que `TipoCambioService.cs` tenga la API key correcta

## Tus archivos

### Backend

```
Controllers/
├── OfertaController.cs
└── TipoCambioController.cs

Infrastructure/Repositories/
└── OfertaRepository.cs

Core/
├── Services/
│   └── TipoCambioService.cs
├── Interfaces/
│   ├── IOfertaRepository.cs
│   └── ITipoCambioService.cs
└── DTOs/
    ├── CrearOfertaDTO.cs
    ├── OfertaResponseDTO.cs
    ├── TomarOfertaDTO.cs
    └── MontoOperacionDTO.cs
```

### Frontend

```
src/
├── pages/
│   ├── CrearOfertaPage.vue
│   ├── OfertasPage.vue
│   └── MisOfertasPage.vue
└── services/
    ├── ofertaService.js
    └── tipoCambioService.js
```
