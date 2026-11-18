# Modelagem Inicial do Banco de Dados

## Visão geral
A modelagem inicial utiliza quatro tabelas: `usuarios`, `categorias`, `produtos` e `movimentacoes`.

## Tabela `usuarios`
| Campo | Tipo sugerido | Regra |
|---|---|---|
| id | INT | PK, auto incremento |
| nome | VARCHAR(100) | obrigatório |
| email | VARCHAR(150) | obrigatório, único |
| senha | VARCHAR(255) | hash, nunca texto puro |
| data_cadastro | DATETIME | obrigatório |

## Tabela `categorias`
| Campo | Tipo sugerido | Regra |
|---|---|---|
| id | INT | PK, auto incremento |
| nome | VARCHAR(100) | obrigatório |

## Tabela `produtos`
| Campo | Tipo sugerido | Regra |
|---|---|---|
| id | INT | PK, auto incremento |
| nome | VARCHAR(150) | obrigatório |
| categoria_id | INT | FK para categorias.id |
| quantidade | INT | não negativa |
| estoque_minimo | INT | não negativo |
| preco | DECIMAL(10,2) | não negativo |
| data_cadastro | DATETIME | obrigatório |

## Tabela `movimentacoes`
| Campo | Tipo sugerido | Regra |
|---|---|---|
| id | INT | PK, auto incremento |
| produto_id | INT | FK para produtos.id |
| usuario_id | INT | FK para usuarios.id |
| tipo | VARCHAR(10) | ENTRADA ou SAIDA |
| quantidade | INT | maior que zero |
| data | DATETIME | obrigatório |

## Relacionamentos
- Uma categoria possui vários produtos (1:N).
- Um produto possui várias movimentações (1:N).
- Um usuário registra várias movimentações (1:N).

## Observações
- `categoria_id`, `produto_id` e `usuario_id` são chaves estrangeiras.
- Recomenda-se desativar produtos em vez de apagá-los fisicamente quando houver movimentações associadas.
- As movimentações devem ser registradas junto da atualização de estoque em uma transação do banco de dados.
