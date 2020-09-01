### Comentarios Generales

Tania, queria felicitarte primero por un gran portfolio. Tu web está hermosa: me encanta como adaptaste las tarjetas, los colores, la imagen, todo te refleja y da una imagen maravillosa de vos en tus primeros pasos como desarrolladora front end. Se nota en cada linea de codigo que pusiste un monton de esfuerzo. 

Entiendo que no llegaste tan bien con el tiempo, por lo que noto que algunas consignas no estan incumplidas. El responsive no funciona correctamente, en parte por algunos detalles en el CSS que te voy a comentar mas en detalle. 
- En todas las resoluciones de escritorio, los textos debajo de "Mis conocimientos" y la cita se ven algo desprolijos por ocupar todo el ancho de la pantalla. Quiza darles un width a .parrafo-conocimientos y a .frase-texto ayude a que se vean mejor. 
- En resoluciones de escritorio pequeñas (1024px) la sección principal queda tirada a la izquierda, algo que podriamos corregir con un justify-content: center en .seccion-mi-info.
- En tablet (768px) la barra de navegacion no entra, por lo que el último link queda tirado hacia abajo. Tenés dos opciones: modificar la media query para que la barra de navegación desaparezca antes, y aparezca en esta resolución el ícono hamburguesa, o reducir el margin que tiene .elemento-menu. Tambien en esta resolución tus tarjetas de Proyectos se ven de a una, aunque entrarían comodamente dos: eso es porque .contenedor-proyectos tiene un width de 60vw, que si bien funciona en escritorio, no queda tan bien aquí. Por último, nota que en esta resolución tu barra de navegación del footer rebalsa su contenedor y pisa los iconos. Eso ocurre porque tanto .menu-footer como .lista-navegacion-footer tienen un height, algo que no es recomendable justamente por casos como este. 
- En celulares tu maquetado se ve mucho mejor, y me alegra que es allí donde enfocaste tus esfuerzos para la media query, ya que es realmente lo más importante. El unico problema que noto alli es cierto scroll horizontal (lo vas a ver como una barra blanca a la izquierda) que ocurre porque .foot tiene width:100%. Con sacarlo se soluciona. Quiza tambien se le podria agregar un margin-right a .menu-hamburguesa para que no se vea tan pegado al borde de la pantalla. 

Tu repositorio está ordenado, y cuenta con un buen README. Debo mencionar que hay relativamente pocos commits. Si bien entiendo que no es fácil subir un código cuando está recién empezado y lleno de problemas, es lo mejor, tanto para irse acostumbrando una a hacerlo, como para permitir que colegas (y profes!) puedan ver la evolución del código y encontrar rapidamente los commits en donde se hicieron determinados cambios. Cuando trabajamos en equipo es muy importante hacer commits breves, asi cualquier cambio puede identificarse facilmente. 

Dejo algunos comentarios generales sobre tu trabajo: 

- Tu HTML esta muy prolijo, ordenado y bien tabulado. Usas correctamente las etiquetas semánticas, no agregaste mucho código de más (algo que suele ser habitual al comenzar) y se nota el esfuerzo por dejarlo lo más claro posible. 

- Tu CSS esta muy bien ordenado. Se nota que le pusiste trabajo. Aprecio que te hayas tomado el trabajo de ordenar los estilos generales arriba de todo y que tu CSS vaya siguiendo la estructura de tu web. Noto que usas un tabulado particular, me da la impresión de que pones mas hacia la derecha los elementos que son hijos de otros; sin embargo esto no es lo habitual, ni lo recomendable: el tabulado siempre se mantiene igual, al menos cuando trabajamos con CSS puro (vamos a ver más adelante algunas herramientas como SASS que hacen algo similar a lo que vos haces aca)

- Ocasionalmente usas alturas fijas para las secciones, y eso no es buena práctica: salvo cuando se trata de elementos pequeños (como tarjetas o botones), la altura de un elemento tiene que estar dada por sus contenidos. Tambien noto que usas mucho height 100%, pero eso no tiene mucho sentido para una seccion: es una orden que no se va a aplicar. 

- Noto que repetis muchas veces font family. Recorda que esta se hereda, asi que lo mas habitual es poner la que mas vamos a usar (en tu caso, si no me equivoco, Varela) en el body. Asi solo tenemos que modificar las de los titulos, etc. 

Dejo algunos comentarios específicos a lo largo de tu código. 

Notarás, viendo esos comentarios, que comento muchisimas cosas y soy bastante quisquillosa con las correcciones. La idea es comentarte todo lo que vea para que puedas mejorar tu código y que tu portfolio quede lo mejor posible. Ojala te sirva :)  


### Nota final: 8

Nota desagregada: 
✅ Estructura correcta de documento HTML 
✅ Respeta la consigna 
✅ Respeta el diseño dado 
✔️  Responsive funciona correctamente ---> con observaciones
❌ Código bien indentado. 
✅ Comentarios que permiten mejorar la legibilidad del código.
✅ Uso correcto de etiquetas semánticas.
✔️ Buenos nombres de clases ---> con observaciones
✅ Reutilización de estilos.
✔️ Código CSS ordenado 
❌ Commits con mensajes adecuados.
