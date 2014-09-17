**Device Independent Pixels and Scaled Pixels**
===================

----------
Screen size
--------------

 - Medida física de la diagonal
 - 4 medidas generales: 
	 - small (2.8)
	 - normal (3.1)
	 - large (3.7)
	 - extra large (4.2)


----------
Screen density
-----------------
- Número de pixeles en una pulgada = DPI (Dots Per Inch)
- 4 densidades generales:
	- ldpi: 1 unit = 1 pixel
	- mdpi: 1 unit = 4 pixel
	- hdpi: 1 unit = 9 pixel
	- xhdpi

- La medida que se usa como base es mdpi y a partir de ahí se escalan las demás medidas
	- ldpi = 0.75x
	- mdpi = baseline
	- hdpi = hdpi
	- xhdpi = xhdpi

-------------------
Screen resolution
---------------------

- Número de pixeles en la pantalla
- En Android debido a la gran variedad de resoluciones en los diferentes dispositivos no tiene sentido diseñar interfaces para una sola medida
- En Android se debe de trabajar sólo con las screen sizes y screen desities para abarcar los diferentes dispositivos. 

---------------------------
Screen orientation
----------------------

- Portrait: tall
- Landscape: wide

-------------------
Measurement Units
-----------------------

| Atributo | Unidad | Descripción|
| :-------: | :----: | :--- |
| Dimensión| mm    |  Basada en el tamaño físico de la pantalla. No recomendable.|
| | in   | Basada en el tamaño físico de la pantalla. No recomendable. |
| | px    | Basada en el tamaño físico de la pantalla. No recomendable. |
| | pt| 1/72 de una pulgada basada en el tamaño físico de la pantalla. No recomendable. |
| | dp| Basada en 160 dpi de pantalla y escalable apropiadamente para otros dispositivos. RECOMENDABLE.|
| | sp| Para fuentes, basada en las preferencias del usuario. RECOMENDABLE.|


--------------------
Density (Device) Independet Pixel
-----------------------------------------

- Se usa un pixel virtual para definir las dimensiones y posición.
- Con esto nos evitamos tener que preocuparnos por cómo se verá la aplicación en diferentes dispositivos.

| Screen density | dp | px|
| :------- | ----: | :--- |
| ldpi| 1 dp	|  0.75 px    |
| mdpi| 1 dp   |  1 px|
| hdpi| 1 dp   |  1.5 px|
| xhdpi| 1 dp   |  2 px|


- El sistema convierte los dp a px cuando la aplicación corre.
	- px = dp * (dpi del dispositivo / 160)
- Android se encarga de mantener las proporciones.
- Density Independence significa mantener el tamaño físico de la UI en diferentes dispotivios con diferentes screen densities.

------------------------------
Scaled Pixels
----------------
- Es un pixel escalado de acuerdo a la densidad y a las preferencias del usuario.
- Se maneja el mismo concepto de independencia de pixeles usado para fuentes.
- Nos permite manejar las fuentes con la misma proporción para diferentes pantallas en diferentes dispositivos.

------
Referencia
--------------
https://www.youtube.com/watch?v=gd_7wKZiuW0&index=35&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa


> Written with [StackEdit](https://stackedit.io/).
