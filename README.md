# atividades_UPDATE-BCD

Atualizações SQL — Vendas de Informática
Descrição

Este projeto contém comandos SQL utilizando UPDATE para atualizar registros nas tabelas do banco de dados vendas_informatica.

Banco de Dados
USE vendas_informatica;

Comandos SQL
1. Atualizar a cidade dos clientes

Altera a cidade dos clientes cujo estado seja DF ou ES para Senailandia.
````
UPDATE cliente
SET cidade = "Senailandia"
WHERE estado IN ("DF", "ES");
````
2. Atualizar a data de cadastro

Define a data de cadastro como 2026-01-01 para os clientes que residem em Manaus.
````
UPDATE cliente
SET data_cadastro = "2026-01-01"
WHERE cidade = "Manaus";
````
3. Atualizar o nome do cliente

Altera o nome do cliente com ID 10 para Michael Jackson.
````
UPDATE cliente
SET nome_cliente = "Michael Jackson"
WHERE id_cliente = 10;
````
4. Atualizar o nome do produto

Altera o nome do produto com ID 1 para Notebook Lenovo IdeaPad 7.
````
UPDATE produto
SET nome_produto = "Notebook Lenovo IdeaPad 7"
WHERE id_produto = 1;
````
5. Atualizar o preço dos notebooks Dell

Define o preço unitário como 4999.99 para os produtos da marca DELL cuja categoria seja Notebook.
````
UPDATE produto
SET preco_unitario = 4999.99
WHERE marca = "DELL"
AND categoria = "Notebook";
````
6. Atualizar o desconto das vendas

Define o desconto percentual como 0.01 para as vendas cuja quantidade seja maior ou igual a 2.
````
UPDATE venda
SET desconto_percentual = 0.01
WHERE quantidade >= 2;

