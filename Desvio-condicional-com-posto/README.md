Introdução

Os desvios condicionais, também chamados de estruturas de seleção ou decisão, são utilizados quando existe a necessidade de verificar condições para a realização de uma instrução ou de uma sequência de instruções. Os testes de seleção também podem ser utilizados para verificar opções de escolha. A tomada de decisão sempre deve estar de acordo com o resultado de uma expressão lógica.

Existem quatro tipos de desvios condicionais: simples, composto, encadeado e o de múltipla escolha. Neste tópico serão abordados conceitos sobre o desvio condicional composto.

 

Desvio Condicional Composto
Quando tivermos situações em que duas alternativas dependem de uma mesma condição, uma de a condição ser verdadeira e outra de a condição ser falsa, usamos o desvio condicional composto.

Nesta instrução, se a condição estabelecida for verdadeira, são executadas todas as instruções definidas entre se...então e senão. Se a condição estabelecida for falsa, são executadas todas as instruções que estiverem definidas entre senão e fimse. Somente após a execução de uma das possibilidades anteriores é que o programa executa as instruções existentes após o fimse.

Em Português Estruturado, a instrução para o desvio condicional composto deve seguir o seguinte modelo:

se <condicao> entao
    instrucoes para cond. verdadeira
senao
   instrucoes para cond. falsa
fimse
Na Figura a seguir, podemos observar o diagrama da sintaxe desse tipo de desvio:

Apresentar o Diagrama da sintaxe do desvio condicional composto
Diagrama da sintaxe do desvio condicional composto
Fonte: FORBELLONE, A. L. V; EBERSPACHER, H. F. Lógica de Programação: a construção de algoritmos e estruturas de dados (3a. edição). São Paulo: Prentice Hall, 2005.
Exemplo 1
Neste exemplo é feita a leitura de dois valores numéricos inteiros. Caso a adição entre eles resulte em um valor maior ou igual a 10, será atribuído a uma nova variável o valor resultante somado a 5. Caso contrário (adição menor que 10), será atribuído a uma nova variável o valor resultante subtraído de 7. Por fim, o valor da nova variável será exibido.

algoritmo Soma_Numeros		
var
  A, B, X, R : inteiro
inicio
 
  escreva "Digite dois numeros inteiros"
  leia A, B
  X <- A + B
 
  se X >= 10 entao
    R <- X + 5   
  senao
    R <- X - 7
  fimse
 
  escreva "Valor de R=", R
 
fim
Pela animação a seguir, é possível observar a execução do algoritmo passo a passo (linha por linha).

Apresentar a Execução passo a passo do Exemplo 1 - Desvio Condicional Composto
Execução passo a passo do Exemplo 1 - Desvio Condicional Composto
Exemplo 2
No exemplo a seguir, é feita a leitura do salário de um funcionário. Em seguida, caso o salário informado seja menor ou igual a 2000, então é feito o acréscimo de 30% sobre seu valor. Caso contrário (salário maior do que 2000), será feito um acréscimo de 10% sobre seu valor. Por fim, o novo salário é exibido.

algoritmo Acrescimo_Salario
var
  salario, novo_salario : real
inicio
 
  escreva "Digite o salario do funcionario"
  leia salario
 
  se salario <= 2000 entao
       novo_salario <- salario * 1.30   
  senao
       novo_salario <- salario * 1.10
  fimse
 
  escreva "Novo salario=", novo_salario
 
fim
Pela animação a seguir, é possível observar a execução do algoritmo passo a passo (linha por linha).

Apresentar a Execução passo a passo do Exemplo 2 - Desvio Condicional Composto
Execução passo a passo do Exemplo 2 - Desvio Condicional Composto
Exercícios complementares
 

1. Escreva um algoritmo em Português Estruturado para exibir a situação de um aluno (Aprovado ou Reprovado) a partir do cálculo da média de 4 avaliações. O aluno é considerado aprovado caso sua média seja maior ou igual a 6; caso contrário ele é reprovado.

2. Escreva um algoritmo em Português Estruturado para verificar a paridade (par ou ímpar) de um número inteiro digitado pelo usuário. 

3. Escreva um algoritmo em Português Estruturado que mostre se um número inteiro, digitado pelo usuário, é positivo ou negativo.

