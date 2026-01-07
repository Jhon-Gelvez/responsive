1 use @media screen and (max-width: x) para detectar el ancho y asi cambiar el background-color

2 con @media screen and (max-width: x) para detectar el ancho y variar el justify-content: x; 

3 para el diseño del dispositivo movil la lista esta a la izq y los demas elementos estan centrados, para una vista desde pc la lista se centra para mayor comodidad al leer en una pantalla grande

4 para el diseño en el computador estan todos los elemetos centrados y el tamaño del texto un mas grande para mejor legibilidad, al verlo desde movil muevo la lista y el titulo a la izq ya que no afecta negativamente la experiencia al leer y reduzco el tamaño de la letra 

5 el menu por defecto es vertical y para pantallas grandes (>900px) es hoorizontal y la letra es mas grande

6 en los puntos de queibre 768, 992 y 1200 px cambio el tamaño de la letra a 1.2, 1.5 y 1.7 rem respectivamente

7 si la pantalla es mayor a 900px uso el display grid y grid-template-columns: 1fr 1fr 1fr; para crear tres columnas del mismo ancho, si es menor por defecto solo hay una columna

8 las tarjetas por defecto estan apiladas y la ser la pantalla mayor a 768px tiene display flex con flex direction row que las ubica en horizontal

9 en los diseños para impresion usamos la regla @media print {...} para especificar los estilos como fondo blaco y letra en negro, tipografia Times New Roman y tamaño de 11px, etc.

10 para pantallas menores a 720px la direccion del display flex es column para asegurarnos que todos los elementos quepan en la pantalla y no se desborden 

11  La unidad rem toma como referencia el tamaño de fuente del elemento raíz del documento (html) 
La unidad em toma como referencia el tamaño de fuente de su elemento padre directo.
Esto hace que todas las fuentes dependan de esta medida (em/rem) y si se llega a cambiar hara que todas las demas cambien automaticamente

el elemeto padre es .container_rem_em y su font-size: 51px hace que el 
.container_rem_em h2{
        font-size: 1.7em;
    }
tenga un tamaño de 86.7px

12 para cambiar imagenes segun el tamaño de la pantalla se cambia el background-image: url("x"); segun la imagen que se desee mostrar en la @media screen and (x: z)