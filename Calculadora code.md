def suma(num1, num2):
    return num1 + num2

def resta(num1, num2):
    return num1 - num2

def multiplicacion(num1, num2):
    return num1 * num2

def division(num1, num2):
    if num2 != 0:
        return num1 / num2
    else:
        return "Error: división por cero"

def menu():
    print("Selecciona la operación que deseas realizar:")
    print("1. Suma")
    print("2. Resta")
    print("3. Multiplicación")
    print("4. División")
    print("5. Salir")

while True:
    menu()
    opcion = input("Ingresa el número de la operación que deseas realizar (o '5' para salir): ")

    if opcion == '5':
        print("¡Hasta luego!")
        break

    num1 = float(input("Ingresa el primer número: "))
    num2 = float(input("Ingresa el segundo número: "))

    if opcion == '1':
        print("El resultado de la suma es:", suma(num1, num2))
    elif opcion == '2':
        print("El resultado de la resta es:", resta(num1, num2))
    elif opcion == '3':
        print("El resultado de la multiplicación es:", multiplicacion(num1, num2))
    elif opcion == '4':
        print("El resultado de la división es:", division(num1, num2))
    else:
        print("Opción no válida. Por favor, selecciona una opción válida.")
