# Persona 1 — Autenticación & Base

## Branch
`feature/auth` ← Persona 1

## Dependencia
Ninguna. Eres la base de todo el proyecto.

---

## Tareas

1. Crear los 2 repos en GitHub (vacíos):
   - `github.com/tu-org/exchange-pro-backend`
   - `github.com/tu-org/exchange-pro-frontend`

2. Subir el proyecto completo a `develop`:

**Backend**
```bash
git init
git add .
git commit -m "feat: backend completo"
git branch -M main
git remote add origin https://github.com/tu-org/exchange-pro-backend.git
git push -u origin main

git checkout -b develop
git push -u origin develop

git checkout -b feature/auth
git push -u origin feature/auth
```

**Frontend**
```bash
git init
git add .
git commit -m "feat: frontend completo"
git branch -M main
git remote add origin https://github.com/tu-org/exchange-pro-frontend.git
git push -u origin main

git checkout -b develop
git push -u origin develop

git checkout -b feature/auth
git push -u origin feature/auth
```

3. Ejecutar `database/script-completo.sql` en tu SQL Server
4. Correr scaffold (Database-First) para regenerar entidades
5. Verificar que el proyecto compila y corre

---

## Tus archivos

### Backend
```
Controllers/
├── AuthController.cs

Core/
├── Services/
│   └── AuthService.cs
├── Interfaces/
│   ├── IAuthService.cs
│   └── IUsuarioRepository.cs
├── DTOs/
│   ├── RegistroDTO.cs
│   ├── LoginDTO.cs
│   └── AuthResponseDTO.cs

Infrastructure/Repositories/
└── UsuarioRepository.cs

Program.cs
appsettings.json
database/
└── script-completo.sql
```

### Frontend
```
src/
├── pages/
│   ├── LoginPage.vue
│   ├── RegisterPage.vue
│   ├── IndexPage.vue
│   ├── ErrorNotFound.vue
│   ├── ForgotPasswordPage.vue
│   └── ResetPasswordPage.vue
├── layouts/
│   ├── MainLayout.vue
│   └── AdminLayout.vue
├── stores/
│   └── authStore.js
├── services/
│   ├── api.js
│   └── authService.js
├── router/
│   ├── routes.js
│   └── index.js
└── utils/
    └── formatCurrency.js
```

---

## Cronograma

```
Día 1: Subes todo a develop.
       Los demás clonan desde tus repos.

Días 2-4: Todos trabajan en paralelo en sus branches.

Día 3-4: Cada uno hace PR a develop.
         Tú revisas y apruebas los PRs.

Día 5: develop → main.
```

## Posibles conflictos

| Situación | Solución |
|---|---|
| Necesitas agregar una columna a la BD | Escribe el script SQL, ejecútalo, re-scaffoldea y súbelo |
| Alguien modifica un archivo que no le pertenece | No pasa, cada uno tiene los suyos asignados |
| Al mergear hay conflictos | Como cada uno toca archivos distintos, git mergea automáticamente |

---

## Al terminar
PR `feature/auth` → `develop` en **ambos repos** y avisa a los demás.
