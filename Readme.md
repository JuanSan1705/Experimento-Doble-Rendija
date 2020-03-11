# Experimento de la doble rendija 
# Escuela Colombiana de Ingenieria Julio Garavito
## Juan Pablo Sánchez Suárez
****************************************************

# Descripción
En este repositorio se habla sobre el experimento de la doble redija o tambien llamado el experimento de Young. 
Se muestra los materiales basicos para la construcción de este y el objetivo por el cual se hace el experimento para así
hacer una introducción hacia este comportamiento de esto en el mundo cuántico. Posteriormente se muestra una determinada simulación sobre
este experiemento.

# Información de Experimento e historia
Este experimento de Young (o mas conocida como experimento de la doble rendija) realizado en 1801 por Thomas Young en un intento de 
discernir sobre la naturaleza corpuscular u ondulatoria de la luz. Se tiene en cuenta que este experimento no fue presentado formalmente hasta 
1961 con electrones y así mostrando la dualidad. Lo importante de este experimento y lo que podemos observar es que la materia es indeterminista 
y es afectada por nuestra observación. Este experimento no se hizo principalmente bajo el contexto de la mecanica cuantica debido a que en aquel 
tiempo no existia aún la teoria de esta para responder a la pregunta si la luz tenia una naturaleza corpuscular o si mas bien consistia en
ondas viajando por el éter. 

# Materiales
- Carton paja y/o Carton piedra
- Palos de balso (para dar mayor sostenibilidad)
- Laser 
- Papel aluminio
- Tijeras o Bisturí
- Lupa (Para mejores cortes)

# Explicación paso por paso
1. Para el primero procedimiento se procede a hacer la base donde se quiere proyectar el laser y conseguir la figura esperada , para este procedimiento se hace dos bases en forma de triangulo con carton paja o carton piedra para mejor sostenibilidad. A continuacion se muestra el claro ejemplo. 
![](/Imagenes/Pared.png)

2. En siguiendo esto se procede a hacer lo mas importante del experimento, la pared de la doble rendija, o más rendijas. Para este experimento se tomaron como material de trabajo el papel aluminio, prodece a hacer dos lineas en el papel de manera muy delicada, asi no romper el papel, y se pega en la parte de atras del carton base con cinta. Estas lineas tienen que ser lo mas junto posible sin dañar el espacio de aluminio que esta entre las dos lineas, así mismo se procede a hacer lo mismo con las demas rendijas si se desea experimentar con mas de una rendija. A continuacion, se muestra una imagen sobre este procedimiento.
![](/Imagenes/aluminio.png)

3. Por ultimo procedimiento respecto a la construcción del experimento se procede a hacer una base para el laser, debido a que es una parte muy importante para que este experimento salga como se desea. Este tiene que tener un diseño tal que cuando sea disparado el laser pueda ir directo a las rendijas, asi poder reflectar lo mejor posible. 

A continuación se muestra el experimento completado y su resultado.
![](/Imagenes/Completo.png)

# Conclusiones del experimento
Mediante este pequeño pero muy significativo experimento se logra observar un comportamiento curioso en los fotones del laser, y al final se logra concluir que depende de sus probabilidades y en que pasa por cada rendija los electrones debido a que existe una probabilidad de que pase por alguna de las dos rendijas es del 50%, nunca pasa el rayo del laser al mismo tiempo por las dos, solo puede pasar por alguna de las dos, debido a que este procedimiento se repite tantas veces como para no notarlo a la vista del ojo, pero se puede entender mediante esta simulación que es un comportamiento muy parecido al del experimento.
![](/Imagenes/ImagenSimulación.png)
Existen dos formas de representar la probabilidad y comportamiento despues de cada click, mediante numeros reales como se muestra en la simulación anterior que es una forma de verlo de manera muy simple, se suele usar los numeros reales entre 0 y 1 para calcular la probabilidad clasica de llegada de los electrones en un punto determinado. Tambien hay otra forma mas completa la cual es de la forma cuantica (con numeros complejos), la cual se mostrara a continuacion. Simulacion Cuántica. 
![](/Imagenes/SImulacionCuantica.png)
En esta simulación cuantica no se toma como probabilidades clasicas como con los numeros reales, debido a que ahora lo analizaremos con numeros complejos, como el complejo c, para lo cual se tiene en cuenta que |c| es un real entre 0 a 1. Pero la verdadera pregunta es: ¿Que diferencia tiene calcular la probabilidad con numeros complejos o numeros reales?. La principal diferencia es que los numeros reales nos sirven solo para encontrar la probabilidad de cuerpos muy grandes, como las balas, en cambio, con la mecanica cuantica se logra encontrar probabilidades como por ejemplo la de los fotones o electrones. Una diferencia tambien es que cuando se suman las probabilidades se aumenta la probabilidad en los numeros reales en cambio con numeros complejos se logra cancelar entre si y reducir su probabilidad. 
Debido a que dichos complejos se puedan cancelar, lo cual es muy importante en la mecanica cuantica, llamado este interferencia. Para la explicación anterior se toma en cuenta que para la conseguir la probabilidad de encontrar la cantidad de electrones llega a un punto en especifico, se toma como relacion entre "Vectores", una matriz y un estado base (presentado en vector), donde en el caso de la matriz se tiene que cumplir que la suma de sus columnas dan como resultado 1 al igual que sus filas, y en el caso del vector la suma de cada uno de sus componentes debe dar como resultado 1. La multiplicación de la matriz que llamaremos M con el vector llamado X debe dar como resultado la probabilidad de cada punto especifico. 
Para el caso de los numeros complejos, se debe hacer el mismo procedimiento pero la suma de cada componente de X no se pide que sea estocastica, sino, la suma de sus modulos al cuadrado deben dar como resultado 1. Pero, ¿Qué se puede decir de la matriz M?, para esta matriz se pide que sea unitaria. 
Para concluir con la explicacion y objetivo de este experimento se lo concluye que no hay una sola posicion donde se encuentre los fotones, si no que debido a que no se puede hacer este experiemento con un solo foton, se asegura que los fotones estan en muchas posiciones, anulandocen y sumandocen entre si, estas posiciones pueden ser llamadas "Superposiciones". ¿Por qué pasa esto?, debido a que los fotones estan pasando simultaneamente por ambas rendijas. Este comportamiento es imposible investigarlo por la fisica clasica, es estrictamente analizado desde el mundo cuantico, debido a que no se puede pensar en este caso del experimento de la doble rendija sobre la probabilidad de encontrarlo con certeza, solamente que despues de medir el estado X (vector anteriormente mencionado)se encontrar en la posicion i con la probabilidad |Ci|^2.  


# Simulación con codigo Python
Teniendo en cuenta los objetivos concluidos anteriormente se procede a mostrar imagenes sobre las simulaciones con Python. Teniendo matriz M y vector base X. Se hara simulacion clasica y simulación cuantica.
![](/Imagenes/Imagencodigo.png)
![](/Imagenes/Imagen3.png)


Resultado de simulación : [0, 0.5, 0.5, 0.0, 0.0, 0.0, 0.0, 0.0]
Resultado de simulación cuantica: [0, 0.5, 0.5, 0.0, 0.0, 0.0, 0.0, 0.0]

# Bibliografía 
https://www.ecured.cu/Experimento_de_Young
QUANTUM COMPUTING FOR COMPUTER SCIENTISTS




