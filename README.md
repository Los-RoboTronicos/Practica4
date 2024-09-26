# Practica4

## Integrantes
- Uriel Vladimir Alvarez Tapia 20121191
- Miguel Angel Castañeda Garcia 20120015
- Diana Alejandra Mendoza Mendoza 20121226

## Introducción 
Es bien sabido que la robotica industrial esta enfocada hacia la repetición de ciclos durante largos periodos de tiempo, sin embargo, en ocasiones estos ciclos requieren cambios entre ellos antes de reiniciar el ciclo general. En este sentido, los ciclos *for* permiten realizar un número específico de actualizaciones constantes al programa realizado, permitiendo asi una rutina de mayor versatilidad y aplicaciones en la industria.

## Objetivos
Apilar 4 fusibles en la caja que se encuentra al frente del robot.
## Desarrollo
Como primer paso, se deben "enseñar" los puntos al robot, es decir, la posicion de recogida del fusible, la posicion de la base de la caja y puntos de apoyo para evitar movimientos curvos que propicien las colisiones (figura 1).

![Puntos](https://github.com/user-attachments/assets/a0a70777-af40-46e4-805c-3f8faa3e21a7)

Una vez enseñados los puntos, se procede a medir un fusible con el apoyo de un vernier para asi determinar el aumento en el eje Z.

Tras determinar la altura de un fusible en 1.5cm, se procede a agregar ese aumento en el ciclo for; sin embargo, es necesario dar la instrucción en mm de acuerdo con la sintaxis del robot (Figura 2).
![Codigo 1](https://github.com/user-attachments/assets/6ca9a298-a997-47a4-84bd-a7d49fabc4ad)

## Resultados
Tras la simulacion del codigo se procedio a su implementacion fisica (Figura 3). 
![image](https://github.com/user-attachments/assets/a4a4a08c-d396-4dbb-a7b5-e2db5690f901)

En la figura 4, se puede observar como se apilaron 3 fusibles mas sobre el fusible incial gracias a ese aumento sobre el eje Z de ciclo for. 
![image](https://github.com/user-attachments/assets/9fa6588a-f3a3-4feb-b797-dd7f0561afb3)

Cabe resaltar, que debido a una mala lectura de la medida del vernier, el robot soltaba el fusible desde una posicion ligeramente superior a la esperada.

## Conclusiones
- **Uriel Vladimir Alvarez Tapia:** La herramienta de ciclos *for* en el robot permite la implementacion de codigos repetitivos mas complejos, permitiendo aumentar el alcance de las soluciones a las que este robot se puede aplicar. Sin embargo, esta practica sirvio para ejemplificar que las herraminetas de codigo y los codigos en si mismos son poco utiles si el entorno fisico no esta bien caracterisado y por lo tanto trasladado al mundo virtual, desembocando en problemas como los vistos en los resultados de este documento. Estas discrepancias entre la programacion y la realidad pueden poner en peligro tando al equipo en si mismo, como a los operadores que se encuentren en zonas aledañas.
- **Miguel Angel Castañeda Garcia:** Durante la práctica, fue necesario repetir varias veces las acciones programadas para verificar que el robot realizara correctamente los movimientos deseados. Esta repetición ayudó a detectar y corregir posibles errores en la secuencia, asegurando que el robot operara de manera consistente. Esto nos muestra la importancia de probar continuamente la programación para lograr un rendimiento óptimo en tareas automatizadas, y tras las dificultades se obtuvo una mayor práctica con la manipulación del robot, permitiendo sustentar la teoría vista en clase.
- **Diana Alejandra Mendoza Mendoza:** En esta práctica, se utilizó un ciclo for para apilar fusibles ajustando el eje Z según la medida de cada uno. A pesar de un pequeño error de medición que afectó la posición de liberación del fusible, el proceso fue exitoso y se logró observar cómo los ciclos for permiten realizar tareas repetitivas con modificaciones precisas en cada iteración. Esto demostró la importancia de los ciclos en la programación de robots industriales, brindando eficiencia en tareas automatizadas.
