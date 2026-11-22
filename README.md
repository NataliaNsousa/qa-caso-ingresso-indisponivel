# Caso fictício de QA — ingresso indisponível após pagamento confirmado

## Contexto

Este exercício simula o checkout de uma plataforma fictícia de ingressos. Uma cliente conclui a compra. O pedido aparece como pago, mas o ingresso não está disponível na conta dela.

## Comportamento esperado e simulado

| Esperado | Observado na simulação |
|---|---|
| Depois da confirmação do pagamento, o ingresso fica disponível no pedido correspondente. | O pedido aparece como pago, mas o ingresso não pode ser acessado. |

**Impacto no cenário** — A cliente pode precisar acionar o suporte para acessar um ingresso já pago.

## Como eu investigaria

1. Conferiria se o pagamento confirmado está associado ao pedido certo.
2. Acessaria o pedido novamente para verificar se a indisponibilidade persiste.
3. Registraria os passos para reproduzir o problema e compararia o resultado esperado com o observado.
4. Se conseguisse reproduzir o problema em um ambiente de teste, anexaria evidências com dados fictícios ao relatório de defeito.

## Cenários de teste propostos

| ID | Cenário | Resultado esperado |
|---|---|---|
| CT-01 | Concluir uma compra com pagamento confirmado e abrir o pedido. | O ingresso fica disponível na conta sem intervenção manual. |
| CT-02 | Abrir um pedido cujo pagamento ainda está pendente. | O ingresso continua indisponível enquanto o pagamento estiver pendente. |
| CT-03 | Confirmar o pagamento de um pedido pendente e consultar o pedido novamente. | O ingresso é liberado no pedido certo e aparece uma única vez. |

Os cenários acima foram propostos como exercício de documentação e planejamento de testes.
