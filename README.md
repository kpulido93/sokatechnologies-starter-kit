# SokaTechnologies Starter Kit

Starter kit base para iniciar proyectos B2B de SokaTechnologies sin acoplar el repositorio a un framework, proveedor cloud o caso de uso concreto.

## Objetivo

Este repositorio existe para acelerar el arranque de proyectos de:

- software a medida
- dashboards y herramientas internas
- integraciones con terceros
- automatizaciones y sistemas operativos de negocio

El alcance de esta base es deliberadamente limitado: estructura, documentación y convenciones iniciales. No incluye código funcional ni dependencias.

## Qué incluye

- Estructura de carpetas para aplicación, configuración, módulos, código compartido e integraciones.
- Documentación inicial para arquitectura, seguridad, despliegue y decisiones técnicas.
- Checklists reutilizables para arranque de proyecto y onboarding de cliente.
- Plantilla de variables de entorno con valores ficticios.
- Reglas operativas para que Codex mantenga el repositorio con criterio.

## Principios del starter kit

- Mantener la base simple, pequeña y revisable.
- No asumir stack técnico antes de validar el contexto del proyecto.
- No almacenar secretos, credenciales ni datos de clientes.
- Separar claramente configuración, dominio, integraciones y utilidades compartidas.
- Documentar decisiones pendientes antes de implementar.
- Preparar la base para pruebas, despliegue y mantenimiento desde el inicio.

## Estructura inicial

```text
.
|-- AGENTS.md
|-- README.md
|-- .env.example
|-- .gitignore
|-- docs/
|   |-- architecture.md
|   |-- client-onboarding.md
|   |-- decisions.md
|   |-- deployment.md
|   |-- project-checklist.md
|   `-- security.md
|-- scripts/
|   |-- deployment/
|   |-- maintenance/
|   `-- setup/
|-- src/
|   |-- app/
|   |-- config/
|   |-- integrations/
|   |-- modules/
|   `-- shared/
`-- tests/
    |-- e2e/
    |-- integration/
    `-- unit/
```

## Cómo usar este starter kit

1. Crear un repositorio nuevo a partir de esta base o copiar su estructura al proyecto inicial.
2. Revisar `docs/decisions.md` y cerrar primero las decisiones de stack, despliegue, seguridad y datos.
3. Actualizar `README.md` con el contexto del proyecto real cuando exista alcance aprobado.
4. Completar `.env.example` con las variables realmente necesarias, siempre con valores ficticios.
5. Añadir implementación solo cuando la estructura, las reglas y las decisiones técnicas estén claras.

## Flujo recomendado

1. Definir objetivo, alcance, usuarios y restricciones del cliente.
2. Completar `docs/client-onboarding.md` y `docs/project-checklist.md`.
3. Resolver decisiones abiertas en `docs/decisions.md`.
4. Diseñar la arquitectura base en `docs/architecture.md`.
5. Establecer requisitos de seguridad y despliegue antes de escribir código.

## Reglas importantes

- No instalar dependencias en esta fase.
- No añadir código de ejemplo que parezca implementación real.
- No incorporar convenciones específicas de Node, Python, Java, .NET u otro stack salvo que el proyecto lo exija.
- No incluir nombres, accesos o datos de clientes.

## Estado actual

La estructura actual está pensada como punto de partida. Quedan pendientes, entre otras, estas decisiones:

- framework o runtime principal
- estrategia de autenticación y autorización
- proveedor de hosting o infraestructura
- base de datos y almacenamiento
- pipeline de CI/CD
- observabilidad, backups y soporte operativo

Estas decisiones se documentan en [docs/decisions.md](/D:/repos/sokatechnologies-starter-kit/docs/decisions.md).
