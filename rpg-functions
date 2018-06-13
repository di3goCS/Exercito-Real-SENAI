def racial(race):
    racas = [0, 'Humano', 'Hobbit', 'Dríade', 'Goblin', 'Elfo', 'Gigante', 'Troll', 'Anão', 'Orc']
    race = racas[race]
    return race

def classes(classe):
    classList = [0,'Guerreiro', 'Arqueiro', 'Lanceiro', 'Mago', 'Ladino', 'Paladino', 'Druida', 'Bárbaro']
    guerreiro, arqueiro, lanceiro, mago, ladino, paladino, druida, barbaro = 0, 0, 0, 0, 0, 0, 0, 0
    classe = classList[classe]
    return classe

def questionario():

    pontuacao = 0

    print("Responda as seguintes perguntas pessoais: ")
    print("Escolha 1 para SIM e 2 para NÃO.")

    dentes = int(input("Você tem todos os dentes (e inteiros)?"))
    if dentes == 1:
        pontuacao = pontuacao + 3
        print("Você ganhou 3 pontos!")
    else:
        print("Você não passou nesse teste!")

    guerra = int(input("Já lutou em alguma guerra?"))
    if guerra == 1:
        pontuacao = pontuacao + 1
        print("Você ganhou +1 ponto!")
    else:
        print("Você não passou nesse teste!")

    unigen = int(input("Você é filho único?"))
    if unigen == 1:
        print("Que pena, você não ganha nada...")
    else:
        pontuacao = pontuacao + 2
        print("Parabéns, +2 pontos.")

    armadura = int(input("Você possui armadura própria?"))
    if armadura == 1:
        pontuacao = pontuacao + 1
        print("Uau, +1 ponto!")
    else:
        print("Poxa, não tem nem uma armadura?")

    indicacao = int(input("Você foi indicado por um nobre?"))
    if indicacao == 1:
        pontuacao = pontuacao + 2
        print("Você tem QI, Quem Indique... Parabéns, +2 pontos")
    else:
        print("Bem... vamos prosseguir...")

    return pontuacao


def main():

    aprov = 0
    reserv = 0
    reprov = 0
    inscritos = 0

    aprovados = []
    reprovados = []
    reservas = []

    start = 0  # Variavel de parada
    while start == 0:
        humano, hobbit, driade, goblin, elfo, gigante, troll, anao, orc = 0, 0, 0, 0, 0, 0, 0, 0, 0
        inscritos = 0
        print("\nOh nobres participantes!")
        print("Você está na pré-seleção para o exército do reino de Tão Tão Distante!")
        print("Para saber se você tem aptidão para fazer parte da nossa armada, terá que passar")
        print("por alguns pré-requisitos e uma prova especifica.")
        print("Vamos lá!")
        nome = input("Digite seu nome! ")
        print("Vamos começar com as Raças e Classes")

        race = 0
        stop = False
        while stop == False:
            print("Essas são as raças")
            print("[1]Humano\n[2]Hobbit\n[3]Dríade\n[4]Goblin\n[5]Elfo\n[6]Gigante\n[7]Troll da montanha\n[8]Anão\n[9]Orc")
            race = int(input("Digite o numero da sua raça: "))
            if race < 1 or race > 9:
                stop = False
            else:
                stop = True
            race = racial(race)
        print("Hm... {}, o {}!".format(nome, race))

        classe = 0
        stop = False
        while stop == False:
            print("Essas são as classe")
            print("[1]Guerreiro\n[2]Arqueiro\n[3]Lanceiro\n[4]Mago\n[5]Ladino\n[6]Paladino\n[7]Druida\n[8]Bárbaro")
            classe = int(input("Digite o numero da sua classe: "))
            if classe < 1 or classe > 9:
                stop = False
            else:
                stop = True
            classe = classes(classe)
            print("Hm... um {} {} " .format(race, classe))
        pontuacao = questionario()
        print(pontuacao)

        prova = -1
        while prova < 0 or prova > 20:
            prova = int(input("Qual foi a sua nota na prova específica?"))
            if prova > 20 or prova < 0:
                print("Ladrãozinho!! Digite um valor entre 0 e 20!!")
        pontuacao = pontuacao + prova
        print("Você obteve: {} pontos.".format(pontuacao))

        if pontuacao >= 23:
            candid = []
            aprov = aprov + 1
            candid.append(nome)
            candid.append(race)
            candid.append(classe)
            candid.append(pontuacao)

            aprovados.append(candid)
        else:
            candid = []
            reprov = reprov + 1
            candid.append(nome)
            candid.append(race)
            candid.append(classe)
            candid.append(pontuacao)

            reprovados.append(candid)
            inscritos = inscritos + 1

        op = int(input("Digite 0 para continuar ou -1 para parar."))
        if op == 0:
            start = 0
        elif op == -1:
            start = -1
        else:
            print("Opção Inválida!")

    if len(aprovados) > 0:
        contador = 0
        print("=" * 70)
        print("Lista de Aprovados: \n")
        while contador < len(aprovados):
            print('''Nome: {} | Raça: {} | Classe: {} | Pontuação: {}'''
                   .format(aprovados[contador][0], aprovados[contador][1], aprovados [contador][2], aprovados[contador][3]))
            contador += 1

    if len(reprovados) > 0:
        contador = 0
        print("=" * 70)
        print("Lista de Reprovados: \n")
        while contador < len(reprovados):
            print('''Nome: {} | Raça: {} | Classe: {} | Pontuação: {}'''
                  .format(reprovados[contador][0], reprovados[contador][1], reprovados[contador][2],
                          reprovados[contador][3]))
            contador += 1

main()
