  Spinner
==========================

- Es un control parecido a un Drop-down menu.

- Permite al usuario seleccionar un elemento desde una lista corta de opciones.

- El usuario sólo ve 1 valor (el seleccionado).

- El Spinner maneja sus datos a través de un Adapter.

**Pasos para utilizar un Spinner**

1. Definir el array o DataSource
2. Decirle al Adapter cómo se van a desplegar los datos definiendo un Layout para el drop down.
3. Definir qué pasa cuando el usuario selecciona una opción del Spinner.

**Existen 2 layouts para el Spinner**
1. ```android.R.layout.simple_spinner_item```: Usa un TextView
2. ```android.R.layout.simple_spinner_dropdown_item```: Usa un CheckTextView

Se puede cambiar la view que se muestra en el Spinner utilizando el método ```setDropDownViewResource``` en el Adapter.

Referencias
------------
- [#104 Android Spinner Tutorial: Android Application Development Tutorial [HD 1080p]](https://www.youtube.com/watch?v=VEgw3Ia6PIs&index=104&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&nohtml5=False)