# Responsive Design ::: https://platzi.com/clases/responsive-design/ 

## Clase 2

### Patrones en Reponsive Design:

Mostly Fluid
Colocación de columnas
Layout shifter
Tiny tweaks
Off canvas
Para mas información: https://mediaqueri.es

### Conceptos nuevos:

Viewport: área visible del navegador
Portrait: vertical
Landscape: horizontal
Mobile first: empezar un websit desde la menor resolución soportada
Deskto first: empezar un websit desde la mayor resolución soportada
¿Cúal es mejor?: Técnicamente Mobile First

## Clase 4 Developer tools para Responsive Design

Usando la herramienta de inspeccion, seleccion responsivo o bien tipo de pantalla... Luego con el menu lateral se puede ver las medias queries y/o la regla.
 - AZUL se muestras las medias queries con max-width (hasta)
 - NARANJA se muestras las medias queries con min-width (desde)


## Clase 5
INDEX.html

```
<meta name="viewport" content="width=device-width, initial-scale=1.0">

width=device-width para que se adapte según la pantalla del dispositivo
initial-scale=1.0 para indicar el escalado según el dispositivo
maximun-scale 
```

---------------------------------
## Clase 6
Unidades relativas de medida:

### Porcentaje: longitud referente al tamaño de los elementos padre
em: unidad relativa al tamaño de fuente especificada más cercano
rem: unidad relativa al tamaño de fuente especificada en el ancestro más lejano (html o body)
vw / vh: unidad relativa porcentual con respecto al viewport

---------------------------------
## Clase 7 Medias Queries
max-width = hasta
min-width = desde

### Mobile First usa min-width y Desktop First usa max-width
```
@media media type and (condición) { }
@media screen and (max-width: 768px) and (min-width: 480px) {}
```

### Mobile Firts
```
@media screen and (min-width: 320px) { }
@media screen and (min-width: 480px) { }
@media screen and (min-width: 768px) { }
@media screen and (min-width: 1024px) { }
```

### Desktop Firts
```
@media screen and (max-width: 1024px) { }
@media screen and (max-width: 768px) { }
@media screen and (max-width: 480px) { }
@media screen and (max-width: 320px) { }
```

-----------------------------------
## Clase 8 Formas de incluir medias queries 

Breakpoints estandarizados que debemos de tener en cuenta:

Móviles: entre 320 y 480 píxeles.
Tablets: entre 768 y 1024 píxeles.
Pantallas grandes: más de 1024 píxeles o más.

VER....
```
full-4k{
	@media screen and (max-width: 2000px){
		content;
	}
}
desk{
	@media screen and (max-width: 1024px){
		content;
	}
}
tablet{
	@media screen and (max-width: 768px){
		content;
	}
}
phone{
	@media screen and (max-width: 480px){
		content;
	}
}
mini-phone{
	@media screen and (max-width: 320px){
		content;
	}
}
```

## Clase 9
REPOSITORIO >>> https://github.com/LeonidasEsteban/responsive-design-portafolio

## Clase 10
Diseño elástico con max-width y flex-wrap

```
flex-wrap: wrap;
```

Para ver >>> https://flexboxfroggy.com/#es 

## Clase 13 Ajustando la sección de eventos

## Clase 15 CSS Positions
https://codepen.io/LeonidasEsteban/pen/VGWzWK

https://github.com/MineiToshio/CursosPlatzi/tree/master/Curso%20de%20Responsive%20Design

https://github.com/MineiToshio/CursosPlatzi

## Clase 18 Video Insertado

Para calcular la proporción de nuestro vídeo:
height * 100 / width

```
.flexible-video {
    width: 100%;
    height: 0;
    padding-top: 56.25%;
    position: relative;
}
```

```
.html-video {
    width: 100%;
    height: auto;
}
```

## Clase 19 Fuentes de Iconos 
https://icomoon.io/

## Clase 20 Menu Hamburg

```
.burger-button {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  background-color: rgba(0,0,0,.5);
  display: none;
  line-height: 40px;
  text-align: center; 
  position: fixed;
  z-index: 13;
  top: 5px;
  left: 5px; 
  color: white;
}
```

## Clase 21 Posicionando el menú
```
.menu {
	position: fixed;
	background-color: rgba(5, 111, 255, .9);
	z-index: 3;
	top: 0;
	left:-100vw; /* Para que el menu se oculte a la izquierda y se cree el efecto al hacer click*/
	width: 100vw;
	bottom: 0;/* height: 100vw; */ /*A partir de aqui para centrar*/
	display: flex;
	align-items: center;
	justify-content: center; /* centrar hasta aqui */
	transition: .3s; /* Para crear efecto de transición */
}
.menu.is-active {
	left: 0;
}
```

## Clase 22 Posicionando el menú
```
 <script>
console.log('Hola mundo');

const menu= document.querySelector('.menu')
console.log(menu);
const burgerButton=document.querySelector('#burger-menu');
console.log(burgerButton);

burgerButton.addEventListener('click', hideshow);

function hideshow(){
	if(menu.classList.contains('is-active')){
	menu.classList.remove('is-active');
}
else{
	menu.classList.add('is-active');
}
}
</script>
```

## Clase 23 Media queries con JavaScript

```
const ipad = window.matchMedia('screen and (max-width: 767px)');
const menu = document.querySelector('.menu');
const burgerButton = document.querySelector('#burger-menu');

ipad.addListener(validation);
function validation(event) {
	if (event.matches) {
        	console.log('true');
                burgerButton.addEventListener('click', hideShow);
        } else {
        	console.log('false');
                burgerButton.removeEventListener('click', hideShow);
        }
}

function hideShow() {
	menu.classList.contains('is-active') ? menu.classList.remove('is-active') : menu.classList.add('is-active');
}
```

```
if(ipad.matches && window.screen.width < 768) {
  console.log(ipad.matches);
        
  menuButton.addEventListener('click', (e) => {
    menuBurger.classList.toggle('is-active')
  })
}
```

## Clase 24 Creando un servidor de archivos estáticos con Node

https://www.npmjs.com/package/static-server

https://nodejs.org/es/

https://chrome.google.com/webstore/detail/web-server-for-chrome/ofhbbkphhbklhfoeikjpcbhemlocgigb

https://www.makeuseof.com/tag/mirror-android-screen-pc-mac-without-root/

## Clase 26 Remote debbuging iOS

```
validation(ipad)
```

## Clase 27 Remote debbuging Android

https://chrome:inspect/#devices

https://developers.google.com/web/tools/chrome-devtools/remote-debugging?hl=es






