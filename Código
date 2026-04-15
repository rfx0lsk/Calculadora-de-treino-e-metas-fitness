print("\n---------------------Seja bem-vindo ao FitFit GRR'sss-----------------------------\n")
print("Insira os dados para realizar o cadastro ")

nome_user = input("Informe seu nome: ")
genero_user = input("Informe seu genero: (M/F)").lower()

while genero_user not in ['m', 'f']:
    print("Opção inválida! Tente novamente.")
    genero_user = input("Informe seu gênero (m/f): ").lower()

altura_user = float(input("Informe sua altura (cm): ")) / 100
peso_user = float(input("Informe seu peso (kg): "))

resultado = peso_user / (altura_user * altura_user)

print("\nOlá", nome_user, "seu IMC é", round(resultado, 2))

if resultado < 18.5:
    print("Baixo peso")
elif resultado < 25:
    print("Peso normal")
elif resultado < 30:
    print("Sobrepeso")
elif resultado < 34:
    print("Obesidade 1")
elif resultado < 40:
    print("Obesidade 2")
else:
    print("Obesidade 3")

# Inicialização de variáveis
tmb = 0
get = 0
idade = 0
atividade_fisica = 0
objetivo = 0
calorias = 0

while True:
    print("\nOlá", nome_user, "deseja:\n")
    print("1. Atualizar seu IMC")
    print("2. Meta diária de hidratação!")
    print("3. Treino inicial")
    print("4. Gasto calórico de treino")
    print("5. Taxa metabólica basal (TMB)")
    print("6. Gasto Calórico Total")
    print("7. Objetivo")
    print("8. Histórico")
    print("9. Meta diária")
    print("10. Sair")

    opcao_central = input("Selecione uma opção: ")

    match opcao_central:
        case '1':
            ##Atualização de IMC
            informacao_cadastro = input("A informação do cadastro mudou? (s/n): ").lower()

            while informacao_cadastro not in ['s', 'n']:
                print("Opção inválida! Tente novamente.")
                informacao_cadastro = input("A informação do cadastro mudou? (s/n): ").lower()

            if informacao_cadastro == 's':
                altura_user = float(input("Informe sua altura (cm): ")) / 100
                peso_user = float(input("Informe seu peso (kg): "))

            # usa os dados atualizados ou antigos
            resultado = peso_user / (altura_user * altura_user)

            print("Seu IMC é", round(resultado, 2))

            if resultado < 18.5:
                print("Baixo peso")
            elif resultado < 25:
                print("Peso normal")
            elif resultado < 30:
                print("Sobrepeso")
            elif resultado < 34:
                print("Obesidade 1")
            elif resultado < 40:
                print("Obesidade 2")
            else:
                print("Obesidade 3")
        case '2':
          ##Calculo de hidratação
            print ("Meta diária de hidratação!")
            informacao_cadastro = input("A informação do cadastro mudou? (s/n): ")

            while informacao_cadastro not in ['s', 'n']:
                  print("Opção inválida! Tente novamente.")
                  informacao_cadastro = input("A informação do cadastro mudou? (s/n): ").lower()
            if informacao_cadastro == 's':
                  peso_user = float(input("Informe seu peso (kg): "))

            agua = peso_user * 0.035
            print("A quantidade mínima diária de água que você deve beber em litros é: ", agua)

        case '3':
            print("Treino inicial \n")
            print("1. Treino A (Peito + Tríceps)   \n2. Treino B (Costas + Bíceps) \n3. Treino C (Pernas + Ombro)")
            opcao_treino = input("Selecione a uma opção: ")
            match opcao_treino:
                case '1':
                    print("\nSupino reto – 3x10 \nSupino inclinado – 3x10 \nPeck deck – 3x10 \nTríceps na polia – 3x10 \nTríceps banco – 3x10")
                    print("Bom treino!\n")
                case '2':
                    print("\nPuxada na frente – 3x10 \nRemada baixa – 3x10 \nRemada unilateral – 3x10 \nRosca direta – 3x10 \nRosca alternada – 3x10")
                    print("Bom treino!\n")
                case '3':
                    print("\nAgachamento – 3x10 \nLeg press – 3x10 \nCadeira extensora – 3x10 \nDesenvolvimento de ombro – 3x10 \nElevação lateral – 3x10 \nAbdominal – 3x15")
                    print("Bom treino!\n")
        case '4':
            ## Gasto calórico
            print ("Gasto calórico")
            tempo = float(input("Tempo de treino (minutos): "))
            informacao_cadastro = input("A informação do cadastro mudou? (s/n): ")

            while informacao_cadastro not in ['s', 'n']:
                  print("Opção inválida! Tente novamente.")
                  informacao_cadastro = input("A informação do cadastro mudou? (s/n): ").lower()
            if informacao_cadastro == 's':
                  peso_user = float(input("Informe seu peso (kg): "))
                  genero_user = input("Informe seu genero: m (Masculino) ou f (Feminino): )")
                  while genero_user not in ['m', 'f']:
                    print("Opção inválida! Tente novamente.")
                    sexo = input("Informe seu sexo (m/f): ")

            if genero_user == 'm':
                gasto_genero = 1
            else:
                gasto_genero = 0.9

            tempo_horas = tempo / 60

            print("Seu treino foi:")
            print("\n1. Musculação leve \n2. Musculação moderada\n3. Musculação intensa")
            nivel = input("Escolha: ")

            while nivel not in ['1', '2', '3']:
                print("Opção inválida! Tente novamente.")
                nivel = input("Escolha (1, 2 ou 3): ")

            if nivel == '1':
                met = 3.5
            elif nivel == '2':
                met = 5
            else:
                met = 7

            calorias = met * peso * tempo_horas * gasto_genero

            print("\nGasto calórico estimado:", calorias, "kcal\n")

        case '5':
            print(" --- CALCULO DE TMB --- ")
            idade = int(input("Insira sua idade: "))
            informacao_cadastro = input("A informação do cadastro mudou? (s/n): ").lower()

            while informacao_cadastro not in ['s', 'n']:
                print("Opção inválida!")
                informacao_cadastro = input("A informação do cadastro mudou? (s/n): ").lower()

            if informacao_cadastro == 's':
                peso_user = float(input("Informe seu peso (kg): "))
                altura_user = float(input("Informe sua altura (cm): ")) / 100
                genero_user = input("Informe seu genero (m/f): ").lower()

                while genero_user not in ['m', 'f']:
                    print("Opção inválida!")
                    genero_user = input("Informe seu genero (m/f): ").lower()

            if genero_user == 'f':
                tmb = (10 * peso_user) + (6.25 * (altura_user * 100)) - (5 * idade) - 161
            else:
                tmb = (10 * peso_user) + (6.25 * (altura_user * 100)) - (5 * idade) + 5

            print("Seu TMB é:", tmb)

        case '6':
            print("\n --- GASTO ENERGÉTICO TOTAL (GET) --- ")

            if tmb == 0:
                print("Calcule a TMB primeiro (opção 5)")
                continue
                ##'continue' é uma instrução de controle de loop que pula a iteração atual e passa imediatamente para a próxima.

            print("1: Sedentário - Não pratica exercícios (0-1x/semana)")
            print("2: Baixo - Atividade leve (1-2x/semana)")
            print("3: Moderado - Exercícios regulares (3-5x/semana)")
            print("4: Alto - Treinos intensos (5-6x/semana)")
            print("5: Muito Alto - Treino intenso diário (6-7x/semana)")

            atividade_fisica = 0
            while atividade_fisica < 1 or atividade_fisica > 5:
                atividade_fisica = int(input("Escolha (1-5): "))
                if atividade_fisica < 1 or atividade_fisica > 5:
                    print("Número inválido")

            if atividade_fisica == 1:
                fator = 1.2
            elif atividade_fisica == 2:
                fator = 1.375
            elif atividade_fisica == 3:
                fator = 1.55
            elif atividade_fisica == 4:
                fator = 1.725
            else:
                fator = 1.9

            get = tmb * fator
            print("Seu GET é:", get)

        case '7':
            print("\n--- OBJETIVO ---")

            if get == 0:
                print("Calcule o GET primeiro (opção 6)")
                continue
            ##'continue' é uma instrução de controle de loop que pula a iteração atual e passa imediatamente para a próxima.
            objetivo = 0
            while objetivo < 1 or objetivo > 3:
                objetivo = int(input("Emagrecer: 1 | Manter: 2 | Ganhar massa: 3: "))
                if objetivo < 1 or objetivo > 3:
                    print("Número inválido")

            if objetivo == 1:
                calorias = get - 500
                print("Para emagrecer:", calorias, "kcal/dia")
            elif objetivo == 2:
                calorias = get
                print("Para manter:", calorias, "kcal/dia")
            else:
                calorias = get + 500
                print("Para ganhar massa:", calorias, "kcal/dia")

        case '8':
            print("\n--- HISTÓRICO ---")

            print("Nome:", nome_user)
            print("Peso:", peso_user, "kg")
            print("Altura:", altura_user * 100, "cm")
            print("Sexo:", "Feminino" if genero_user == 'f' else "Masculino")

            if idade != 0:
                print("Idade:", idade)

            if tmb != 0:
                print("TMB:", tmb)

            if get != 0:
                print("GET:", get)

            if atividade_fisica != 0:
                niveis = ["", "Sedentário", "Baixo", "Moderado", "Alto", "Muito Alto"]
                print("Atividade:", niveis[atividade_fisica])

            if objetivo != 0:
                objetivos = ["", "Emagrecer", "Manter", "Ganhar massa"]
                print("Objetivo:", objetivos[objetivo])

            if calorias != 0:
                print("Calorias recomendadas:", calorias)

        case '9':
          ##resumo diario
          print("\n--- Resumo Diário ---")

          if calorias == 0:
              print("Defina seu objetivo primeiro (opção 7)")
              continue

          calorias_dia = float(input("Informe as calorias consumidas hoje: "))
          hidratacao_dia = float(input("Informe a quantidade de água consumida (L): "))

          # cálculo caloria
          diferenca_calorias = calorias_dia - calorias

          print("\n--- CALORIAS ---")
          print("Meta:", calorias, "kcal")
          print("Consumido:", calorias_dia, "kcal")

          if diferenca_calorias > 0:
              print("Você consumiu", diferenca_calorias, "kcal a mais.")
          elif diferenca_calorias < 0:
              print("Você consumiu", abs(diferenca_calorias), "kcal a menos.")
          else:
              print("Meta de calorias atingida!")

          # hidratação 
          if 'agua' in locals():
              diferenca_agua = hidratacao_dia - agua

              print("\n--- HIDRATAÇÃO ---")
              print("Meta:", agua, "L")
              print("Consumido:", hidratacao_dia, "L")

              if diferenca_agua > 0:
                  print("Você bebeu", diferenca_agua, "L a mais.")
              elif diferenca_agua < 0:
                  print("Faltaram", abs(diferenca_agua), "L de água.")
              else:
                  print("Meta de água atingida!")
          else:
              print("\nMeta de água não definida (use opção 2)")
              
        case '10':
            print("Saindo do sistema...")
            break

        case _:
            print("Opção inválida!")
