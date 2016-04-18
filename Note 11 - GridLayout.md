 Grid Layout
==========================

- Las Views son ordenadas en filas y columnas.

- Se especifica el número de filas y columnas utilizando ```android:rowCount``` y ```android:columnCount``` dentro de la etiqueta ```<GridLayout>```

- Se puede controlar si una View abarca más de una fila o columna.

- Se puede controlar dentro de cuál columna se va a colocar una View.

- Múltiples Views pueden estar en la misma columna y overlap.

- Las views contenidas dentro del ```GridLayout``` son ```WRAP_CONTENT``` en width y height.

- **Definir filas y columnas**

    ```xml
    android:rowCount = "2"
    android:columnCount = "3"
    ``` 
    
    las Views se colocan diréctamente dentro del ```GridLayout```.

- **Agregar espacios entre las Views**
     - Se puede utilizar ``` android:layout_margin``` en la View diréctamente (por ejemplo un TextView)
     - Se puede utilizar un margin general``` android:useDefaultMargins="true"``` dentro del ```GridLayout```. Este maregen varía dependiendo de la versión de Android.

- **Dejar una columna vacía** se puede agregar una tag de Space
    ```
    <Space android:layout_width="wrap_content" android:layout_height="wrap_content"/>
    ```
    entre las Views.

- **Controlar el tamaño de una View** dentro de un GridLayout se puede utilizar la etiqueta ``` android:layout_gravity ``` pero esto también depende del tamaño de las Views en la misma fila o columna.

    ```xml
    android:layout_gravity = "fill_horizontal"
    ```

    Para que el código anterior funcione, si la view tiene otra view en la misma columna, entonces se debe de aplicar el mísmo codigo a las dos Views.

- **Especificar la orientación** de las views dentro del GridLayout se utiliza ``` android:orientation``` por ejemplo:

    ```xml
        android:orientation = "horizontal"
        ó
        android:orientation = "vertical" 
    ```

- **Controlar en qué columan y en qué fila** se quieren mostrar las Views utilizando los attributos ```android:layout_row``` y ```android:layout_column``` (en la vista que se quiere posicionar)

    ```xml
        android:layout_row = "1"
        android:layout_column = "0"
    ```
    al utilzar estos atributos, las Views que estan a un lado símplemente siguen a la View que se movió

- **Utilizar Spanning** con los atributos ``` android:layout_columnSpan``` y ``` android:layout_rowSpan``` pero es obligatorio utilizar ``` android:layout_gravity = "fill"``` para notar los efectos.

    ```xml
        android:layout_columnSpan = "2"
        android:layout_gravity = "fill"
    ```

    ```xml
        android:layout_rowSpan = "2"
        android:layout_gravity = "fill"
    ```


Referencias
------------
- [#66 Android GridLayout Basics: Android Tutorials [HD 1080p]](https://www.youtube.com/watch?v=TaCW4uL4P6c&index=66&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&nohtml5=False)
- [#67 Android Tutorial For Beginners : Advanced Grid Layout [HD 1080p]](https://www.youtube.com/watch?v=Mkc1xQ0wsbU&index=67&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&nohtml5=False)