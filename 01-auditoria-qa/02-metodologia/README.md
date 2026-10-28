# Metodología de Auditoría QA de Sistemas Empresariales

## 1. Objetivo

Establecer una metodología de auditoría QA para revisar las funciones de un sistema empresarial, contrastar su funcionamiento con la documentación disponible, ejecutar pruebas funcionales, registrar evidencias, identificar hallazgos y organizar las recomendaciones y la documentación de los procesos.

La metodología permite mantener trazabilidad sobre los procesos revisados, los resultados obtenidos y las mejoras identificadas durante la auditoría.

## 2. Flujo de trabajo de la auditoría

El proceso se desarrolla mediante las siguientes etapas:

**Manual → Sistema → Seguridad → Prueba QA → Evidencia → Matriz de auditoría → Hallazgo → Recomendación → Documentación y seguimiento**

### Etapa 1. Revisión del manual

Se revisa el manual disponible para identificar el objetivo de la función, los pasos descritos y el resultado esperado.

Durante esta revisión se determina si existe documentación, si corresponde al proceso que se está evaluando y si requiere actualización o elaboración.

**Se registra:** el objetivo del proceso, la documentación disponible y las observaciones iniciales.

### Etapa 2. Revisión de la función en el sistema

Se localiza la función que se va a auditar y se revisa su comportamiento real, sus opciones, campos y pasos de ejecución.

Se compara lo observado con las instrucciones del manual para identificar diferencias entre la documentación y el funcionamiento del sistema.

**Se registra:** el proceso revisado, su funcionamiento y las diferencias identificadas.

### Etapa 3. Revisión de seguridad y accesos

Se consulta la información disponible en la herramienta de seguridad para comprender los accesos asociados a la función y las restricciones que puedan afectar su validación.

Esta revisión ayuda a distinguir una limitación de permisos de un problema funcional. Un mensaje de acceso denegado no demuestra, por sí solo, que una función esté en desuso.

**Se registra:** la información relevante sobre accesos, permisos y restricciones.

### Etapa 4. Ejecución de pruebas QA

Se realizan pruebas funcionales para comprobar el comportamiento de la función y contrastarlo con el resultado esperado.

Debido a que no se disponía de un entorno independiente de pruebas, las validaciones se efectuaron bajo las condiciones de acceso autorizadas, evitando acciones que pudieran afectar los datos o la operación.

Cada prueba se clasifica según el resultado observado:

- **PASS:** el comportamiento cumple con lo esperado.
- **FAIL:** se identifica una diferencia o un comportamiento que no cumple con lo esperado.
- **N/A:** la prueba no aplica o no puede evaluarse bajo las condiciones disponibles; se documenta el motivo.

**Se registra:** la prueba realizada, el resultado y las observaciones correspondientes.

### Etapa 5. Recopilación de evidencias

Se recopilan las evidencias necesarias para respaldar las pruebas y los resultados registrados.

La evidencia permite relacionar lo observado en el sistema con la prueba ejecutada y facilita la revisión posterior de los resultados.

**Se registra:** la evidencia asociada a cada proceso o prueba, respetando la confidencialidad de la información.

### Etapa 6. Registro en la matriz de auditoría

La información recopilada se organiza en la matriz de auditoría, que funciona como registro central para controlar los procesos revisados y sus resultados.

Según corresponda, la matriz contempla:

- Sistema, módulo, menú y proceso.
- Uso identificado: activo, normal, posible desuso o no usado.
- Objetivo del proceso.
- Fecha de creación o último acceso, cuando está disponible.
- Validez del flujo.
- Estado del manual.
- Prueba realizada y resultado PASS, FAIL o N/A.
- Hallazgo, recomendación, observaciones y evidencia.

La clasificación de uso se determina a partir de la información disponible y no únicamente por la frecuencia de utilización. Asimismo, una función relacionada con un proceso no necesariamente forma parte de su flujo principal.

La matriz se actualiza durante el trabajo de auditoría para mantener la trazabilidad de cada revisión.

### Etapa 7. Registro de hallazgos

Cuando la revisión identifica un problema, una diferencia funcional, una inconsistencia documental u otra situación que requiere atención, se registra el hallazgo correspondiente.

La descripción debe explicar qué se observó y en qué consiste la situación identificada, con respaldo en la evidencia disponible.

No todas las pruebas generan hallazgos. Los resultados satisfactorios también se documentan para mantener un registro completo de la auditoría.

### Etapa 8. Elaboración de recomendaciones

A partir de los hallazgos, se plantean recomendaciones orientadas a corregir o mejorar la situación identificada.

Las recomendaciones deben ser claras y estar relacionadas con el hallazgo que las origina. Cuando no corresponde proponer una mejora, no se debe crear una recomendación artificial.

### Etapa 9. Documentación y seguimiento

Finalmente, se actualiza la documentación existente o se prepara un manual cuando es necesario describir un proceso que no cuenta con instrucciones suficientes.

La documentación busca facilitar la comprensión del proceso mediante su contexto, explicación, pasos de ejecución y evidencias ilustrativas cuando corresponde.

Los registros de procesos, hallazgos, recomendaciones y seguimiento permiten organizar las actividades pendientes y consultar el estado de las revisiones.

## 3. Ejemplo ficticio de aplicación

**Proceso:** Consulta de existencias en un sistema ficticio de inventario.

1. **Manual:** se revisan las instrucciones disponibles para consultar las existencias.
2. **Sistema:** se localiza la función y se comprueba cómo presenta la información.
3. **Seguridad:** se revisan los accesos disponibles para la función.
4. **Prueba QA:** se ejecuta una consulta autorizada y se compara el resultado con lo esperado.
5. **Evidencia:** se registra el resultado observado.
6. **Matriz:** se documentan el proceso, la prueba y su resultado.
7. **Hallazgo:** se registra únicamente si se identifica una situación que requiere atención.
8. **Recomendación:** se propone una mejora si el hallazgo lo amerita.
9. **Documentación y seguimiento:** se actualizan las instrucciones y se registra el estado de las actividades correspondientes.

Este ejemplo es ficticio y tiene fines demostrativos; no representa resultados de una auditoría real.

## 4. Herramientas de apoyo

- **Sistema empresarial:** revisión y validación de las funciones auditadas.
- **Herramienta de seguridad:** consulta de accesos y restricciones.
- **Excel:** organización y análisis de la matriz de auditoría.
- **SharePoint:** organización de documentación y registros de seguimiento.
- **Power BI:** visualización de indicadores de avance y resultados.
- **Power Automate:** apoyo en los flujos de seguimiento que se encuentren efectivamente configurados.
- **GitHub:** documentación del proyecto y presentación de ejemplos no confidenciales.

## 5. Criterios de la auditoría

- Mantener relación entre el proceso revisado, la prueba, el resultado y su evidencia.
- Diferenciar las limitaciones de acceso de los problemas funcionales.
- Registrar los resultados observados sin asumir causas que no hayan sido comprobadas.
- Justificar la clasificación de uso con información disponible.
- Documentar las limitaciones que afecten la ejecución de una prueba.
- Mantener la matriz actualizada durante la auditoría.
- Proteger la información interna y utilizar ejemplos ficticios en el portafolio público.
