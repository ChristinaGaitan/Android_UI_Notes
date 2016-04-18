 Grid Layout
==========================

- Las Views son ordenadas en filas y columnas.

- Se especifica el n�mero de filas y columnas utilizando ```android:rowCount``` y ```android:columnCount``` dentro de la etiqueta ```<GridLayout>```

- Se puede controlar si una View abarca m�s de una fila o columna.

- Se puede controlar dentro de cu�l columna se va a colocar una View.

- M�ltiples Views pueden estar en la misma columna y overlap.

- Las views contenidas dentro del GridLayout son WRAP_CONTENT en width y height.

- Definir filas y columnas:

    ```xml
    android:rowCount = "2"
    android:columnCount = "3"
    ``` 
    
    las Views se colocan dir�ctamente dentro del GridLayout.

- Para agregar espacios entre las Views:
     - Se puede utilizar ``` android:layout_margin``` en la View dir�ctamente (por ejemplo un TextView)
     - Se puede utilizar un margin general``` android:useDefaultMargins="true"``` dentro del GridLayout. Este maregen var�a dependiendo de la versi�n de Android.

- Para dejar una columna vac�a se puede agregar una tag de Space ```<Space android:layout_width="wrap_content" android:layout_height="wrap_content"/>``` entre las Views.


Referencias
------------
- [#66 Android GridLayout Basics: Android Tutorials [HD 1080p]](https://www.youtube.com/watch?v=TaCW4uL4P6c&index=66&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&nohtml5=False)