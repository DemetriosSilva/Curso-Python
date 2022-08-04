# Curso-Python
-------------------------------------------------------------------
SAIDA DE DADOS

print('') = saida de dados 
print(" ") 

-------------------------------------------------------------------
ADICIONANDO COMENTARIOS 

# Meu primeiro codigo = comentado em uma linha

''' Meu segundo comentario '''  = comentando um bloco de código 
-------------------------------------------------------------------
STRINGS EM PYTHON 

STRING = TEXTO 

STR  = TEXTO

======================================================================
NUMEROS EM PYTHON

INTEGER = NUMEROS INTEIROS 
FLOAT = NUMEROS FRACIONAIS 


BOOLEAN TYPE = TRUE OU FALSE 
======================================================================
VARIAVEIS 

É UM ESPAÇO NA MEMÓRIA QUE ARMAZENA ALGO QUE VC QUISER 

x = 2

nome = "Demetrios"

idade = 35

cidade = "São Paulo"
=====================================================================================
MODIFICAÇÃO DE DADOS 

x = str(5)
y = int(4)
z = float(8)

print(x + x)
print(y + y)
print(z + z)
=====================================================================================
PRATICANDO COM STRINGS E INTEGERS

# O Demetrios Tem a idade de 35 anos e mora na cidade de São Paulo

nome = "Demetrios"
idade = 35
cidade = "São Paulo"

print (f' O {nome} tem {idade} anos de idade e mora na cidade de {cidade}')
=====================================================================================
USANDO INPUT 

nome = input("Digite seu nome por favor: ")
idade = input("Digite a sua idade por favor: ")
cidade = input("Digite a sua cidade natal: ")

print (f' O {nome} tem a idade de {idade} anos e mora na cidade de {cidade}')
=====================================================================================
CALCULANDO IDADE COM INPUT 

ano_nascimento = input("Em que ano vc nasceu: ")

idade = 2020 - int(ano_nascimento)

print(f'Voce tem {idade} anos de idade')
=====================================================================================
ENTENDENDO SLICE

fruta = "abacaxi"
#index   0123456

print(fruta[2:6])
=====================================================================================
UTILIZANDO FORMATAÇÃO EM STRINGS 

nome = "Demetrios"
sobrenome = "Alves"
profissao = "Programador"

texto = (f' O {nome} {sobrenome} é um excelente {profissao}')

print(texto)
=====================================================================================
METODOS PARA STRINGS 

TUDO EM LETRA MINUSCULA
mensagem = "Eu adoro lasanha"
print(mensagem.lower())

eu adoro lasanha
-------------------------------------------------------------------------------------
COLOCA A PRIMEIRA LETRA DA FRASE EM MAIUSCULO
mensagem = "eu adoro lasanha"
print(mensagem.capitalize())

Eu adoro lasanha
-------------------------------------------------------------------------------------
ME DA A POSIÇÃO DA LETRA 
mensagem = "eu adoro lasanha"
print(mensagem.find("l"))

9
-------------------------------------------------------------------------------------
TROCA AS LETRAS QUE EU DESEJAR 
mensagem = "Eu adoro lasanha"
print(mensagem.replace('a','w'))

Eu wdoro lwswnhw
-------------------------------------------------------------------------------------
TROCA PALAVRAS 
mensagem = "Eu adoro lasanha"
print(mensagem.replace('lasanha','Biscoito'))

Eu adoro Biscoito
-------------------------------------------------------------------------------------
GARANTE O PREENCHIMENTO DE ESPAÇOS 

mensagem = "       Eu adoro lasanha"
print(mensagem.strip())

Eu adoro lasanha
-------------------------------------------------------------------------------------
OPERAÇOES MATEMATICAS EM PYTHON

calculo = 2 ** 3 + 4

print(calculo)


# Parenteses
# Exponenciais
# Multiplicação e Divisão 
# Adição e Subtração 
====================================================================================
OPERADORES DE COMPARAÇÃO 

# == igual 
# != diferente
# > maior
# < menor
# >= maior ou igual 
# <= menor ou igual 

EXEMPLOS

Operadores = 10 == 10
Operadores = 10 < 20
Operadores = 10 > 8
Operadores = 10 != 20
Operadores = 10 <= 100
Operadores = 100 >= 1000
====================================================================================
OPERADORES DE ATRIBUIÇÃO 

EXEMPLOS

x = 10 
x += 5

print(x)
-----------------------------------------------------------------
x = 10 
x -= 5

print(x)
=================================================================
IF /ELSE

EXEMPLOS

idade = int(input('Digite sua idade: '))

if(idade < 18):
  print('Não pode votar')
else:
  print('Pode votar')
----------------------------------------------------------------
velocidade = 100

if velocidade > 100:
  print('Acima da velocidade permoitida')
  print('Favor reduzir velocidade')
elif velocidade < 60:
  print('Favor dirigir acima de 80km/h')
else:
  print('Velocidade OK')
=================================================================
OPERADORES LÓGICOS 

EXEMPLOS

Renda_acima_5mil = True
nome_limpo = True

if Renda_acima_5mil and nome_limpo:
  print("Financiamneto aprovado")
else:
  print("Financimaento Negado")
-----------------------------------------------------------------
Renda_acima_5mil = False
nome_limpo = True

if Renda_acima_5mil or nome_limpo:
  print("Financiamneto aprovado")
else:
  print("Financimaento Negado")
-----------------------------------------------------------------
nome = input("Digite seu nome por favor:")
sobrenome = input("Digite seu sobrenome por favor:")

if nome == "Demetrios" or sobrenome == "Alves":
  print("Estão Ok")
else:
  print("Estão Errados os nomes digite novamente por favor")
=================================================================
OPERADOR TERNARIO

EXEMPLOS

idade = 13

resultado = "Voto Permitido" if idade >= 18 else "Voto não Permitido"

print(resultado)
-------------------------------------------------------------------------------
nome = "Davi"

resultado  = "Nome esta correto" if nome == "Demetrios" else "Nome incorreto"

print(resultado)
-------------------------------------------------------------------------------
cor = "Blue"

resultado = "Cor certa" if cor == "Azul" else "Cor não é Azul"

print(resultado)
-------------------------------------------------------------------------------
nome = input("Digite seu nome:")

resultado = "Nome correto" if nome == "Demetrios" else "Nome incorreto"

print(resultado)
===============================================================================
MULTIPLOS OPERADORES DE COMPARAÇÃO 

EXEMPLOS

valor = 10

if 20 <= valor < 40:
  print("Valor aceito")
else:
  print("Produto não aceito")
=============================================================================
FOR LOOP

EXEMPLOS

IMPRIME DE 0 A 5 
for numero in range(6):
  print(numero)
---------------------------------------------------------------------
IMPRIME DE 1 ATÉ 1000
for numero in range(1,1000):
  print(numero)
---------------------------------------------------------------------
PULANDO DE DOIS EM DOIS 

for numero in range(1,20,2):
  print(numero)
---------------------------------------------------------------------
FOR LOOPS PARA STRINGS

EXEMPLOS

for letra in "Google":
  print(letra)
---------------------------------------------------------------------
FOR LOOP UTILIZANDO IF ELSE 

EXEMPLOS

compra_comfirmada = False
dados_compra = 'Compra no valor de R$12.50 e entrega comfirmada'

for enviar in range(3):
  if compra_comfirmada:
    print(dados_compra)
    print("Detalhes enviados par o email")
    break
else:
  print("Falha na Compra")
=======================================================================
FOR LOOP - NESTED LOOPS

EXEMPLOS

for numero1 in range(5):
  print(numero1)
  for numero2 in range(5):
    print(numero2)
---------------------------------------------------------------------------
for numero1 in range(1,6):
  print('Produto' + str(numero1))
  for numero2 in range(5):
    print(numero1,numero2)
================================================================================
FOR LOOPS SEPARANDO STRINGS

EXEMPLOS

palavra = "Fantastico"

for espaco in palavra:
  print(f' {espaco}' ,end = '')
================================================================================
WHILE 

EXEMPLOS

valor = 100
dia = 0

while valor > 10:
  dia -= 0
  print(f' No dia {dia} o produto vai ser vendido por R${valor}')
  valor -=5
---------------------------------------------------------------------------------
CRIANDO CONDIÇOES COM WHILE LOOP

EXEMPLOS

valor = int(input("Digite o valor do seu produto em reais: "))

while valor > 20:
  valor = (valor * 0.10) + valor
  print(f' O valor final do seu produto sera de R${valor}')
  break
=================================================================================
COMO FUNCIONA UMA FUNÇÃO 

EXEMPLO

def boas_vindas():
  print("Óla Pessoal")
  print("Sejam bem vindos")


boas_vindas()
---------------------------------------------------------------------------------
def nome():
  print('Meu nome é Demetrios Alves')

nome()

def nome1():
  print('Seu nome é Marcia')

nome1()
---------------------------------------------------------------------------------
CRIANDO UMA FUNÇÃO DE SOMA 

EXEMPLO

def somar_dois_numeros():
  numero1 = 10
  numero2 = 5
  resultado = numero1 + numero2
  print(resultado)


somar_dois_numeros()
----------------------------------------------------------------------------------
def somar_dois_numeros():
  numero1 = 10
  numero2 = 5
  resultado = numero1 + numero2
  print(resultado)


def somar_dois_numeros1():
  numero1 = 20
  numero2 = 30
  soma = numero1 + numero2
  print(soma)


somar_dois_numeros()
somar_dois_numeros1()
=================================================================
PARAMETROS E ARGUMENTOS EM FUNÇÃO

EXEMPLO

def boas_vindas(nome,quantidade):
  print(f'Óla {nome} temos {quantidade} em estoque')

boas_vindas('Marcos',5)
boas_vindas('Demetrios',7)
boas_vindas('Debora',10)
=================================================================
ARGUMENTOS DEFAULT E NO-DEFAULT

EXEMPLO

def boas_vindas(nome,quantidade = 6):
  print(f'Óla {nome} temos {quantidade} em estoque')

boas_vindas('Marcos')
================================================================
PRINT OU RETURN EM FUNÇOES

EXEMPLO

def cliente1(nome):
  print(f'Olá {nome}')

cliente1('Demetrios')


def cliente2(nome):
 return f'Olá {nome}'

print(cliente2('jose'))
=================================================================
VARIOS ARGUMENTOS XARGS COM NUMEROS 

EXEMPLO 

def soma(*numeros):
  resultado = 0
  for num in numeros:
    resultado += num
  return resultado
    

x = soma(2,3,4,7)

print(x)
==================================================================
VARIOS ARGUMENTOS XARGS NOMEANDO PARAMETROS

EXEMPLOS

def agencia(**carro):
  return carro 


print(agencia(modelo ='Gol', cor = 'Branca',motor = 1.0))
------------------------------------------------------------------
def agencia(**carro):
  return carro 


print(agencia(modelo ='Gol', cor = 'Branca',motor = 1.0,placa = 1234))
print(agencia(modelo ='Voiage', cor = 'preto',motor = 1.8,placa = 1244))
print(agencia(modelo ='Passat', cor = 'azul',motor = 1.5,placa = 1255))
==========================================================================
IMPORTANDO MODULO 

EXEMPLO

import math 

print(math.factorial(4))
-----------------------------------------------------------------------------
import math 

print(math.ceil(2.7))
=============================================================================
INTRODUCAO A LISTAS 

cidades = ['São Paulo','Rio de Janeiro','Salvador']

print(cidades)
=============================================================================
MANIPULANDO LISTAS 

cidades = ['São Paulo','Rio de Janeiro','Salvador','Goiania']

print(cidades[0])
-----------------------------------------------------------------------------
cidades = ['São Paulo','Rio de Janeiro','Salvador','Goiania']

cidades[0] = 'madagasgar'

print(cidades)
=============================================================================
FUNÇOES DENTRO LISTAS 

EXEMPLO

cidades = ['São Paulo','Rio de Janeiro','Salvador','Goiania']

cidades.sort()

print(cidades)
=============================================================================
CONCATENANDO LISTAS 

EXEMPLO 

itens = [['item1','item2'],['item3','item4']]

print(itens[1][1])
-----------------------------------------------------------------------------
letras = ['a','b'],['c','d']

print(letras[0][1])
=============================================================================
EXTRAIR VARIAVEIS DE UMA LISTA 

EXEMPLO

produtos = ['arroz','feijao','banana','laranja',1,2,3,4]

item1,item2,item3,*outros = produtos

print(item1)
print(item2)
print(item3)
print(outros)
=============================================================================
LOOPING DENTRO DE UMA LISTA 

EXEMPLO

valores = [40,80,100,120]

for x in valores:
  print(f'O valor final do produto é de {x}.')
-----------------------------------------------------------------------------
nomes = ['Demetrios','Marcia','Melissa']

for varios in nomes:
  print(f' Os nomes das pessoas cadastrados são esses {varios}.')
=============================================================================
VERIFICANDO ITENS EM UMA LISTA 

EXEMPLO

cor_cliente = input('Digite a cor Desejada: ')
cores = ['amarelo','verde','azul','vermelho']

if cor_cliente in cores:
  print('Temos essa cor em estoque')
else:
  print('Cor não esta disponivel')
-----------------------------------------------------------------------------
cor_cliente = input('Digite a cor Desejada: ')
cores = ['amarelo','verde','azul','vermelho']

if cor_cliente.lower() in cores:
  print('Temos essa cor em estoque')
else:
  print('Cor não esta disponivel')
=============================================================================
AGREGANDO DUAS LISTAS COM O ZIP

EXEMPLO

cores = ['amarelo','azul','vermelho','roxo']
valores = [10,20,30,40]

duas_listas = zip(cores,valores)

print(list(duas_listas))
-----------------------------------------------------------------------------
INPUT EM UMA LISTA 

EXEMPLO

frutas_usuario = input("Digite o nome das frutas separados por virgula: ")

frutas_lista = frutas_usuario.split(', ')


print(frutas_lista)
-----------------------------------------------------------------------------
cores = input("Digite suas cores favoritas: ")

varias_cores = cores.split(', ')

print(varias_cores)
=============================================================================
ENTENDENDO MELHOR TUPLES

EXEMPLO

TUPLES NÃO PODEM SER MUDADOS SEUS DADOS 
cores_list = ['amarelo','azul','rosa']
# lista 
cores_tuples = ('vermelho','verde','marron')
# tuple

cores_tuples.append('roxo')

print(cores_tuples)

Traceback (most recent call last):
  File "main.py", line 6, in <module>
    cores_tuples.append('roxo')
AttributeError: 'tuple' object has no attribute 'append'
-----------------------------------------------------------------------------
LISTAS PODEM SER MUDADO OS SEUS DADOS 
cores_list = ['amarelo','azul','rosa']
# lista 
cores_tuples = ('vermelho','verde','marron')
# tuple

cores_list.append('roxo')

print(cores_list)

['amarelo', 'azul', 'rosa', 'roxo']
=============================================================================
TRABALHANDO COM ARRAYS

EXEMPLOS 

from array import array 

letras = ['a','b','c','d']
numeros_i = [1,2,3,4,5]
numeros_f = [1.2,3.4,5.6]

letras = array('u',['a','b','c','d'])
numeros_i = array('i', [1,2,3,4,5])
numeros_f = array('f',[1.2,3.4,5.6])

print(letras)
print(numeros_i)
print(numeros_f)


array('u', 'abcd')
array('i', [1, 2, 3, 4, 5])
array('f', [1.2000000476837158, 3.4000000953674316, 5.599999904632568])
-----------------------------------------------------------------------------
from array import array

nomes = ['D','M','M','V']

nomes = array('u', ['D','M','M','V'])

print(nomes)

array('u', 'DMMV')
=============================================================================
CRIANDO SETS

EXEMPLO

list1 = [20,30,40,60,70]
list2 = [20,30,50,90,100]

num1 = set(list1)
num2 = set(list2)

print(num1 | num2) # union
print(num1 - num2) # Difference
print(num1 ^ num2) # Symmetric Difference
print(num1 & num2) # And
=============================================================================
FUNÇOES EM SETS 

EXEMPLOS



s1 = {1,2,3,4,5,6}

s1.update([7,8,9,10])
s1.remove(10)
s1.discard(9)

print(s1)
=============================================================================
SETS COM STRINGS

EXEMPLOS 

set1 ={'a','b','c'}
set2 ={'a','d','e'}
set3 ={'c','d','f'}

set4 = set1.union(set2)

print(set4)

{'b', 'c', 'a', 'e', 'd'}
-----------------------------------------------------------------------------
set1 ={'a','b','c'}
set2 ={'a','d','e'}
set3 ={'c','d','f'}

set4 = set1.difference(set2)

print(set4)

{'b', 'c'}
-----------------------------------------------------------------------------
set1 ={'a','b','c'}
set2 ={'a','d','e'}
set3 ={'c','d','f'}

set4 = set1.intersection(set2)

print(set4)

{'a'}
-----------------------------------------------------------------------------
set1 ={'a','b','c'}
set2 ={'a','d','e'}
set3 ={'c','d','f'}

set4 = set1.symmetric_difference(set3)

print(set4)

{'b', 'a', 'd', 'f'}
=============================================================================
INTRODUÇÃO A DICIONARIO 

EXEMPLOS

aluno = {'nome':'Demetrios','idade':32,'nota final':'A','aprovação':True}

print(aluno)
-----------------------------------------------------------------------------
aluno = {'nome':'Demetrios','idade':32,'nota final':'A','aprovação':True}

print(aluno['nome'])
=============================================================================
ATUALIZANDO ITENS NO DICIONARIO

EXEMPLOS

aluno = {'nome':'Demetrios','idade':32,'nota final':'A','aprovação':True}

aluno['nome']='jose'

print(aluno)
-----------------------------------------------------------------------------
aluno = {'nome':'Demetrios','idade':32,'nota final':'A','aprovação':True}

aluno.update({'nome':'jose','idade':35})

print(aluno)
-----------------------------------------------------------------------------
aluno = {'nome':'Demetrios','idade':32,'nota final':'A','aprovação':True}

aluno.update({'endereço':'rua leonidas'})

print(aluno)
-----------------------------------------------------------------------------
aluno = {'nome':'Demetrios','idade':32,'nota final':'A','aprovação':True}

# aluno.update({'endereço':'rua leonidas'})

print(aluno.get('endereço','O valor não existe'))
-----------------------------------------------------------------------------
aluno = {'nome':'Demetrios','idade':32,'nota final':'A','aprovação':True}

del aluno['idade']
print(aluno)
=============================================================================
LOOPING DENTRO DE UM DICIONARIO

EXEMPLOS

IMPRIMINDO SÓ OS VALORES

aluno = {'nome':'Demetrios','idade':32,'nota final':'A','aprovação':True}

for x in aluno.values():
  print(x)
-----------------------------------------------------------------------------
IMPRIMINDO TUDO KEYS/VALUES

aluno = {'nome':'Demetrios','idade':32,'nota final':'A','aprovação':True}

for x in aluno.items():
  print(x)


('nome', 'Demetrios')
('idade', 32)
('nota final', 'A')
('aprovação', True)
==============================================================================
VISUALIZANDO ITENS, KEYS E VALUES

EXEMPLOS

aluno = {'nome':'Demetrios',
         'idade':32,
         'nota final':'A',
         'aprovação':True,
         'materias':['fisica','matematica','ingles']}

print(aluno.items())
print(aluno.keys())
print(aluno.values())

dict_items([('nome', 'Demetrios'), ('idade', 32), ('nota final', 'A'), ('aprovação', True), ('materias', ['fisica', 'matematica', 'ingles'])])
dict_keys(['nome', 'idade', 'nota final', 'aprovação', 'materias'])
dict_values(['Demetrios', 32, 'A', True, ['fisica', 'matematica', 'ingles']])
============================================================================================================================================================
CONHECENDO A FUNÇÃO LAMBDA É UTILIZADA SÓ UMA VEZ
EXEMPLOS

somar10 = lambda x: x + 10

print(somar10(2))
----------------------------------------------------------
somar10 = lambda x,y: (x * y) + 10

print(somar10(2,4))
=============================================================================================================================
LAMBDA DENTRO DE UMA FUNÇÃO 

EXEMPLOS

def somar(x):
  resultado = lambda x:x + 10
  return resultado(x) * 4
 
print(somar(2))
=============================================================================================================================
FUNÇÃO FILTER 

EXEMPLO 

valores = [10,20,30,40]

def remover20(x):
  return x > 20

print(list(filter(remover20,valores)))
=============================================================================================================================
ENTENDENDO LIST COMPREHENSION COM STRINGS

EXEMPLOS

frutas1 = ['abacaxi','uva','banana','laranja']
frutas2 = []

for iten in frutas1:
  if 'u' in iten:
      frutas2.append(iten)

print(frutas2)
-----------------------------------------------------------------------------------------------------------------------------
frutas = ['abacaxi','morango','laranja','kiwi']

frutas2 = [iten for iten in frutas if 'k' in iten]

print(frutas2)
=============================================================================================================================
ENTENDENDO LIST COMPREHENSION COM NÚMEROS

EXEMPLOS

valores = [x * 10 for x in range(6)]

print(valores)
------------------------------------------------------------------------------------------------------------------------------
valores =[]

for x in range(6):
  valores.append(x * 10)

print(valores)
==============================================================================================================================
TRABALHANDO COM O TRY E EXCEPT COM UMA LISTA

EXEMPLO

try:
  letras = ['a','b','c']
  print(letras[3])
except IndexError:
  print('index não existe')
==============================================================================================================================
TRABALHANDO COM O TRY E EXCEPT COM O INPUT

EXEMPLOS

try:
  valor = int(input('Digite o valor do seu Produto: '))
  print(valor)
except ValueError:
  print('Favor Digitar um valor em numeros !!!')


Digite o valor do seu Produto: r
Favor Digitar um valor em numeros !!!
===============================================================================================================================
ADICIONANDO O ELSE E FINALLY

EXEMPLOS


try:
  valor = int(input('Digite o valor do seu Produto: '))
  print(valor)
except ValueError:
  print('Favor Digitar um valor em numeros !!!')
else:
  print('Usuario Digitou um valor correto')
  resultado = valor * 2
  print(resultado)


print('Existe mais código abaixo')
-------------------------------------------------------------------------------------------------------------------------------
try:
  valor = int(input('Digite o valor do seu Produto: '))
  print(valor)
except ValueError:
  print('Favor Digitar um valor em numeros !!!')
finally:
  print('Código OK')

print('Existe mais código abaixo')
===============================================================================================================================
CRIANDO SUA PRIMEIRA CLASSE 

EXEMPLOS

class Funcionarios:
   nome = 'Demetrios'
   sobrenome = 'Alves'


usuario1 = Funcionarios()

print(usuario1.nome)
print(usuario1.sobrenome)
--------------------------------------------------------------------------------------------------------------------------------
class Amigos:
  nome1 = 'demetrios'
  nome2 = 'acacio'
  nome3 = 'denis'

nomes_amigos = Amigos()

print(nomes_amigos.nome1)
print(nomes_amigos.nome2)
print(nomes_amigos.nome3)
===============================================================================================================================
CRIANDO OBJETOS DENTRO DE UMA CLASSE 

EXEMPLO

# Criar a Classe
class Funcionario:
  pass 



# Criar o Objeto
usuario1 = Funcionario()
usuario2 = Funcionario()


# Criar os parametros do usuario1
usuario1.nome = 'Demetrios'
usuario1.sobrenome = 'Alves'
usuario1.data_nasc = '19/12/1986'

# Criar os parametros do usuario2
usuario2.nome = 'Joana'
usuario2.sobrenome = 'Medeiros'
usuario2.data_nasc = '19/12/1977'


# print
print(usuario1.nome)
print(usuario2.nome)
===================================================================================================================
CRIANDO CONSTRUTORES 

EXEMPLO

class Funcionarios:

  def __init__(self,nome,sobrenome,data_nasc):
    self.nome = nome
    self.sobrenome = sobrenome
    self.data_nasc = data_nasc

nome1 = Funcionarios('Demetrios','Alves','10/12/1986')
nome2 = Funcionarios('Denise','Fonseca','11/12/1986')
nome3 = Funcionarios('Debora','santos','13/10/1990')

print(nome1.nome)
print(nome2.nome)
print(nome3.sobrenome)
--------------------------------------------------------------------------------------------------------------------
class Frutas:
  def __init__(self,nome,data_fabricacao):
    self.nome = nome
    self.data_fabricacao = data_fabricacao

fruta1 = Frutas('banana','12/12/2000')
fruta2 = Frutas('cajú','10/11/1990')

print(fruta1.nome)
print(fruta1.data_fabricacao)
print(fruta2.nome)
print(fruta2.data_fabricacao)
=====================================================================================================================
ADICIONANDO MAIS FUNÇÕES A CLASSE

EXEMPLOS

class Frutas:
  def __init__(self,nome,data_fabricacao):
    self.nome = nome
    self.data_fabricacao = data_fabricacao

  def dados_completos(self):
    return self.nome + ' ' + self.data_fabricacao

fruta1 = Frutas('banana','12/12/2000')
fruta2 = Frutas('cajú','10/11/1990')

print(Frutas.dados_completos(fruta1))
print(Frutas.dados_completos(fruta2))
=====================================================================================================================
CRIANDO PRIMEIRO MODULO

EXEMPLOS

PASTA FUNCOES

def somar():
    print('Esta função vai somar valores')


def multi():
    print('Esta função vai multiplicar valores')


PASTA MAIN 
import funcoes


funcoes.somar()
funcoes.multi()

========================================================================================================
CRIANDO E IMPORTANDO PACKAGES

EXEMPLOS

from funcoes import somar
from funcoes import multi
from items.cadastro import cliente

somar()
multi()
cliente()

========================================================================================================
DESAFIOS 


1 

tem_cel = int(input("Qual é a temperatura da carne ?"))

if tem_cel < 48:
  print("Cozinhar por mais alguns minutos")
elif tem_cel in range(48,53):
  print("Selada")
elif tem_cel in range(54,59):
  print("Ao ponto para mal")
elif tem_cel in range(60,64):
  print("Ao ponto")
elif tem_cel in range(65,70):
  print("Ao ponto para bem")
elif tem_cel in range(71,99):
  print("Bem passada")
elif tem_cel >= 100:
  print("Carne queimou")
=========================================================================================================
2 

Rendimento = int(input("Qual é o rendimento da lata ?"))
Altura = int(input("Qual é a altura da parede ?"))
Largura = int(input("Qual a largura da parede ?"))


area = Altura * Largura/Rendimento

print(f' Voce precisa de {area} latas de tinta')
=========================================================================================================
3

funcionarios = ['Ana','Marcos','Alice','Pedro','Sophia','Bruno','Melissa']
turno_dia = ['Ana','Marcos','Alice','Melissa']
turno_noite = ['Pedro','Sophia','Bruno']
tem_carro = ['Marcos','Alice','Bruno','Melissa']


# Lista1

lista1 = set(tem_carro).intersection(turno_noite)
print(lista1)

# Lista2

lista2 = set(tem_carro).intersection(turno_dia)
print(lista2)

# Lista3

lista3 = set (funcionarios).difference(tem_carro)
print(lista3)
=========================================================================================================
4 

Altura = float(input("Qual é a sua Altura em cm: "))
Peso = float(input("Qual é o seu peso em kg: "))

imc = Peso / (Altura / 100)**2

if imc < 18.5:
    print("MAGREZA")
elif imc >= 18.5 and imc < 24.9:
    print("NORMAL")
elif imc >= 24.0 and imc < 29.9:
    print("SOBREPESO")
elif imc >= 30.0 and imc < 39.9:
    print("OBSIDADE")
else:
    print("OBSIDADE GRAVE")
=========================================================================================================

