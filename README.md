# <u>Trabajo Practico-1</u>
## <u>Character Counter</u>
### <span style="color: violet;"> <u>Objetivo:</u></span>
El proyecto consistio, en mi caso, en crear componente de una web, estructurado en HTML y estilado con CSS.
El mismo, aunque no tiene funcionalidad todavia, tiene el objetivo de analizar un texto y su contenido , interpretando cantidad y variedad de letras como tambien cantidad de palabras y oraciones.

### <span style="color: violet;"> <u>Funcionalidad:</u></span>
Su funcionalidad consta de escribir texto dentro del recuadro y la web cumpliria la funcion del conteo de los datos que seteemos.

### <span style="color: violet;"><u>Tecnologias</u> :</span>
#### <u>Languages</u>
- HTML
- CSS
#### <u>External Assets</u>
- GoogleFonts: "Inter" Typography:(https://fonts.google.com/specimen/Inter)
- BoxShadow Generator: (https://html-css-js.com/css/generator/box-shadow/)
- FontAwesome: Used Icons: "Angle-Down","Sun".(https://fontawesome.com/)

## <span style="color: orange;"><u> HTML Estructure </u></span>
- head: metadata styles, typography (googlefonts) , icons (fontawesome),

El archivo HTML lo estructure principalmente con una **` <section class="main">`** para principalmente, tener control de mi contenedor dentro del **`<body>`**. Luego implemente **`<nav>`** con el objetivo de implementar una barra de navegacion que dentro tenga el logo **(`<img>`)**, el nombre del componente **(`<h3 class="subtitle">`)** y el boton **(`button class="switch"`)**; seguido de un contenedor **(`<div class="title">`)** para el subtitulo **(`<h2>`)** ,**(_lo considere como subtitulo ya que el proyecto en si lo tome como un componente de una web y no la web en si_)**
Cree un recuadro donde escribir texto **(`<textarea class="text-area">`)**, luego, considere hacer un contenedor padre (**`<div class="inputs">`)** para los **_inputs_** y el parrafo **(`<p>`)** con el objetivo de tener el control del estilado para los tres elementos, y a su vez anide un contenedor dentro solo para los  **_labels con sus inputs type="checkbox"_**.
Investigando implemente `<span class="icon-checked"></span>` para armar el estilado de marcado del **_checkbox_**.
Seguido, arme un contenedor padre **(`<section class="cards">`)** para las cajas de valores de conteo que dentro cada una de ellas estaria contenida por un **`<div>`** con su respectiva **_"class="_** y dentro su **`<h2>`** y su **`<p>`**.
En el caso de las barras de conteo aplique el mismo metodo que en las cajas de valores, un contenedor padre **(`<section class="progress-bar">`)** que dentro contiene un **(`<div>`)** para cada fila de letra y a su vez dentro, utilice **(`<progress>`)** para la barra de conteo.
Por ultimo, cree un contenedor **(`<div class="see-more">`)** para el texto **(`<h4>`)** y el botton **(`<button class="btn-more">`)** con el icono dentro.


## <span style="color: orange;"><u> CSS (Styles) </u></span>
Para los estilos:
1. Resetee los valores y coloque la tipografia brindada *{
    padding: 0;
    margin: 0;
    font-family: "Inter", sans-serif;}
2. Agregue las variables de las paletas de colores de los fondos y textos.   
3. Le di tamaño y elegi el espacio dentro de mi body para comenzar a estilar lo demas.
4. Le di forma y color de fondo a mi contenedor principal, aplique **_display: flex_** y **_flex-direction= column_** para que mis elementos se situen verticalmente.
5. Le di tamaño a mi **`<nav>`**, aplique **_display: flex_** y **_justify-content= between_** para que mis elementos se situen uno al lado de otro generando espacio entre ellos.
6. Le di **_display: flex; flex-direction: column_** a mi contenedor **(`<div class="nav-bar">`)** y un **_gap_** para generar el espacion entre la *`<img>`*y el **`<h3>`**. Agregue **_object-fit: contain;_** al logo para que no me desproporcione la imagen. 
7. Aplique fondo, colores, tamaño y **_hover:_** al boton.
8. Le di color y tamaño de letra al **`<h2>`**
9. Aplique estilos de colores, fondo, tamaño, al **`<textarea>`**. Coloque _resize: none;_ para que el usuario no pueda cambiar las dimensiones del area, y tambien agregue un **_box-shadow:_** para darle sombreado ya que me parecio adecuado utilizarlo aqui.
10. Coloque un contenedor padre **(`<div class="inputs">`)** para los **_inputs y el `<p>`_**, para tener el control de estilos de toda la linea.
Dentro del mismo anide un contenedor hijo (**`<div class="checkbox">`**) solo para los **_inputs type= "checkbox"_**.
Elimine los estilos por defecto de los inputs y asigne un **`<span class="icon-checked">`** para crear la nueva caja de marcado.
Cree el simbolo desde cero, lo rote y le asigne color.
11. Le di **_display: flex;_** a **`<section class="cards">`** para alinearlos horizontalmente con un **`<gap>`** determinado.
Luego a cada contenedor de cada caja le di estilos utilizando **.card1, .card2, .card3**: les brinde un tamaño y aplique **_flex: 1;_** para redimencionar las cajas en el espacio disponible, aplique imagenes de fondo **_background-image:_**,  y le di sus propiedades. Luego estile los textos dentro mediante clases diferentes (**.value**) y (**p**)
12. Para las barras de progreso cree un contenedor padre (**`<section class="progress-bar">`**) para aplicarles **_display: flex; flex-direction: column;_** para ubicarlos verticalmente con un **_gap** determinado.
    Dentro del mismo contenedor anide otros para cada fila de letra **`<div class="letter">`** aplicando **_display: flex; justify-content: space-between_** para darles un mismo espaciado interno, el mismo contenedor contiene dos **`<h4>`** para los textos de los lados y un **`<progress>`** para la barra.
    Tuve que investigar para estilar las barras y entendi que **_.letter progress::-webkit-progress-bar_** es para estilar la barra de progreso y **_.letter progress::-webkit-progress-value_** es para el valor indicado en **_value=_**.
  13. Aplique sus estilos correspondientes y continue con el ultimo contenedor (**`<div class="see-more">`**) el cual contiene el **`<h4>`** y el **`<button class="btn-more">`**  con el objetivo de aplicar **_flex_** y alinearlos horizontalmente.
  14. Inserte el icono de **"angle-down"** desde "fontawesome" y lo estile con su clase ya definida en el html.
## <span style= "color: orange;"><u>Imagen Proyecto terminado</u></span>
![Preview Proyecto Terminado](/assets/screenshots-readme/proyecto-terminado.png)





