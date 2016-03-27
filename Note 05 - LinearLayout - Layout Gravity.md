LinearLayout: Layout Gravity
======
- `layout_gravity` permite especificar en dónde aparecerán los elementos dentro de su elemento padre.

- Si la view y el parent son del mismo tamaño, entonces no se notará ningún efecto al utilizar `layout_gravity`, por ejemplo al utilizar `match_parent`.

- Sólo cuando el elemento padre es más grande que la vista con `layout_gravity` se notará el efecto.

- Se pueden asignar varios valores al atributo `layout_gravity`:
	- top|left
	- right
	- center
	- bottom
	- bottom|right 

- No todos los valores pueden ser utilizados con todos los *LinearLayout*, cuando se utiliza un valor que no sirve con un layout no se muestran errores, ni problemas, simplemente la interfaz no cambia.

Layout_gravity con Horizontal LinearLayout
--------
- En un Horizonal *LinearLayout* los elementos se colocan uno al lado del otro en diferentes columnas (dentro de la misma fila).

- Para un Horizontal *LinearLayout* el atributo `layout_gravity` NO cambia a los elementos de columna.


- En este caso, los elementos se pueden colocar desde el **top** hasta el **bottom** (sin cambiar de columna), los valores que se pueden utilizar son:
  - `layout_gravity = "top"` o `layout_gravity = "top"`
  - `layout_gravity = "center"` o `layout_gravity = "center_vertical"`
  - `layout_gravity = "bottom"`

- Los valores que no tendrán efecto en este caso son, al utilizar estos valores el elemento tomará su posición por default (top|left):
  - `layout_gravity = "right"`
  - `layout_gravity = "center_horizontal"`

Layout_gravity con Vertical LinearLayout
--------
- En un Vertical *LinearLayout* los elementos se colocan uno debajo del otro en diferentes filas (dentro de la misma columna).

- Para un Vertical *LinearLayout* el atributo `layout_gravity` NO cambia a los elementos de fila.

- Sólo cuando el elemento padre es más grande que la vista con `layout_gravity` se notará el efecto.

- En este caso, los elementos se pueden colocar desde el **left** hasta el **right** (sin cambiar de fila), los valores que se pueden utilizar son:
  - `layout_gravity = "left"`
  - `layout_gravity = "center"` o `layout_gravity = "center_horizontal"`
  - `layout_gravity = "right"`

- Los valores que no tendrán efecto en este caso son, al utilizar estos valores el elemento tomará su posición por default (top|left):
  - `layout_gravity = "bottom"`
  - `layout_gravity = "center_vertical"`
	
Referencia
--------------

- [Android layout gravity](https://www.youtube.com/watch?v=C56druJtByI&index=38&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa)