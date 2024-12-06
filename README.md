# Desafio de Projeto: Modelo Conceitual de E-commerce

Você deve criar um modelo conceitual de banco de dados que atenda aos seguintes requisitos:

1 Cliente PJ e PF: Uma conta pode ser de Pessoa Física (PF) ou Jurídica (PJ), mas não ambas.
2 Pagamento: Uma conta pode ter mais de uma forma de pagamento associada.
3 Entrega: Deve registrar o status da entrega e o código de rastreio.


# Etapas para Resolver
1. Modelo Conceitual - Um modelo conceitual usa diagramas para mostrar entidades e suas relações, sem entrar em detalhes técnicos. Vamos identificar as entidades e seus atributos com base no problema.

2. Aqui está uma explicação de como abordar cada parte:

# Entidades principais:

Cliente:
- Subtipos: Pessoa Física (PF) e Pessoa Jurídica (PJ).
- Usaremos generalização/especialização para representar isso.

  
Pagamento:
- Deve permitir múltiplas formas de pagamento associadas a um cliente.


Entrega:
- Precisa registrar status e código de rastreio.

#Relacionamentos:
- Um cliente pode ter múltiplos pagamentos associados.
- Uma entrega estará associada a um cliente ou pedido.


# O Diagrama Conceitual incluiria algo como:

# Entidades e Atributos:
Cliente: ID_Cliente, Nome, Email, Telefone, Tipo (PJ/PF)
Pessoa Física (PF): CPF, Data_Nascimento
Pessoa Jurídica (PJ): CNPJ, Razão_Social, Nome_Fantasia
Pagamento: ID_Pagamento, Tipo_Pagamento (cartão, boleto, etc.), Detalhes
Entrega: ID_Entrega, Status_Entrega, Código_Rastreio, Data_Entrega
Pedido: ID_Pedido, Data_Pedido, Valor_Total

# Relacionamentos:
1. Cliente pode ter 0 ou mais formas de Pagamento.
2. Um Pedido é associado a um único Cliente.
3. Cada Pedido tem exatamente uma Entrega associada.

![modelo_conceitual_simples](https://github.com/user-attachments/assets/8073c5d4-b7f8-4984-a30b-f48a460c35fb)
