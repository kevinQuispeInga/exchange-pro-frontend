# Persona 2 — Wallet, Recargas, Retiros, Datos de Pago

## Branch

`feature/wallet` ← Persona 2

## Dependencia

Persona 1 debe haber subido el proyecto a github

## Tareas

1. Clonar ambos repos

2. Crear tu branch `feature/wallet`

## Tus archivos

### Backend

```
Controllers/
├── WalletController.cs
├── RetiroController.cs
├── DatosPagoController.cs
└── MovimientoWalletController.cs

Infrastructure/Repositories/
└── RecargaRepository.cs

Core/
├── Interfaces/
│   └── IRecargaRepository.cs
└── DTOs/
    ├── RecargaDTO.cs
    ├── SolicitarRetiroDTO.cs
    ├── MovimientoWalletResponseDTO.cs
    └── DatosPagoResponseDTO.cs
```

### Frontend

```
src/
├── pages/
│   ├── WalletPage.vue
│   └── DatosPagoPage.vue
├── stores/
│   └── walletStore.js
├── services/
│   ├── walletService.js
│   ├── retiroService.js
│   ├── movimientoWalletService.js
│   └── datosPagoService.js
└── components/
    └── EmptyState.vue
```
