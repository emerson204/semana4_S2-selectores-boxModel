## SELECTORES SIMPLES

1. Selector de etiqueta -> El selector de etiqueta es el de menor especificidad , sirve para dar estilos generales como al inicio del proyecto

h2{
color:red;
}

2. Selector de clase -> El selector de clase es el que mas utilizaremos en dar estilos a las etiquetas , es como un identificador a la etiqueta que se le va a dar estilo , se llama con un .nombreClase

.heading{
colore:blue;
}

3. Selector id -> El selector Id es un identificador unico en las etiquetas osea si tu le pones un nombre de id a un etiqueta , ese nombre no debe de ser llamado en otra etiqueta , se llama con #nombreId
   #texto{
   color:red;
   }

## SELECTORES COMPUESTOS

1. Elemento descendiente -> Este sirve para dar estilos a todos los que estan dentro de algun padre

.padre h2 {
color:red;
}

2. Elemento hijo directo -> Solo se le aplica al hijos que le siguen , se representa (>) y esos hijos deben de estar en el mismo nivel

.padre > h3{
color:red;
}

3. Hermano siguiente o adyacente -> Es el hermano siguiente en singular , solo el primero hermano siguiente , no importan los demas , solo el primero y se representa mediante el +

h2 + p {
color:red;
}

4. Hermanos siguientes -> Este es en plural , osea toma todos los hermanos siguientes que esten en el mismo nivel y se representa con la cola de caballo ~

h3 ~ p{
color:red;
}

## OTRO TIPO

Esto es para darle estilos a dos elementos juntos

1. h2 , a{
   color: red;
   }
