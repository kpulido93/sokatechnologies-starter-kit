# Arquitectura base

## Objetivo

Definir una arquitectura inicial simple, entendible y adaptable a distintos tipos de proyectos B2B sin acoplarla a un framework concreto.

## Principios

- Favorecer composición simple antes que capas innecesarias.
- Separar lógica de negocio, configuración, integraciones y utilidades compartidas.
- Mantener bajo acoplamiento entre módulos.
- Tratar dependencias externas como adaptadores reemplazables.
- Hacer visibles las decisiones técnicas antes de escalar la solución.

## Estructura lógica sugerida

- `src/app`: punto de entrada del proyecto, bootstrap y wiring.
- `src/config`: configuración, lectura de entorno y convenciones transversales.
- `src/modules`: dominio y casos de uso organizados por capacidad de negocio.
- `src/shared`: utilidades compartidas, tipos base y helpers reutilizables.
- `src/integrations`: conectores con APIs, servicios externos, colas o proveedores.

## Reglas de diseño

- Un módulo no debe depender de detalles internos de otro módulo.
- La configuración debe centralizarse y no dispersarse por el código.
- Las integraciones externas deben aislarse para facilitar cambios y pruebas.
- El código compartido debe mantenerse pequeño para evitar convertirse en un contenedor genérico.

## Decisiones pendientes

Antes de implementar, el proyecto debe resolver al menos:

- framework o runtime principal
- tipo de interfaz principal: API, dashboard, worker o solución híbrida
- estrategia de persistencia y modelado de datos
- autenticación y autorización
- observabilidad y manejo de errores

Registrar cada decisión en [decisions.md](/D:/repos/sokatechnologies-starter-kit/docs/decisions.md).

## Validación mínima

- La estructura soporta crecimiento modular sin asumir proveedor.
- Cada carpeta tiene una responsabilidad clara.
- Las dependencias externas quedan encapsuladas.
- Las decisiones abiertas están documentadas antes de construir.
