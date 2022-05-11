def esta(cadena,caracter):
    for char in cadena:
        if(char==caracter):
            return True
    return False

def subcadena(cadena,caracter):
    if not(esta(cadena,caracter)):
        return ""
    Encontrado = False
    nuevaCadena  = ""
    for char in cadena.lower():
        if char == caracter:
            nuevaCadena = nuevaCadena + char
            Encontrado = True
        else:
            if Encontrado:
                nuevaCadena = nuevaCadena + char
    return nuevaCadena

# programa ppal

cadena = input("ingrese una frase")
caracter = input ("ingrese un caracter")

print(subcadena(cadena,caracter))
