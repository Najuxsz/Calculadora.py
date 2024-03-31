#Pedir 2 numeros ao usuario 
#Usuario escolhe a operação
#(1 - soma ; 2 -  subtração ; 3 - multiplicação ; 4 - divisão ; 5 - sair )
# Imprimir a operação que foi feita e o resulado. Por exemplo: "A operação foi soma: 5+7 = 12")

operacao = 0

while operacao != 5:
    operacao = int(input("Qual operação você deseja fazer?\n 1 - Soma\n 2 - Subtração\n 3 - Divisão\n 4 - Multiplicação\n 5 - SAIR\n"))
    if operacao == 5:
        continue
    numero1 = float(input("Digite o primeiro número, por favor: \n"))
    numero2 = float(input("Agora o segundo número: \n"))
    
    if operacao == 1:
        soma = numero1 + numero2
        print(f"A operação exercida foi soma: {numero1} + {numero2} = {soma}")

    elif operacao == 2:
        subtracao = numero1 - numero2
        print(f"A operação exercida foi subtração: {numero1} - {numero2} = {subtracao}")
    
    elif operacao == 3:
        if numero2 == 0:
            print("Não é possível dividir por zero, por gentileza digite outro número.")
        else:
            divisao = numero1 / numero2
            print(f"A operação exercida foi divisão: {numero1} / {numero2} = {divisao}")

    elif operacao == 4:
        multiplicacao = numero1 * numero2
        print(f"A operação exercida foi multiplicação: {numero1} * {numero2} = {multiplicacao}")
        