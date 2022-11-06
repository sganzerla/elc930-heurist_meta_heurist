# 1-Introdução

## Otimização Combinatória

Tomar a decisão mais adequada segundo restrições de recursos e uma função objetivo definida.

As decisões possíveis formam um conjunto finito (grande), mas a melhor deve ser escolhida.

Exemplos:

* Coloração de Grafos (Graph Coloring)
* Caixeiro Viajante (TSP)
* Mochila
* Partição de Números
* Job Shop Scheduling

## Complexidade Computacional

Problemas onde existem algoritmos que resolvem em tempo polinomial são chamados de bem resolvidos.

Porém há outros mais difíceis onde o tempo torna-se exponencial, resolvidos apenas por métodos enumerativos.

Classes de complexidade:

* "P":
  * Para todos os problemas de decisão há um algoritmo polinomial para encontrar uma solução.
* "NP":
  * Para problemas de decisão para os quais existe um algoritmo não determinístico de tempo polinomial.
  * Algorítmo não determinístico, checa se uma solução responde à questão (ORÁCULO).
  * "NP-Completo"
  * "NP-Difícil"

## Problemas NP-Difíceis

Algoritmos exatos não polinominais:

* programação dinâmica
* branch-and-bound
* backtracking

Algoritmos pseudo-polinominais:

* polinominais no tamanho da instância e no valor do maior dado de entrada
* exemplo: mochila

Processamento Paralelo:

* aceleração na prática, sem redução da complexidade.

Algoritmos aproximativos:

* encontram uma solução viável próxima do ótimo garantido.
* exemplo: bin packing

Algoritmos probabilísticos:

* convergência em valor esperado.
* convergência em probabilidade.

## Heurísticas

Definição: qualquer método aproximado projetado com base nas características das soluções dos problemas, com complexidade reduzida em relação à dos métodos exatos que fornecem boas soluções (sem garantia da factibilidade).

Alguns problemas são tão complexos que não encontram soluções ótimas por métodos exatos em tempo computacional satisfatório.

As heurísticas por sua vez, encontram boas soluções num tempo computacional razoável.

Elas não garantem uma solução ótima, por isso são indicadas somente quando:

* tempo computacional da solução pelo método exato é muito alto.
* solução inicial para alimentar um método exato.
* quando há limitação de tempo ou espaço.

Tipos de Heurísticas:

* Métodos Construtivos:
  * vão passo a passo, adicionando itens até obter uma solução.
* Métodos de Decomposisão:
  * dividem o problema em problemas menores, de modo que os subproblemas resolvidos ao serem juntados resolvem o problema original.
* Métodos de Redução:
  * fixam o valor de aluma variável.
* Manipulação do Modelo:
  * modificar o modelo para que fique mais fácil de resolver.
* Métodos de Busca:
  * categoria da maioria das heurísticas.
  * partem de uma solução inicial.
  * definição: vizinhança, vizinho, movimento.

