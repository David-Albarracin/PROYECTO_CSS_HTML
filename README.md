![css](https://raw.githubusercontent.com/David-Albarracin/README_MATERIALS/main/css-html-js.png)

# PROYECTO HTML Y CSS

La creación de la página de E-Commerce comienza con un paso crucial Primero se establece la estructura de carpetas, cuidadosamente diseñada para cumplir con los requisitos específicos del proyecto. Este proceso sienta las bases sólidas para el desarrollo, asegurando una implementación eficiente y cumpliendo con las expectativas y necesidades del proyecto de comercio electrónico tecnodoctor punto cell

![Estructura](https://raw.githubusercontent.com/David-Albarracin/README_MATERIALS/main/estructure-folders.png)

Con la estructura diseñada, avanzamos hacia la creación de 'base.css'. Esta base desempeña un papel fundamental al proporcionarnos un diseño sólido para nuestro proyecto. Introducimos variables locales en la declaración ':root{}', permitiéndonos establecer una paleta de colores cohesiva y generalizar el tamaño de las fuentes. Además, personalizamos los estilos predeterminados de las etiquetas a, ul, button, img, garantizando así una coherencia visual en toda la interfaz

![base](https://raw.githubusercontent.com/David-Albarracin/README_MATERIALS/main/base-css.png)

Ahora, nos enfocaremos en la creación de breakpoints para diversas visualizaciones en dispositivos móviles, tomando como referencia la temática de [Bootstrap](https://getbootstrap.com/docs/5.0/layout/grid/). Nos inspiraremos en las clases proporcionadas por Bootstrap para lograr un diseño más responsivo y adoptaremos el concepto de clases reusables, facilitando así un desarrollo rápido y eficiente. Es importante destacar que, aunque nos apoyamos en esta biblioteca como referencia, no se utilizará directamente en nuestro proyecto

```

/*========== Small (sm) ==========*/
@media (min-width: 576px) {

}

/*========== Medium (md) ==========*/
@media (min-width: 768px) {

}

/*========== Large (lg) ==========*/
@media (min-width: 992px) {

}


/*========== Extra large (xl) ==========*/
@media (min-width: 1200px) {

}

/*========== Extra extra large (xxl) ==========*/
@media (min-width: 1400px) {

}
```

Considerando lo mencionado anteriormente, avanzamos al siguiente paso donde alimentaremos el layout.css con clases reusables. Algunas de ellas son

```
/*Vuelve en Contenedor Flexible*/
.d-flex{
    display: flex;
}

/*Vuelve en Contenedor Grid*/
.d-grid{
    display: grid;
}

/*Nos da un margen en el eje x (izquierda y derecha de 0.5rem)*/
.mx-1{
    margin-left: 0.5rem;
    margin-right: 0.5rem;
}

/*Nos da un margen en el eje x y un tamaño maximo del contenedor*/
.container {
    --bs-gutter-x: 1.5rem; /* Variable que almacena 1.5rem como espacio horizontal */
    --bs-gutter-y: 0;      /* Variable que almacena 0 como espacio vertical */

    width: 100%;           /* Hace que el contenedor ocupe toda la pantalla */

    /* Margenes y padding en el eje x. Se utiliza calc() para realizar la operación de multiplicación */
    padding-right: calc(var(--bs-gutter-x) * 0.5);
    padding-left: calc(var(--bs-gutter-x) * 0.5);
    
    margin-right: auto;    /* Margen derecho automático para centrar el contenedor horizontalmente */
    margin-left: auto;     /* Margen izquierdo automático para centrar el contenedor horizontalmente */
}

```

Después de establecer la estructura de carpetas y los estilos base, nuestro próximo paso consiste en avanzar con el desarrollo de 'home.html'. Esta página servirá como la primera impresión para el usuario, presentando inicialmente el encabezado (header) con el logo y enlaces de navegación, que incluyen opciones como inicio, catálogo, contáctanos y sobre nosotros. A continuación, se presenta un banner publicitario, seguido por una sección de tres productos destacados. Finalmente, el (footer) incluirá información de contacto, enlaces rápidos y un buscador. Es importante destacar que tanto el (header) como el (footer) se mantendrán consistentes a lo largo de las demás páginas de nuestro proyecto, proporcionando una experiencia cohesiva y fácil de navegar



![header](https://raw.githubusercontent.com/David-Albarracin/README_MATERIALS/main/PROYECTO-HTML-CSS-JS/header.png)

Esta es la hoja de estilo del header que contiene diferentes clases de estilo.    La primera es .header, que es un contenedor flex con posición fijada que nos ayuda para cuando el cursos baje el header se mantenga en pantalla y un nivel 3D 1 para que este por encima de los demas objetos y se le agrego un sombreado sutil en la parte inferior.

Luego tenemos la clase .nav la cual se le aplica a la etiqueta nav que contiene los enlaces de navegación, como el logo y el menú desplegable.    Tiene un ancho y alto del 100%, y su contenido está distribuido con espacio entre ellos y alineados al centro.

La clase .nav__logo se utiliza para especificar el estilo del logo.    Establece un ancho de 160px y evita que la imagen supere este límite.

La clase .nav__menu se encarga del estilo del menú desplegable.    Inicialmente, está oculta (display: none) y se posiciona fija en la parte superior del contenedor.    Tiene un fondo de color diferente y un nivel 3D superior para superponerse al header.

.nav__link establece el estilo de los enlaces de navegación.    Se aplica un relleno, margen y tamaño de fuente específicos. Luego a esto se le aplica una clase de estado de tipo hover que le da un borde y un color de fondo

Luego la clase .nav__buttons, .nav input y close hacen parte del menu mobile las cuales se les aplica estilos en una media query entonces esta la clase .nav input:checked que hace que cuando el input este en el estado check este active la clase nav_menu con el display block la siguiente lo que hace es que cambie el label por un icono de x y esconda el icono de menu luego lo que hacemos es que el input checado cambie el estado del menu para poderlo ver

![footer](https://raw.githubusercontent.com/David-Albarracin/README_MATERIALS/main/PROYECTO-HTML-CSS-JS/footer.png)

Ahora la hoja de estilo footer que nos ayuda con los estilos de pie de pagina empezando con la clase `.footer` define los estilos aplicados al pie de página de la página web. Este componente proporciona espaciado, sombra y color de fondo.

![product](https://raw.githubusercontent.com/David-Albarracin/README_MATERIALS/main/PROYECTO-HTML-CSS-JS/product.png)

Esta hoja de estilo product.css es la que contiene todos las clases que se le aplican al producto en la vista de su card y la vista de su visualizacion completa en su propia product.html, 

![category](https://raw.githubusercontent.com/David-Albarracin/README_MATERIALS/main/PROYECTO-HTML-CSS-JS/category.png)

Esta es la hoja de estilos que se le aplica a las categorias para que parescan botones y que tengan un border sutil y que entre categorias se separe un poco entre ellas 

![about](https://raw.githubusercontent.com/David-Albarracin/README_MATERIALS/main/PROYECTO-HTML-CSS-JS/about.png)

Esta hoja de estilos nos ayuda a darle estilos a about.html y contact.html la clase que mas resalta es la de swiper esta nos ayuda a hacer un pequeño estilo tipo carrusel para darle una forma mas profecional 

![style](https://raw.githubusercontent.com/David-Albarracin/README_MATERIALS/main/PROYECTO-HTML-CSS-JS/style.png)

Esta es la hoja de estilos principal que nos ayuda a importar todos las otras hojas de estilos como es la principal es la que se importa en todos los html y nos ayuda a tener una maquetado mas modular 
