# Listas que irão gravar o nome, pontuação, raças e classe dos aprovados.
listNomesAprov = []
listPtsAprov = []
listRacesAprov = []
listClassAprov = []
listCharAprov = []

# Listas que irão gravar o nome, pontuação, raças e classe dos reprovados.
listNomesReprov = []
listPtsReprov = []
listRacesReprov = []
listClassReprov = []
listCharReprov = []

# Listas que irão gravar o nome, pontuação, raças e classe dos reservas.
listNomesReserv = []
listPtsReserv = []
listRacesReserv = []
listClassReserv = []
listCharReserv = []

# Variaveis de aprovação por raça, inicializadas.
humano, hobbit, driade, goblin, elfo, gigante, troll, anao, orc = 0, 0, 0, 0, 0, 0, 0, 0, 0

# Lista de variáveis de classe, inicializados com valor 0.
guerreiro, arqueiro, lanceiro, mago, ladino, paladino, druida, barbaro = 0, 0, 0, 0, 0, 0, 0, 0
inscritos = 0
aprov = 0  # Quantidade de aprovados
reserva = 0  # Quantidade de reservas
start = 0  # Variavel de parada

while start == 0:
    print("\nOh nobres participantes!")
    print("Você está na pré-seleção para o exército do reino de Tão Tão Distante!")
    print("Para saber se você tem aptidão para fazer parte da nossa armada, terá que passar")
    print("por alguns pré-requisitos e uma prova especifica.")

    print("Vamos lá!")
    nome = input("Digite seu nome! ")
    valid = 0  # Essa variável vai servir para atender a condição do laço while.
    while valid < 1 or valid > 9:
        print("Essas são as raças:\n")
        print(" 1) Humano \n 2) Hobbit \n 3) Dríade \n 4) Goblin \n 5) Elfo \n 6) Gigante \n 7) Troll da Montanha ")
        print(" 8) Anão \n 9) Orc")
        race = int(input("Escolha o número correspondente a sua: \n"))

        # Esses contadores servem para contabilizar os aprovados/inscritos por raça.
        if race == 1:
            valid = race
            humano = humano + 1
            race = 'Humano'
        elif race == 2:
            valid = race
            hobbit = hobbit + 1
            race = 'Hobbit'
        elif race == 3:
            valid = race
            driade = driade + 1
            race = 'Dríade'
        elif race == 4:
            valid = race
            goblin = goblin + 1
            race = 'Goblin'
        elif race == 5:
            valid = race
            elfo = elfo + 1
            race = 'Elfo'
        elif race == 6:
            valid = race
            gigante = gigante + 1
            race = 'Gigante'
        elif race == 7:
            valid = race
            troll = troll + 1
            race = 'Troll da Montanha'
        elif race == 8:
            valid = race
            anao = anao + 1
            race = 'Anão'
        elif race == 9:
            valid = race
            orc = orc + 1
            race = 'Orc'
        else:
            valid = 0
            print("Opção Inválida!")
    title = nome + race
    print("Hm... {}, o {}!" .format(nome, race))

    print("Responda as seguintes perguntas pessoais: ")
    print("Escolha 1 para SIM e 2 para NÃO.")
    pontuacao = 0

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
        print("Parabéns, +2 pontos.")
        pontuacao = pontuacao + 2

    armadura = int(input("Você possui armadura própria?"))
    if armadura == 1:
        print("Uau, +1 ponto!")
        pontuacao = pontuacao + 1
    else:
        print("Poxa, não tem nem uma armadura?")

    indicacao = int(input("Você foi indicado por um nobre?"))
    if indicacao == 1:
        print("Você tem QI, Quem Indique... Parabéns, +2 pontos")
        pontuacao = pontuacao + 2
    else:
        print("Bem... vamos prosseguir...")

    validClass = 0
    while validClass != 1:
        print("Muito bem, vamos para o próximo teste...")
        print("As provas específicas contam a quantidade de acertos de golpes específicos para cada classe.")
        print("Essas são as classes")
        print("1)Arqueiro \n2)Guerreiro \n3)Lanceiro \n4)Mago \n5)Ladino \n6)Paladino \n7)Druida \n8)Bárbaro")
        classe = int(input("Escolha o número referente a sua Classe\n"))

        if classe == 1:
            validClass = 1
            guerreiro = guerreiro + 1
            classe = "Guerreiro"
        elif classe == 2:
            validClass = 1
            arqueiro = arqueiro + 1
            classe = "Arqueiro"
        elif classe == 3:
            validClass = 1
            lanceiro = lanceiro + 1
            classe = "Lanceiro"
        elif classe == 4:
            validClass = 1
            mago = mago + 1
            classe = "Mago"
        elif classe == 5:
            validClass = 1
            ladino = ladino + 1
            classe = "Ladino"
        elif classe == 6:
            validClass = 1
            paladino = paladino + 1
            classe = "Paladino"
        elif classe == 7:
            validClass = 1
            druida = druida + 1
            classe = "Druida"
        elif classe == 8:
            validClass = 1
            barbaro = barbaro + 1
            classe = "Bárbaro"
        else:
            validClass = 0
            print("Opção Inválida!")
    print(classe)

    prova = -1
    while prova < 0 or prova > 20:
        prova = int(input("Qual foi a sua nota na prova específica?"))
        if prova > 20:
            print("Ladrãozinho!! Digite um valor entre 0 e 20!!")
    pontuacao = pontuacao + prova
    print("Você obteve: {} pontos." .format(pontuacao))

    if pontuacao >= 23:
        if aprov < 21:
            aprov = aprov + 1
            listNomesAprov.append(nome)
            pontuacao = str(pontuacao)
            char = nome+", o(a) "+race+" " + classe + " fez " + pontuacao + " pontos"
            listPtsAprov.append(pontuacao)
            listRacesAprov.append(race)
            listCharAprov.append(char)
            listClassAprov.append(classe)
        if aprov > 20:
            reserva = reserva + 1
            listNomesReserv.append(nome)
            pontuacao = str(pontuacao)
            char = nome+", o(a) "+race+" " + classe + " fez " + pontuacao + " pontos"
            listPtsReserv.append(pontuacao)
            listRacesReserv.append(race)
            listCharReserv.append(char)
            listClassReserv.append(classe)
        pontuacao = int(pontuacao)
        inscritos = inscritos + 1
    else:
        listNomesReprov.append(nome)
        pontuacao = str(pontuacao)
        char = nome + ", o(a) " + race+" " + classe + " fez " + pontuacao + " pontos"
        listPtsReprov.append(pontuacao)
        listRacesReprov.append(race)
        listCharReprov.append(char)
        listClassReprov.append(classe)
        pontuacao = int(pontuacao)
        inscritos = inscritos + 1

# Decisão de parada.
    op = int(input("Digite 0 para continuar ou -1 para parar."))
    if op == 0:
        start = 0
    elif op == -1:
        start = -1
    else:
        print("Opção Inválida!")


print("Nesse processo seletivo, se inscreveram {} candidatos!" .format(inscritos))

print("\n Numero de Inscritos por raça:")
if hobbit == 1:
    print("Foi inscrito 1 hobbit!")
if hobbit > 1:
    print("Foram inscritos {} hobbits" .format(hobbit))
if humano == 1:
    print("Foi inscrito 1 humano!")
if humano > 1:
    print("Foram inscritos {} humanos" .format(humano))
if anao == 1:
    print("Foi inscrito 1 anão!")
if anao > 1:
    print("Foram inscritos {} anões" .format(anao))
if gigante == 1:
    print("Foi inscrito 1 gigante!")
if gigante > 1:
    print("Foram inscritos {} gigantes" .format(gigante))
if driade == 1:
    print("Foi inscrito 1 dríade!")
if driade > 1:
    print("Foram inscritos {} dríades" .format(driade))
if troll == 1:
    print("Foi inscrito 1 troll!")
if troll > 1:
    print("Foram inscritos {} trolls" .format(troll))
if elfo == 1:
    print("Foi inscrito 1 elfo!")
if elfo > 1:
    print("Foram inscritos {} elfos" .format(elfo))
if orc == 1:
    print("Foi inscrito 1 orc!")
if orc > 1:
    print("Foram inscritos {} orcs" .format(orc))
if goblin == 1:
    print("Foi inscrito 1 goblin!")
if goblin > 1:
    print("Foram inscritos {} goblins" .format(goblin))

print("Pontuação e informações dos aprovados: \n")
for i in listCharAprov:
    print(i)
print("\nInformações dos reprovados: \n")
for i in listCharReprov:
    print(i)

print("=" * 70)
melhorGuerreiro = max(listPtsAprov)
posicaoGuerreiroM = listPtsAprov.index(melhorGuerreiro)
piorGuerreiro = min(listPtsAprov)
posicaoGuerreiroP = listPtsAprov.index(piorGuerreiro)

melhorCharAprov = listCharAprov[posicaoGuerreiroM]
piorCharAprov = listCharAprov[posicaoGuerreiroP]

print("{} e foi o(a) melhor classificado entre os aprovados! PARABÉNS!" .format(melhorCharAprov))
print("=" * 70)
print("{} e foi o(a) pior classificado entre os aprovados!" .format(piorCharAprov))

