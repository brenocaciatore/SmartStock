# Documento de Requisitos — SmartStock

## 1. Objetivo
Desenvolver uma plataforma web inteligente para facilitar o gerenciamento de estoques empresariais. O sistema permitirá cadastrar produtos, controlar entradas e saídas, acompanhar quantidades disponíveis, gerar relatórios e receber alertas de estoque baixo. Futuramente, poderá integrar Inteligência Artificial para apoiar análises e decisões.

## 2. Problema
O controle manual por planilhas ou anotações pode dificultar o acompanhamento do estoque, causar erros de registro, falta de produtos, compras desnecessárias e desorganização das informações. O SmartStock centraliza esses dados em uma única plataforma.

## 3. Público-alvo
- Pequenas e médias empresas;
- Lojas, mercados, comércios e distribuidoras;
- Empresas que armazenam produtos;
- Funcionários responsáveis pelo estoque;
- Gerentes e administradores.

## 4. Funcionalidades
1. Cadastro de produtos com nome, categoria, quantidade, estoque mínimo, preço e data de cadastro.
2. Consulta e pesquisa de produtos.
3. Atualização de informações dos produtos.
4. Exclusão lógica ou desativação de produtos, preservando o histórico.
5. Registro de entrada de produtos.
6. Registro de saída de produtos.
7. Dashboard com indicadores de estoque.
8. Relatórios de produtos e movimentações.
9. Definição e acompanhamento de estoque mínimo.
10. Alertas quando a quantidade atingir ou ficar abaixo do mínimo.
11. Preparação para consultas e automações com IA.

## 5. Benefícios
- Melhor organização;
- Redução de erros de registro;
- Facilidade no controle de entradas e saídas;
- Identificação de produtos com estoque baixo;
- Economia de tempo;
- Visualização centralizada das informações;
- Apoio à tomada de decisões.

## 6. Requisitos funcionais
| Código | Descrição |
|---|---|
| RF01 | Permitir login de usuários. |
| RF02 | Cadastrar produtos. |
| RF03 | Consultar e pesquisar produtos. |
| RF04 | Atualizar produtos. |
| RF05 | Excluir ou desativar produtos. |
| RF06 | Registrar entradas de estoque. |
| RF07 | Registrar saídas de estoque. |
| RF08 | Atualizar as quantidades após movimentações. |
| RF09 | Definir estoque mínimo. |
| RF10 | Identificar produtos com estoque baixo. |
| RF11 | Exibir indicadores no dashboard. |
| RF12 | Gerar relatórios de estoque. |
| RF13 | Consultar histórico de movimentações. |
| RF14 | Permitir configurações da conta. |
| RF15 | Preparar integração futura com IA e n8n. |

## 7. Requisitos não funcionais
| Código | Descrição |
|---|---|
| RNF01 | Interface responsiva. |
| RNF02 | Navegação simples e intuitiva. |
| RNF03 | Armazenamento em banco de dados. |
| RNF04 | Acesso protegido por autenticação. |
| RNF05 | Senhas armazenadas com hash seguro. |
| RNF06 | Validação dos dados informados. |
| RNF07 | Desempenho adequado nas operações. |
| RNF08 | Código organizado e de fácil manutenção. |
