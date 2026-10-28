# Seguimiento de hallazgos y automatización

Los ejemplos de este documento son ficticios y se crearon solo con fines demostrativos. No corresponden a ningún sistema ni empresa real.

## 1. Objetivo

Mantener organizados los procesos revisados, los hallazgos y las recomendaciones, de modo que cada situación identificada tenga un responsable, un estado y una fecha de revisión.

## 2. Organización de la información en SharePoint

La información de la auditoría se organiza en listas relacionadas entre sí:

| Lista | Qué registra |
|---|---|
| Procesos | Proceso revisado, módulo, uso identificado y estado del manual |
| Casos de prueba | Prueba realizada, resultado (PASS / FAIL / N/A) y evidencia |
| Hallazgos | Descripción, tipo, prioridad, responsable y estado |
| Recomendaciones | Mejora propuesta y hallazgo que la origina |
| Riesgos | Posible impacto de una situación identificada |

## 3. Ejemplo ficticio de seguimiento de hallazgos

| ID | Proceso | Tipo | Descripción | Prioridad | Responsable | Estado |
|---|---|---|---|---|---|---|
| H-001 | Registro de productos | Documental | El manual no describe un campo nuevo | Media | Responsable de documentación | En revisión |
| H-002 | Consulta de movimientos | Usabilidad | No se indican los campos obligatorios | Alta | Responsable de sistemas | Pendiente |
| H-003 | Reporte mensual de ventas | Por confirmar | No se pudo validar con los accesos disponibles | Baja | Área usuaria | Pendiente de confirmación |

**Estados posibles:** Pendiente → En revisión → Corregido → Verificado.

## 4. Automatización con Power Automate

Power Automate apoya el seguimiento mediante flujos que reducen las tareas manuales:

| Evento | Acción automática |
|---|---|
| Se registra un nuevo hallazgo | Se notifica al responsable asignado |
| Un hallazgo cambia de estado | Se actualiza el registro y se avisa a quien lo reporta |
| Una revisión pendiente supera su fecha | Se envía un recordatorio |

## 5. Visualización del avance con Power BI

Los datos de las listas alimentan indicadores como:

- Procesos revisados frente a procesos pendientes.
- Resultados de pruebas por tipo (PASS, FAIL, N/A).
- Hallazgos por tipo y por estado.
- Avance general de la auditoría.

Los indicadores se presentan en la sección de resultados del repositorio con datos ficticios.

## 6. Criterios de seguimiento

- Cada hallazgo tiene un responsable y un estado.
- Los cambios de estado se registran para mantener la trazabilidad.
- Las limitaciones de acceso no se registran como fallas funcionales.
- Los datos publicados en este portafolio son ficticios o anonimizados.
