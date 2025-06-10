# 🛒 Projeto Banco de Dados E-Commerce

Este repositório contém o modelo relacional de um banco de dados para um sistema de E-Commerce, incluindo estrutura das tabelas, relacionamentos, inserções de dados e consultas SQL.

## 📚 Descrição

O projeto simula o funcionamento de um comércio eletrônico com as seguintes funcionalidades:

- Cadastro de clientes (Pessoa Física e Pessoa Jurídica)
- Cadastro de produtos, fornecedores e vendedores
- Registro de pedidos, entregas e métodos de pagamento
- Controle de estoque e localização de armazenamento
- Relações entre fornecedores, produtos e vendedores

---

## 🗂️ Estrutura das Tabelas

### 👥 Clientes
- `clients` – dados comuns (nome, endereço)
- `client_pf` – dados exclusivos de pessoa física (CPF)
- `client_pj` – dados exclusivos de pessoa jurídica (CNPJ)

### 📦 Produtos e Fornecimento
- `product` – dados dos produtos
- `productSupplier` – relação entre fornecedores e produtos
- `productStorage` – estoque geral
- `storageLocation` – localização física do estoque

### 🧾 Pedidos
- `orders` – pedidos realizados
- `productOrder` – itens de cada pedido
- `delivery` – status e código de rastreio das entregas

### 💳 Pagamentos
- `payment_methods` – formas de pagamento associadas ao pedido

### 👨‍💼 Vendedores e Fornecedores
- `seller` – vendedores cadastrados
- `supplier` – fornecedores cadastrados
- `productSeller` – produtos oferecidos por vendedores

---

## 🛠️ Funcionalidades Implementadas

- Suporte a múltiplos métodos de pagamento por pedido
- Registro de entregas com status e código de rastreio
- Clientes com distinção entre PF e PJ
- Relacionamento muitos-para-muitos entre produtos, fornecedores e vendedores

---
