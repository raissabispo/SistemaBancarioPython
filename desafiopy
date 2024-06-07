
menu = print("*==========================*")
print("|        MENU              |")
print("| 1 - Depositar            |")
print("| 2 - Sacar                |")
print("| 3 - Extrato              |")
print("| 4 - Sair                 |")
print("*==========================*")

saldo = 0
limite = 500
extrato = ""
numero_saques = 0
LIMITE_SAQUES = 3

while True:
   
    opcao = int(input("Bem-vindo(a)! Digite umas das opções: "))

    if opcao == 1:
        print("Depósito: ")
        valor_depositado = float(input("Digite o valor do depósito: "))
        if valor_depositado > 0:
            saldo += valor_depositado
            extrato += f'Depósito: R${valor_depositado:.2f}\n'
            
        else:
            print("Erro na operação, tente novamente.")
    elif opcao ==2:
        print("Saque: ")
        valor_saque = float(input("Digite o valor do saque: "))
        if valor_saque > saldo:
            print("Você não tem saldo suficiente. A operação falhou!")
        elif valor_saque > limite:
            print(" O valor do seu saque excede o limite. A operação falhou!")
        elif numero_saques >= LIMITE_SAQUES:
            print("O número máximos de saldos excedidos. A operação falhou!")
        elif valor_saque > 0:
            saldo -= valor_saque 
            extrato += f'Saque: R${valor_depositado:.2f}\n'
            numero_saques += 1
        else:
            print(" A operação falhou! O valor informado é inválido")
            
    elif opcao ==3:
        print("\n=============EXTRATO==============")
        print("Não foram realizadas movimentações." if not extrato else extrato)
        print(f'\n Saldo: R${saldo:.2f}')
        print("\n==================================")
        
    elif opcao ==4:
        break
    
    else:
        print("Operação inválida, por favor digite a operação desejada.")