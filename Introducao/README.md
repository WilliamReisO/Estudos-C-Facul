Introdução
A linguagem de programação, como qualquer linguagem, é formada por palavras. Essas palavras são agrupadas em frases para produzir um determinado significado. Dessa forma, pode-se chamar as palavras de uma linguagem de programaçnao de palavras-chave e as frases criadas com essas palavras de estruturas de programação.

Assim, um programa é constituído de palavras-chave e estruturas de programação definidas segundo as regras dessa linguagem, elaboradas de modo que sejam mais facilmente compreendidas pelo ser humano. A exemplo da linguagem usada em nossa comunicação no dia-a-dia, a linguagem de programação possui uma sintaxe, definida por essas regras.

A linguagem C foi, primeiramente, criada por Dennis M. Ritchie e Ken Thompson no laboratório Bell em 1972. É uma linguagem estruturada utilizada até pouco tempo para o desenvolvimento de aplicações comerciais. Ultimamente, tem grande aplicação no desenvolvimento de software básico e aplicações com forte interação com o hardware. Podemos citar como exemplo o sistema operacional UNIX, que é desenvolvido em C. Além disso, as linguagens Java e C# foram concebidas a partir da linguagem C.

A linguagem C foi desenhada para que o usuário possa planejar programas estruturados e modulares. Assim, o resultado é um programa mais legível e documentado. Além disso, os programas em C tendem a ser bastante compactos e de execução rápida.

Para que um computador possa "entender" um programa escrito em uma linguagem de alto nível, torna-se necessário um meio de tradução entre a linguagem utilizada no programa e a linguagem de máquina. Este meio pode ser de dois tipos: compilador e interpretador.

Compiladores e interpretadores são responsáveis por traduzir os programas que estão nas diferentes linguagens de programação para a linguagem que a máquina entende.

O Interpretador faz a análise sintática (verifica se o programa fonte está escrito de acordo com a gramática definida pela linguagem) e a análise semântica (verifica, por exemplo, uma multiplicação entre tipos de dados diferentes). Ele traduz e envia para execução, instrução por instrução e o programa permanece na forma fonte. Como exemplo de linguagem interpretada podemos citar a linguagem HTML. Na Figura a seguir podemos observar o esquema de um interpretador.

Apresentar o Esquema de um Interpretador
Esquema de um Interpretador
 O Compilador, tal como o interpretador, faz a análise sintática e semântica do programa fonte. O compilador lê o arquivo contendo o programa escrito em uma dada linguagem de programação e gera um programa em linguagem de máquina que seja equivalente ao programa inicial de tal forma que o computador o entenda. O programa final é colocado num formato compatível com as necessidades do sistema operacional (programa executável) para carregá-lo em memória e colocá-lo em execução. Como exemplo de linguagem compilada podemos citar a linguagem C. Na Figura a seguir podemos observar o esquema de um compilador.

Apresentar o Esquema de um Compilador
Esquema de um Compilador
Criação de um Programa em Linguagem C
A criação de um programa em linguagem C segue basicamente três passos:

Criação do programa fonte (texto).
Compilação desse programa, para a sua tradução em código executável.
Execução do código produzido.
 
Estrutura básica de um programa em C
Um programa C consiste em uma ou várias "funções", uma das quais precisa ser denominada main. O programa sempre começará executando a função main. Definições de funções adicionais podem preceder ou suceder a função main. A forma geral da função main é a seguinte:

main (){
 
//instrucoes
 
}
Algumas regras devem ser seguidas para a definição de uma função em C. São elas:

Toda função em C (inclusive a main) deve ser iniciada por uma chave e abertura: {e encerrada por uma chave de fechamento: } .
Toda função é procedida de parênteses ( ).
Todo programa deverá conter a função main (é uma palavra reservada).
As instruções em C são sempre encerradas por um ponto-e-vírgula (;).
A formatação dos programas é absolutamente livre, mas temos por conveniência, manter a legibilidade.
Os comandos são executados na ordem em que foram escritos.
Os comentários devem ser delimitados por /* no início e */ no final e podem ocupar desde algumas colunas entre as instruções a até várias linhas. Pode ser usando também os caracteres // para comentários de uma linha. 
 

O Pré-processador C
O pré-processador C é um programa que examina o programa-fonte em C e executa certas modificações nele, baseado em instruções chamadas diretivas.

O pré-processador faz parte do compilador e pode ser considerado uma linguagem dentro da linguagem C. Ele é executado automaticamente antes da compilação. Diretivas do pré-processador seriam instruções desta linguagem.

Instruções para o pré-processador devem fazer parte do texto que criamos, mas não farão parte do programa que compilamos, pois são retiradas do texto pelo compilador antes da compilação.

Todas a diretivas do pré-processador são iniciadas com o símbolo (#). As diretivas podem ser colocadas em qualquer parte do programa, mas é costume serem colocadas no início do programa, antes de main(), ou antes do  começo de uma função particular.

Não há ponto-e-vírgula após qualquer diretiva do pré-processador.

 

A diretiva include#
A diretiva #include causa a inclusão de um programa-fonte em outro. Ela diz ao compilador para incluir, na hora da compilação, um arquivo especificado.

Sua forma geral é:

#include "nome_do_arquivo" ou #include <nome_do_arquivo>
A diferença entre usar “ ” e < > é somente a ordem de procura nos diretórios pelo arquivo especificado. Se o arquivo estiver nos caminhos de procura pré-especificados do compilador (como é o caso do arquivo stdio.h) use < >.

 

Principais bibliotecas da linguagem C
Na Tabela abaixo é possível observar as principais bibliotecas utilizadas na linguagem C.

 

Nome da biblioteca	Uso geral
stdio.h	standard input output - entrada e saída padrão
stdlib.h	standard library - diversas utilidades
conio.h	console input output - uso de teclado e monitor
ctype.h	character type - manuseio de caracteres
math.h	mathematics - operações matemáticas
string.h	strings - manuseio de strings
 

Biblioteca stdio.h 

Esta biblioteca é a responsável pela entrada e saída padrão (standard input output). Nela, encontramos funções para estes fins. O que pode ser a leitura do teclado, escrita formatada ou não na tela e operações com arquivos.

Algumas funções dessas bibliotecas: fprintf, printf, fscanf, scanf, getchar, putc, getc, fopen, fclose, dentre outras.
 

Biblioteca stdlib.h 

Esta biblioteca é a responsável por conversões de números, alocação na memória e outras tarefas. Com ela podemos: Converter um char em um double, converter um char para long, criar um número randômico, alocar na memória, realocar na memória, desalocar da memória , execução de comandos do sistema operacional. Respectivamente, as funções citadas são: atof, atol, rand, malloc, realloc, free e system, dentre outras. Também não podia deixar de citar que ela retorna o valor absoluto de um número inteiro usando abs.

 

Biblioteca conio.h 

A biblioteca conio.h não é uma biblioteca padrão ANSI, e com isso não está presente em outros Sistemas Operacionais. Responsável pelo console input output (uso de teclado e monitor). É útil para manipular caracteres na tela, especificar cor de caracter e de fundo.

Algumas funções dessas bibliotecas: getch, getche, textcolor, textbackground, cprintf, dentre outras.

 

Biblioteca ctype.h 

Esta biblioteca serve para - manuseio de caracteres. Alguns testes possíveis com caracteres são: testar se é maiúsculo, testar se é minúsculo, testar se é espaço, testar dígito decimal. Além disso, essa biblioteca permite converter maiúscula em minúscula e vice-versa.

Algumas funções: isupper, islower, isspace, isdigit, toupper, tolower, dentre outras.

 

Biblioteca math.h 

Está biblioteca declara funções matemáticas que podem servir para: achar a raiz quadrada, achar o seno, co-seno, tangente, logaritmo na base 10. As funções referentes a isso são: sqrt, sin, cos, tan, log10. Fora isso, um outro uso para declaração desta biblioteca é a possibilidade de arredondar um número. Para isso, usamos a função que retorna o valor absoluto: fabs.

 

Biblioteca string.h 

A biblioteca string é responsável por disponibilizar funções para trabalhar com conjuntos de caracteres, isto é, strings. Este header possui dois grupos de comandos, os que começam com str e os que começam com mem.

O primeiro grupo permite, por exemplo: copiar, concatenar, comparar e ver o tamanho de uma string.

As funções referentes a isso são: strcpy, strcat, strcmp e strlen.

As funções do segundo grupo mencionado fazem coisas semelhantes como copiar, mover e comparar: memcpy, memmove, memcmp. 

 

Estrutura de um programa
A estrutura de um programa em C que iremos utilizar nos primeiros exemplos é a seguinte:

#include <stdio.h>
#include <stdlib.h> 
 
main()                     
{                              
 
     //**********Dados de entrada
 
     //*********Processamento - cálculo
      
     //******** Dados de saída
 
     system("pause"); //pausa
}
Variáveis em C
As variáveis são o aspecto fundamental de qualquer linguagem de computador. Uma variável em C é um espaço de memória reservado para armazenar um certo tipo de dado e tendo um nome para referenciar o seu conteúdo. Uma variável é um espaço de memória que pode conter, a cada tempo, valores diferentes.

Algumas regras devem ser seguidas para a definição de variáveis em C. São elas:

Em C, todas variáveis utilizadas no programa devem ser declaradas previamente.
A declaração indica, no mínimo, o nome e o tipo de cada uma delas.
Na ocorrência de mais de uma variável do mesmo tipo, podemos declará-Ias de uma única vez, separando seus nomes por vírgula.
As letras minúsculas são diferenciadas das respectivas maiúsculas.
O tamanho máximo significante para uma variável é de 31 posições.
Todo nome de variável é iniciado por uma letra (a a z ou A a Z), ou o caractere underline (_), sendo o restante podendo conter letras, underline ou números.
As palavras reservadas, descritas a seguir não podem ser usadas como nome de variável.
 

auto	break	else	enum	extern	register	typedef
do	double	int	long	main	switch	public
goto	if	sizeof	static	struct	class	 
short	signed	void	volatile	while	default	 
union	unsigned	virtual	protected	continue	for	 
private	case	char	const	float	return	 
 

O tipo de uma variável informa a quantidade de memória, em bytes, que esta irá ocupar e a forma como o seu conteúdo será armazenado. Na tabela a seguir é possível observar os tipos de dados mais utilizados em C.

 

Tipo	Bits	Escala
void	0	sem valor
char	8	-128 a 127
int	16	-32768 a 32768
float	32	3.4E-38 a 3.4E+38
double	64	1.7E-308 a 1.7E+308
long int	32	3.4E-38 a 3.4E+38
unsigned char	8	0 a 255
unsigned int	16	0 a 65533
 

Uma declaração de variável é uma instrução para reservar uma quantidade de memória apropriada para armazenar o tipo especificado. A forma de declaração de variáveis é a seguinte:

tipo <nome_variavel>;
Alguns exemplos de declarações de variáveis podem ser observados na Tabela a seguir.

 

Pseudocódigo	C	Exemplos
Inteiro	int	int numInt;
Real	float	float numReal;
Caractere	char	char letra;
Lógico	Não possui	int achou; // Utilizar o valor uma variável int, onde 0 = falso e 1= verdadeiro
 

Observações:

Em C todas as variáveis devem ser declaradas.
Se você tiver mais de uma variável do mesmo tipo, poderá declará-las de uma única vez, separando seus nomes por  vírgulas. Exemplo: int num1, num2, num3;
 

É possível combinar uma declaração de variável com o operador de atribuição para que a variável tenha um valor ao mesmo tempo de sua declaração; é o que chamaremos de inicialização de variáveis. Eis alguns exemplos de inicialização de variáveis:

 

int numInt = 15;
 
float cotacao = 3.40;
 
char letra = 'D';
Algumas regras devem ser seguidas para a inicialização de variáveis:

As variáveis deverão ser declaradas antes de qualquer instrução.
As variáveis do tipo caracter deverão receber valores entre aspas simples (').
Em C, não existe o tipo booleano nem o tipo string.
O Valor zero (0) representa um valor falso em C, os demais valores (1 ,'a','z',-1 ,-0.7) são considerados verdadeiros.
 

Em C também é possível atribuir o mesmo valor a muitas variáveis, usando atribuições múltiplas em um único comando, como é mostrado no exemplo a seguir.

int x, y, z;
 
x = y = z = 10;
Função de Saída de Dados em C
A função printf() é uma das funções de E/S (entrada e saída) que pode ser usada em C. Ela não faz parte da definição de C, mas todos os sistemas têm uma versão de printf() implementada. Esta função é utilizada para imprimir dados na tela do computador, sendo os dados a serem impressos passados como argumentos da função printf(). Ela pertence a uma biblioteca padrão do C (stdio.h). Para utilizar a  função printf() a biblioteca stdio.h deve ser incluída com a diretiva #include.

A função printf() pode ter um ou mais argumentos. A expressão de controle pode conter caracteres que serão exibidos na tela e códigos de formatação que indicam o formato que os argumentos devem ser impressos. Sua sintaxe (maneira de escrever) é a seguinte:

printf("expr. controle", lista de argumentos); 
A expressão de controle pode conter caracteres que serão exibidos na tela e códigos de formatação que indicam o formato em que os argumentos devem ser impressos e caracteres especiais de impressão, os quais podem ser observados nas Tabelas a seguir. 

 

Código	Formato
%d	Um número inteiro decimal (int)
%c	Um caracter (char)
%f	Ponto flutuante decimal (float)
%s	String
%i	O mesmo que %d
%e	Número em notação científica com o "e"minúsculo
%o	Número octal
%u	Decimal "unsigned" (sem sinal)
%x	Hexadecimal com letras minúsculas
%l	Inteiro longo (long int)
 

Caractere especial de impressão	Significado
\n	Nova linha ("new line")
\a	Sinal sonoro ("beep")
\b	Retrocesso ("back")
\t	Tabulação horizontal ("tab")
\r	Retorno do cursor
\"	Aspas duplas
%%	Imprimir o sinal %
 

No exemplo a seguir, podemos observar a utilização da função printf() para imprimir na tela uma mensagem de texto e um valor, o qual deve ser formatado. O código de formatação %d solicita a função printf() imprimir o segundo argumento em formato decimal.

#include <stdio.h>
#include <stdlib.h>
 
main () {
 
      printf ("Este eh o numero dois: %d", 2);  
      system ("PAUSE");
 
}
Neste outro exemplo, a expressão de controle contém apenas os caracteres que devem ser impressos na tela e um caractere especial de impressão  (“\n”) que indica ao programa para colocar o cursor na próxima linha. Quando não temos nenhum código de formatação na expressão de controle,  não deve ser passado nenhum outro argumento para a função printf().

#include <stdio.h>
#include <stdlib.h>
 
main () {
 
  printf ("Ola Mundo! \n");
  system ("PAUSE");
 
}
Quando queremos somente imprimir os valores de variáveis, devemos utilizar os códigos de formatação necessários. No exemplo a seguir, foram utilizados os códigos de formatação %d e %f para imprimir, respectivamente, um número inteiro e um número real.

#include <stdio.h>
#include <stdlib.h>
 
main () {
 
  int numInt = 10;
  float numReal = 15.25;
  printf ("%d %f", numInt, numReal);
 
  system ("PAUSE"); 
 
}
Juntamente com os códigos de formatação, modificadores de formato também podem ser utilizados. Modificadores de formato incluem o Especificador de Largura Mínima de Campo e o Especificador de Precisão.

Um número colocado entre o símbolo % e o código de formato age como um especificador de largura mínima de campo. Isso preenche a saída com espaços, para assegurar que ela atinja um certo comprimento mínimo. Para preencher com 0s, deve-se colocar um 0 antes do especificador de largura mínima de campo. Por exemplo, %05d preencherá um número de menos de cinco dígitos com 0s de forma que seu comprimento total seja cinco.

O especificador de precisão segue o especificador de largura mínima de um campo (se houver algum), consistindo em um ponto seguido de um número inteiro. O seu significado exato depende do tipo de dado a que está sendo aplicado.

No exemplo a seguir, foram utilizados os modificadores de formato. 

#include <stdio.h>
#include <stdlib.h>
 
main () {
 
	printf ("%.4f\n", 123.1234567);
	printf ("%6.4d\n", 21);
	printf ("%6.0d\n", 21);
	printf ("%.15s\n", "Este e um teste simples");
        
        system ("PAUSE");
}
Função de Entrada de Dados em C
A função scanf() é outra das funções de E/S implementada em todos os compiladores C. Ela é o complemento de printf() e nos permite ler dados formatados da entrada padrão (teclado). Sua sintaxe é similar à de printf(), isto é, uma expressão de controle seguida por uma lista de argumentos separados por vírgula. scanf() é uma função da biblioteca padrão do C (stdio.h). Para utilizar a  função scanf() a biblioteca stdio.h deve ser incluída com a diretiva #include.

A expressão de controle pode conter códigos de formatação precedidos por um sinal %. A lista de argumentos deve consistir nos endereços das variáveis. C oferece um operador para tipos básicos chamado operador de endereço e referendado pelo símbolo & que retoma o endereço do operando. Sua sintaxe (maneira de escrever) é a seguinte:

scanf ("expr. de controle", lista de argumentos);
No exemplo a seguir é mostrada a utilização da função scanf(). A leitura da variável anos será feita via teclado pela scanf().

#include <stdio.h>
#include <stdlib.h>
 
main () {
 
	float anos, dias;
	printf ("Digite sua idade em anos: ");
	scanf ("%f", &anos);
	dias = anos * 365;
        printf ("Sua idade em dias e? %.0f.\n", dias);
 
        system ("PAUSE");
 
}
Toda variável ocupa uma certa localização na memória, e seu endereço é o do primeiro byte ocupado por ela. Um inteiro ocupa 2 bytes. Se você declarou uma variável n como inteira e atribui a ela o valor 2, quando n for referenciada devolverá 2. Entretanto, se você referenciar n precedido de & (&n) devolverá o endereço do primeiro byte onde n está guardada. No exemplo a seguir, será impresso na tela "Saída: Valor=2, endereco=1370". O valor 1370 atribuído ao endereço da variável é somente uma simulação do endereço de memória, pois este valor é gerado aleatoriamente pelo compilador no momento da execução do programa.

#include <stdio.h>
#include <stdlib.h>
 
main () {
 
	int num = 2;
	printf ("Valor=%d, endereco=%u", num, &num);
	
	system ("PAUSE");
 
}
Algoritmo (português estruturado) versus Programa em C
A seguir são apresentadas duas versões para a resolução do problema da Soma de dois números inteiros. Na primeira versão, o problema é resolvido por um algoritmo em Português Estruturado e, na segunda versão, sob a forma de um programa em C. 

algoritmo Soma_Numeros
var
     num1, num2, soma: inteiro
inicio
        escreva "Informe o primeiro numero:"
        leia num1
        escreva "Informe o segundo numero:"
        leia num2
        soma <- num1 + num2
        escreva "Soma: ", soma
fim
#include <stdio.h>
#include <stdlib.h>
 
main () {
 
	int num1, num2, soma;
 
	printf ("Digite o primeiro valor:");
        scanf ("%d", &num1);
        printf ("Digite o segundo valor:");
        scanf ("%d", &num2);
 
        soma = num1 + num2;
 
        printf ("Soma: %d", soma);
 
        system ("PAUSE");
 
}
As linhas 2 e 3, no Português Estruturado, correspondem à linha 6 no programa. Já as linhas 5, 6, 7 e 8, no Português Estruturado, correspondem às linhas 8, 9, 10 e 11 no programa. A linha 9, no Português Estruturado, corresponde à linha 13 no programa. E, finalmente, a linha 10, no Português Estruturado, corresponde à linha 15 no programa.

Na animação a seguir é possível observar as linhas de instrução equivalentes no algoritmo que soma dois números inteiros em Português Estruturado e no mesmo algoritmo escrito em Linguagem C.

Apresentar a Equivalência entre o algoritmo em Português Estruturado e o algoritmo em C
Equivalência entre o algoritmo em Português Estruturado e o algoritmo em C
Constantes em C
A diretiva #define pode ser usada para definir constantes simbólicas com nomes apropriados em C. A sintaxe para a utilização desta diretiva é a seguinte:

#define <nome_constante> <valor_constante>
Por convenção, o identificador (nome da constante) é escrito em letras maiúsculas. Só é permitido escrever um comando deste por linha. No exemplo a seguir é mostrada a definição da constante PI. Quando o compilador encontra #define, ele substitui cada ocorrência de PI por 3.1415.

#include <stdio.h>
#include <stdlib.h>
#define PI 3.1415
 
main () {
 
	float raio;
	printf ("Digite o valor do raio:");
        scanf ("%f", &raio);
	float area = PI * raio * raio;
	printf ("Area: %.2f", area);
 
	system ("PAUSE");
 
}
