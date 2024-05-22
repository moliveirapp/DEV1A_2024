# Desenvolvimento de um Programa de Gerenciamento de Alunos
### Desenvolva um programa em Python para gerenciar uma lista de alunos. O programa deve fornecer as seguintes funcionalidades:

* Adicionar Aluno: Permite ao usuário adicionar um novo aluno à lista.

* Listar Alunos: Exibe a lista de alunos cadastrados.

* Ordenar Lista: Ordena a lista de alunos em ordem alfabética.

* Apagar Aluno: Permite ao usuário remover um aluno da lista, fornecendo a posição na lista.

O programa deve apresentar um menu de opções e executar a funcionalidade escolhida pelo usuário. 
Além disso, o programa deve validar a entrada do usuário, garantindo que apenas números sejam aceitos como entrada para as opções do menu.

## Exemplo do Menu de Opções:

### Qual opção deseja?
0 - Sair \
1 - Adicionar Aluno \
2 - Listar alunos \
3 - Organizar Lista \
4 - Apagar um aluno \
\
Ao selecionar a opção **"Sair"**, o programa deve **encerrar** sua execução. Ao selecionar uma opção inválida, deve exibir uma mensagem de erro e solicitar ao usuário que tente novamente.

Certifique-se de fornecer mensagens informativas ao usuário durante a execução do programa, como confirmações de adição, exclusão e ordenação de alunos, bem como mensagens de erro quando a entrada do usuário for inválida.

### Algumas dicas de comandos a serem utilizados no geral:
#### Comandos de condições, repetições, listas, breaks, blocos de tratamentos de erros, inputs, e mais alguns.

# Boa Sorte!

### Reflexão: "Bora codificar, pois nós nascemos lindos, não ricos 😂😝😜🫠😅🙃🤪"




# Resolução do exercício:

```
alunos = []

def adicionarAluno(nome):
    alunos.append(nome)
    print("Aluno adicionado")

def ordenarLista():
    alunos.sort()
    print("Sua lista foi ordenada")

def apagarAluno(posicao):
    del alunos[posicao]
    print("Aluno deletado")

def listarAlunos():
    print("------------ Lista de alunos cadastrados ------------")
    for i in range(len(alunos)):
        print(i, " - ", alunos[i])
    print("------------ Fim de alunos cadastrados ------------")

acao = 1
while acao != 0:
    try:
        acao = int(input("Qual opção deseja? \n 0 - Sair \n 1 - Adicionar Aluno \n 2 - Listar alunos \n 3 - Organizar Lista \n 4 - Apagar um aluno "))
    except ValueError:
        print("Por favor, digite um número.")
        continue

    if acao == 0:
      print("Encerrando o programa")
      break
    elif acao == 1:
        nome = input("Digite o nome do aluno : ")
        adicionarAluno(nome)
    elif acao == 2:
        listarAlunos()
    elif acao == 3:
        ordenarLista()
    elif acao == 4:
        listarAlunos()
        try:
            posicao = int(input("Digite qual posição você quer apagar:"))
        except ValueError:
            print("Por favor, digite um número para a posição.")
            continue
        apagarAluno(posicao)
    else:
        print("Operação inválida, digite novamente")
