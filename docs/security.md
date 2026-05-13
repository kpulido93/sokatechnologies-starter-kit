# Seguridad

## Objetivo

Establecer controles mínimos de seguridad desde el inicio del proyecto, incluso antes de elegir stack o infraestructura.

## Reglas base

- No guardar secretos, credenciales ni tokens en el repositorio.
- No reutilizar datos reales de clientes en entornos de desarrollo o prueba.
- Aplicar principio de mínimo privilegio para accesos humanos y de sistema.
- Revisar integraciones externas antes de conectarlas a datos sensibles.
- Registrar decisiones de seguridad relevantes junto con el contexto del proyecto.

## Controles mínimos recomendados

- Gestión de secretos en un sistema externo al repositorio.
- Separación de entornos y accesos.
- Revisión de permisos para usuarios, servicios e integraciones.
- Trazabilidad básica de cambios operativos.
- Estrategia de logs y alertas acorde al riesgo del proyecto.
- Validación de dependencias cuando se incorporen en el futuro.

## Datos e integraciones

- Clasificar qué datos manejará el sistema antes de implementarlo.
- Identificar si existirán datos personales, financieros o confidenciales.
- Documentar origen, destino y permisos de cada integración externa.
- Evitar copiar información de clientes entre proyectos.

## Checklist inicial

- Los ejemplos de entorno usan valores ficticios.
- No existen secretos en commits ni documentación.
- Las decisiones de autenticación y autorización siguen abiertas o documentadas.
- Las integraciones previstas están inventariadas.
- El responsable del proyecto conoce las exigencias regulatorias aplicables.
