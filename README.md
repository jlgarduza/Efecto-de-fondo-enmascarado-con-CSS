# Efecto-de-fondo-enmascarado-con-CSS
Hoy vamos a crear paso a paso una técnica realmente asombrosa que puedes usar como un efecto muy parecido al desplazamiento parallax, sin usar nada de JavaScript, se puede lograr simplemente a través de solo CSS
<p><img src="https://cms-assets.tutsplus.com/uploads/users/53/posts/21112/image/scrolling.gif"></p>
<p>Esta técnica podría ser usada para crear páginas con geniales descripciones de productos, o incluso algo parecido a una presentación PowerPoint/Keynote, y sería genial para las ilustraciones de alguna historia en linea.</p>
<br />
Todo esta en el CSS
La clave para esta técnica con CSS es background-attachment: fixed;, disponible desde la versión 2.1. Cualquier imagen de fondo con este estilo se aplicará a la misma y se mantendrá en una posición fija con respecto a la ventana (no al elemento que se aplica). Lo usaremos para mantener nuestras ilustraciones en un lugar mientras nuestro contenido se desplaza independientemente de él.

Un par de cosas a tener en cuenta con esta propiedad son que como imágenes de fondo se fijarán en relación a la ventana, su posición no se verá afectada por cosas como márgenes en el camino como otra imagen de fondo lo haría.

También deberías saber que, si bien la propiedad funciona de maravilla en todos los navegadores de escritorio, no funciona correctamente con la versión móvil de Chrome y puede ser un poco distinto en los otros navegadores móviles. Así, mientras los visitantes ven las imágenes bien, el efecto de este desplazamiento puede verse mucho mejor en los navegadores de escritorio.

Cómo se hace
Los pasos básicos para lograr tal efecto como se ve en la versión online son:

Crear un elemento contenedor y agregar el contenido a él.
Ajusta el contenedor (un div en nuestro caso) para tener padding en un lado alrededor del 50% de anchura, y así empuje el contenido hacia el otro lado.
Agrega una imagen de fondo, también con un 50% de anchura, y posiciónala en el lado contrario al contenido.
Ajusta la propiedad background-attachment: fixed; y ve la magia del desplazamiento.
Vamos a ver paso a paso cómo hacer todo esto. Necesitarás los archivos iniciales para este tutorial con las imágenes requeridas.

1. Configuración Básica
Empieza por crear la carpeta del proyecto, y agrega un archivo index.html dentro, también una carpeta css con un archivo de nombre style.css y guárdalo. Copia y pega las cuatro imágenes que descargaste de los archivos iniciales dentro de una carpeta de nombre images.

Agrega este HTML al index.html:
