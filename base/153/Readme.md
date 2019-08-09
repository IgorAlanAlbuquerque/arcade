## @153 #06_mat L3 - OBI 2015 - Fase 2 - Nível 1 - Torre
## @qxcode
![](capa.png)

## Motivação

Dada uma matriz quadrada M de números naturais, o índice i de uma certa linha e o índice j de uma certa coluna, vamos definir o peso do cruzamento da linha i com a coluna j, como sendo a soma de todos os elementos que estejam na linha i ou na coluna j, mas não nas duas. Quer dizer, excluindo o elemento que está exatamente no cruzamento! Neste problema, você deve descobrir qual é o peso mínimo entre todos os possíveis cruzamentos da matriz!

No jogo de xadrez, a torre é uma peça que pode se mover para qualquer outra posição do tabuleiro na linha ou na coluna da posição que ela ocupa. O professor Paulo está tentando inventar um novo tipo de jogo de xadrez onde todas as peças são torres, o tabuleiro também é quadrado mas pode ter qualquer dimensão e cada posição do tabuleiro é anotada com um número inteiro positivo, como na figura abaixo.

Ele definiu o peso de uma posição (i,j) como sendo a soma de todos os números que estejam na linha i com todos os números da coluna j, mas sem somar o número que está exatamente na posição (i,j). Quer dizer, se uma torre estiver na posição (i,j), o peso da posição é a soma de todas as posições que essa torre poderia atacar.

O professor Paulo está solicitando a sua ajuda para implementar um programa que determine qual é o peso máximo entre todas as posições do tabuleiro.

No exemplo da figura acima, com um tabuleiro de dimensão seis (ou seja, seis linhas por seis colunas), o peso máximo é 67, referente à posição (4,4).

### Entrada

- A primeira linha da entrada contém um inteiro N, representando a dimensão do tabuleiro.

- Cada uma das N linhas seguintes contém N inteiros positivos X\_i, definindo os números em cada posição do tabuleiro.

### Saída

Seu programa deve produzir uma única linha, contendo um único inteiro, o peso máximo entre todas as posições do tabuleiro.

## Restrições

*   3 ≤ N ≤ 1000
*   0 < X\_i ≤ 100

## Informações sobre a pontuação

*   Em um conjunto de casos de teste cuja soma é 60 pontos, N ≤ 300.

## Exemplos

```
>>>>>>>>
6
4 1 3 8 4 5
9 2 8 9 2 7
5 5 4 3 2 5
8 2 9 1 9 8
7 1 3 2 1 2
5 1 2 9 3 8
========
67
<<<<<<<<

>>>>>>>>
3
5 1 1
5 2 1
8 5 5
========
20
<<<<<<<<
```

#

<!---
>>>>>>>> 0
10
97 98 4 18 54 71 43 16 77 33
96 62 53 23 70 66 18 55 16 87
26 65 47 85 49 31 80 66 34 86
26 15 24 8 96 12 6 69 69 60
33 10 52 6 63 20 19 56 75 80
3 69 85 89 6 50 38 51 67 16
36 76 50 43 60 75 89 16 1 1
32 24 96 14 20 19 78 94 23 69
36 48 46 67 91 5 97 64 56 74
83 88 100 23 79 57 55 45 12 57
========
1060
<<<<<<<<


>>>>>>>> 02
10
67 54 10 76 43 73 13 30 38 47
50 37 50 41 61 88 28 41 27 56
5 43 20 47 10 16 78 75 22 29
52 74 72 82 2 60 49 34 73 3
97 72 65 39 81 34 84 79 57 63
32 90 72 42 79 33 82 73 76 79
30 38 75 52 8 1 78 70 37 41
13 15 27 3 70 42 86 75 91 84
64 50 16 24 89 67 63 4 72 18
92 80 51 30 62 61 44 14 95 2
========
1145
<<<<<<<<


>>>>>>>> 03
10
25 93 61 91 24 65 38 22 93 57
9 93 22 3 70 14 65 9 63 80
94 81 44 11 73 91 90 100 66 42
16 67 70 65 33 5 29 84 10 12
73 44 17 14 93 23 67 44 44 11
76 66 64 81 4 78 34 14 85 82
42 81 84 63 10 70 78 51 94 92
24 6 88 43 20 35 3 73 55 68
66 65 60 47 81 96 51 78 40 69
13 61 2 38 15 88 30 61 43 77
========
1198
<<<<<<<<


>>>>>>>> 04
10
79 23 66 79 35 2 22 68 56 27
63 84 28 15 17 55 94 94 83 17
85 81 99 31 12 95 64 4 12 21
20 90 65 29 92 75 7 65 9 44
73 82 53 38 69 65 45 18 63 58
85 55 91 94 54 77 14 30 38 86
52 54 57 93 12 98 84 29 83 82
99 1 78 21 16 90 48 23 76 39
5 95 27 55 44 100 83 83 62 66
42 65 67 28 11 16 62 90 15 65
========
1213
<<<<<<<<


>>>>>>>> 05
10
100 100 100 100 100 100 100 100 100 100
100 73 30 32 37 75 60 60 42 26
100 97 84 42 87 89 96 19 37 91
100 12 10 73 96 53 52 90 71 20
100 87 92 48 11 79 31 32 85 9
100 67 6 91 58 24 14 22 66 79
100 71 83 55 10 24 55 71 58 93
100 3 84 49 84 78 27 51 44 71
100 18 52 50 24 42 19 64 100 13
100 48 44 40 74 91 42 9 53 52
========
1800
<<<<<<<<


>>>>>>>> 06
10
76 60 29 12 14 98 11 14 86 100
96 18 72 71 10 83 89 69 18 100
16 60 57 100 13 41 35 45 30 100
45 32 89 54 99 47 45 19 36 100
14 50 95 18 91 50 73 82 99 100
92 42 65 89 39 42 88 83 9 100
61 45 6 16 14 58 62 1 95 100
41 52 56 83 46 91 5 76 63 100
65 85 13 9 18 13 14 62 47 100
100 100 100 100 100 100 100 100 100 100
========
1800
<<<<<<<<


>>>>>>>> 07
10
100 100 100 100 100 100 100 100 100 100
100 75 60 82 9 93 47 24 1 48
100 82 24 61 67 84 22 2 12 84
100 100 93 83 85 52 99 82 40 8
100 2 23 28 23 62 39 13 48 54
100 49 57 23 61 94 55 34 61 52
100 25 72 98 75 34 49 38 57 66
100 39 98 27 35 2 17 69 4 96
100 43 45 73 63 74 33 79 86 83
100 38 82 43 75 58 47 97 11 66
========
1800
<<<<<<<<


>>>>>>>> 08
10
46 69 11 82 88 72 10 53 90 100
18 34 18 14 62 96 87 64 83 100
42 95 97 52 69 99 76 20 5 100
18 100 7 74 38 94 11 6 95 100
17 30 90 97 7 56 25 45 48 100
45 41 71 99 36 37 93 87 76 100
20 57 51 83 68 56 99 82 17 100
20 18 86 2 74 93 80 50 97 100
77 29 3 41 38 91 13 28 38 100
100 100 100 100 100 100 100 100 100 100
========
1800
<<<<<<<<
--->