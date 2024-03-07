# 1) (DESAFIO 1) 

INDICE = 13
SOMA = 0
K = 0

while K < INDICE:
    K = K + 1
    SOMA = SOMA + K

print(SOMA) 
#O resultado ao final do processamento será a soma dos números de 1 a 13, ou seja, 91.

# 2) (DESAFIO 2)

def pertence_sequencia_fibonacci(numero):
    a, b = 0, 1
    while a <= numero:
        if a == numero:
            return True
        a, b = b, a + b
    return False

# Exemplo de uso
numero_informado = 13
if pertence_sequencia_fibonacci(numero_informado):
    print(f"{numero_informado} pertence à sequência de Fibonacci.")
else:
    print(f"{numero_informado} não pertence à sequência de Fibonacci.")

# 3 (DESAFIO 3) ESSE FOI BEM FACIL 

#a) 1, 3, 5, 7, 9 - A lógica aqui é adicionar 2 a cada termo anterior.
#b) 2, 4, 8, 16, 32, 64, 128 - A lógica aqui é multiplicar cada termo por 2.
#c) 0, 1, 4, 9, 16, 25, 36, 49 - 
#Essa sequência representa os quadrados dos números naturais. Portanto, o próximo elemento é 7^2 = 49.
#d) 4, 16, 36, 64, 100 - Essa sequência representa os quadrados perfeitos: 2^2, 4^2, 6^2, 8^2. ou seja 10^2 = 100.
#e) 1, 1, 2, 3, 5, 8, 13 - Essa sequência segue a lógica da série de Fibonacci, onde cada termo é a soma dos dois anteriores. no caso 8 + 5 = 13
#f) 2, 10, 12, 16, 17, 18, 19, 20 -  A lógica aqui é adicionar 8, 2, 4, 1, 1, 1 consecutivamente. o proximo seria 19 + 1 = 20
    
    # 4 (DESAFIO 4) 

# 1 - Ligue um interruptor e espere alguns minutos.
# 2 - Desligue esse interruptor e ligue outro.
# 3 - Entre na sala.
# As lâmpadas correspondentes aos interruptores que foram ligados e desligados estão associadas ao último interruptor ligado e ao interruptor que permaneceu desligado. Assim, você pode determinar qual interruptor controla cada lâmpada.
     
     # 5 (DESAFIO 5) 
    
def inverte_string(s):
    string_invertida = ""
    for char in s:
        string_invertida = char + string_invertida
    return string_invertida

# EXEMPLO PARA USAR
entrada = "Olá, mundo!"
saida = inverte_string(entrada)
print(saida)
