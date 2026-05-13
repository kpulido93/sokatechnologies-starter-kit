# Decisiones técnicas

## Objetivo

Registrar decisiones técnicas y operativas del proyecto antes de convertir el starter kit en una implementación concreta.

## Cómo usar este documento

- Añadir una entrada por cada decisión relevante.
- Mantener el estado actualizado: pendiente, aprobada, descartada.
- Incluir contexto suficiente para entender por qué se tomó la decisión.
- Referenciar riesgos, impacto y próximos pasos.

## Plantilla sugerida

| Tema | Estado | Contexto | Opciones | Decisión | Responsable |
| --- | --- | --- | --- | --- | --- |
| Ejemplo | Pendiente | Describir necesidad o restricción | Opción A / Opción B | Por definir | Equipo |

## Pendientes iniciales

| Tema | Estado | Contexto | Opciones | Decisión | Responsable |
| --- | --- | --- | --- | --- | --- |
| Runtime o framework principal | Pendiente | El starter kit no debe asumir stack por defecto | Node.js, Python, .NET, Java, otro | Por definir según proyecto | Equipo |
| Tipo de aplicación base | Pendiente | El proyecto puede requerir API, dashboard, worker o combinación | API, web, worker, monolito modular | Por definir según alcance | Equipo |
| Base de datos y almacenamiento | Pendiente | No todos los proyectos necesitan la misma persistencia | SQL, NoSQL, archivos, servicios gestionados | Por definir según datos y volumen | Equipo |
| Autenticación y autorización | Pendiente | El modelo de acceso depende del cliente y usuarios finales | SSO, credenciales internas, proveedor externo | Por definir según seguridad requerida | Equipo |
| Proveedor de infraestructura | Pendiente | No se debe asumir cloud ni on-premise | AWS, Azure, GCP, on-premise, híbrido | Por definir según cliente | Equipo |
| CI/CD y estrategia de release | Pendiente | Aún no existe pipeline de validación ni despliegue | GitHub Actions, Azure DevOps, GitLab CI, otro | Por definir según entorno | Equipo |
| Observabilidad y soporte | Pendiente | Deben definirse logs, métricas, alertas y ownership | Stack centralizado o servicios gestionados | Por definir según operación | Equipo |
| Backups y recuperación | Pendiente | Debe existir estrategia para sistemas con datos persistentes | Snapshots, backups programados, réplica | Por definir según criticidad | Equipo |

## Criterio de cierre

No implementar componentes base sensibles sin haber resuelto y documentado primero las decisiones que los afectan.
