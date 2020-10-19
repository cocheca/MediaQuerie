# MediaQuerie

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


