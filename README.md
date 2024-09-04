def pertence_fibonacci(numero):
    # Início da sequência de Fibonacci
    a, b = 0, 1
    
    # Verifica se o número informado é 0 ou 1
    if numero == 0 or numero == 1:
        return True
    
    # Calcula a sequência de Fibonacci
    while b < numero:
        a, b = b, a + b
    
    # Verifica se o número pertence à sequência
    return b == numero

# Número a ser verificado
numero = int(input("Informe um número para verificar se pertence à sequência de Fibonacci: "))

# Verifica e exibe o resultado
if pertence_fibonacci(numero):
    print(f"O número {numero} pertence à sequência de Fibonacci.")
else:
    print(f"O número {numero} NÃO pertence à sequência de Fibonacci.")
