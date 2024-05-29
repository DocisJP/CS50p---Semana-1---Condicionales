# Home Federal Savings Bank

En la temporada 7, episodio 24 de Seinfeld, Kramer visita un banco que promete dar $100 a cualquiera que no sea saludado con un “hola”. En su lugar, saludan a Kramer con un “hey”, lo cual él insiste que no es un “hola”, y por lo tanto pide $100. El gerente del banco propone un compromiso: “Recibiste un saludo que empieza con una ‘h’, ¿qué tal si te damos $20?” Kramer acepta.

En un archivo llamado bank.py, implementa un programa que le pida al usuario un saludo. Si el saludo empieza con “hola”, muestra $0. Si el saludo empieza con una “h” (pero no “hola”), muestra $20. De lo contrario, muestra $100. Ignora cualquier espacio en blanco al principio del saludo del usuario y trata el saludo del usuario sin importar mayúsculas y minúsculas.

Pistas
Recuerda que una cadena (str) tiene bastantes métodos, según docs.python.org/3/library/stdtypes.html#string-methods.
Asegúrate de dar $0 no solo por “hola” sino también por “hola a todos”, “hola, Newman” y similares.

## Antes de Comenzar

Inicia sesión en cs50.dev, haz clic en tu ventana de terminal y ejecuta `cd` por sí solo. Deberías ver que el indicador de la ventana de tu terminal se asemeja a lo siguiente:

```bash
$
```

Luego ejecuta

```bash
mkdir bank
```

para crear una carpeta llamada bank en tu espacio de código.

Luego ejecuta

```bash
cd bank
```

para cambiar de directorio a esa carpeta. Ahora deberías ver el indicador de tu terminal como bank/ $. Ahora puedes ejecutar

```bash
code bank.py
```

para crear un archivo llamado bank.py donde escribirás tu programa.

## Cómo Probar

Así es como puedes probar tu código manualmente:

Ejecuta tu programa con

```bash
python bank.py
```

Escribe Hello y presiona Enter. Tu programa debería mostrar:

$0

Ejecuta tu programa con

```bash
python bank.py
```

Escribe Hello, Newman y presiona Enter. Tu programa debería mostrar:

$0

Ejecuta tu programa con

```bash
python bank.py
```

Escribe How you doing? y presiona Enter. Tu programa debería mostrar:

$20

Ejecuta tu programa con

```bash
python bank.py
```

Escribe What's happening? y presiona Enter. Tu programa debería mostrar:

$100

Puedes ejecutar lo siguiente para verificar tu código usando check50, un programa que CS50 usará para probar tu código cuando lo envíes. ¡Pero asegúrate de probarlo tú mismo también!

```bash
check50 cs50/problems/2022/python/bank
```

Las caritas verdes significan que tu programa ha pasado una prueba. Las caritas rojas indicarán que tu programa mostró algo inesperado. Visita la URL que check50 te proporciona para ver la entrada que check50 entregó a tu programa, qué salida esperaba y qué salida dio tu programa realmente.

Cómo Enviar
En tu terminal, ejecuta lo siguiente para enviar tu trabajo.

```bash
submit50 cs50/problems/2022/python/bank
```
