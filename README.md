<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projeto de Calculadora em Ruby</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f7f7f7;
            color: #333;
            margin: 0;
            padding: 0;
        }
        h1, h2, h3 {
            color: #2c3e50;
        }
        h1 {
            text-align: center;
            margin-top: 20px;
            font-size: 2.5em;
        }
        h2 {
            font-size: 1.8em;
            margin-top: 30px;
        }
        h3 {
            font-size: 1.4em;
            margin-top: 20px;
        }
        p {
            font-size: 1.1em;
            line-height: 1.6;
            margin: 15px 0;
            padding: 0 20px;
        }
        pre {
            background-color: #2c3e50;
            color: #ecf0f1;
            padding: 10px;
            border-radius: 5px;
            overflow-x: auto;
            font-size: 1em;
            margin: 20px 0;
            max-width: 100%;
            white-space: pre-wrap;
            word-wrap: break-word;
        }
        code {
            background-color: #34495e;
            padding: 2px 6px;
            border-radius: 3px;
            color: #ecf0f1;
        }
        blockquote {
            background-color: #ecf0f1;
            padding: 15px;
            border-left: 5px solid #3498db;
            margin: 20px 0;
            font-style: italic;
        }
        ul {
            padding-left: 40px;
        }
        li {
            font-size: 1.1em;
            line-height: 1.5;
        }
        .step {
            margin-left: 20px;
            padding: 5px 0;
            background-color: #e7f1f7;
            border-left: 4px solid #3498db;
        }
        footer {
            text-align: center;
            font-size: 0.9em;
            margin-top: 50px;
            padding: 10px;
            background-color: #2c3e50;
            color: white;
        }
    </style>
</head>
<body>

    <h1>Projeto de Calculadora em Ruby</h1>

    <h2>Objetivo do Projeto</h2>
    <p>Este é um projeto simples feito em Ruby para criar uma calculadora interativa. O programa solicita ao usuário que escolha entre cinco opções: soma, subtração, multiplicação, divisão ou sair. Dependendo da escolha, o programa executa a operação e exibe o resultado.</p>

    <h2>Descrição do Código</h2>
    <p>O código foi estruturado em um loop que exibe um menu com cinco opções. O programa pede para o usuário escolher uma das opções, e de acordo com a escolha, ele solicita dois números e realiza a operação correspondente.</p>

    <h3>Menu de Opções</h3>
    <p>O menu exibido para o usuário é o seguinte:</p>
    <div class="step">
        <pre><code>Escolha uma das opções:
1 - Soma
2 - Subtração
3 - Multiplicação
4 - Divisão
5 - Sair</code></pre>
    </div>

    <h3>Estrutura do Código</h3>
    <p>O código funciona da seguinte maneira:</p>
    <ul>
        <li>O programa exibe o menu e aguarda a entrada do usuário.</li>
        <li>Dependendo da opção escolhida, o programa pede dois números e realiza a operação desejada.</li>
        <li>Se o usuário escolher a opção 5 (Sair), o programa termina.</li>
        <li>Se o usuário escolher uma opção inválida, o programa solicita que ele tente novamente.</li>
    </ul>

    <h3>Exemplo de Execução</h3>
    <blockquote>
        Exemplo de execução do programa:
        <pre><code>$ ruby calculadora.rb
Escolha uma das opções:
1 - Soma
2 - Subtração
3 - Multiplicação
4 - Divisão
5 - Sair
1
Digite o primeiro número:
3
Digite o segundo número:
2
Resultado da soma: 5.0</code></pre>
    </blockquote>

    <h2>Código Completo</h2>
    <pre><code># Calculadora em Ruby
loop do
    # Exibe o menu de opções
    puts "Escolha uma das opções:"
    puts "1 - Soma"
    puts "2 - Subtração"
    puts "3 - Multiplicação"
    puts "4 - Divisão"
    puts "5 - Sair"
  
    # Lê a opção escolhida
    escolha = gets.to_i
  
    # Verifica qual operação o usuário escolheu
    if escolha == 1
      puts "Digite o primeiro número:"
      num1 = gets.to_f
      puts "Digite o segundo número:"
      num2 = gets.to_f
      soma = num1 + num2
      puts "Resultado da soma: #{soma}"
  
    elsif escolha == 2
      puts "Digite o primeiro número:"
      num1 = gets.to_f
      puts "Digite o segundo número:"
      num2 = gets.to_f
      subtracao = num1 - num2
      puts "Resultado da subtração: #{subtracao}"
  
    elsif escolha == 3
      puts "Digite o primeiro número:"
      num1 = gets.to_f
      puts "Digite o segundo número:"
      num2 = gets.to_f
      multiplicacao = num1 * num2
      puts "Resultado da multiplicação: #{multiplicacao}"
  
    elsif escolha == 4
      puts "Digite o primeiro número:"
      num1 = gets.to_f
      puts "Digite o segundo número:"
      num2 = gets.to_f
      if num2 == 0
        puts "Erro: Não é possível dividir por zero!"
      else
        divisao = num1 / num2
        puts "Resultado da divisão: #{divisao}"
      end
  
    elsif escolha == 5
      puts "Saindo..."
      break  # Sai do loop se a opção 5 for escolhida
  
    else
      puts "Opção inválida! Tente novamente."
    end
end</code></pre>

    <footer>
        <p>Projeto desenvolvido como parte do desafio de Ruby. © 2025</p>
    </footer>

</body>
</html>
