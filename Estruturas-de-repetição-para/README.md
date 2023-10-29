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
Estrutura de Repetição Para
Os laços que possuem um número finito de execuções poderão ser processados por meio de estrutura de laço para. A estrutura para... de...ate... passo...faça... fimpara tem o seu funcionamento controlado por uma variável denominada contador. Sendo assim, pode executar um determinado conjunto de instruções certo número de vezes. Além disso, este tipo de estrutura prevê uma condição e possui limites fixos.

A estrutura Para é utilizada quando precisamos repetir um conjunto de comandos um número pré-definido de vezes. Ela deve ser utilizada da seguinte forma:

para <V> de <inicio> até <fim> passo <p> faça
 
      instruções
 
fimpara
Em que:

V: variável de controle;
inicio: é o valor inicial da variável V;
fim: é o valor final da variável V, ou seja, o valor até o qual ela vai chegar;
p: é o valor do incremento dado à variável V.

Possuímos, então, um laço com contador de forma compacta, em que sempre temos uma inicialização da variável de controle (V), um teste para verificar se a variável atingiu o limite e um acréscimo na variável de controle após cada execução do bloco de repetição.

 

Exemplo 1
No exemplo a seguir é feito o cálculo da média aritmética para 5 alunos. A cada iteração (passo) da estrutura Para, é feita a leitura das 3 avaliações (N1, N2 e N3) e, em seguida, o cálculo da média. É possível observar que a variável de controle é definida como cont, a qual começa em 1 e termina em 5. A cada iteração do laço é feito o incremento de 1 na variável cont.

 

algoritmo Calcula_medias
var
  cont : inteiro
  n1, n2, n3, m : real
inicio
 
  para cont de 1 até 5 passo 1 faça 
 
    escreva "Digite 3 notas"
    leia n1, n2, n3
    m <- (n1 + n2 + n3) / 3
    escreva "Media: ", m 
      
  fimpara
 
fim
Na animação a seguir, é possível observar a execução passo a passo do algoritmo do Exemplo 1.

MATERIAL COMPLEMENTAR
Exemplo 2
No exemplo a seguir é feito o cálculo do somatório dos números inteiros de 1 até N, onde N é um valor definido pelo usuário. É possível observar que a variável de controle é definida como cont, a qual começa em 1 e termina em N. A cada iteração do laço é feito o incremento de 1 na variável cont.

 

algoritmo Calcula_somatorio
var
  cont : inteiro
  N, soma : inteiro
inicio
  soma <- 0
  escreva "Digite o valor de N:"
  leia N
 
  para cont de 1 até N passo 1 faça 
 
      soma <- soma + cont 
      
  fimpara
  
  escreva "Somatorio: ", soma
fim
Na animação a seguir, é possível observar a execução passo a passo do algoritmo do Exemplo 2.

MATERIAL COMPLEMENTAR
Exercício complementar
 

Escreva um algoritmo em Português Estruturado que mostre todos os inteiros entre dois números digitados pelo usuário. Exemplo: usuário digita os números 8 e 15, e aparecem em tela: 9, 10, 11, 12, 13, 14.

