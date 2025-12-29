## Refinamento de Projeto Conceitual de Banco de Dados (E-commerce)
O projeto consiste no refinamento de um modelo conceitual de banco de dados para um sistema de E-commerce, conforme requisitos definidos no desafio da DIO. O objetivo foi melhorar o modelo existente, garantindo maior consistência, redução de redundância e aderência às regras de negócio.


### 🎯 Objetivo do Refinamento
O modelo foi ajustado para atender aos seguintes pontos:
Cliente PJ e PF
Uma conta pode ser Pessoa Física ou Pessoa Jurídica, mãs não pode ser os dois tipos ao mesmo tempo

Foi aplicada a técnica de especialização (ER Estendido)
Subtipos criados:
Cliente_PF
Cliente_PJ

### Pagamento
Um cliente pode cadastrar várias formas de pagamento
Cada forma possui informações como:
tipo
número do cartão
nome impresso no cartão
validade
bandeira
Relacionamento: 1 Cliente → N Formas de Pagamento

### Entrega
A entrega possui:
status
código de rastreio
datas de envio e entrega
transportadora
Criada como entidade separada ligada ao Pedido

### 🧩 Principais Entidades
Cliente
Cliente_PF
Cliente_PJ
Produto
Pedido
Forma de Pagamento
Entrega
Fornecedor
Estoque

### 🗂️ Arquivos do Repositório
diagrama-ecommerce.png → imagem do modelo
README.md → documentação do projeto

✅ Resultado
O refinamento garantiu:
melhoria na organização do modelo de dados, eliminação de redundâncias, implementação correta de regras de negócio, uso adequado de especialização PF / PJ, modelagem alinhada ao cenário real de E-commerce

###🚀 Tecnologias Utilizadas
MySQL Workbench (Modelagem EER)
