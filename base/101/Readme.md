## @101 #04_vet L2 - Mostrar mão de cartas (Imprimir vetor formatado)
## @qxcode

![](capa.jpg)

## Ação

Leia um vetor contendo uma mão de cartas e mostre as cartas para o usuário.

As cartas estão codificadas da seguinte forma. O 1 vale A, os valores 11, 12 e 13 valem respectivamente J, Q e K.

### Entrada
- 1ª linha: 'N' quantidade de cartas na mão
- 2ª linha: 'N' valores representando as cartas do usuário.
### Saída
- Vetor formatado entre [ ], separados por ' , '.

## Exemplos

```
>>>>>>>>
0
========
[]
<<<<<<<<

>>>>>>>>
11
1 2 3 4 5 6 7 8 9 10 11 12 13
========
[A, 2, 3, 4, 5, 6, 7, 8, 9, 10, J]
<<<<<<<<

>>>>>>>>
4
1 1 3 13
========
[A, A, 3, K]
<<<<<<<<

>>>>>>>>
6
1 12 13 1 1 10
========
[A, Q, K, A, A, 10]
<<<<<<<<

>>>>>>>>
6
10 10 2 2 11 1
========
[10, 10, 2, 2, J, A]
<<<<<<<<
```

#