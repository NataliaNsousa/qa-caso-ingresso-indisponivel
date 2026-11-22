# Registro de incidente — ingresso indisponível após pagamento recebido

## Resumo

Uma cliente entrou em contato com o suporte porque havia concluído a compra, mas o ingresso não estava disponível para ela. Ao consultar a compra, confirmei que o valor havia sido recebido e que o ingresso continuava indisponível.

## Resultado esperado e resultado observado

| Resultado esperado | Resultado observado |
|---|---|
| Após o reconhecimento do pagamento, o ingresso fica disponível para a cliente acessar. | O valor da compra havia sido recebido, mas a cliente não conseguia acessar o ingresso. |

**Impacto observado** — A cliente precisou acionar o suporte para obter acesso a um ingresso já pago.

## Investigação e atendimento

1. Consultei a compra e a situação do pagamento.
2. Confirmei o recebimento do valor e verifiquei que o ingresso estava indisponível.
3. Fiz um ajuste manual no registro da compra e pedi à cliente que verificasse novamente a disponibilidade do ingresso.
4. Registrei o incidente na ferramenta de chamados para investigação pela equipe de desenvolvimento.
5. Avisei a equipe no canal interno.

## Evidências e situação

- **Evidências registradas** — O chamado interno registra a evidência da indisponibilidade e a referência usada para localizar o pedido.
- **Atendimento** — Ajuste manual realizado. A confirmação da cliente após a nova verificação não consta no relato.
- **Investigação técnica** — Incidente encaminhado ao desenvolvimento. A causa e a correção definitiva não foram informadas.

## Validações sugeridas para a correção

| Cenário | Resultado esperado |
|---|---|
| Concluir uma compra e confirmar o pagamento. | O ingresso correspondente fica disponível sem intervenção manual. |
| Consultar uma compra com pagamento pendente. | O ingresso permanece indisponível até a confirmação do pagamento. |
| Confirmar o pagamento de um pedido que estava pendente. | O ingresso passa a ficar disponível no pedido correto, sem emissão duplicada. |
