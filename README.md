# calculadores-de-rank
def print_options():
    print("Seja bem vindo herói!\n")
    print("Selecione uma opção:\n")
    print("[1] - Continuar")
    print("[2] - Sair")

def victory_function(name, level, victories, defeats):
    result = victories - defeats
    print(f"O herói {name}, tem saldo de {result} vitórias e está no nível {level}")

def defeat_function(name, level, victories, defeats):
    result = victories - defeats
    print(f"O herói {name}, tem saldo de {result} derrotas e está no nível {level}")

print_options()

while True:
    opcao = int(input("Digite a opção: "))
    if opcao == 1:
        print("Você escolheu continuar!\n")
        name = input("Digite o nome do seu herói: ")
        level = int(input("Digite o nível: "))
        victories = int(input("Digite o número de vitórias do seu herói: "))
        defeats = int(input("Digite o número de derrotas do seu herói: "))
        victory_function(name, level, victories, defeats)

        
        if level < 10:
            print("Ferro")
        if level > 10 and level <=20:
            print("Bronze")
        elif level > 20 and level <=50:
            print("Prata")
        elif level > 50 and level <= 80:
            print("Ouro")
        elif level > 80 and level <= 90:
            print("Diamante")
        elif level > 90 and level <= 100:
            print("Lendário")
        elif level > 100:
            print("Imortal")
            
            
        

    

        print(f"Seu herói está no nível {level}")

    elif opcao == 2:
        print("Até a próxima!")
        break
    else:
        print("Opção inválida, tente novamente.")
