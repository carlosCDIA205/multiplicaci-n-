# multiplicaci-n-
programa de carlos leonel 
def multiplicar(a, b):
    """
    Multiplica dos números y retorna el resultado.
    """
    return a * b

def dividir(a, b):
    """
    Divide el primer número entre el segundo y retorna el resultado.
    Si el divisor es 0, retorna un mensaje de error.
    """
    if b == 0:
        return "Error: División por cero"
    return a / b

if __name__ == "__main__":
    print("Calculadora de multiplicación y división")
    num1 = float(input("Ingresa el primer número: "))
    num2 = float(input("Ingresa el segundo número: "))

    print(f"{num1} x {num2} = {multiplicar(num1, num2)}")
    division = dividir(num1, num2)
    print(f"{num1} / {num2} = {division}")
def sumar(a, b):
    return a + b

def restar(a, b):
    return a - b

def main():
    print("Calculadora simple: suma y resta")
    while True:
        print("\nOpciones:")
        print("1. Sumar")
        print("2. Restar")
        print("3. Salir")
        opcion = input("Elige una opción (1/2/3): ")
        
        if opcion == "3":
            print("¡Hasta luego!")
            break

        if opcion in ["1", "2"]:
            try:
                num1 = float(input("Ingresa el primer número: "))
                num2 = float(input("Ingresa el segundo número: "))
            except ValueError:
                print("Por favor, ingresa números válidos.")
                continue

            if opcion == "1":
                resultado = sumar(num1, num2)
                print(f"Resultado: {num1} + {num2} = {resultado}")
            else:
                resultado = restar(num1, num2)
                print(f"Resultado: {num1} - {num2} = {resultado}")
        else:
            print("Opción no válida. Intenta de nuevo.")

if __name__ == "__main__":
    main()
