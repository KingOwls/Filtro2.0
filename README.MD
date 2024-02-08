# R0equerimientos Tecnicos

<https://kingowls.github.io/Filtro2.0/>

Para desarrollar la división del proyecto FrontEnd se deben tener los siguientes puntos en cuenta:

1. El sitio debe ser totalmente responsivo
2. Se debe utilizar metodología BEM para nombrar las clases CSS.
3. Para el diseño responsivo solo se permite el uso de grid y flex para posicionamiento
4. El proyecto debe ser publicado en git como page.
5. El sitio debe contener transiciones y animaciones.
6. Cada producto debe estar contenido en una tarjeta. En una imagen y debajo un funcioamiento de Nombre
7. Cuando el usuario seleccione algún producto se debe mostrar una pagina con la descripción del producto.
8. Cuando el usuario seleccione una imagen pequeña se debe cambiar la imagen central. Se debe hacer el cambio aplicando una transición.
9. El repositorio debe contar con readme donde se debe explicar las reglas de estilo creadas en el proyecto.
10. Debe verse unicamente por Bem, y Greed
11. La imagen debe cambiar por medio de una animacion y estilizaion
12. Hacer una trancision de opacidad y color donde muestre un pequeño resumen de nombre, y caracteristicas.

## Criterios de entrega

1. Se debe cargar en el classroom el enlace del repositorio.
2. El plazo de entrega del proyecto es a las 14:00
3. No se aceptaran entregas posteriores a la fecha y hora.
4. No se reciben trabajos vía correo electrónico.
5. El proyecto debe estar publicado como Page en git.

### Anotaciones

Extender y programar un grupo de opacidad para el funcionamiento de extencion, y en caso de ser requerido cambio de imagen por medio de una transicion.
De la misma forma hacer correctamente las tablas y su funcionamiento extendido
recordar Posicionamiento dependiendo del navegador
ademas de eso tener en cuenta las margenes y su modelado para celulares teniendo que recordar el ajustarse

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

` * {
	font-family: 'Open Sans', sans-serif;
	margin: 0;
	padding: 0;
	box-sizing: border-box;
}`
Esta primera parte se trata de la definicon total del codumento siendo este mismo el que presenta un formato estandar a toda la pagina web por lo que se maneja el modelado y el cual pueda adaptarse

`
:root {
	--grey: #9fd5d1;
	--light: #ffda9e;
}
`

Este se trata de los colores utilizados en el decorado de la pagina web, estando centrado en el diseño y los colores de fondo buscando un margen mas agradable a la vista y su diseño estandar

`
body {
	background: var(--grey);
	overflow-x: hidden;
}
`

En esta parte se trata las formas utilizadsas en el cuerpo y los mismos como se ven afectados para el diseño del trabajo

`
/* SIDEBAR */
#sidebar {
	position: fixed;
	max-width: 260px;
	width: 100%;
	background: var(--light);
	top: 0;
	left: 0;
	height: 100%;
	overflow-y: auto;
	scrollbar-width: none;
	transition: all .3s ease;
	z-index: 200;
	overflow: scroll;
}`
Este se trata de hacer el diseño de como se ve cada uno de las cadas y el funcionamiento de su contenido, dandole una marge, una visibilidad una estructuracion y su funcionamiento, esta es la caja lateral que se encuentra en la pagina
/* CONTENT */

` #content {
	position: relative;
	width: calc(100% - 260px);
	left: 260px;
	transition: all .3s ease;
}`
Este es el contenido, cada una de las csoasas que se tratan dentro de los cajones funcionando con cada uno de las cajas internas

/* MAIN */

`main {
	width: 100%;
	padding: 24px 20px 20px 20px;
}`
ajuste para las margenes del main
` main .info-data {
	margin-top: 36px;
	display: grid;
	grid-template-columns: repeat(auto-fit, minmax(150px, 3fr));
	grid-gap: 20px;
}`
contenido de informacion del mismo

` main .info-data .card {
	padding: 20px;
	border-radius: 10px;
	background: var(--light);
	box-shadow: 4px 4px 16px rgba(0, 0, 0, .05);
}`
cada una de las targetas y como estas tienen margenes y sombreado

`main .card .head {
	display: flex;
	justify-content: space-between;
	align-items: flex-start;
}`

`main .card .head p {
	font-size: 14px;
}`
/*classes ain*/

`.buttonContact{
    padding: 10px;
    background-color: #b0f2c2;
    border-radius: 50px;
    margin: 0 auto;
}`
Los botones decorados dentro de los productos propuestos
`.buttonContact:hover{
    filter: opacity(0.95);
    transform: scale(1.14);
}`

`@media screen and (max-width: 768px) {
	#content {
		position: relative;
		width: calc(100% - 60px);
		transition: all .3s ease;
	}
}`
Ajuste del respansivo
/*colores usados*/
`.other{

    color: #b2e2f2;
    color: #b0f2c2;
}`
/*animacion*/
Animacion del carrito de compras defineindolo para que se pueda mover de derecha a izquierda
`.carrito-compras {
    animation-name: Carrito;
    animation-duration: 5s;
  }`
  
`@keyframes Carrito{
    0% {
      transform: translateX(0);
    }
    50% {
      transform: translateX(200px);
    }
    100% {
      transform: translateX(0);
    }
  }`