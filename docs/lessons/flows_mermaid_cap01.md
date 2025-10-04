# Flujos de trabajo — Lección 1

## Registro de cuenta
```mermaid
graph TD
  A[apphive.io] -->|Get Started| B(Login)
  B -->|Create one| C(Registro)
  C --> D{Método}
  D -->|Facebook/Google/Email| E[Completar datos]
  E --> F[Verificar teléfono por SMS]
  F --> G[Cuenta creada]
```

## Creación de proyecto y apps
```mermaid
graph TD
  A[Dashboard] --> B[Project's name]
  B --> C[Start without template]
  C --> D[Icono + Plan Free]
  D --> E[Create]
  E --> F[Editor]
  F --> G[Project dashboard]
  G --> H[New app (Anunciante/Admin)]
```