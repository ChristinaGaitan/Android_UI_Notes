 Text Customization Attributes
==========================

| Atributo| XML | Java | Tipo de value |
| ----: | :--- | :--- | :--- |
| **string** | ```android:text``` | ```setText(CharSequence c)``` | Cualquier string |
| **Font Size** | ```android:textSize``` | ```setTextSize(float f)``` | Valores de dimensión |
| **Font Color** | ```android:textColor``` | ```setTextColor(int c)``` | Cualquier valor como #rgb, #argb, #rrggbb, #aarrggbb o un color estandar |
| **Background Color** | No existe un atributo directo, pero se puede utilizar ```android:background``` | ```setBackgraoundColor(int c)``` | Cualquier valor de color |

android:text
------------
```xml
    android:text="Hola mundo"
```

```xml
    android:text="@string/hello_world"
```

android:textSize
------------

- Medida recomendada

    ```xml
        android:textSize="35sp"
    ```

```xml
    android:textSize="35dp"
```

```xml
    android:textSize="35px"
```

```xml
    android:textSize="35mm"
```

```xml
    android:textSize="35in"
```

- La mejor manera de asignar el textSize es generar un archivo llamado ```dimensions.xml``` dentro de la carpeta ```values``` y poner los valores de las dimensiones ahí.

```xml
    <resources>
        <dimen name="text_size">30dp</dimen>
    </resources>
```

    y así se puede utilizar en el xml como:
    
```xml
    android:textSize="@dimen/text_size"
```

android:textColor
------------

```xml
    android:textColor="#f00"
```

```xml
    android:textColor="#af00"
```

```xml
    android:textColor="#ff0000"
```

```xml
    android:textColor="#aaff0000"
```

```xml
    android:textColor="@android:color/holo_red_dark" //depende de las versiones de android
```

- La mejor manera de asignar el textColor es generar un archivo llamado ```colors.xml``` dentro de la carpeta ```values``` y poner los valores de las dimensiones ahí.

```xml
    <resources>
        <color name="my_red">#af0000</color>
    </resources>
```

    y así se puede utilizar en el xml como:
    
```xml
    android:textSize="@color/my_red"
```


Referencias
------------
- [#68 Android Tutorial For Beginners: Android Text Customization Part 1 [HD 1080p]](https://www.youtube.com/watch?v=H049IDor6XI&index=68&list=PLonJJ3BVjZW6hYgvtkaWvwAVvOFB7fkLa&nohtml5=False)
