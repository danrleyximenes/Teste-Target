Dado a sequência de Fibonacci, onde se inicia por 0 e 1 e o próximo valor sempre será a soma dos 2 valores anteriores (exemplo: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34...), escreva um programa na linguagem que desejar onde, informado um número, ele calcule a sequência de Fibonacci e retorne uma mensagem avisando se o número informado pertence ou não a sequência.

def pertence_sequencia_fibonacci(numero):
    a, b = 0, 1

    while a <= numero:
        if a == numero:
            return True
        a, b = b, a + b

    return False

# número informado pelo usuário
numero_informado = int(input("Digite um número para verificar se pertence à sequência de Fibonacci: "))


if pertence_sequencia_fibonacci(numero_informado):
    print(f"{numero_informado} pertence à sequência de Fibonacci.")
else:
    print(f"{numero_informado} não pertence à sequência de Fibonacci.")




    Escreva um programa que inverta os caracteres de um string.


IMPORTANTE:

a) Essa string pode ser informada através de qualquer entrada de sua preferência ou pode ser previamente definida no código;

b) Evite usar funções prontas, como, por exemplo, reverse;


def inverter_string(s):
    # Inicializa uma string vazia para armazenar o resultado
    resultado = ""

    # Itera sobre a string de trás para frente
    for i in range(len(s) - 1, -1, -1):
        # Adiciona cada caractere ao resultado
        resultado += s[i]

    return resultado

string_original = input("Digite uma frase: ")
string_invertida = inverter_string(string_original)

print(f"A string original é: {string_original}")
print(f"A string invertida é: {string_invertida}")

    
