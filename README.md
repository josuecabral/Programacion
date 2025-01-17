Lo realice con la siguiente logica, se que no es la manera correcta ya que tiene una demora considerable al ejecutarlo pero funciona (de ser necesario probar con posicion 50). Sé que las herramientas estan ahi (internet) y son muy utiles pero quise realizarlo por mi cuenta:

#Se crean las 3 primeras posiciones

p1 = 0

p2 = 1

p3 = 2

#Se crea una lista con las posiciones iniciales

lista = [2023,2024,2025]

contador = 0

posicion = 2023202320232023 - 3

#Se crea un bucle con un contador hasta una posicion determinada (menos 3 ya que la lista contiene 3 posiciones iniciales)

while contador < posicion:

    #se crea una variable la cual suma los 3 primeros elemenos de la lista
    
    #proxpos = 2023 + 2024 + 2025 = 6072
    
    proxpos = lista[p1] + lista[p2] + lista [p3]
    
    #Se agrega este nuevo valor a la lista
    
    lista.append(proxpos)

    #Se elimina el primer valor de la lista
    
    del lista[0]
    
    contador = contador + 1
    

#Por ultimo mostramos el resultado de la posicion deseada

print(proxpos)

#buscamos los ultimos 4 digitos

proxpos = str(proxpos)

print(proxpos[-4:])
