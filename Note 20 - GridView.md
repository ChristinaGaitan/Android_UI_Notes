  GridView
==========================

- Es un AdapterView que despliega los items en un grid scroleable de 2 dimensiones.

- Conforme el usuario llega al final se generan y despliegan más elementos.

- Cuando el usuario hace click sobre algún elemento alguna acción puede ser desencadenada.

- Los elementos son insertados en el GridView automáticamente usando un BaseAdapter.

**Pasos para generar utilizar un GridView**

1. Definir el array o DataSource
2. Decirle al BaseAdapter cómo se van a desplegar los datos definiendo un Layout para cada View.
3. Definir qué pasa cuando el usuario interactúa con una fila en el GridView.

**Propiedades**

| Atributo XML| Propiedad | Descripción |
| ----: | :--- | :--- |
| ```android:numColumns``` | Número de columnas en el GridView | Indica el número de columnas o establece el valor de ```auto_fit``` para determinar el número de columnas en el espacio disponible. Usar ```auto_fit``` es lo recomendado debido a los múltiples tamaños de pantalla.|
| ```android:verticalSpacing="5dp"```  ```android:horizontalSpacing="5dp"``` | Establece el espacio entre columnas | Indican cuánto espacio debería existir entre los elementos en el Grid |
| ```android:columnWidth``` | Ancho de las columnas | Indica el ancho de las columnas en pixeles |
| ```android:stretchMode="none"``` ```android:stretchMode="columnWidth"``` ```android:stretchMode="spacingWidth"``` ```android:stretchMode="spacingWidthUniform"``` | Establece qué hacer con el espacio extra | Establece qué hacer con el espacio extra una vez que las columnas ya han ocupado su espacio. 
 |

```none```: el espacio sobrante queda al final, no se distribuye.

```columnWidth```: el espacio sobrante se distribuye de manera equitativa entre las columnas (las columnas se hacen más grandes).

```spacingWidth```: el espacio sobrante se distribuye de manera equitativa entre los espacios entre columnas (los espacios se hacen más grandes).

```spacingWidthUniform```: el espacio sobrante se distribuye de manera equitativa a los lados de las columnas.

Referencias
------------
- [#97 Android GridView Tutorial Part 1: Android Application Development Tutorial [HD 1080p]](https://www.youtube.com/watch?v=8NoHxfIu0MQ&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&index=97&nohtml5=False)