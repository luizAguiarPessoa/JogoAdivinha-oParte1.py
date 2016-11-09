# JogoAdivinha-oParte1.py
from random import *
rdn = randint(100)
tent = 3
print()
print("Tente adivinhar o número secreto de 1 a 100! Você terá 3 tentativas!")
print()
while tent > 0:
    tent = tent - 1
    ch = int(input("Número: "))
    print()
    if ch > rdn:
        print("O número secreto é menor!")
        print("Número de tentativas: %d" % tent)
        print()
    elif ch < rdn:
        print("O número secreto é maior!")
        print("Número de tentativas = %d" % tent)
        print()
    else:
        print("Parabéns! Você acertou! O número secreto é: %d" % rdn)
        tent = -1
if tent == 0:
    print()
    print("Que pena! Você perdeu! Mais sorte da próxima vez ")
    print("O número secreto é: %d" % rdn)
    input()
elif tent == -1:
    input()
