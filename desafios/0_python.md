# Lista de Exécicios de Python

Essa lista visa exercitar os conhecimentos na linguem de programação Python.

## Problema 1

Crie  uma  função  que  converta  uma  temperatura  digitada  em  Celsius  para  Fahrenheit.

```console
user@computer:~$ python temperatura.py

Insira a temperatura em Fahrenheit: 12

12ºF, em Celsius equivalem 53ºC
```

## Problema 2

Faça um Programa que  peça os três ladosde um triângulo. O programa deverá informar se os  valores  podem  serum  triângulo.  Indique,  caso  os  lados  formem  um  triângulo,  se  o mesmo é: equilátero, isósceles ou escaleno

```console
user@computer:~$ python traingulos.py
Lado 1: 5
Lado 2: 6
Lado 3: 10

O triângulo e isósceles
```

## Problema 3

Um  funcionário  de uma  determinada  empresa,  ganha  uma  quantidade  X  de  reais  por  mês.  Faça um  Programa  que  pergunte  quanto  um  dos  funcionários  ganha  por  hora  e  o  número  de  horas trabalhadas no mês. Em seguida, calcule e mostre o total do seu salário no referido mês, sabendo-se que são descontados 11% para o Imposto de Renda, 8% para o INSS e 5% para o sindicato, faça um programa que nos dê o salário bruto, quanto pagou ao INSS, quanto pagou ao sindicato e o salário líquido.**Observe que Salário Bruto -Descontos = Salário Líquido**.

```console
user@computer:~$ python salario.py

Quantidade recebida por hora: 10
Horas trabalhadas no mes: 20

+ Salário Bruto : R$ 200.00
-IR: R$ 22.00
-INSS: R$ 16.00
-Sindicato: R$ 10.00
= Salário Liquido: R$ 152.00
```

## Problema 4

A seqüência de Fibonacci é a seguinte: 0, 1, 1, 2, 3, 5, 8, 13, 21, ... Sua regra deformação é: os dois primeiros elementos são 0 e 1; a partir de então, cada elemento é a soma dos dois anteriores. Faça um algoritmo que leia um número inteiro calcule o seu número da sequencia que estaria em sua posição.

```console
user@computer:~$ python fib.py

Insira um número: 8

Fib(8): 21
```

## Problema 5

Receba um número inteiro positivo e defina se ele é primo.

```console
user@computer:~$ python primo.py

Insira um número: 5

5 é um número primo.
```

## Problema 6

Utilise *list comprehension* para formar uma lista com 20 inteiros entre 1 e 100, então utilizando a mesma técnica para formar as sublistas *pares* e *impares* contendo os numeros pares e impares gerados respectivamente. Imprima as três listas.

```console
user@computer:~$ python listas.py

Lista: [32, 51, 24, 4, 57, 50, 40, 44, 11, 11, 94, 33, 94, 22, 59, 53, 11, 41, 74, 74]
Pares: [32, 24, 4, 50, 40, 44, 94, 94, 22, 74, 74]
Impares: [51, 57, 11, 11, 33, 59, 53, 11, 41]
```

## Problema 7

Faça  um  jogo  em  que  o  usuário  tenha  que  adivinhar  uma  palavra  apresentada  com  as  letras embaralhadas.  Deve haver um arquivo com uma lista  de  palavras  lidas e o programa escolherá uma aleatoriamente. O jogador terá seis tentativas para adivinhar a palavra. Ao final a palavra deve ser mostrada na tela, informando se o usuário ganhou ou perdeu o jogo.

```console
user@computer:~$ python jogo.py

A M C A
Tente adivinhar a palavra: cama
Voce acertou!
```

## Problema 8

Crie uma classe que modele um Pokémon. Sua classe deve conter:

Atributos:

* Nome
* Tipo
* Saúde
* Fome
* Humor
* Level
* Habilidades.

Métodos:

* Evoluir: Altera nome de se level for multiplo de 16.
* Alterar fome: Receber um novo valor de fome do usuário.
* Alterar saúde: Receber um novo valor de saúde do usuário.
* Aprender nova habilidade: Deve possuir no máximo 4, quando tiver 4 deve selecionar uma para ser esquecida.
* Batalhar: Sobe 1 level, diminiu a saúde em 5 e o humor em 2. Se humor estiver abaixo de 5 o Pokémon deve se recusar a batalhar

```console
user@computer:~$ python pokemon.py

Pokemon
 Nome: Bulbassaur
 Tipo: Grama
 Saude: 100
 Fome: 0
 Level: 10
 Humor: 100

Deu fome...
Nova fome: 20

Bater em outro pokemon machuca...
Nova saude: 15

Pokemon
 Nome: Bulbassaur
 Tipo: Grama
 Saude: 95
 Fome: 20
 Level: 11
 Humor: 8

Evoluir...
Novo nome: Ivysaur

Adicionar habilidade...
Muitas Habilidades
0 => Arranhar
1 => Investida
2 => Golpe
3 => Golpe
Seleciona qual deve ser esquecida: 2
Nova habilidade: Chicote de vinha

Pokemon
 Nome: Ivysaur
 Tipo: Grama
 Saude: 95
 Fome: 20
 Level: 11
 Humor: 8
 Golpes: ['Arranhar', 'Investida', 'Folha navalha', 'Chicote de vinha']
```
