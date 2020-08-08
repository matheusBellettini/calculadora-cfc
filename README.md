# calculadora-cfc

def space():
    print('                       ')
    
def linha():
    print('-------------------------')

print ( 'CALCULO DA MÉDIA CFC. (OBS: UTILIZE PONTO AO INVES DE VIRGULA)')
linha()

nota_cfsd = float(input('Escreva sua nota do CFSD: '))
nota_cesd = float(input('Escreva sua nota do CESD: '))
nota_chefe = float(input('Escreva sua nota do chefe: '))
nota_tacf = float(input('Escreva sua nota do TACF: '))

print('Niveis de escolaridade: MI (5) | FIC (6) | MC (7)| MT (8) | SI (9) | SC (10)')

space()

nota_ne = float(input('Selecione o número relacionado ao seu nivel de escolaridade: '))  

adp = nota_chefe * 3
tacf = nota_tacf / 10 * 3
cfsd = nota_cfsd * 2
cesd = nota_cesd * 4
ne = nota_ne * 4

final = adp + tacf + cfsd + cesd + ne 

media = final / 16 

space()

print('Sua média final é:', media)

space()

if media >= 7.5:
    print('Você tem grandes chances de entrar nas vagas, pois sua nota está acima da média')
else:
    print('Sua nota pode não ser o suficiente para entrar nas vagas')
