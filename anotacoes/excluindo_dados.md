# Excluir todos os produtos
DELETE FROM produtos;

# Excluir apenas os produtos com preço acima de 25.00
DELETE FROM produtos
WHERE preco > 25.00;

# Excluir apenas o produto com ID 2
DELETE FROM produtos
WHERE id = 2;
