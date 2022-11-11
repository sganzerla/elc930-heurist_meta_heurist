# Exemplo com Bin Packing

$n = 20$

$w_j = \{ 42 , 69 , 67 , 57 , 93 , 90 , 38 , 36 , 45 , 42
 33 , 79 , 27 , 57 , 44 , 84 , 86 , 92 , 46 , 38 \} $
$ c = 200 $

## FASE 1 - Solução Inicial

* 1º: Utilizando algum método construtivo encontre uma solução incumbente
* 2º: Use o valor da função objetivo como limite superior. (7)
* 3º: Calcule o limite inferior. (6)

## FASE 2 - Eliminando GAP

Se o limite superior é igual ao limite inferior a solução incumbente já é a ótima.

Senão, eliminar o Bin com menor número de itens e realocar o seu conteúdo aos outros bins de modo a causar a menor infactibilidade possível, em caso de empate escolher o bin de menor índice.

