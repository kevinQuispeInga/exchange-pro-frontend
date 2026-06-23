# Plan de Trabajo — 5 Personas, 2 Repos

## Estructura

```
github.com/tu-org/exchange-pro-backend   (backend ASP.NET)
github.com/tu-org/exchange-pro-frontend  (frontend Quasar)
```

## Branches

```
main (estable, solo se mergea desde develop)
 └─ develop (todos mergean aquí)
     ├─ feature/auth            ← Persona 1
     ├─ feature/wallet          ─ Persona 2
     ├─ feature/ofertas         ─ Persona 3
     ├─ feature/transacciones   ─ Persona 4
     └─ feature/admin           ─ Persona 5
```

## Regla de oro

Cada persona solo modifica **sus archivos**. Así nunca hay conflictos al mergear.

---

## Planes individuales

Cada persona tiene su propio archivo en `plan-equipo/`:

| Archivo | Para |
|---|---|
| `plan-equipo/persona1-auth.md` | Persona 1 — Autenticación |
| `plan-equipo/persona2-wallet.md` | Persona 2 — Wallet |
| `plan-equipo/persona3-ofertas.md` | Persona 3 — Ofertas |
| `plan-equipo/persona4-transacciones.md` | Persona 4 — Transacciones |
| `plan-equipo/persona5-admin.md` | Persona 5 — Admin |
