# proyecto-junior
Repositorio para mostrar en una entrevista de trabajo para una posición de programador junior.
def suma(num1, num2):
    return num1 + num2

def resta(num1, num2):
    return num1 - num2

def multiplicacion(num1, num2):
    return num1 * num2

def division(num1, num2):
    if num2 == 0:
        return "No se puede dividir por cero"
    else:
        return num1 / num2

print("Calculadora básica")
print("Operaciones disponibles: + - * /")

while True:
    operacion = input("Ingrese la operación que desea realizar (+,-,*,/): ")
    if operacion in ['+', '-', '*', '/']:
        num1 = float(input("Ingrese el primer número: "))
        num2 = float(input("Ingrese el segundo número: "))

        if operacion == '+':
            print(num1, "+", num2, "=", suma(num1, num2))

        elif operacion == '-':
            print(num1, "-", num2, "=", resta(num1, num2))

        elif operacion == '*':
            print(num1, "*", num2, "=", multiplicacion(num1, num2))

        elif operacion == '/':
            print(num1, "/", num2, "=", division(num1, num2))

        break

    else:
        print("Operación inválida. Inténtelo de nuevo.")
