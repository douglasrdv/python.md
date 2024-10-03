<h1 style="display: flex; justify-content: center">Conceitos Básicos de Python</h1>

## Sumário:
- [Sintaxe Básica](#sintaxe-básica)
- [Variáveis](#variáveis)
- [Operadores](#operadores)
- [Estruturas Condicionais](#estruturas-condicionais)
- [Estruturas de Repetição (Loops)](#estruturas-de-repetição-loops)
- [Listas e Sequências](#listas-e-sequências)
- [Tuplas e Sequências Imutáveis](#tuplas-e-sequências-imutáveis)
- [Dicionários](#dicionários)
- [Funções](#funções)
- [Modulos e Bibliotecas](#módulos-e-bibliotecas)
- [Tratamento de Exceções](#tratamento-de-exceções)
- [Entrada e Saída de Dados](#entrada-e-saída-de-dados)
- [Hotkeys](#hotkeys)

<h2 style="display: flex; justify-content: space-between;" id="sumário">
Sintaxe Básica:
<a href="#sumário" style="font-size: 14px">Início</a>
</h2>

A sintaxe é a estrutura ou a gramática que define como você deve escrever seu código em Python. Aqui estão alguns pontos-chave:
* **Indentação**: Em Python, a indentação (espaço em branco no início das linhas) é fundamental. Você usa a indentação para estruturar seu código. Por exemplo, em um bloco de código dentro de um if ou um for, você deve indentar o código para mostrar que ele faz parte desse bloco.
~~~
if condicao:
    # Este é um bloco de código dentro do if
    print("Este código está indentado corretamente.")
~~~    
* **Comentários**: Você pode adicionar comentários ao seu código usando o símbolo #. Comentários são linhas que o Python ignora ao executar o programa. Eles são úteis para adicionar notas explicativas ao código.
~~~
# Este é um comentário. O Python não o executará.
variavel = 42  # Comentários também podem ser adicionados após código.
~~~
* **Comentários de várias linhas:** são delimitados por três aspas simples (''') ou três aspas duplas (""") no início e no final do comentário.
~~~
'''
Este é um comentário
de várias linhas.
'''
~~~
* **Pontuação**: Python usa símbolos de pontuação para terminar instruções. Isso inclui dois pontos (:) para indicar o início de blocos de código, e ponto e vírgula (;) para separar múltiplas instruções em uma única linha (embora isso não seja comum em Python).
~~~
if condicao:
    print("Isso é uma instrução dentro do bloco.")
~~~

<h2 style="display: flex; justify-content: space-between;" id="variáveis">
Variáveis:
<a href="#sumário" style="font-size: 14px">Início</a>
</h2>


Variáveis são usadas para armazenar dados em um programa. Você pode pensar nelas como caixas onde você guarda informações. Em Python, você pode criar uma variável simplesmente atribuindo um valor a ela.
~~~
nome = "Maria"  # Criei uma variável chamada 'nome' e atribuí o valor "Maria" a ela.
idade = 30      # Criei outra variável chamada 'idade' e atribuí o valor 30 a ela.
~~~
Neste exemplo, temos duas variáveis: nome e idade. A variável nome contém uma string com o nome "Maria", e a variável idade contém um número inteiro, que é 30.

As variáveis são úteis porque você pode usá-las em seu programa para armazenar informações e manipulá-las conforme necessário. Você pode alterar o valor de uma variável a qualquer momento:
~~~
idade = 31  # Agora a variável 'idade' contém o valor 31 em vez de 30.
~~~
Variáveis podem ser usadas em cálculos, em instruções de controle de fluxo (como if), e em muitos outros lugares em seu código Python. Elas desempenham um papel fundamental na programação, permitindo que você armazene e manipule dados de forma dinâmica.
~~~
# Inteiros (int): Números inteiros
idade = 25
~~~

~~~
# Número Flutuante (float): Números com decimais
altura = 1.75
~~~

~~~
# Caracteres (str): Letras, números e símbolos
nome = "João"
~~~
~~~
# Booleanos (bool): Verdadeiro ou falso
tem_permissao = True
~~~
~~~
# Listas (list): Coleção de valores mutáveis
numeros = [1, 2, 3, 4, 5]
~~~
~~~
# Tuplas (tuple): Coleção de valores imutáveis
coordenadas = (3, 4)
~~~
~~~
# Dicionários (dict): Associação de chaves a valores
pessoa = {"nome": "Maria", "idade": 30}
~~~
~~~
# Conjuntos (set): Elementos únicos e não ordenados
cores = {"vermelho", "verde", "azul"}
~~~
~~~
# Nenhum (None): Usado em variáveis antes de atribuir um valor
valor = None
~~~
~~~
# Bytes (bytes): representam sequências de bytes imutáveis. Por exemplo, ao lidar com dados binários.
~~~

<h2 style="display: flex; justify-content: space-between;" id="operadores">
Operadores:
<a href="#sumário" style="font-size: 14px">Início</a>
</h2>

Os operadores em Python são símbolos especiais que você usa para realizar operações em valores e variáveis. Existem vários tipos de operadores em Python, mas vou destacar os operadores mais comuns:
* **Operadores Aritméticos:**
  + '+'(adição): Soma dois valores.
  + '-' (subtração): Subtrai o segundo valor do primeiro.
  + '*' (multiplicação): Multiplica dois valores.
  + '/' (divisão): Divide o primeiro valor pelo segundo.
  + '%'(módulo): Retorna o resto da divisão do primeiro valor pelo segundo.
  + '**'(exponenciação): Eleva o primeiro valor à potência do segundo.

 ~~~
x = 10
y = 3
soma = x + y   # soma contém 13
divisao = x / y  # divisao contém 3.3333333333333335
resto = x % y  # resto contém 1
~~~
* **Operadores de Comparação:**
  - '==' (igual a): Verifica se dois valores são iguais.
  - '!=' (diferente de): Verifica se dois valores são diferentes. 
  -  '>' (maior que): Verifica se o valor da esquerda é maior que o valor da direita.
  -  '<' (menor que): Verifica se o valor da esquerda é menor que o valor da direita.
  -  '>=' (maior ou igual a): Verifica se o valor da esquerda é maior ou igual ao valor da direita.
  -  '<=' (menor ou igual a): Verifica se o valor da esquerda é menor ou igual ao valor da direita.
~~~
a = 5
b = 7
igual = a == b   # igual contém False
maior_que = a > b  # maior_que contém False
~~~
* **Operadores Lógicos:**
  - and (e): Retorna True se ambas as condições forem verdadeiras.
  - or (ou): Retorna True se pelo menos uma das condições for verdadeira.
  - not (não): Inverte o valor de uma condição.
~~~
x = True
y = False
resultado = x and y  # resultado contém False
~~~
Esses são alguns dos operadores básicos que você usará com frequência em Python. Eles são usados para realizar cálculos, comparar valores e criar expressões lógicas em seu código.

<h2 style="display: flex; justify-content: space-between;" id="estruturas-condicionais">
Estruturas Condicionais:
<a href="#sumário" style="font-size: 14px">Início</a>
</h2>

As estruturas condicionais permitem que você tome decisões em seu código com base em condições específicas. Em Python, a estrutura condicional mais básica é a instrução if.
* **Instrução if:**
A instrução if permite que você execute um bloco de código somente se uma condição for verdadeira (True).
~~~
idade = 18
if idade >= 18:
    print("Você é maior de idade.")
~~~
Neste exemplo, a mensagem "Você é maior de idade" será impressa somente se a idade for maior ou igual a 18.

Você também pode usar a instrução else para executar um bloco de código quando a condição não for verdadeira:
~~~
idade = 15
if idade >= 18:
    print("Você é maior de idade.")
else:
    print("Você é menor de idade.")
~~~
Aqui, a mensagem "Você é menor de idade" será impressa porque a idade é menor que 18.

Além disso, você pode usar a instrução elif para testar condições adicionais:
~~~
nota = 85
if nota >= 90:
    print("Você tirou uma nota A.")
elif nota >= 80:
    print("Você tirou uma nota B.")
else:
    print("Você tirou uma nota C ou inferior.")
~~~
Neste caso, o programa verifica a nota e imprime a mensagem apropriada com base na faixa de notas.

<h2 style="display: flex; justify-content: space-between;" id="estruturas-de-repetição-loops">
Estrutura de Repetição (Loops):
<a href="#sumário" style="font-size: 14px">Início</a>
</h2>

As estruturas de repetição, também conhecidas como loops, permitem que você execute um bloco de código várias vezes. Em Python, os loops mais comuns são for e while.
* **Loop 'for':** O loop for é usado quando você sabe antecipadamente quantas vezes deseja executar um bloco de código. Ele é geralmente usado para iterar sobre uma sequência (por exemplo, uma lista ou uma string).
~~~
frutas = ["maçã", "banana", "laranja"]
for fruta in frutas:
    print(fruta)
~~~
Neste exemplo, o loop for percorre a lista frutas e imprime cada elemento da lista.
* **Loop 'while':**
O loop while é usado quando você quer executar um bloco de código enquanto uma condição for verdadeira.
~~~
contador = 0
while contador < 5:
    print(contador)
    contador += 1
~~~
Neste exemplo, o loop while executa o bloco de código enquanto a variável contador for menor que 5. A cada iteração, o valor de contador é incrementado em 1.

* **Comando _'break'_:** O comando break é usado para interromper imediatamente a execução de um loop em Python, independentemente da condição de término, quando uma determinada condição é atendida. Isso permite sair do loop prematuramente com base em uma condição específica.
~~~
for i in range(1, 11):
    if i == 5:
        break  # Interrompe o loop quando i é igual a 5
    print(i)
~~~

<h2 style="display: flex; justify-content: space-between;" id="listas-e-sequências">
Listas e Sequências:
<a href="#sumário" style="font-size: 14px">Início</a>
</h2>

Listas são uma das estruturas de dados mais fundamentais em Python. Elas permitem que você armazene uma coleção de valores em uma única variável. Listas podem conter elementos de diferentes tipos, como números, strings ou até mesmo outras listas.

* **Criando uma Lista:**
Você pode criar uma lista usando colchetes [] e separando os elementos por vírgulas.
~~~
frutas = ["maçã", "banana", "laranja"]
numeros = [1, 2, 3, 4, 5]
misturado = [1, "hello", True, 3.14]
~~~
* **Acessando Elementos:**
Você pode acessar elementos individuais em uma lista usando um índice (posição). Lembre-se de que a indexação em Python começa em 0.
~~~
fruta = frutas[0]  # Acessa o primeiro elemento (índice 0) da lista.
numero = numeros[2]  # Acessa o terceiro elemento (índice 2) da lista.
~~~
* **Modificando Elementos:**
Você pode alterar o valor de um elemento em uma lista atribuindo um novo valor ao seu índice.
~~~
frutas[1] = "uva"  # Modifica o segundo elemento da lista para "uva".
~~~
* **Adicionando e Removendo Elementos:**
Você pode adicionar elementos ao final de uma lista usando o método append(), ou inserir um elemento em uma posição específica usando o método insert(). Para remover elementos, você pode usar os métodos pop() ou remove().
~~~
frutas.append("morango")  # Adiciona "morango" ao final da lista.
frutas.insert(1, "pera")  # Insere "pera" na posição 1 da lista.
frutas.pop(0)  # Remove o primeiro elemento da lista.
frutas.remove("banana")  # Remove o elemento "banana" da lista.
~~~
* **Comprimento da Lista:**
Você pode verificar o comprimento de uma lista usando a função len().
~~~
tamanho = len(frutas)  # Retorna o número de elementos na lista 'frutas'.
~~~
As listas são muito versáteis e amplamente usadas em Python para armazenar coleções de dados. Elas são essenciais para muitas tarefas de programação, como armazenar informações, processar dados e iterar sobre elementos.

<h2 style="display: flex; justify-content: space-between;" id="tuplas-e-sequências-imutáveis">
Tuplas e Sequências Imutáveis:
<a href="#sumário" style="font-size: 14px">Início</a>
</h2>

Uma tupla é uma estrutura de dados semelhante a uma lista, mas com uma diferença importante: as tuplas são imutáveis, o que significa que seus elementos não podem ser alterados após a criação. As tuplas são frequentemente usadas para representar coleções ordenadas de valores que não devem ser modificados.
* **Criando uma Tupla:**
Você pode criar uma tupla usando parênteses () e separando os elementos por vírgulas.
~~~
coordenadas = (3, 4)
cores = ("vermelho", "verde", "azul")
~~~
* **Acessando Elementos:**
Você pode acessar elementos individuais em uma tupla usando um índice, assim como em listas.
~~~
x = coordenadas[0]  # Acessa o primeiro elemento (índice 0) da tupla.
cor = cores[1]  # Acessa o segundo elemento (índice 1) da tupla.
~~~
* **Imutabilidade:**
Uma vez que uma tupla é criada, seus elementos não podem ser modificados. Isso significa que você não pode adicionar, remover ou alterar elementos em uma tupla existente.
~~~
# Isso causará um erro, pois as tuplas são imutáveis.
coordenadas[0] = 5
~~~
Tuplas são frequentemente usadas quando você deseja garantir que os dados não sejam alterados acidentalmente, por exemplo, quando você tem um conjunto de valores que representam algo como as coordenadas de um ponto ou os nomes dos meses do ano.

Além disso, você pode desempacotar tuplas para atribuir seus elementos a variáveis individuais:
~~~
ponto = (3, 4)
x, y = ponto  # x receberá 3, y receberá 4
~~~
Tuplas são úteis em muitas situações, especialmente quando você precisa de coleções de dados imutáveis.

<h2 style="display: flex; justify-content: space-between;" id="dicionários">
Dicionários:
<a href="#sumário" style="font-size: 14px">Início</a>
</h2>

Dicionários são estruturas de dados em Python que permitem associar chaves a valores. Eles são semelhantes a listas, mas, em vez de usar índices numéricos, você usa chaves para acessar os valores. Os dicionários são também conhecidos como "mapas" ou "tabelas de hash".

* **Criando um Dicionário:**
Você pode criar um dicionário usando chaves {} e especificando pares chave-valor separados por dois pontos ':' .
~~~
pessoa = {"nome": "João", "idade": 30, "cidade": "São Paulo"}
~~~
Neste exemplo, temos um dicionário chamado pessoa com três pares chave-valor.
* **Acessando Valores:**
Você pode acessar os valores em um dicionário usando as chaves correspondentes.
~~~
nome = pessoa["nome"]  # Acessa o valor associado à chave "nome" (que é "João").
idade = pessoa["idade"]  # Acessa o valor associado à chave "idade" (que é 30).
~~~
* **Adicionando e Modificando Valores:**
Você pode adicionar novos pares chave-valor a um dicionário ou modificar os valores existentes.
~~~
pessoa["profissao"] = "engenheiro"  # Adiciona uma nova chave "profissao" ao dicionário.
pessoa["idade"] = 31  # Modifica o valor da chave "idade" para 31.
~~~
* **Removendo Chaves e Valores _'del'_:**
Você pode remover um par chave-valor de um dicionário usando a palavra-chave del.
~~~
del pessoa["cidade"]  # Remove a chave "cidade" e seu valor do dicionário.
~~~
* **Usando a função _'pop'_:** Para remover um item específico mas retornar os demais valores associados a chave.
~~~
agenda = {'João': '123-456', 'Maria': '789-1011'}

# Remover 'Maria' e obter o número de telefone associado
telefone_maria = agenda.pop('Maria')  # telefone_maria conterá '789-1011'

# Remover 'José', com tratamento para chave inexistente
telefone_jose = agenda.pop('José', 'Chave não encontrada')  # telefone_jose conterá 'Chave não encontrada'

~~~
Os dicionários são extremamente úteis quando você precisa associar informações relacionadas entre si. Eles são frequentemente usados para representar dados em formato de tabela, como informações de contato, configurações de aplicativos e muito mais.

<h2 style="display: flex; justify-content: space-between;" id="funções">
Funções:
<a href="#sumário" style="font-size: 14px">Início</a>
</h2>

Funções são blocos de código reutilizáveis que realizam tarefas específicas. Elas permitem que você divida seu programa em partes menores e mais gerenciáveis. Em Python, você pode criar suas próprias funções usando a palavra-chave _'def'_.
* **Criando uma Função:**
Para criar uma função, você usa a palavra-chave _'def'_, seguida do nome da função, uma lista de parâmetros entre parênteses e um bloco de código indentado.
~~~
def saudacao(nome):
    """Esta função imprime uma saudação."""
    print(f"Olá, {nome}!")
~~~
Neste exemplo, criamos uma função chamada _'saudacao'_ que aceita um parâmetro _'nome'_ e imprime uma saudação personalizada.

* **Chamando uma Função:**
Para usar uma função, você a chama pelo nome, passando os argumentos necessários entre parênteses.
~~~
saudacao("Maria")  # Chama a função e passa "Maria" como argumento.
~~~
A chamada acima resultará na impressão da saudação "Olá, Maria!".
* **Retorno de Valores:**
Uma função pode retornar um valor usando a palavra-chave return. Isso permite que você obtenha um resultado específico após a execução da função.
~~~
def soma(a, b):
    """Esta função retorna a soma de dois números."""
    resultado = a + b
    return resultado
~~~
Você pode usar o valor retornado pela função em uma variável:
~~~
resultado_da_soma = soma(3, 4)
~~~
Funções são uma parte fundamental da programação, pois permitem que você crie código reutilizável e estruture seu programa de maneira mais organizada. À medida que você avança em seu aprendizado, pode criar funções mais complexas para executar tarefas específicas.

<h2 style="display: flex; justify-content: space-between;" id="módulos-e-bibliotecas">
Módulos e Bibliotecas:
<a href="#sumário" style="font-size: 14px">Início</a>
</h2>

Em Python, um módulo é um arquivo contendo definições e instruções Python. Um pacote é uma coleção de módulos organizados em diretórios. Módulos e pacotes são usados para organizar e reutilizar código em Python.
* **Importando Módulos:**
Você pode usar a palavra-chave import para incluir módulos em seu programa. Isso permite que você acesse as funções, classes e variáveis definidas no módulo.
~~~
import math  # Importa o módulo math, que fornece funções matemáticas.
~~~
Agora, você pode usar funções do módulo _'math'_ em seu código, como _'math.sqrt()'_ para calcular a raiz quadrada.

* **Alias de Módulos:**
Você pode usar um alias (apelido) ao importar um módulo, o que permite que você se refira a ele de forma mais concisa.
~~~
import math as m  # Importa o módulo math com o alias 'm'.
raiz_quadrada = m.sqrt(25)  # Usa o alias para chamar a função sqrt().
~~~
* **Importando Funções Específicas:**
Você também pode importar funções específicas de um módulo em vez de importar o módulo inteiro.
~~~
from math import sqrt  # Importa apenas a função sqrt do módulo math.
raiz_quadrada = sqrt(25)  # Pode usar a função diretamente, sem prefixo.
~~~
* **Bibliotecas Python:**
Bibliotecas são conjuntos de módulos que fornecem funcionalidades adicionais. Python possui uma vasta biblioteca padrão que inclui módulos para tarefas comuns, como manipulação de arquivos, acesso à internet, análise de dados, entre outras.
~~~
import urllib.request  # Módulo para fazer solicitações HTTP (acesso à internet).
~~~
Você pode instalar bibliotecas externas usando um gerenciador de pacotes como o _'pip'_.

Módulos e bibliotecas são essenciais para expandir as capacidades do Python e economizar tempo na escrita de código. À medida que você avança em sua jornada de programação, provavelmente usará muitas bibliotecas diferentes para lidar com tarefas específicas em seus projetos.

<h2 style="display: flex; justify-content: space-between;" id="tratamento-de-exceções">
Tratamento de Exceções:
<a href="#sumário" style="font-size: 14px">Início</a>
</h2>

O tratamento de exceções em Python permite que você lide com erros e exceções de maneira controlada, evitando que seu programa pare abruptamente quando algo inesperado acontece. Isso torna seu código mais robusto e capaz de lidar com situações imprevistas.

* **Blocos try e except:**
Você pode usar blocos try e except para capturar exceções e tomar medidas apropriadas quando um erro ocorre.
~~~
try:
    resultado = 10 / 0  # Tentando dividir por zero
except ZeroDivisionError:
    print("Erro: Divisão por zero não é permitida.")
~~~
Neste exemplo, o código dentro do bloco _'try'_ é executado, mas quando ocorre uma exceção de divisão por zero, o código dentro do bloco _'except'_ é executado em vez de interromper o programa.

* **Blocos _'finally'_:**
Você também pode usar um bloco _'finally'_ para executar código que deve ser executado, independentemente de uma exceção ser lançada ou não.
~~~
try:
    arquivo = open("arquivo.txt", "r")
    # Código para ler o arquivo
except FileNotFoundError:
    print("Arquivo não encontrado.")
finally:
    arquivo.close()  # Garante que o arquivo seja fechado, mesmo se ocorrer uma exceção.
~~~
* **Capturando Exceções Genéricas:**
Você pode usar _'except'_ sem especificar um tipo de exceção para capturar exceções de qualquer tipo. No entanto, isso deve ser feito com cautela, pois pode ocultar erros que você deseja tratar de maneira diferente.
~~~
try:
    resultado = 10 / 0
except:
    print("Ocorreu um erro.")
~~~
É uma boa prática especificar o tipo de exceção que você espera tratar, sempre que possível, para evitar capturar exceções indesejadas.

O tratamento de exceções é uma parte importante da programação defensiva e ajuda a garantir que seu código seja mais confiável em situações inesperadas.

<h2 style="display: flex; justify-content: space-between;" id="entrada-e-saída-de-dados">
Entrada e Saída de Dados:
<a href="#sumário" style="font-size: 14px">Início</a>
</h2>

A entrada (input) e saída (output) de dados são operações fundamentais em programação. Em Python, você pode interagir com os usuários e manipular dados usando as funções _'input()'_ e _'print()'_.

* **Função input():**
A função _'input()'_ permite que você receba entrada do usuário. Ela exibe uma mensagem (prompt) para o usuário e espera que o usuário digite uma resposta.
~~~
nome = input("Digite seu nome: ")
~~~
Neste exemplo, o programa exibirá "Digite seu nome:" na tela e aguardará até que o usuário digite seu nome, que será armazenado na variável _'nome'_.

* **Função print():**
A função _'print()'_ é usada para exibir informações na tela. Você pode imprimir valores de variáveis, mensagens de texto e resultados de cálculos.
~~~
print("Olá, mundo!")
~~~
Neste exemplo, o programa imprimirá "Olá, mundo!" na tela.

* **Convertendo Tipos de Dados:**
A função _'input()'_ retorna sempre uma string. Se você desejar tratar a entrada como um número, precisará convertê-la usando funções como _'int()'_ ou _'float()'_.
~~~
idade_texto = input("Digite sua idade: ")
idade = int(idade_texto)
~~~
Isso permite que você converta a entrada de texto em um valor numérico que possa ser usado em cálculos.

* **Formatação de Saída:**
Você pode formatar a saída usando f-strings ou o método _'format()'_ para inserir valores em mensagens.
~~~
#Exemplo com f-string:
nome = "Maria"
idade = 30
print(f"Olá, {nome}! Você tem {idade} anos.")
~~~
~~~
# Exemplo com o método format():
nome = "Maria"
idade = 30
mensagem = "Olá, {}! Você tem {} anos.".format(nome, idade)
print(mensagem)
~~~
A entrada e saída de dados são cruciais para criar programas interativos e úteis. Com essas ferramentas, você pode criar programas que recebam informações dos usuários e forneçam resultados úteis.

<h2 style="display: flex; justify-content: space-between;" id="hotkeys">
Hotkeys:
<a href="#sumário" style="font-size: 14px">Início</a>
</h2>

- Ctrl + D = Seleciona o cursor de palavras das próximas ocorrências
- Ctrl + Alt + Setas = Duplica o cursor de palavra
- Shift + Alt + Setas = Duplica a linha
- Ctrl + B = Oculta a barra lateral
- Ctrl + J ou " = Abre o terminal
- Ctrl + Shift + P = Abre busca de settings do VSCode
- Ctrl + P = Abre busca de arquivos