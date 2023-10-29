Introdução

Em determinadas situações, temos de repetir o programa ou parte dele várias vezes, como no cálculo das médias das notas de um grupo de alunos. Uma forma de solucionar este problema, seria escrever o algoritmo em questão uma vez para cada aluno, ou seja, se forem 10 alunos, teríamos de escrevê-lo 10 vezes, o que é inviável.

Outro modo de resolver essa questão seria utilizar a mesma sequência de comandos novamente, ou seja, teríamos de realizar um retrocesso (ao início dos comandos) para cada aluno, fazendo, portanto, com que o fluxo de execução repetisse certo trecho do algoritmo, o que nessa aplicação corresponderia a repetir o mesmo trecho 30 vezes, sem, no entanto, ter de escrevê-lo 10 vezes.

A esses trechos do algoritmo que são repetidos damos o nome de estruturas de repetição. O número de repetições pode ser indeterminado, porém necessariamente finito.

O conceito de repetição (looping ou laço) é utilizado quando se deseja repetir um certo trecho de instruções por um número de vezes. 

As estruturas de repetição se dividem em ENQUANTO, RE­PITA, PARA. Para determinamos qual é a estrutura mais adequa­da para determinado programa, devemos saber qual o número de vezes que o trecho do programa vai ser executado (laços conta­dos) ou a condição para que ele aconteça (laços condicionais). 

Nem todas as estruturas de repetição possuem recursos para fazer a contagem do número de vezes que o laço deverá ser repetido. Por isso, devemos utilizar uma variável de apoio (contador), sempre do tipo inteiro. A seguir é possível observar a utilização de um contador dentro do contexto das estruturas de repetição.

var contador: inteiro
 
inicio
 
    ......
 
    contador <- contador + 1
 
fim
Estrutura de Repetição Enquanto
Consiste de uma estrutura de controle do fluxo de execução que permite repetir diversas vezes um mesmo trecho do algoritmo, porém, sempre verificando antes de cada execução se é permitido executar o mesmo trecho.

Desse modo, na estrutura enquanto, a condição de repetição é verificada antes de entrar no laço, isto é, uma condição é testada inicialmente e, se o resultado for verdadeiro, o bloco de instrução será executado.

Em Português Estruturado, a utilização do enquanto é feita a partir do conjunto de instruções enquanto...faça...fim_enquanto, sendo seu funcionamento controlado por decisão.

Assim, enquanto o valor da condição for verdadeiro, as ações dos comandos são executadas. No momento em que a condição se torna falsa, o processamento da rotina é desviado para fora do laço. Se a condição for falsa logo de início, os comandos não são executados nenhuma vez, ou seja, as instruções contidas no laço são ignoradas.

A estrutura enquanto deve ser utilizada da seguinte forma:

enquanto ( <condicao> ) faça
 
      instruções
 
fimenquanto
O enquanto é utilizado quando:

Não sabemos o número de repetições.
Quando possuímos uma expressão que deve ser avaliada para que os comandos da estrutura sejam executados.  
 

Quando utilizamos os laços contados, conhecemos previa­mente quantas vezes o conjunto de instruções será repetido; en­tão, precisamos do auxílio de um contador, que auxiliará no looping (laço) da estrutura. A utilização da variável (cont) pos­sibilita a repetição da estrutura até que o contador atinja o limi­te estipulado na condição da estrutura. Assim, ele deixa de exe­cutar as instruções seguindo o fluxo do programa. 

 

Exemplo 1
Um exemplo da utilização de um laço enquanto com contador é o cálculo da média para 10 alunos. O processo de contagem ocorre por meio da expressão aritmética que obtém o valor da variável cont e adiciona 1, armazenando esse resultado na própria variável cont. Repetindo esse comando várias vezes, perceberemos que a variável vai aumentando gradativamente de valor (de 1 em 1), simulando a contagem das execuções. Este exemplo pode ser observado a seguir:

algoritmo Calcula_Medias
var
  cont : inteiro
  n1, n2, n3, m : real
inicio
  cont <- 1
 
  enquanto (cont <= 10) faça
 
       escreva "Digite 3 notas"
       leia n1, n2, n3
       m <- (n1 + n2 + n3) / 3
       escreva "Media: ", m
       cont <- cont + 1   
 
  fimenquanto
 
fim
Na animação a seguir, é possível observar a execução passo a passo do algoritmo para o cálculo da média dos 10 alunos.


Simulação da execução da estrutura de repetição enquanto - Exemplo 1
Outra forma de utilizarmos a estrutura de repetição enquanto é quando não sabemos, ao certo, o número de repetições. Nesse caso, não há a necessidade da utilização de uma variável como contador, em contrapartida, a variável utilizada na condição deve ser controlada dentro do laço. Tal controle é feito, normalmente, por leitura dessa variável.

 

Exemplo 2
Para exemplificar esta forma de utilização do enquanto, no exemplo a seguir é feito cálculo do somatório (soma acumulada) de apenas número positivos, os quais deverão ser definidos pelo usuário (por leitura). O somatório é feito enquanto o usuário digitar um número positivo e, quando ele digitar um número negativo, o laço é encerrado. Por fim, o valor do somatório é mostrado no final do algoritmo.

algoritmo Calcula_Somatorio
var
  num, soma: inteiro
inicio
  escreva "Digite um numero inteiro:"
  leia num
  soma <- 0
 
  enquanto (num >= 0) faça
       
       soma <- soma + num
       escreva "Digite um numero inteiro:"
       leia num
 
  fimenquanto
  
  escreva "Somatorio:", soma
fim
Na animação a seguir, é possível observar a execução passo a passo do algoritmo para o cálculo do somatório dos números positivos.


Simulação da execução da estrutura de repetição enquanto - Exemplo 2
CONTADOR E ACUMULADOR
Nos exemplos apresentados, dois conceitos foram utilizados: o contador e o acumulador.

O contador é uma variável cujo conteúdo é alterado pelo seu pró­prio valor adicionado ou subtraído de uma constante. Pode ser utilizado para acumular a quantidade de vezes que o programa executa as instruções do looping. O contador deve ser iniciado com um valor e deve ser incrementado ou decrementado. No primeiro exemplo é possível observar a utilização de um contador denominado cont.

O acumulador, também conhecido como somador, é utilizado para obter somatórios. Em estruturas de repetição, um acumulador ajuda a acumular valores cada vez que um laço é executado. Um acumulador é uma variável que recebe ela mesma mais o valor de outra variável. O acumulador deve ser iniciado, normalmente, com um valor nulo. O valor adicionado ao acumulador a cada execução de laço é variável, diferente do contador, cujo valor adicionado é sempre constante. No segundo exemplo é possível observar a utilização de um acumulador denominado soma.

Exercícios complementares
 

Escreva o português estruturado que verifique se uma "senha" numérica digitada pelo usuário está correta. O programa deve repetir o pedido até que o usuário escreva o valor correto. A senha deve estar definida no próprio programa.
Escreva o português estruturado que mostre na tela todos os números múltiplos de 3 até um certo número N digitado pelo usuário. Exemplo: usuário digita 14, aparece em tela: 3, 6, 9, 12.