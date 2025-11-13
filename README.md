# Projetos-DIO-SQL# Projeto Conceitual de Banco de Dados - E-commerce  
Repositório destinado ao desafio de SQL da **Digital Innovation One (DIO)**, com foco em **modelagem conceitual** de um sistema de e-commerce.  
O objetivo é refinar o modelo inicial proposto pela especialista, implementando regras adicionais.

---

## **Objetivo do Desafio**

Refinar o modelo conceitual de banco de dados incluindo os seguintes pontos obrigatórios:

### Cliente PF e PJ  
Uma conta pode ser Pessoa Física (PF) ou Pessoa Jurídica (PJ), **mas nunca as duas ao mesmo tempo**.  
Implementação:
- Atributo `Tipo de Cliente` (ENUM).
- Campos `CPF` e `CNPJ` como opcionais (NULLABLE).
- Índices únicos em ambos.

### Pagamento com mais de uma forma de pagamento  
Um pedido pode conter **múltiplas formas de pagamento**.  
Implementação:
- Entidade **Forma de Pagamento**  
- Suporte a tipos como credito ou debito.

### Entrega com status e código de rastreio  
Cada pedido possui uma entrega vinculada com:
- Status 

Implementado com a entidade **Entrega**.

---

## **Descrição das Principais Entidades**

### Cliente  
Representa clientes PF ou PJ, diferenciados por tipo.  
Inclui CPF/CNPJ e dados de identificação.

### Pedido  
Armazena os pedidos realizados no sistema, incluindo frete, status e vínculo com o cliente.

### Entrega  
Controla o processo de envio do pedido.

### Forma de Pagamento  
Lista os tipos de pagamento permitidos.

### Produto  
Itens comercializados no e-commerce, com categoria, descrição e valor.

### Fornecedor  
Origem institucional dos produtos ofertados pela própria loja.

### Vendedor Terceirizado  
Representa usuários externos que vendem na plataforma (modelo marketplace).

### Estoque  
Locais físicos de armazenamento, permitindo controle multiestoque.


---

## **Diagrama Conceitual**

As imagens do modelo estão disponíveis na pasta:

[`/Diagramas`](./Diagramas)

- `Diagrama_parte1.png`  
- `Diagrama_parte2.png`


