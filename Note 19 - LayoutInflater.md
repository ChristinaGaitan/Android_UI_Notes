  LayoutInflater
==========================

- **Inflation:** Convertir elementos de XML en objetos de Java de tipo View.

- Toma mucho tiempo hacer la conversión, porque necesita hacer lo siguiente: 
	1. Toma la vista en XML.
	2. Crea el objeto en Java.
	3. Establece los valores para los atributos.
	4. Hacerlo recursivamente para todos los nodos en XML.

- Para crear un objeto de LayoutInflater se pueden ustilizar los siguientes métodos:
	- getSystemService() 	// Recomendado
	- getLayoutInflater()

- Sólo archivos XML precompilados por la aapt (precompilador de los recursos XML) pueden ser inflated en tiempo de ejecución, esto es para tener un mejor performance.

- IMPORTANTE: Este es un tema complejo, por lo que se recomienda (especialemente en este caso), ver los videos de referencia.

Referencias
------------
- [#81 Android LayoutInflater Part 1: Android Tutorial For Beginners [HD 1080p]](https://www.youtube.com/watch?v=fxVeFwtIpVc&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&index=81&nohtml5=False)
- [#82 LayoutInflater in Android Part 2:Android Tutorial For Beginners [HD 1080p]](https://www.youtube.com/watch?v=1Y0LlmTCOkM&index=82&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&nohtml5=False)