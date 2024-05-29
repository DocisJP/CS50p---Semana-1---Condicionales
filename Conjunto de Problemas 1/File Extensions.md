Extensiones de Archivos
Aunque Windows y macOS a veces las ocultan, la mayoría de los archivos tienen extensiones de archivo, un sufijo que comienza con un punto (.) al final de su nombre. Por ejemplo, los nombres de archivo para GIFs terminan con .gif, y los nombres de archivo para JPEGs terminan con .jpg o .jpeg. Cuando haces doble clic en un archivo para abrirlo, tu computadora usa su extensión para determinar qué programa lanzar.

Los navegadores web, por el contrario, dependen de los tipos de medios, anteriormente conocidos como tipos MIME, para determinar cómo mostrar los archivos que residen en la web. Cuando descargas un archivo de un servidor web, ese servidor envía un encabezado HTTP, junto con el archivo mismo, indicando el tipo de medio del archivo. Por ejemplo, el tipo de medio para un GIF es image/gif, y el tipo de medio para un JPEG es image/jpeg. Para determinar el tipo de medio de un archivo, un servidor web generalmente observa la extensión del archivo, mapeando una con la otra.

Consulta developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types/Common_types para tipos comunes.

En un archivo llamado extensions.py, implementa un programa que pida al usuario el nombre de un archivo y luego muestre el tipo de medio de ese archivo si el nombre del archivo termina, sin importar mayúsculas o minúsculas, en cualquiera de estos sufijos:

.gif
.jpg
.jpeg
.png
.pdf
.txt
.zip
Si el nombre del archivo termina con otro sufijo o no tiene sufijo en absoluto, muestra application/octet-stream en su lugar, que es un valor predeterminado común.

Pistas
Recuerda que una cadena (str) tiene bastantes métodos, según docs.python.org/3/library/stdtypes.html#string-methods.

## Antes de Comenzar

Inicia sesión en cs50.dev, haz clic en tu ventana de terminal y ejecuta `cd` por sí solo. Deberías ver que el indicador de la ventana de tu terminal se asemeja a lo siguiente:

```bash
$
```

Luego ejecuta

```bash
mkdir extensions
```

para crear una carpeta llamada extensions en tu espacio de código.

Luego ejecuta

```bash
cd extensions
```

para cambiar de directorio a esa carpeta. Ahora deberías ver el indicador de tu terminal como extensions/ $. Ahora puedes ejecutar

```bash
code extensions.py
```

para crear un archivo llamado extensions.py donde escribirás tu programa.

## Cómo Probar

Así es como puedes probar tu código manualmente:

Ejecuta tu programa con

```bash
python extensions.py
```

Escribe happy.jpg y presiona Enter. Tu programa debería mostrar:

image/jpeg

Ejecuta tu programa con

```bash
python extensions.py
```

Escribe document.pdf y presiona Enter. Tu programa debería mostrar:

application/pdf

Asegúrate de probar cada uno de los otros formatos de archivo, variar las mayúsculas y minúsculas de tu entrada, y "accidentalmente" añadir espacios a ambos lados de tu entrada antes de presionar Enter. Tu programa debería comportarse como se espera, sin importar mayúsculas y espacios.

Puedes ejecutar lo siguiente para verificar tu código usando check50, un programa que CS50 usará para probar tu código cuando lo envíes. ¡Pero asegúrate de probarlo tú mismo también!

```bash
check50 cs50/problems/2022/python/extensions
```

Las caritas verdes significan que tu programa ha pasado una prueba. Las caritas rojas indicarán que tu programa mostró algo inesperado. Visita la URL que check50 te proporciona para ver la entrada que check50 entregó a tu programa, qué salida esperaba y qué salida dio tu programa realmente.

Cómo Enviar
En tu terminal, ejecuta lo siguiente para enviar tu trabajo.

```bash
submit50 cs50/problems/2022/python/extensions
```
