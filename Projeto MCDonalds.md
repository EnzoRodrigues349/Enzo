[mc donalds.py](https://github.com/user-attachments/files/24360878/mc.donalds.py)
def linha():
    print('-'*30)

soma=0
qtd=0

cardapio=[['McLanche',9],['McFeliz',9], ['Sundae',6],['Pipoca',4],['Refri',8]]
linha()
print('BEM VINDO AO MCDONALDS')
linha()
print('Faça sua escolha pelos índices 0,1,2..., depois a quantidade.')

for c, v in enumerate(cardapio):
    print(f"{c} - {v[0]}: R$ {v[1]}")

while True:
    escolha=int(input('Qual sua escolha:'))
    qtd=int(input('Qual a quantidade?'))
    soma += cardapio[escolha][1] * qtd
    simounao=str(input('Quer escolher mais algo? informe[s/n]').lower())
    if simounao=='n':
        break
print('O valor a pagar:',soma)














