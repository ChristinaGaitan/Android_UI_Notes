LinearLayout utilizando Java
==========================

- NO es recomendado utilizar código de Java para generar layouts, pero es posible hacerlo.

- Podría utilizarse este método, por ejemplo, cuando las cosas son dinámicas.

- Los pasos para generarlos son:

1. Generar objetos de Java para todas las Views y ViewGroups.
2. Especificar las dimensiones para todas las Views y ViewGroups. Y especificar la layout information de cada hijo del LinearLayout utilizando `LayoutParams`.
3. Establecer otras propiedades a la Views y ViewGroup (text, color, size, gravity, etc.) y utilizar setContentView para establecer el nombre del root layout.

- **Context object:** es un objecto que nos permite acceder a los recursos del sistema y servicios de la plataforma en Android.

Referencia
------------
- [Android Linear Layout Using Java Code Part 1](https://www.youtube.com/watch?v=eb1hJFXANOQ&index=40&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa)