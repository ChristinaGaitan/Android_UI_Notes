**LinearLayout**
==========================

- Los elementos pueden ser colocados sólo de dos maneras: horizontal o vertical. 

	- **Horizontal:** Todos los elementos se colocan en la misma fila. Es  la orientación por default, puede o no especificarse en XML.
	- **Vertical:** Todos los elemento se colocan en la misma columna. Se debe especificar en el XML cuando vamos a utilizar esta orientación.

- **IMPORTANTE**
	-  Solo se mostrarán en pantalla los elementos que quepan, si existen más elementos de los que caben en la pantalla estos NO se verán.
	- NO aparecerá un scrollbar para mostrar los elementos faltantes.
	- Se debe de tener cuidado de generar diferentes UI para considerar los diferentes tamaños de pantalla (No es lo mismo el tamaño de una tableta al de un teléfono).

```xml
 <LinearLayout                                                   --> Elemento raíz. Inicio del ViewGroup
	xmlns:android = "htto://schemas.android.com/apk/res/android" --> Definición de las etiquetas.
	android:layout_width = "match_parent"	                    --> Tamaño del elemento.
	android:layout_height = "match_parent"
	android:orientation = "vertical"                             --> Determina la orientación que tendrá el layout
>

	<TextView	--> Elemento contenido por el elemento raíz
		android:layout_width = "wrap_parent"		--> Tamaño del elemento.
		android:layout_height = "wrap_parent"
		android:text = "Hello World!">

	<Button	--> Elemento contenido por el elemento raíz
		android:layout_width = "wrap_parent"		--> Tamaño del elemento.
		android:layout_height = "wrap_parent"
		android:text = "Button!">
		
</LinearLayout> --> Fin del ViewGroup
```

- **match_parent** = Toma TODO el espacio disponible.
- **wrap_parent** = Toma SÓLO el espacio necesitado por su contenido. 

------
Referencia
--------------
- [Android LinearLayout](https://www.youtube.com/watch?v=70-JVroY1Ng&index=36&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa)