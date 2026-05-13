# Despliegue

## Objetivo

Documentar una base neutral para despliegue y operación sin fijar todavía infraestructura, proveedor cloud ni pipeline.

## Principios de despliegue

- Mantener entornos separados cuando el proyecto los requiera.
- Gestionar configuración y secretos fuera del repositorio.
- Permitir despliegues repetibles y reversibles.
- Evitar cambios manuales no documentados.
- Validar el comportamiento mínimo antes de promover cambios entre entornos.

## Contenido esperado cuando el proyecto avance

- definición de entornos
- estrategia de build y empaquetado
- pipeline de validación y release
- gestión de variables de entorno y secretos
- procedimiento de rollback
- responsables operativos y ventanas de despliegue

## Checklist base

- La infraestructura elegida está documentada.
- El proceso de despliegue está versionado.
- Los secretos se inyectan desde una plataforma segura.
- Existe un procedimiento de rollback o recuperación.
- Se definen logs, métricas y alertas mínimas.

## Pendientes deliberados

Este starter kit no define todavía:

- proveedor de hosting
- contenedores o serverless
- CI/CD concreto
- estrategia de migraciones
- backups, retención y recuperación

Estas decisiones deben resolverse y registrarse en [decisions.md](/D:/repos/sokatechnologies-starter-kit/docs/decisions.md) antes de automatizar despliegues.
