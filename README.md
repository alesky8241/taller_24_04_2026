# Repositorio para el taller de Ampliación de Entornos - CI/CD con GitHub Actions.

## 📦 Archivos principales para CI/CD con Docker y GitHub Actions

### 1. `.github/workflows/ci-cd.yml`
Pipeline de CI/CD usando GitHub Actions.

- Automatiza procesos al hacer cambios en el repositorio
- Permite integrar testing, build y despliegue continuo
- Construye la imagen Docker
- Publica la imagen en un registro como GHCR (gitHub Container Registry)

---

### 2. `Dockerfile`
Define cómo se construye la imagen Docker de la aplicación.

- Describe el entorno de ejecución (imagen base)
- Indica qué archivos se incluyen en la imagen
- Define cómo se arranca la aplicación dentro del contenedor

---

### 3. `docker-compose.yml`
Define y orquesta múltiples servicios Docker.

- Permite levantar varios contenedores (app, base de datos, etc.)
- Centraliza la configuración de red, volúmenes y dependencias
- Facilita el entorno de desarrollo y pruebas local

---

### 4. `.env.example`
Plantilla de variables de entorno necesarias para la aplicación.

- Documenta qué variables son requeridas
- Sirve como base para crear un `.env` real (no versionado)
- Evita exponer credenciales sensibles en el repositorio

---

## Resumen
- `.github/workflows/ci-cd.yml` → automatización CI/CD
- `Dockerfile` → construcción de la imagen    
- `docker-compose.yml` → orquestación de servicios  
- `.env.example` → plantilla de configuración (se usará en docker-compose.yml)

