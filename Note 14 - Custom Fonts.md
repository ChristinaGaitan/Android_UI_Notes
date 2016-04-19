  Custom Fonts
==========================

- El formato de la fuente debe de ser TTF o OTF.

- Si se usan fuentes muy pesadas y son agregadas a los assets, el tamaño de la App puede incrementarse mucho.

- Por el momento, las fuentes sólo son accesibles en código.

- Para cargar la fuente se utilizan los métodos de ```Typeface.create```

- Si una fuente es inválida, entonces Android utilizará la fuente del sistema por default.

- Se deben tener en cuenta el copyright de las fuentes utilizadas.

- Métodos de ```Typeface.create```

	```java
    	Typeface.create(String famliyName, int style)
        Typeface.createFromAsset(AssetManager manager, String path)
        Typeface.create(File path or String path)
	```

Referencias
------------
- [#71 Android Tutorial For Beginners: How to use Custom Font in your App [HD 1080p]](https://www.youtube.com/watch?v=2wBjpn7VmsU&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&index=71&nohtml5=False)