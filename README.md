# dio-refinando-banco-dados-ecommerce
DIO - Refinando um Projeto Conceitual de Banco de Dados – E-COMMERCE

Objetivo:
Refine o modelo apresentado acrescentando os seguintes pontos:

Cliente PJ e PF – Uma conta pode ser PJ ou PF, mas não pode ter as duas informações;
- Para essa questão adiocionei uma entidade chanada TIPO_CLIENTE onde deverá ser informado o tipo de cliente através do campo JURFIS podendo ter os valores "F" e "J". Também adcionei o campo CNPJ_CPF para armezenar os dados de CNPJ ou CPF do cliente.

Pagamento – Pode ter cadastrado mais de uma forma de pagamento;
- Como solução foi adicionado uma entidade chamada PAGAMENTO onde é armazenado a forma de pagamento do cliente (Exemplo: Cartão de Crédito) e um relacionamento com o pedido através da entidade PAGAMENTO_DO_PEDIDO para poder localizar o cartão de crédito já cadastrado pelo cliente.

Entrega – Possui status e código de rastreio;
- Neste caso foi adicionada uma entidade chamada ENTREGA que foi relacionada com a tabela de PEDIDO
