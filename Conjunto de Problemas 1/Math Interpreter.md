# Math Interpreter

Python ya soporta matemáticas, por lo que puedes escribir código para sumar, restar, multiplicar o dividir valores e incluso variables. Pero vamos a escribir un programa que permita a los usuarios hacer matemáticas, incluso sin conocer Python.

En un archivo llamado interpreter.py, implementa un programa que le pida al usuario una expresión aritmética y luego calcule y muestre el resultado como un valor de punto flotante formateado a un decimal. Asume que la entrada del usuario estará formateada como x y z, con un espacio entre x e y y un espacio entre y y z, donde:

x es un número entero
y es +, -, \*, o /
z es un número entero
Por ejemplo, si el usuario ingresa 1 + 1, tu programa debería mostrar 2.0. Asume que, si y es /, entonces z no será 0.

Ten en cuenta que, así como python es un intérprete para Python, tu interpreter.py será un intérprete para matemáticas.

Pistas
Recuerda que una cadena (str) tiene bastantes métodos, según docs.python.org/3/library/stdtypes.html#string-methods, incluyendo split, que separa una cadena en una secuencia de valores, todos los cuales pueden asignarse a variables a la vez. Por ejemplo, si expression es una cadena como 1 + 1, entonces

```python
x, y, z = expression.split(" ")
```

asignará 1 a x, + a y, y 1 a z.

## Antes de Comenzar

Inicia sesión en cs50.dev, haz clic en tu ventana de terminal y ejecuta `cd` por sí solo. Deberías ver que el indicador de la ventana de tu terminal se asemeja a lo siguiente:

```bash
$
```

Luego ejecuta

```bash
mkdir interpreter
```

para crear una carpeta llamada interpreter en tu espacio de código.

Luego ejecuta

```bash
cd interpreter
```

para cambiar de directorio a esa carpeta. Ahora deberías ver el indicador de tu terminal como interpreter/ $. Ahora puedes ejecutar

```bash
code interpreter.py
```

para crear un archivo llamado interpreter.py donde escribirás tu programa.

## Cómo Probar

Así es como puedes probar tu código manualmente:

Ejecuta tu programa con

```bash
python interpreter.py
```

Escribe 1 + 1 y presiona Enter. Tu programa debería mostrar:

2.0

Ejecuta tu programa con

```bash
python interpreter.py
```

Escribe 2 - 3 y presiona Enter. Tu programa debería mostrar:

-1.0

Ejecuta tu programa con

```bash
python interpreter.py
```

Escribe 2 \* 2 y presiona Enter. Tu programa debería mostrar:

4.0

Ejecuta tu programa con

```bash
python interpreter.py
```

Escribe 50 / 5 y presiona Enter. Tu programa debería mostrar:

10.0

Puedes ejecutar lo siguiente para verificar tu código usando check50, un programa que CS50 usará para probar tu código cuando lo envíes. ¡Pero asegúrate de probarlo tú mismo también!

```bash
check50 cs50/problems/2022/python/interpreter
```

Las caritas verdes significan que tu programa ha pasado una prueba. Las caritas rojas indicarán que tu programa mostró algo inesperado. Visita la URL que check50 te proporciona para ver la entrada que check50 entregó a tu programa, qué salida esperaba y qué salida dio tu programa realmente.

Cómo Enviar
En tu terminal, ejecuta lo siguiente para enviar tu trabajo.

```bash
submit50 cs50/problems/2022/python/interpreter
```
