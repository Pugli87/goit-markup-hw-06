# goit-markup-hw-05
Tarea 5


-    Cree el repositorio goit-markup-hw-05.  ----------> OK
-    Clone el repositorio creado y copie los archivos de trabajo anteriores en él.  ----------> OK
-   Agregue efectos decorativos animados a las páginas de diseño de la tarea de casa #5.  ----------> OK
-   Configure las GitHub Pages y agregue un enlace a la página en vivo en el encabezado del repositorio de GitHub.  ----------> OK
-   Los criterios de aceptación de trabajo por parte del tutor  ----------> OK

El proyecto

«A1» Todos los estilos están contenidos en un archivo styles.css, que se encuentra en la carpetacss.  ----------> OK

«A2» El código fuente está formateado con Prettier. «A3» Todas las imágenes y el contenido del texto se toman del diseño.  ----------> OK

«A4» Todas las páginas HTML tienen un normalizador de estilo modern-normalize.  ----------> OK

«A5» El código está escrito siguiendo. la guía.  ----------> OK

«A6» El script de ventana modal está vinculado en HTML como un archivo separado llamado modal.js.   ----------> OK



El marcado

«B1» El marcado HTML se realiza para todos los elementos de diseño. «B2» Las etiquetas se utilizan según su semántica.  ----------> OK



El diseño


«C1» Para todos los efectos de desplazamiento y enfoque (color, fondo, sombra), se realizan transiciones. Tiempo - 250ms, la función de distribución de tiempo - cubic-bezier(0.4, 0,    0.2, 1).

«C2» Las propiedades animadas se especifican explícitamente en transiciones y animaciones. No hay ningún valor de all en ninguna parte.

«C3» En la sección Qué hacemos el texto con fondo se coloca sobre la imagen.

«C4» En la navegación principal, el enlace de la página actual (que el usuario está viendo actualmente) está subrayado usando el pseudo-elemento ::after.

«C5» Aparece una superposición azul con texto en las tarjetas de la página Portafolio al pasar el cursor sobre cualquier parte de la tarjeta.

«C6» La superposición azul se desliza desde la parte inferior de las tarjetas en la página de Portafolio como se muestra en el video.

card overlay preview
«C7» Los pseudo-elementos no tienen contenido de texto en la propiedad content. Se utilizan exclusivamente con fines decorativos.

Ventana modal
«D1» Se realizan el marcado y diseño de «backdrop» (fondo semitransparente oscuro) de la ventana modal.

«D2» «Backdrop» ocupa el 100% de la altura y el ancho de la ventana del navegador y permanece fijo en él.

«D3» El marcado y el diseño de la ventana modal están hechos.

«D4» La ventana modal se coloca vertical y horizontalmente en el medio del backdrop.

«D5» El marcado y el diseño del botón para cerrar la ventana modal en la esquina superior derecha están listos.

«D6» Inicialmente, la ventana modal y el backdrop están ocultos con la ayuda de la clase is-hidden en el backdrop cuyo selector utiliza propiedades visibility, opacity y pointer-events.

«D7» Si eliminar la clase is-hidden del backdrop, aparecerá el backdrop y la ventana modal.

«D8» La aparición y desaparición de la ventana modal se anima mediante una transición con un efecto arbitrario, por ejemplo scale o translate, y opacity.

_____________________________________________________________________________________________________________________________________________________________________________________
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _
_____________________________________________________________________________________________________________________________________________________________________________________


Te recomiendo encarecidamente que revises tu trabajo y lo corrijas si no lo has entregado todavía. O que le des otra ojeada simplemente.

-   El formulario que se encuentra en el pie de página. Fíjate en la manera que que está situado ahí, está pegado al borde derecho del contenedor.

-   El posicionamiento de los iconos en input. Es por lo general este tipo de construcción: un div común, en el que se encuentra label, input и un icono svg. 

-   El ícono se posiciona con  absolute, en relación a su parental div. Input - es el elemento contiguo al icono. 
    También sería erróneo (inútil) indicar al input position: relative. Se puede intuir el posicionamiento hasta que sea parecido visualmente, 
    pero eso tampoco será técnicamente correcto.

-   Para colocar el icono correctamente, hay varias opciones, pero la más fácil y sencilla para usted es input y poner el icono svg en div. 
    A este contenedor hay que asignarle position:relative. 
    svg- position:absolute. Y entonces habrá un posicionamiento de iconos claro y competente, 
    esto debido a que absolute viene del flujo del documento, y div tomó las medidas de input

-   En caso de posicionamiento absoluto, no olvide que se necesitan dos puntos. Por ejemplo: top y left. Aún cuando visualmente no cambie nada.

-   Cuando ponga por ejemplo top:50% no olvides que no es exactamente el centro deseado. Para que éste sea realmente el deseado, añada transform: translateY(-50%);

-   No olvides hacer focus en la casilla personalizada.