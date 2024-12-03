```
print("======================================")
print(" Calculadora Básica - Versión 1.0 ")
print("======================================")

def saludar():
    print("Hola, ¿cómo estás?")

def calcular():
    print("¿Qué operación deseas realizar?")
    print("1. Suma")
    print("2. Resta")
    print("3. Multiplicación")
    print("4. División")

    opcion = input("Ingresa el número de la operación: ")

    if opcion == "1":
        num1 = float(input("Ingresa el primer número: "))
        num2 = float(input("Ingresa el segundo número: "))
        resultado = num1 + num2
        print(f"El resultado de la suma es: {resultado}")
    elif opcion == "2":
        num1 = float(input("Ingresa el primer número: "))
        num2 = float(input("Ingresa el segundo número: "))
        resultado = num1 - num2
        print(f"El resultado de la resta es: {resultado}")
    elif opcion == "3":
        num1 = float(input("Ingresa el primer número: "))
        num2 = float(input("Ingresa el segundo número: "))
        resultado = num1 * num2
        print(f"El resultado de la multiplicación es: {resultado}")
    elif opcion == "4":
        num1 = float(input("Ingresa el primer número: "))
        num2 = float(input("Ingresa el segundo número: "))
        if num2 != 0:
            resultado = num1 / num2
            print(f"El resultado de la división es: {resultado}")
        else:
            print("Error: No se puede dividir por cero")
    else:
        print("Opción inválida")

saludar()
while True:
    calcular()
    respuesta = input("¿Deseas realizar otra operación? (s/n): ")
    if respuesta.lower() != "s":
        break
```
