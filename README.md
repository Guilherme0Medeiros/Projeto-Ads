# Projeto-Ads Calculadora 
Projeto Guilherme Medeiros da Silva, de ADS
# Adição
def adicao(x, y):
    return x + y

# Subtração
def subtracao(x, y):
    return x - y

# Multiplicação
def multiplicacao(x, y):
    return x * y

# Divisão
def divisao(x, y):
    if y == 0:
        return "Erro! Não é Possivel Dividir Por Zero."
    else:
        return x / y

print("Escolha a operação:")
print("+. Adição")
print("-. Subtração")
print("*. Multiplicação")
print("/. Divisão")
#Escolher a Operação
escolha = input("Digite o caractere da operação desejada: ")
if escolha in ['+', '-', '*', '/']:
    num1 = float(input("Digite o primeiro número: "))
    num2 = float(input("Digite o segundo número: "))

    if escolha == '+':
        print("Resultado: ", adicao(num1, num2))
    elif escolha == '-':
        print("Resultado: ", subtracao(num1, num2))
    elif escolha == '*':
        print("Resultado: ", multiplicacao(num1, num2))
    elif escolha == '/':
        print("Resultado: ", divisao(num1, num2))
else:
    print("Opção inválida.")
