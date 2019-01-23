# PROYECTO-IST
# Integrante del grupo: Rubén Diab Martínez

# 1.	Descripción del proyecto

Se ha realizado una ampliación del juego del Solitario implementado en las prácticas correspondientes a la asignatura de IST.

Las ampliaciones o mejoras añadidas son:

•	Estética mejorada: 

o	Cabecera y tapete visualmente más estéticos.
o	Nueva fuente añadida de Google Fonts denominada Syncopate.
o	Se han cambiado las posiciones de los tapetes inicial, receptores y sobrantes.
o	Se han añadido tres botones visualmente estéticos, cuyas funcionalidades se explican en el siguiente apartado. Estos botones son: Reiniciar, Barajar y Auto. 

•	Funcionalidades implementadas:

o	El botón de Reiniciar reinicia la partida, poniendo a cero el tiempo y todos los contadores, además de barajar todas las cartas.

o	El de Barajar baraja el mazo inicial teniendo en cuenta el mazo de sobrantes y sin modificar ni el tiempo ni los contadores. De esta manera, es posible barajar las cartas en cualquier momento sin necesidad de vaciar todo el mazo inicial en el mazo de sobrantes.

o	El de Auto tiene la funcionalidad de jugar de manera automática. Más detalladamente explicado, esta función lo que realiza es, dado un mazo inicial barajado aleatoriamente generado, todos los pasos para ganar de manera perfecta haciendo el mínimo número de movimientos posibles para el caso dado. 

o	Se muestra en consola mensajes que informan del transcurso del juego o de acciones que no están disponibles.

o	A parte de la funcionalidad de Arrastrar y soltar ya realizada en las prácticas, se ha añadido una función que al hacer click en las cartas, esto funciona únicamente para las cartas que se hallen en el tapete inicial, las cartas se colocan de manera automática donde deberían situarse.







# 2.	¿Cómo se ha realizado?

Para la parte estética se han utilizado unas imágenes de Google para el diseño de la cabecera y del tapete. 

Para la parte funcional, la implementación de la funcionalidad del click se consigue con la propiedad de JavaScript “onclick” utilizada adecuadamente.

La que corresponde al botón Auto se ha conseguido mediante un condicionante que consiste en que, si el número de cartas en el tapete inicial o sobrante es diferente de cero, se aplica un bucle for que hace click de manera automática a las cartas del tapete inicial, y estas se van situando donde les corresponde. En el caso de que el número de cartas del tapete inicial sea igual a cero y el del tapete de sobrantes desigual a cero, entonces se barajan las cartas del mazo sobrantes. Se repite este proceso hasta que el número de cartas tanto en el tapete inicial como en el de sobrantes sea igual a cero, y llegados a este punto, finaliza el juego con el mínimo número de movimientos posibles realizables para ganar.

Los mensajes en consola se muestran mediante el comando console.log(), utilizando condiciones para mostrar el mensaje correspondiente a la acción o problema que se está produciendo en ese momento.
