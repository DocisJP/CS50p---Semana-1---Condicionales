# Meal Time

Supón que estás en un país donde es costumbre desayunar entre las 7:00 y las 8:00, almorzar entre las 12:00 y las 13:00, y cenar entre las 18:00 y las 19:00. ¿No sería genial tener un programa que te diga qué comer y cuándo?

En meal.py, implementa un programa que le pida al usuario una hora y muestre si es hora de desayunar, almorzar o cenar. Si no es hora de una comida, no muestres nada. Asume que la entrada del usuario estará en formato de 24 horas como #:## o ##:##. Y asume que el rango de tiempo de cada comida es inclusivo. Por ejemplo, ya sea 7:00, 7:01, 7:59, o 8:00, o cualquier hora intermedia, es hora de desayunar.

Estructura tu programa según lo siguiente, donde convert es una función (que puede ser llamada por main) que convierte time, una cadena en formato de 24 horas, al número correspondiente de horas como un flotante. Por ejemplo, dado un tiempo como "7:30" (es decir, 7 horas y 30 minutos), convert debería devolver 7.5 (es decir, 7.5 horas).

```python
def main():
    ...


def convert(time):
    ...


if __name__ == "__main__":
    main()
```

## Pistas

Recuerda que una cadena (str) tiene bastantes métodos, según docs.python.org/3/library/stdtypes.html#string-methods, incluyendo split, que separa una cadena en una secuencia de valores, todos los cuales pueden asignarse a variables a la vez. Por ejemplo, si time es una cadena como "7:30", entonces

```python
hours, minutes = time.split(":")
```

asignará "7" a hours y "30" a minutes.

Ten en cuenta que hay 60 minutos en 1 hora.

Antes de Comenzar
Inicia sesión en cs50.dev, haz clic en tu ventana de terminal y ejecuta `cd` por sí solo. Deberías ver que el indicador de la ventana de tu terminal se asemeja a lo siguiente:

```bash
$
```

Luego ejecuta

```bash
mkdir meal
```

para crear una carpeta llamada meal en tu espacio de código.

Luego ejecuta

```bash
cd meal
```

para cambiar de directorio a esa carpeta. Ahora deberías ver el indicador de tu terminal como meal/ $. Ahora puedes ejecutar

```bash
code meal.py
```

para crear un archivo llamado meal.py donde escribirás tu programa.

## Desafío

Si estás preparado para un desafío, opcionalmente agrega soporte para tiempos de 12 horas, permitiendo al usuario ingresar horas en estos formatos también:

```bash
#:## a.m. y ##:## a.m.
#:## p.m. y ##:## p.m.
```

Cómo Probar
Así es como puedes probar tu código manualmente:

Ejecuta tu programa con

```bash
python meal.py
```

Escribe 7:00 y presiona Enter. Tu programa debería mostrar:
breakfast time

Ejecuta tu programa con

```bash
python meal.py
```

Escribe 7:30 y presiona Enter. Tu programa debería mostrar:
breakfast time

Ejecuta tu programa con

```bash
python meal.py
```

Escribe 12:42 y presiona Enter. Tu programa debería mostrar:
lunch time

Ejecuta tu programa con

```bash
python meal.py
```

Escribe 18:32 y presiona Enter. Tu programa debería mostrar:
dinner time

Ejecuta tu programa con

```bash
python meal.py
```

Escribe 11:11 y presiona Enter. Tu programa no debería mostrar nada.

Puedes ejecutar lo siguiente para verificar tu código usando check50, un programa que CS50 usará para probar tu código cuando lo envíes. ¡Pero asegúrate de probarlo tú mismo también!

```bash
check50 cs50/problems/2022/python/meal
```

Las caritas verdes significan que tu programa ha pasado una prueba. Las caritas rojas indicarán que tu programa mostró algo inesperado. Visita la URL que check50 te proporciona para ver la entrada que check50 entregó a tu programa, qué salida esperaba y qué salida dio tu programa realmente.

Si no pasas las pruebas pero estás seguro de que tu programa se comporta correctamente, asegúrate de no haber eliminado la línea

```python
if __name__ == "__main__":
    main()
```

de la estructura del código que te dieron. Esto permite a check50 probar tu función convert por separado. Aprenderás más sobre esto en las próximas semanas.

Cómo Enviar
En tu terminal, ejecuta lo siguiente para enviar tu trabajo.

```bash
submit50 cs50/problems/2022/python/meal
```
