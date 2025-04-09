<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projeto 01 - Ruby</title>
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

    <h1>Projeto 01 - Ruby</h1>

    <h2>Descrição do Projeto</h2>
    <p>Esse é o meu primeiro projeto de Ruby, onde criamos um programa simples que solicita o nome, sobrenome e idade do usuário, e depois exibe essas informações na tela. O objetivo é entender os conceitos básicos de entrada e saída de dados no Ruby.</p>

    <blockquote>
        Exemplo de execução:
        <pre><code>$ ruby projeto_01.rb</code></pre>
    </blockquote>

    <h2>Como Funciona o Programa</h2>

    <h3>Passo 1: Solicitação do Nome</h3>
    <p>O programa solicita ao usuário para digitar o seu primeiro nome:</p>
    <div class="step">
        <p><strong>Comando:</strong></p>
        <pre><code>print "Digite o seu primeiro nome: "</code></pre>
    </div>
    <p>O valor digitado é armazenado na variável <code>nome</code>:</p>
    <div class="step">
        <pre><code>nome = gets.chomp</code></pre>
    </div>

    <h3>Passo 2: Solicitação do Sobrenome</h3>
    <p>Em seguida, o programa solicita o sobrenome do usuário:</p>
    <div class="step">
        <p><strong>Comando:</strong></p>
        <pre><code>print "Digite o seu sobrenome: "</code></pre>
    </div>
    <p>O sobrenome é armazenado na variável <code>sobrenome</code>:</p>
    <div class="step">
        <pre><code>sobrenome = gets.chomp</code></pre>
    </div>

    <h3>Passo 3: Solicitação da Idade</h3>
    <p>Após o nome e sobrenome, o programa pede a idade do usuário:</p>
    <div class="step">
        <p><strong>Comando:</strong></p>
        <pre><code>print "Qual a sua idade: "</code></pre>
    </div>
    <p>A idade é lida e convertida para número inteiro e armazenada na variável <code>num1</code>:</p>
    <div class="step">
        <pre><code>num1 = gets.chomp.to_i</code></pre>
    </div>

    <h2>Resultado na Tela</h2>
    <p>Depois de coletar todos os dados, o programa exibe uma mensagem com as informações fornecidas pelo usuário:</p>
    <div class="step">
        <pre><code>puts "O resultado da solicitação dos dados será: Seu nome completo é: #{nome} #{sobrenome}, e sua idade é: #{num1}"</code></pre>
    </div>

    <h2>Código Completo</h2>
    <pre><code>
# Código completo do programa Ruby

print "Digite o seu primeiro nome: "
nome = gets.chomp

print "Digite o seu sobrenome: "
sobrenome = gets.chomp

puts "Nome completo #{nome} #{sobrenome} ! "

print "Qual a sua idade: "
num1 = gets.chomp.to_i

puts "O resultado da solicitação dos dados será: Seu nome completo é: #{nome} #{sobrenome}, e sua idade é: #{num1}"
    </code></pre>

    <footer>
        <p>Projeto desenvolvido como parte de um exercício para aprender Ruby. © 2025</p>
    </footer>

</body>
</html>
