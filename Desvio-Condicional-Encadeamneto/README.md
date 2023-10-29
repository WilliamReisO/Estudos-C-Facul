

     
Introdução
Os desvios condicionais, também chamados de estruturas de seleção ou decisão, são utilizados quando existe a necessidade de verificar condições para a realização de uma instrução ou de uma sequência de instruções. Os testes de seleção também podem ser utilizados para verificar opções de escolha. A tomada de decisão sempre deve estar de acordo com o resultado de uma expressão lógica.

Existem quatro tipos de desvios condicionais: simples, composto, encadeado e o de múltipla escolha. Neste tópico serão abordados conceitos sobre o desvio condicional encadeado.

 

Desvio Condicional Encadeado
Quando, devido à necessidade de processamento, agruparmos vários desvios, formamos um desvio encadeado. Um desvio condicional encadeado é uma seuquência de testes de seleção, os quais serão executados ou não de acordo com o resultado das condições e de acordo com o encadeamento dos testes. Normalmente, tal formação ocorre quando uma determinada ação ou bloco deve ser execiutado se um grande conjunto de possibilidades ou combinações de situações for satisfeito.

Em Português Estruturado, a instrução para o desvio condicional encadeado deve seguir o seguinte modelo:

 

se <condicao1> entao
     instruções para condicao1 verdadeira
senao
     se <condicao2> entao
          instruções para condicao2 verdadeira, porém condicao1 falsa
     senao
         instruções para condicao1 e condição2 falsa
  fimse
fimse
Exemplo 1
Neste exemplo é efetuado o cálculo do reajuste do salário de um funcionário. Considere que o funcionário deve receber um reajuste de 15% caso seu salário seja menor que 500. Se o salário for maior ou igual a 500, mas menor ou igual a 1000, seu reajuste será de 10%; caso seja ainda maior que 1000, o reajuste deverá ser de 5%. No final do algoritmo, o valor do novo salário é exibido.

algoritmo ReajustaSalario
var
  salario: real
  novoSalario: real
inicio
  escreva "Salario: "
  leia salario
  se salario < 500 entao
       novoSalario <- salario * 1.15
  senao
       se salario <= 1000 entao
            novoSalario <- salario * 1.10
      senao
           novoSalario <- salario * 1.05
    fimse
  fimse
  escreva "Novo salario = ", novoSalario
fim
Pela animação a seguir, é possível observar a execução do algoritmo passo a passo (linha por linha).

Apresentar a Simulação da execução do desvio condicional encadeado - Exemplo 1
Simulação da execução do desvio condicional encadeado - Exemplo 1
Exemplo 2
Neste exemplo é feita uma operação sobre um número inteiro de acordo com o seu sinal (positivo, negativo ou igual a zero). Caso o número seja positivo, será adicionado 5 ao seu valor; se ele for negativo, será multiplicado 7 ao seu valor e, caso seja igual a zero, será subtraído 3 ao seu valor. Por fim, o número inteiro atualizado será exibido.

algoritmo AtualizaNumero
var num: inteiro
inicio
  escreva "Digite um numero inteiro: "
  leia num
  se num > 0 entao
       num <- num + 5
  senao
       se num < 0 entao
            num <- num * 7
      senao
           num <- num -3
    fimse
  fimse
  escreva "Novo numero = ", num
fim
Pela animação a seguir, é possível observar a execução do algoritmo passo a passo (linha por linha).

Apresentar a Simulação da execução do desvio condicional encadeado - Exemplo 2
Simulação da execução do desvio condicional encadeado - Exemplo 2