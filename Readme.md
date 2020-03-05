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
- Carton paja
- Palos de balso (para dar mayor sostenibilidad)
- Laser 
- Papel aluminio
- Tijeras o Bisturí
- Lupa (Para mejores cortes)

# Simulación
![](ImagenSimulación.png/ImagenSimulación.png)

# Simulación con codigo Python
def Cambio(m,x,NumRend,cont):
    n = m
    DobleRendija(m, x, NumRend, cont, n)

def DobleRendija(m, x, NumRend, cont, n):
    matriz = []
    if NumRend == 1:
        com = []
        for i in range(len(m)):
            Sum = 0
            for j in range(len(m)):
                mult = x[j] * m[i][j]
                Sum = Sum + mult
            com.append(Sum)
        return print(com)
    else:
        if NumRend == cont:
            mat = []
            for i in range(len(m)):
                Sum = 0
                for j in range(len(m)):
                    mult = x[j] * m[i][j]
                    Sum = Sum + mult
                mat.append(Sum)

            return print(mat)
        else:
            cont += 1
            for h in range(len(m)):
                matriz.append([0] * len(m))
            for i in range(len(m)):
                for j in range(len(m[0])):
                    for k in range(len(m)):
                        matriz[i][j] += m[i][k] * n[k][j]
            m = matriz
            DobleRendija(m, x, NumRend, cont, n)

def main():
    m = [[0, 0, 0, 0, 0, 0, 0, 0],
         [1/2, 0, 0, 0, 0, 0, 0, 0],
         [1/2, 0, 0, 0, 0, 0, 0, 0],
         [0, 1/3, 0, 1, 0, 0, 0, 0],
         [0, 1/3, 0, 0, 1, 0, 0, 0],
         [0, 1/3, 1/3, 0, 0, 1, 0, 0],
         [0, 0, 0, 1/3, 0, 0, 1, 0],
         [0, 0, 0, 1/3, 0, 0, 0, 1]]

    x = [1, 0, 0, 0, 0, 0, 0, 0]

    NumRend = 1
    cont = 1
    Cambio(m, x, NumRend, cont)


main()

Resultado de simulación : [0, 0.5, 0.5, 0.0, 0.0, 0.0, 0.0, 0.0]





