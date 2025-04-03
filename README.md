# Projeto-01-Ruby
Esse é o meu primeiro projeto de Ruby, o objeto é criar um programa que solicita ao usuário o seu nome e sobrenome (separado) e em seguida a sua idade. Terão 3 solicitações:  1- Nome  2- Sobrenome  3- Idade    Irá mostrar na tela ao digitar todos os dados. 

# usuário digite o seu nome completo:
# usuário irá digitar o nome e depois o sobrenome:
# # peça ao usuário digitar o seu nome completo:

#2) Entrada de dados ---> Ler o que o usuário digitou e guardar na variável - programa permita que o usuário preencha 
# o que foi pedido

#3) Saída de dados na tela ---> Aparecer um comando na tela
# Para chamar um dado #{variável}

print "Digite o seu primeiro nome:   "

nome = gets.chomp # gets = lê o que o usuário digitou e chomp = tira o \n do final da string

print "Digite o seu sobrenome:   "

sobrenome = gets.chomp # gets = lê o que o usuário digitou e chomp = tira o \n do final da string

puts "Nome completo #{nome} #{sobrenome} ! "

# usuário digita a idade:
# peça ao usuário digitar a sua idade:
print "qual a sua idade:   "
num1 = gets.chomp.to_i # gets = lê o que o usuário digitou e chomp = tira o \n do final da string e to_i = transforma em inteiro

# Aparecer o resultado na tela:
puts "O resultado da solicitação dos dados será: Seu nome completo é: #{nome} #{sobrenome}, e sua idade é:#{num1}" 
