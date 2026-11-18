# Regras de Negócio — SmartStock

- **RN01:** Todo produto deverá possuir identificador único.
- **RN02:** Todo produto deverá possuir nome, categoria e quantidade.
- **RN03:** A quantidade em estoque não poderá ser negativa.
- **RN04:** Uma entrada deverá aumentar a quantidade disponível.
- **RN05:** Uma saída deverá diminuir a quantidade disponível.
- **RN06:** Não será permitida saída maior que a quantidade disponível.
- **RN07:** Quando a quantidade for igual ou inferior ao estoque mínimo, deverá ser gerado um alerta.
- **RN08:** Toda movimentação deverá registrar produto, tipo, quantidade, data e usuário responsável.
- **RN09:** O histórico de movimentações deverá ser preservado mesmo quando um produto for desativado.
- **RN10:** A atualização do estoque e o registro da movimentação deverão ocorrer de forma consistente, evitando divergências.
