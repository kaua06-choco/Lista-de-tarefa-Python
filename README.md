tarefas = []

def adicionar():
    tarefa = input("Digite a tarefa: ")
    tarefas.append(tarefa)

def listar():
    for i, t in enumerate(tarefas):
        print(f"{i} - {t}")

def remover():
    listar()
    i = int(input("Qual remover? "))
    tarefas.pop(i)

while True:
    print("\n1-Adicionar 2-Listar 3-Remover 4-Sair")
    op = input("Escolha: ")

    if op == "1":
        adicionar()
    elif op == "2":
        listar()
    elif op == "3":
        remover()
    else:
        break
