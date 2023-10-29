Introdução
Os desvios condicionais, também chamados de estruturas de seleção ou decisão, são utilizados quando existe a necessidade de verificar condições para a realização de uma instrução ou de uma sequência de instruções. Os testes de seleção também podem ser utilizados para verificar opções de escolha. A tomada de decisão sempre deve estar de acordo com o resultado de uma expressão lógica.

Existem quatro tipos de desvios condicionais: simples, composto, encadeado e o de múltipla escolha. Neste tópico serão abordados conceitos sobre o desvio condicional com múltipla escolha.

 

Desvio Condicional com Múltipla Escolha
Um desvio condicional com múltipla escolha ou estrutura de selsção de múltipla escolha é uma estrutura de seleção que funciona como um conjunto de opções para escolha. Este tipo de desvio deve ser utilizado quando houver a necessidade de construir um programa no qual seja necessário utilizar uma seqüência grande de instruções do tipo se.

Em Português Estruturado, a instrução para o desvio condicional com múltipla escolha deve seguir o seguinte modelo:

escolha <variavel>
 
    caso <valor1>: 
       instruções 
    caso <valor2>:
       instruções
    ...
    caso contrario:
       instruções
 
fimescolha 
Exemplo 1
No exemplo a seguir, é feita a leitura do código de um produto conforme a tabela. A partir da escolha do código, é feita a exibição do nome do produto.

 

Código do Produto	Nome do produto
001	Caderno
002	Lápis
003	Borracha
algoritmo Escolha_Produtos
var codigo: inteiro
inicio
        leia codigo
        escolha codigo
            caso 001: 
                escreva "O produto eh caderno"
            caso 002: 
                escreva "O produto eh lapis"
            caso 003: 
                escreva "O produto eh borracha"
            caso contrario:
                escreva "Diversos"
         fimescolha 
fim
Pela animação a seguir, é possível observar a execução do algoritmo passo a passo (linha por linha).

Apresentar a Simulação da execução do desvio condicional com múltipla escolha - Exemplo 1
Simulação da execução do desvio condicional com múltipla escolha - Exemplo 1
Exemplo 2
No exemplo a seguir, é feita a leitura do código de origem e do preço de um determinado produto. A partir da escolha do código, é feita a exibição do preço junto com sua procedência de acordo com a tabela. Caso o código não seja nenhum dos especificados, o produto deve ser encarado como importado.

Neste exemplo é possível observar que algumas procedências (Nordeste, Sudeste, Centro-Oeste e Nordeste) possuem vários códigos de origem.

 

Código de Origem	Procedência
1	Sul
2	Norte
3	Leste
4	Oeste
5 ou 6	Nordeste
7, 8 ou 9	Sudeste
10 até 20	Centro-Oeste
 

algoritmo Escolha_Produto_Procedencia
var codigo: inteiro
      preco: real
inicio
        leia codigo, preco
        escolha codigo
            caso 1: 
                escreva "Produto do Sul - preco=", preco
            caso 2: 
                escreva "Produto do Norte - preco=", preco
            caso 3: 
                escreva "Produto do Leste - preco=", preco
            caso 4: 
                escreva "Produto do Oeste - preco=", preco
            caso 5, 6: 
                escreva "Produto do Nordeste - preco=", preco
            caso 7, 8, 9: 
                escreva "Produto do Sudeste - preco=", preco
            caso 10..20: 
                escreva "Produto do Centro-Oeste - preco=", preco
            caso contrario:
                escreva "Produto Importado - preco=", preco
         fimescolha 
fim
Pela animação a seguir, é possível observar a execução do algoritmo passo a passo (linha por linha).

Apresentar a Simulação da execução do desvio condicional com múltipla escolha - Exemplo 2
Simulação da execução do desvio condicional com múltipla escolha - Exemplo 2
