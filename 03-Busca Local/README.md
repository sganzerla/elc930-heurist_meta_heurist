# Busca Local

## Vizinhança

Definição para o conjunto de soluções $S$ que são próximas umas das outras representadas por $N$.

## Espaço de Busca

Definido pelos conjunto de soluções $S$ e por uma vizinhança $N$

Em uma representação em grafo os caminhos seriam todos os arcos com nós em intersecção.

* Partida: solução inicial obtida através de um método construtivo.
* Iteração: melhoria sucessiva da solução corrente através de uma busca na sua vizinhança.
* Parada: primeiro ótimo local encontrado (quando nenhuma solução aprimorante dos vizinhos melhora a solução incumbente).
* Heurística subordinada: utilizada para obter uma solução aprimorante na vizinhança.

## Pontos de atenção

* Definição da vizinhança
* Estratégia de busca na vizinhança
* Complexidade de cada iteração
  * Proporcional ao tamanha da vizinhança
  * Eficiência depende da forma como a função objetivo é atualizada. Evitar cálculos repetitivos.

## Estratégias

* Melhoria iterativa: a cada iteração, selecionar qualquer (pode ser a primeira) solução aprimorante na vizinhança.
* Descida mais rápida: selecionar a melhor solução aprimorante na vizinhaça.
  
## Observações

Diferentes aspectos do espaço de busca influenciam o desempenho de algoritmos de busca local.

* Conexidade: deve existir um caminho entre qualquer par de soluções no espaço de busca.
* Distância: o caminho mais curto entre duas soluções será o mais visitado.
* Diâmetro: distância entre duas ou mais soluções mais afastadas.
* Bacia de atração de um ótimo local: conjunto de soluções iniciais a partir das quais o algoritmo de descida mais rápida leva a este ótimo local.

## Dificuldades

Término prematuro da iteração no primeiro ótimo local

* Sensível à solução de partida
* Sensível à vizinhança escolhida
* Sensível à estratégia de busca
* Pode exigir um número exponencial de iterações

Para evitar esses problemas

* Reduzir vizinhança: investigar um subconjunto da vizinhança da solução corrente de forma aleatória.
* Multi-partida: repetir a busca local de diferentes soluções
* Multi-vizinhança: considera mais de uma vizinhança. Busca um ótimo local em cada uma tendo como critério de parada se o mesmo ótimo local é comparilhado para ambas.
* Segmentação da vizinhança: utilizada para aumentar a eficiência quando vizinhanças muito grandes são utilizadas, pode ser vista como uma estratégia multi-vizinhança.

