# Matriz de auditoría y casos de prueba

Los datos de este documento son ficticios y se crearon solo con fines demostrativos. No corresponden a ningún sistema ni empresa real.

## 1. Matriz de auditoría (ejemplo)

| Módulo | Menú | Proceso | Objetivo (según manual) | Uso | Flujo válido | Manual actualizado | Prueba ejecutada | Resultado | Hallazgo | Recomendación |
|---|---|---|---|---|---|---|---|---|---|---|
| Inventario | Mantenimientos | Registro de productos | Crear y editar productos del catálogo | Activo | Sí | No | Consulta de un registro existente | PASS | Documental: el manual no describe un campo nuevo | Actualizar el manual y las capturas |
| Inventario | Consultas | Consulta de existencias | Consultar el stock por bodega | Activo | Sí | Sí | Consulta por bodega | PASS | Sin hallazgo | Sin recomendación |
| Inventario | Consultas | Consulta de movimientos | Ver entradas y salidas por producto | Normal | Sí | Sí | Consulta sin llenar campos obligatorios | FAIL | Usabilidad: no indica qué campos se deben llenar | Resaltar los campos obligatorios y mostrar un mensaje claro |
| Ventas | Reportes | Reporte mensual de ventas | Generar el resumen de ventas del mes | Posible desuso | Sin verificar | No | No se pudo ejecutar con los accesos disponibles | N/A | Sin hallazgo | Confirmar con el área usuaria si el reporte sigue vigente |
| Ventas | Movimientos | Anulación de pedidos | Anular pedidos registrados por error | Poco uso | Sí | Sí | Validación del mensaje de bloqueo | PASS | Sin hallazgo | Sin recomendación |

## 2. Cómo se interpreta

- **PASS:** el comportamiento cumple con lo esperado.
- **FAIL:** hay una diferencia o un comportamiento que no cumple con lo esperado.
- **N/A:** la prueba no aplica o no pudo evaluarse; se documenta el motivo.
- Un resultado PASS puede tener un hallazgo documental sin que el proceso falle.
- Una limitación de acceso no se registra como falla funcional.

## 3. Caso de prueba (ejemplo)

| Campo | Detalle |
|---|---|
| Código | CP-001 (ficticio) |
| Proceso | Consulta de movimientos |
| Objetivo | Verificar que la consulta muestre las entradas y salidas de un producto |
| Condición previa | Usuario con permiso de consulta |
| Pasos | 1. Abrir la consulta. 2. Dejar vacío el campo de producto. 3. Ejecutar la consulta |
| Resultado esperado | El sistema indica qué dato falta |
| Resultado obtenido | No aparece ningún mensaje ni indicación |
| Estado | FAIL |
| Evidencia | Captura de pantalla (se omite en el ejemplo público) |
| Tipo de hallazgo | Usabilidad |
| Recomendación | Mostrar un mensaje que indique los campos requeridos |
