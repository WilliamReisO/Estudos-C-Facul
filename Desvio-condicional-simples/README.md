Introdução
Os desvios condicionais, também chamados de estruturas de seleção ou decisão, são utilizados quando existe a necessidade de verificar condições para a realização de uma instrução ou de uma sequência de instruções. Os testes de seleção também podem ser utilizados para verificar opções de escolha. A tomada de decisão sempre deve estar de acordo com o resultado de uma expressão lógica.

Existem quatro tipos de desvios condicionais: simples, composto, encadeado e o de múltipla escolha. Neste tópico serão abordados conceitos sobre o desvio condicional simples.

 

Desvio Condicional Simples
 

Esse tipo de desvio é representado por uma instrução que avalia uma expressão lógica, resultando um valor que pode ser verdadeiro ou falso. Ele deve ser utilizado caso seja necessário executar instruções somente se uma condição for verdadeira.

A tomada de decisão simples utiliza a instrução se...então...fim_se. Nesta instrução, se a condição estabelecida for verdadeira, são executadas todas as instruções definidas entre se...então e fim_se, depois são executadas todas as condições existentes após fim_se. Se a condição estabelecida for falsa, são executadas as instruções que estão definidas após a instrução fim_se.

Em Português Estruturado, a instrução para o desvio condicional simples deve seguir o seguinte modelo:

se <condicao> entao
 
      instrucoes
 
fimse
 A condição estabelecida é uma expressão lógica que, quando analisada, pode gerar um valor lógico: verdadeiro ou falso. Se a condição for verdadeira, o bloco de instruções sob a cláusula então será executado; caso contrário ( for falsa), encerra-se a seleção (fimse). Neste caso, sem executar nenhuma instrução. Na Figura a seguir, podemos observar o diagrama da sintaxe desse tipo de desvio:

Apresentar o Diagrama da sintaxe do desvio condicional simples
Diagrama da sintaxe do desvio condicional simples
Fonte: FORBELLONE, A. L. V; EBERSPACHER, H. F. Lógica de Programação: a construção de algoritmos e estruturas de dados (3a. edição). São Paulo: Prentice Hall, 2005.
Exemplo 1
No exemplo a seguir, é feita a leitura de dois valores numéricos inteiros, denominados A e B. Em seguida, é efetuada a adição entre eles e o resultado dessa operação só é exibido caso seu valor seja maior que 10.

algoritmo MostraSoma_MaiorQueDez
var
  A, B, X : inteiro
inicio
 
  escreva "Digite dois numeros inteiros"
  leia A, B
  X <- A + B
 
  se X > 10 entao
       escreva "Valor de X=", X   
  fimse
 
fim
Pela animação a seguir, é possível observar a execução passo a passo do algoritmo.

Apresentar a Execução passo a passo do Exemplo 1 - Desvio Condicional Simples
Execução passo a passo do Exemplo 1 - Desvio Condicional Simples
Fonte:
Exemplo 2
No exemplo a seguir, é feita a leitura do salário de um funcionário. Em seguida, caso o salário informado seja menor ou igual a 2000, então é feito o acréscimo de 30% sobre seu valor. Por fim, o novo salário é exibido.

algoritmo Acrescimo_Salario
var
  salario, novo_salario : real
inicio
 
  escreva "Digite o salario do funcionario"
  leia salario
 
  se salario <= 2000 entao
       novo_salario <- salario * 1.30   
  fimse
 
  escreva "Novo salario=", novo_salario
 
fim
