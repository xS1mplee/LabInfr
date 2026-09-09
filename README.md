# Laboratorio de Infraestructura como Código (IaC)

Este repositorio tiene la configuración declarativa de infraestructura mediante **Docker Compose** y **Nginx** para desplegar una arquitectura multi-contenedor con ambientes aislados de Producción y QA.

## Arquitectura del Sistema

- **Nginx (Reverse Proxy / Load Balancer):** Punto de entrada único (Puerto 80).
- **Ambiente de Producción (PROD):**
    - 2 Instancias de API Java (api-prod-1, api-prod-2) con balanceo de carga.
    -1 Base de Datos PostgreSQL (bd-produccion).
- **Ambiente de QA:**
    - 1 Instancia de API Java (`api-qa`).
    - 1 Base de Datos PostgreSQL (`bd-qa`).

