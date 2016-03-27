LinearLayout: Layout Weight
======
- Cuando se usa `layout_width = "wrap_content"` y el elemento no tiene contenido (por ejemplo un EditText vacío), éste ocupara muy poco espacio.

- Para establecer el ancho del elemento se puede utilizar ** ems** que es una unidad en CSS para el tamño de fuentes. Pero NO es recomendable porque es una medida fija.

- Para asignar cierto espacio en pantalla a los elementos se recomienda utilizar layout_weight.

- **layout_weight** asigna importancia a las Views, sirve para determinar qué tanto espacio va a ocupar un elemento en la pantalla en comparación con las demás.

- Para todos los elementos, por default `android:layout_weight = 0`

- Cuando más de una View declara `layout_weight`, Android calcula cuánto espacio asignarle a cada una.

- ** Cálculo:**
  - Si se tienen 3 elementos con los siguientes valores:
    `android:layout_weight = "1"`
    `android:layout_weight = "4"`
    `android:layout_weight = "8"`
  - Primero se suman los valores: 1 + 4 + 8 = **13**
  - Y después se distribuye el espacio de la siguiente manera:
  	- El primer elemento ocupará **1/13** de la pantalla.
  	- El segundo elemento **4/13**.
  	- Y el tercer elemento **8/13**.
- Cuando se le asigna un valor a `layout_weight` utilizar `layout_width = "wrap_content"` es redundante.

- Si se va a utilizar `layout_weight`, es recomendable establecer `layout_width = "0dp"` para el valor horizontal.

- El cálculo del `layout_weight` depende de la orientación del layout:
 	- **Horizontal orientation:** el cálculo se hace sobre el width.
	```xml
	 <LinearLayout
		xmlns:android = "htto://schemas.android.com/apk/res/android"
		android:layout_width = "match_parent"
		android:layout_height = "match_parent"
		android:orientation = "horizontal">

		<Button
			android:layout_width = "0dp"
			android:layout_height = "wrap_content"
			android:layout_weight = "1"
			android:text = "Button!">

		<TextView
			android:layout_width = "0dp"
			android:layout_height = "wrap_content"
			android:layout_weight = "4"
			android:text = "Hello World!">

		<EditText
			android:layout_width = "0dp"
			android:layout_height = "wrap_content"
			android:layout_weight = "8"
			android:text = "Hello!">

	</LinearLayout>
	```
 	- **Vertical orientation:** el cálculo se hace sobre el height.
	```xml
	 <LinearLayout
		xmlns:android = "htto://schemas.android.com/apk/res/android"
		android:layout_width = "match_parent"
		android:layout_height = "match_parent"
		android:orientation = "vertical">

		<Button
			android:layout_width = "wrap_content"
			android:layout_height = "0dp"
			android:layout_weight = "1"
			android:text = "Button!">

		<TextView
			android:layout_width = "wrap_content"
			android:layout_height = "wrap_content"
			android:layout_weight = "4"
			android:text = "Hello World!">

		<EditText
			android:layout_width = "wrap_content"
			android:layout_height = "0dp"
			android:layout_weight = "8"
			android:text = "Hello!">

	</LinearLayout>
	```
- Al establecer "0dp" nos aseguramos de que Android no calcule 2 veces el ancho (o el alto) del elemento, esto hace a la aplicación más rápida y precisa.

------
Referencia
--------------

- [Android LinearLayout](https://www.youtube.com/watch?v=70-JVroY1Ng&index=36&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa)