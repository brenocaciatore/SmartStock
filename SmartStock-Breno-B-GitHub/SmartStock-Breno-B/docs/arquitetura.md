# Arquitetura da Solução — SmartStock

## Camadas
1. **Usuário:** acessa a plataforma e realiza operações.
2. **Front-end:** apresenta as telas e envia solicitações.
3. **API / Back-end:** valida dados, aplica regras de negócio e consulta ou atualiza o banco.
4. **Banco de Dados:** armazena usuários, categorias, produtos e movimentações.
5. **Agente de IA (futuro):** interpreta perguntas e auxilia na análise do estoque.
6. **n8n (futuro):** executa automações, como notificações e alertas.

## Fluxo de uma operação
1. O usuário realiza uma ação no Front-end.
2. O Front-end envia uma requisição à API.
3. A API valida os dados e aplica as regras de negócio.
4. A API consulta ou altera o Banco de Dados.
5. A API retorna o resultado.
6. O Front-end apresenta a resposta ao usuário.

## Integrações futuras
O agente de IA deverá acessar informações por meio de serviços controlados pela API, respeitando autenticação e permissões. O n8n poderá receber eventos ou executar fluxos de automação, como notificações de estoque baixo.

As integrações com IA e n8n fazem parte do planejamento e não são consideradas implementadas nesta etapa.
