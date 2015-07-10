MAC 0329 - Algebra Booleana e Aplicacoes
EP3 - 2015

-------------------------------------------
integrantes:                n.USP:

Antonio Augusto Abello      8536152
Leonardo Daneu Lopes        8516816
Lucas Sung Jun Hong         8124329
William Shinji Numada       7648325
-------------------------------------------
TÓPICOS:

00 - Como usar?
01 - Lista de instrução "StoH"
02 - O que é esperado com a aplicação do "StoH"
03 - Lista de instrução "Factorial"
04 - O que é esperado com a aplicação do "Factorial"







00 - Como usar?
===============

* No arquivo "ep3.circ" em 'main', temos a memória RAM:
    >   Para inserir a instrução desejada, no teclado, faça CTRL+1 para ativar o botão
        que troca valores nos circuitos ("Change values within circuit (CTRL+1)");
    >   Selecione assim o endereço desejado e teremos um destaque em vermelho;
    >   Feito isso, no teclado, digite a instrução desejada.
    >   Para seguir para próximo endereço, aperte a barra de espaço do teclado;

*  Em 'main', temos o circuito 'CONTROLADOR':
    >   Teremos uma caixa chamada "ENTRADA". Insira um número inteiro X em binário que desejar.

* Inserido todas as instruções, aperte o botão "CLOCK", que se encontra ao lado do botão "RESET",
  para dar início a um clock, ou faça CTRL+T no teclado.

dicas:
------
* Para rodar o mesmo ciclo de instrução novamente, basta apertar o "RESET";
* Para apagar o ciclo e zerar todos os endereços, clique no botão abaixo do RAM, chamado "clr".


01 - Lista de instrução "StoH"
==================================

Temos a seguinte lista de instruções:
(ATENÇÃO: Usaremos o arquivo "StoH" como referência.)

------------+----------
endereço    | instrução
------------+----------
00          | 1f0c
------------+----------
01          | 0b0c
------------+----------
02          | 3407
------------+----------
03          | 180d
------------+----------
04          | 3407
------------+----------
05          | 0c0e
------------+----------
06          | 290e
------------+----------
07          | 4600
------------+----------

.
.
.

------------+----------
0c          | 0000
------------+----------
0d          | 0e10
------------+----------
0e          | 0000
------------+----------


02 - O que é esperado com a aplicação do "StoH"
===================================================

    A lista de instruções do 'StoH' corresponde a um pequeno algoritmo
que recebe como entrada um numero X inteiro em SEGUNDOS e imprime em "SAIDA"
X em HORAS. Ou seja, é um conversor de segundos para horas.

    Caso X <= 0, o programa imprime 0 horas como saída. Caso contrário,
divide X por 3600 (decimal) e verifica novamente se H > 0, em que H = X / 3600.
Caso sim, o programa imprime H. Caso contrário, imprime 0.



03 - Lista de instrução "Factorial"
==================================

Temos a seguinte lista de instruções:
(ATENÇÃO: Usaremos o arquivo "Factorial" como referência.)

------------+----------
endereço    | instrução
------------+----------
00          | 1f07
------------+----------
01          | 0b07
------------+----------
02          | 3609
------------+----------
03          | 3705
------------+----------
04          | 4600
------------+----------
05          | 2908
------------+----------
06          | 4600
------------+----------
07          | 0000
------------+----------
08          | 0001
------------+----------
09          | 1608
------------+----------
0a          | 0c0b
------------+----------
0b          | 0000
------------+----------
0c          | 0b07
------------+----------
0d          | 170b
------------+----------
0e          | 3610
------------+----------
0f          | 4600
------------+----------
10          | 0c07
------------+----------
11          | 0b0b
------------+----------
12          | 2907
------------+----------
13          | 3302
------------+----------


04 - O que é esperado com a aplicação do "Factorial"
===================================================

    A lista de instruções do 'Factorial' corresponde à função fatorial.

    Dado um X, calcula-se X! e imprime-se o resultado em SAIDA.

    Se X = 0, imprime 1. Se X < 0, imprime 0.