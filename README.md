# Atividade-11
MeuDadoThreadsJava

Diferenças observadas: Diferença entre valores armazenados e carregados em diferentes momentos, indicando condição de corrida.

Conclusão: A falta de sincronização permitiu que as threads acessassem a variável Dado ao mesmo tempo, resultando em resultados inconsistentes. A sincronização usando synchronized é necessária para resolver esse problema.

MeuDadoMonitorJava

Análise e Conclusão:
- Observação de melhorias ou manutenção da consistência nos resultados da execução usando `MeuDadoMonitorJava`.
- Comentários sobre como a sincronização por monitor resolveu (ou não) a condição de corrida.

MeuDadoEventJava.


### Comparação dos Logs:

Diferença entre log_execucao1.txt e log_execucao_event.txt:
- Na Atividade 1, houve várias inconsistências devido à falta de sincronização.
- Na Atividade 3, o uso de `wait()` e `notify()` garantiu a consistência dos dados.

Diferença entre log_execucao2.txt e log_execucao_event.txt:
- Ambos garantem a consistência, mas `MeuDadoEventJava` mostra uma eficiência potencialmente maior devido ao uso de `notify()`, que acorda apenas uma thread específica.

Conclusão:
A sincronização com eventos (`wait()` e `notify()`) provou ser uma abordagem mais flexível e eficiente em comparação com a sincronização com monitores. Enquanto ambas garantem consistência, o uso de eventos permite melhor controle sobre a comunicação entre threads.