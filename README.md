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



