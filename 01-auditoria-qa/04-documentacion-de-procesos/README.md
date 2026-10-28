# Documentación de procesos y manuales

Los ejemplos de este documento son ficticios y se crearon solo con fines demostrativos. No corresponden a ningún sistema ni empresa real.

 1. Criterios para documentar un proceso

Durante la auditoría, la documentación se revisa, se actualiza o se elabora según lo observado al comparar el manual con el sistema:

- **Existe y está vigente:** se conserva y se registra como actualizado en la matriz.
- **Existe, pero está desactualizado:** se corrige para reflejar el funcionamiento real.
- **No existe o es insuficiente:** se elabora un manual nuevo.

## 2. Estructura de un manual de usuario

Cada manual sigue la misma estructura para que sea fácil de consultar:

1. Objetivo del proceso
2. Alcance y a quién va dirigido
3. Requisitos y permisos necesarios
4. Pasos de ejecución
5. Resultado esperado
6. Situaciones frecuentes y mensajes del sistema
7. Control de versiones

## 3. Ejemplo ficticio de manual

### Manual de usuario: Consulta de existencias

**Sistema:** Sistema de inventario (ficticio)
**Versión:** 1.1
**Última actualización:** fecha de ejemplo

#### 1. Objetivo
Consultar la cantidad de productos disponibles en cada bodega.

#### 2. Alcance
Dirigido al personal de almacén y de ventas que necesite verificar existencias. No permite modificar datos.

#### 3. Requisitos
- Usuario con permiso de consulta de inventario.
- Conocer la bodega o el producto que se desea consultar.

#### 4. Pasos de ejecución

| Paso | Acción | Resultado |
|---|---|---|
| 1 | Abrir el menú Consultas y seleccionar Consulta de existencias | Se muestra la pantalla de búsqueda |
| 2 | Seleccionar la bodega | El campo muestra la bodega elegida |
| 3 | (Opcional) Escribir el código o nombre del producto | El campo acepta el dato |
| 4 | Hacer clic en Consultar | Se muestra la lista con las existencias |

#### 5. Resultado esperado
La lista presenta cada producto con su cantidad disponible en la bodega seleccionada.

#### 6. Situaciones frecuentes

| Situación | Qué significa | Qué hacer |
|---|---|---|
| No aparecen resultados | No hay productos con ese filtro | Revisar la bodega o ampliar la búsqueda |
| Mensaje de acceso denegado | El usuario no tiene permiso para la consulta | Solicitar el acceso al área responsable |

#### 7. Control de versiones

| Versión | Cambio |
|---|---|
| 1.0 | Elaboración inicial |
| 1.1 | Se actualizaron los pasos por cambios en la pantalla |
