# Metodología de Auditoría QA

## 1. Propósito

Esta metodología describe el proceso utilizado para revisar y validar las funciones de un sistema empresarial, registrar los resultados de las pruebas, identificar posibles hallazgos y organizar la documentación correspondiente.

El objetivo es mantener un proceso de auditoría estructurado, con resultados trazables y documentación que facilite el seguimiento de las validaciones realizadas.

## 2. Etapas de la metodología

### Etapa 1. Revisión de la documentación

Se revisa el manual o la documentación disponible para comprender el objetivo de la función, los pasos indicados y el resultado esperado.

También se identifica si la documentación está actualizada o si requiere mejoras.

### Etapa 2. Validación del proceso en el sistema

Se ingresa a la función que se va a revisar y se compara su comportamiento con la documentación disponible.

Se identifican los campos, opciones, permisos y pasos relevantes para comprender el funcionamiento del proceso.

### Etapa 3. Ejecución de pruebas QA

Se realizan validaciones funcionales para comprobar si la opción revisada responde según lo esperado.

Las pruebas se ejecutan respetando los permisos y las condiciones de acceso autorizadas. Cuando no existe un entorno independiente de pruebas, se priorizan las validaciones que no comprometan datos ni procesos operativos.

### Etapa 4. Registro de evidencias

Se documentan los resultados observados y, cuando corresponde, se recopilan capturas u otras evidencias que permitan respaldar la validación.

Las evidencias deben estar relacionadas con la prueba realizada y evitar la exposición de información confidencial.

### Etapa 5. Registro en la matriz de auditoría

Se registra cada proceso revisado en una matriz de seguimiento. Según corresponda, esta puede incluir:

- Sistema, módulo y función revisada.
- Objetivo y descripción del proceso.
- Estado de uso identificado.
- Resultado de la prueba.
- Estado de la documentación.
- Evidencias y observaciones.
- Hallazgos y recomendaciones.

Los resultados se clasifican como **PASS**, cuando la prueba cumple el resultado esperado; **FAIL**, cuando se identifica un comportamiento que no cumple lo esperado; y **N/A**, cuando la prueba no aplica o no puede evaluarse bajo las condiciones establecidas. El motivo debe quedar documentado para evitar confusiones.

### Etapa 6. Identificación de hallazgos y recomendaciones

Cuando se identifica una diferencia entre el comportamiento esperado y el observado, se registra el hallazgo con una descripción clara de la situación.

Se plantea una recomendación cuando corresponde, procurando que permita comprender qué debe revisarse o mejorarse. La clasificación de un hallazgo debe basarse en la evidencia disponible.

### Etapa 7. Documentación y seguimiento

Se actualiza o prepara la documentación del proceso para facilitar su comprensión por parte de los usuarios.

El seguimiento de los procesos, hallazgos y recomendaciones permite mantener organizada la información y conocer el estado de las actividades pendientes.

## 3. Ejemplo ficticio de aplicación

**Proceso:** Consulta de existencias de un producto en un sistema de inventario ficticio.

**Objetivo:** Comprobar que el sistema permite consultar las existencias registradas de un producto.

**Procedimiento:**
1. Revisar el manual de consulta de inventario.
2. Ingresar a la opción de consulta de productos.
3. Buscar un producto de prueba autorizado.
4. Verificar que se muestre la información esperada.
5. Registrar el resultado y la evidencia correspondiente.
6. Actualizar la matriz de auditoría.

**Resultado de ejemplo:** PASS.

**Observación:** La consulta mostró las existencias registradas para el producto utilizado en la prueba.

*Este ejemplo es ficticio y se incluye únicamente para explicar la metodología. No representa resultados de una auditoría real.*

## 4. Herramientas de apoyo

- **Excel:** organización y análisis de matrices de auditoría.
- **SharePoint:** almacenamiento y organización de documentación y registros.
- **Power BI:** visualización de indicadores de avance y resultados.
- **Power Automate:** automatización de actividades de seguimiento, cuando los flujos correspondientes están configurados.
- **GitHub:** documentación del proyecto y presentación de ejemplos no confidenciales en el portafolio.

## 5. Principios de trabajo

- Mantener trazabilidad entre proceso, prueba, resultado y evidencia.
- Registrar los resultados de forma objetiva.
- Diferenciar los problemas funcionales de las limitaciones de acceso.
- No clasificar una función como obsoleta únicamente porque tenga poco uso.
- Respetar los permisos y evitar acciones que puedan afectar la operación.
- Proteger la información interna y utilizar ejemplos ficticios en el portafolio público.
