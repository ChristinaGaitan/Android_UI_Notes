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

Referencias
------------
- [#63 Android Tutorial For Beginners: Table Layout [HD 1080p]](https://www.youtube.com/watch?v=Cp_ASAkzzVo&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&index=63&nohtml5=False)