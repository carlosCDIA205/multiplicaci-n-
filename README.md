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
