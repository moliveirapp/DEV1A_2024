# Bem-vindos ao Repositório da Turma DEV1A_2024!
### Olá, queridos alunos da turma DEV1A_2024!

Sejam todos muito bem-vindos ao nosso repositório da turma! Este repositório foi criado com o intuito de ser uma ferramenta de apoio e colaboração para todos nós durante o curso.

Exercícios: Serão postados exercícios propostos em aula para prática e fixação dos conteúdos.


Sejam bem-vindos e vamos juntos rumo ao aprendizado!

# Atenciosamente,

## Bruno e Matheus


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

