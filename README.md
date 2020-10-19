# MediaQuerie

##Clase 5
INDEX.html

<meta name="viewport" content="width=device-width, initial-scale=1.0">

width=device-width para que se adapte según la pantalla del dispositivo
initial-scale=1.0 para indicar el escalado según el dispositivo
maximun-scale 

---------------------------------
##Clase 6
Unidades relativas de medida:

Porcentaje: longitud referente al tamaño de los elementos padre
em: unidad relativa al tamaño de fuente especificada más cercano
rem: unidad relativa al tamaño de fuente especificada en el ancestro más lejano (html o body)
vw / vh: unidad relativa porcentual con respecto al viewport

---------------------------------
##Clase 7 Medias Queries
max-width = hasta
min-width = desde

###Mobile First usa min-width y Desktop First usa max-width
@media media type and (condición) { }
@media screen and (max-width: 768px) and (min-width: 480px) {}

###Mobile Firts
@media screen and (min-width: 320px) { }
@media screen and (min-width: 480px) { }
@media screen and (min-width: 768px) { }
@media screen and (min-width: 1024px) { }

Desktop Firts
@media screen and (max-width: 1024px) { }
@media screen and (max-width: 768px) { }
@media screen and (max-width: 480px) { }
@media screen and (max-width: 320px) { }

-----------------------------------
##Clase 8 Formas de incluir medias queries 

Breakpoints estandarizados que debemos de tener en cuenta:

Móviles: entre 320 y 480 píxeles.
Tablets: entre 768 y 1024 píxeles.
Pantallas grandes: más de 1024 píxeles o más.

VER....
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

REPOSITORIO >>> https://github.com/LeonidasEsteban/responsive-design-portafolio
