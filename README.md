# Atividade-11

Diferenças observadas: Diferença entre valores armazenados e carregados em diferentes momentos, indicando condição de corrida.

Conclusão: A falta de sincronização permitiu que as threads acessassem a variável Dado ao mesmo tempo, resultando em resultados inconsistentes. A sincronização usando synchronized é necessária para resolver esse problema.