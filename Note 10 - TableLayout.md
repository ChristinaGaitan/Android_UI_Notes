Table Layout
==========================

- Las vistas son acomodadas en filas y columnas.

- Puede ser definida de dos maneras:
    - Utilizando la clase de java ```TableLayout```.
    - Utilizando la tag ```TableLayout``` de xml.

- **NO** es necesario definir las columnas, no hay equivalente a ```<td></td>```.

- Sólo se definen las filas utilizando ```TableRow```

- Cada elemento que es agregado a una fila es definido como una columna.

- Es una subclase de ```Horizontal LinearLayout```.

- Los valores de width and height del ```TableRow``` y de las views que estan dentro de ella NO importan.

- ```TableRow``` SIEMPRE es ```MATCH_PARENT``` en width y ```WRAP_CONTENT``` en height.

- El **número de columnas** se define por la ```TableRow``` que tenga el **mayor número de Views**.

- El ancho automáticamente se ajusta, basado en el tamaño de la columna con el máximo ancho.

- Cuando se define una View adentro de un ```TableLayout``` pero afuera de un ```TableRow```, la View se va a desplegar y va a tener una width de MATCH_PARENT y una height de WRAP_CONTENT, pero esos valores pueden ser modificados.

Atributos de TableLayout
-------------------------

- **android:stretchColumns:** Estira una columna o un conjunto de columnas (los índices empiezan en 0).
    
    ```xml
    android:stretchColumns = "0"
    android:stretchColumns = "1,2"
    android:stretchColumns = "*"
    ``` 

- **android:shrinkColumns:** Remueve espacios innecesarios de una columna y la comprime (los índices empiezan en 0).
    
    ```xml
    android:shrinkColumns = "0"
    android:shrinkColumns = "1,2"
    android:shrinkColumns = "*"
    ```
 
- **android:collapseColumns:** Esconde las columnas con el índice especificado.
    
    ```xml
    android:collapseColumns = "2" // Esconde la columna con índice = 2
    ```
 
Atributos de cudalquier View dentro de una TableRow
-------------------------

- **android:layout_span:** Hace que la View abarque múltiples columnas especificadas por el número en layout_span
    
    ```xml
    android:layout_span = "2" // Hace que la View abarque 2 columnas
    android:layout_span = "3" // Hace que la View abarque 3 columnas
    ```

- **android:layout_column:** Especifica el índice de la columna dentro de la cual la View aparecerá.
    
    ```xml
    android:layout_column = "2" // Hace que la View aparezca dentro de la columna con índice 2
    ```

Referencias
------------
- [#63 Android Tutorial For Beginners: Table Layout [HD 1080p]](https://www.youtube.com/watch?v=Cp_ASAkzzVo&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&index=63&nohtml5=False)
- [#64 Android Table Layout: android:stretchColumns and android:shrinkColumns [HD 1080p]](https://www.youtube.com/watch?v=KZiP73VHSwY&index=64&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&nohtml5=False)
- [#65 Android Tutorials: Android TableLayout, android:layoutColumn,android:layout_span etc. [HD 1080p]](https://www.youtube.com/watch?v=DxFnSKnQ-OQ&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&index=65&nohtml5=False)