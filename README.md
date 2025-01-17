Lo realice con la siguiente logica, se que no es la manera correcta ya que tiene una demora considerable al ejecutarlo pero funciona (de ser necesario probar con posicion 50). Sé que las herramientas estan ahi (internet) y son muy utiles pero quise realizarlo por mi cuenta:

#Se crean las 3 primeras posiciones
p1 = 0
p2 = 1
p3 = 2

#Se crea una lista con las posiciones iniciales
lista = [2023,2024,2025]

#Se imprime longitud de la lista solo por chequear posiciones
print(len(lista))
contador = 0
posicion = 2023202320232023 - 3
#bucle hasta una posicion determinada
while contador < posicion:
    #se crea una variable la cual suma los 3 primeros elemenos de la lista
    #proxpos = 2023 + 2024 + 2025 = 6072
    proxpos = lista[p1] + lista[p2] + lista [p3]
    #Se agrega este nuevo valor a la lista
    lista.append(proxpos)
    del lista[0]
    #Una vez realizada la suma de esas 3 posiciones continua sumando las ultimas 3 posiciones de la lista
    #para esto debemos indicar que sume un valor mas a cada posicion
    contador = contador + 1

#Por ultimo mostramos el resultado de la posicion deseada
print(proxpos)
#buscamos los ultimos 4 digitos
proxpos = str(proxpos)
print(proxpos[-4:])
