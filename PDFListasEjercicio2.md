#Ejercicio 2

def posMayor(numero):
  posMax = 0
  maxElem = int(numero[0])

  for i in range(len(numero)):
    if ( int(numero[i]) > maxElem ):
      maxElem =  int(numero[i])
      posMax = i
  return posMax


numero = int(input("ingrese un numero"))
num = str(numero)

if(len(num)==7):
  print( posMayor(num))
else: 
  print("el numero debe tener 7 cifras")
