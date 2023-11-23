# Importamos la función input() para capturar la entrada del usuario
from sys import exit

# Funciones para realizar las operaciones matemáticas básicas
def sumar(a, b):
    return a + b

def restar(a, b):
    return a - b

def multiplicar(a, b):
    return a * b

def dividir(a, b):
    if b == 0:
        print("No se puede dividir entre cero")
        exit()
    return a / b

# Bucle principal
while True:
    # Mostramos el menú de opciones
    print("1. Sumar")
    print("2. Restar")
    print("3. Multiplicar")
    print("4. Dividir")
    print("5. Salir")

    # Capturamos la opción del usuario
    opcion = input("Introduce una opción: ")

    # Realizamos la operación matemática seleccionada
    if opcion == "1":
        a = float(input("Introduce el primer número: "))
        b = float(input("Introduce el segundo número: "))
        print("El resultado es: ", sumar(a, b))
    elif opcion == "2":
        a = float(input("Introduce el primer número: "))
        b = float(input("Introduce el segundo número: "))
        print("El resultado es: ", restar(a, b))
    elif opcion == "3":
        a = float(input("Introduce el primer número: "))
        b = float(input("Introduce el segundo número: "))
        print("El resultado es: ", multiplicar(a, b))
    elif opcion == "4":
        a = float(input("Introduce el primer número: "))
        b = float(input("Introduce el segundo número: "))
        print("El resultado es: ", dividir(a, b))
    elif opcion == "5":
        # Salimos del programa
        exit()
    else:
        # Mostramos un mensaje de error
        print("Opción no válida")
