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

Aplicar conceptos y ejemplo de box model

Que es box mode, el uso particulara de selector universal, explicar las capas del box model tanto internas como externas com ejemplos. .

Explicar el shorthand padding , y margin.

En margin explicar que es margin negativo, colapsadao de margenes verticales y el centrado perfecto horizontal.

## BOX MODEL

1. Box-model -> En español es modelo de caja se dice asi porque en los navegadores todo se construye a partir de cajas

2. Selector Universal -> Es un selector que se le aplica a todo el documento , y tiene una propiedad con valor que hace que respete los anchos y altos que le pones a las cajas

\*{
box-sizing: border-box;
}

## CAPAS DE BOX MODEL

1. Box content -> Es el contenido de la caja , es la primera capa interna
2. Padding -> Es el relleno interno que se le da a la caja
3. Border -> El borde es el contorno que se le ve en la caja
4. Margen -> Es la parte externa de la caja , osea cada valor que le des a un margin se dara por lo externo

## SHORTHAND

1. Padding -> Tiene tres , la primera es que si pones un valor que se le da a toda la caja

   - La segunda es como las agujas del reloj -> 1rem(top) 2rem(right) 3rem(bottom) 4rem(left)
   - La tercera es con dos valores -> 2rem(top y bottom) 3rem(right y left)

2. Margin -> Funciona igual que el padding pero ahora con margin que es como una separacion externa

## MARGIN NEGATIVO

- El negativo solo existe en el margin , en el padding no existe , y lo que hace el negativo es que va al lado contrario del que le pongas , si pones

h2{
margin-bottom: -2rem ;
}

- Esto en vez de que se de margin abajo , la caja se dara margen para arriba

## COLAPSADO DE MARGEN VERTICALES

- Solo existe colapso de marge vertical , no horizontal
- Funciona asi, que si tu tienes una caja1 con un margin-bottom con 3rem y una caja2 con margin-top con 3rem . Solo se aplicara un solo 3rem , no se suma , no sera 6 rem ni nada de eso , solo uno
- Ahora si esque ahora se tiene margin-bottom 3rem y margin-top 5rem , pues se aplicara el mayor , que sera 5 rem , no se suma ni nada de eso

## CENTRADO DE CAJA

- El codigo para centrar es

div{
margin: 0 auto
}

- Quiere decir 0 arriba y abajo y auto a los lados y asi es una manera de centrar una caja
