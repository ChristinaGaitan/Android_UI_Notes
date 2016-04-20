  Android Adapter
==========================

Data Source <----> Adapter <----> AdapterView.
------------------------------------------------------------

**Data source**
---------------
- Contiene los datos (DB, array, etc.)

**Adapter**
---------------
- Toma los datos, crea una View con ellos y los pasa al Adsapter View.
- Sólo es responsable del manejo de los datos.
- El tipo de Adapter depende del tipo de Data Source.
- Accede a los datos y crea una View que es desplegada dentro del AdapterView.
- Tipos:
	- **ArrayAdapter:** Toma los datos desde un array y crea una View.
	- **SimpleCursorAdapter:** Toma los datos desde un cursor y crea una View a partir de ellos. Un cursor es un objeto en Android que representa datos obtenidos de la Base de Datos.
	- **BaseAdapter:** Es un adaptador que puede ser customizado para determinar cómo obtener los datos, cómo procesarlos y cómo se debe generar la vista.

**AdapterView**
---------------
- Despliga las datos.
- Controla como se despliegan los datos.
- El tipo de AdapterView depende de cómo se quieran mostrar los datos.
- Contien un conjunto de Views que despliegan los datos desde el DataSource usando el Adapter.
- Tipos:
	- **ListView:** despliega una scroling list de manera vertical, la cual contiene Views con las que el usuario puede interactuar.
	- **GridView:** despliega un Grid (con filas y columnas) de Views con las que el usuario puede interactuar.
	- **Gallery:** despliega una scroling list de manera horizontal, la cual contiene Views con las que el usuario puede interactuar. (DEPRECATED).
	- **Spinner:** despliega una lista de items parecida a un drop down menu.

Referencias
------------
- [#76 Android Tutorial For Beginners: What is Android Adapter?](https://www.youtube.com/watch?v=uic3TVp_j3M&index=76&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&nohtml5=False)