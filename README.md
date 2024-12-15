# Sistema-de-Estoque-ProZ-Educacao
Criar Estoque em Python

def lista_produtos(lst):
  boole = False
  while(boole == False):
    print("Para ver os produtos, digite 1 \nPara substituir um produto, digite 2 \nPara adicionar um produto, digite 3 \nSe deseja sair, digite 0")
    n = int(input())
    if (n == 0):
      boole = True
    elif (n == 1):
      for i in range(len(lst)):
        print(lst[i])
    elif (n == 2):
      print("Qual o produto que deseja substituir?")
      sub1 = input()
      print("Por qual produto deseja substituir " + sub1 + "?")
      sub2 = input()
      for i in range(len(lst)):
        if (lst[i] == sub1):
          lst[i] = sub2
    elif (n == 3):
      print("Qual o produto que deseja adicionar?")
      add = input()
      lst.append(add)
    else:
      print("Opção inválida. Por favor, tente novamente.")

array1 = ["banana","cenoura","abacaxi","tomate","cereja","melancia"]
lista_produtos(array1)
