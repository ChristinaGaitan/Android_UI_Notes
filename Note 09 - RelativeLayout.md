Relative Layout
==========================

- Especifica en dónde se colocará una View con respecto a otras Views o a su Parent.

- Layout weight y layout gravity **NO** existen en este layout

**Posiciones en Relative Layout**
- Colocar una view **centrada** dentro del Relative Layout

| Atributo XML (true/false) | Constante en Java (RelativeLayout class)|
| ----: | :--- |
| ```android:layout_centerInParent``` | ```CENTER_IN_PARENT``` |
| ```android:layout_centerHorizontal``` | ```CENTER_HORIZONTAL``` |
| ```android:layout_centerVertical``` | ```CENTER_VERTICAL``` |


- Alinear el **egde** de una vista con el edge de su parent

| Atributo XML (true/false) | Constante en Java (RelativeLayout class)|
| ----: | :--- |
| ```android:layot_alignParentTop``` | ```ALIGN_PARENT_TOP``` |
| ```android:layot_alignParentBottom``` | ```ALIGN_PARENT_BOTTOM``` |
| ```android:layot_alignParentLeft``` | ```ALIGN_PARENT_LEFT``` |
| ```android:layot_alignParentRight``` | ```ALIGN_PARENT_RIGHT``` |

- Definir la **relación** entre dos vistas

| Atributo XML (ID de la vista) | Constante en Java (RelativeLayout class)|
| ----: | :--- |
| ```android:layout_above``` | ```ABOVE``` |
| ```android:layout_below``` | ```BELOW``` |
| ```android:layout_toLeftOf``` | ```RIGHT_OF``` |
| ```android:layout_toRightOf``` | ```LEFT_OF``` |

- Definir la **alinación** entre dos vistas

| Atributo XML (ID de la vista) | Constante en Java (RelativeLayout class)|
| ----: | :--- |
| ```android:layout_alignTop``` | ```ALIGN_TOP``` |
| ```android:layout_alignBottom``` | ```ALIGN_BOTTOM``` |
| ```android:layout_alignLeft``` | ```ALIGN_LEFT``` |
| ```android:layout_alignRight``` | ```ALIGN_RIGHT``` |
| ```android:layout_alignBaseLine``` | ```ALIGN_BASELINE``` |

Referencias
------------
- [#51 Android Tutorial For Beginners: Relative Layout Part 1 [HD 1080p]](https://www.youtube.com/watch?v=YJd_zZKzKx8&index=51&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&nohtml5=False)
- [#52 Android Tutorial For Beginners: Relative Layout Part 2 [HD 1080p]](https://www.youtube.com/watch?v=EWUrl5h-VA4&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&index=52&nohtml5=False)
- [#53 Android Application Development Tutorial: Relative Layout Part 3 [HD 1080p]](https://www.youtube.com/watch?v=A4ZioB3Oz8A&index=53&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&nohtml5=False)
- [#54 Android Application Development Tutorial: Relative Layout Part 4 [HD 1080p]](https://www.youtube.com/watch?v=iS0t2Suo_JM&index=54&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&nohtml5=False)