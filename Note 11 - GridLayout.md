 Grid Layout
==========================

- Las Views son ordenadas en filas y columnas.

- Se especifica el número de filas y columnas utilizando ```android:rowCount``` y ```android:columnCount``` dentro de la etiqueta ```<GridLayout>```

- Se puede controlar si una View abarca más de una fila o columna.

- Se puede controlar dentro de cuál columna se va a colocar una View.

- Múltiples Views pueden estar en la misma columna y overlap.

- Las views contenidas dentro del GridLayout son WRAP_CONTENT en width y height.

- Definir filas y columnas:

    ```xml
    android:rowCount = "2"
    android:columnCount = "3"
    ``` 
    
    las Views se colocan diréctamente dentro del GridLayout.

- Para agregar espacios entre las Views:
     - Se puede utilizar ``` android:layout_margin``` en la View diréctamente (por ejemplo un TextView)
     - Se puede utilizar un margin general``` android:useDefaultMargins="true"``` dentro del GridLayout. Este maregen varía dependiendo de la versión de Android.

- Para dejar una columna vacía se puede agregar una tag de Space ```<Space android:layout_width="wrap_content" android:layout_height="wrap_content"/>``` entre las Views.


Referencias
------------
- [#66 Android GridLayout Basics: Android Tutorials [HD 1080p]](https://www.youtube.com/watch?v=TaCW4uL4P6c&index=66&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&nohtml5=False)