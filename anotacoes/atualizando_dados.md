# ATUALIZANDO DADOS NA TABELA "clientes"

## Atualizar o nome do cliente com ID=1
UPDATE clientes
SET nome = 'João Silva'
WHERE id = 1;

## Atualizar o e-mail do cliente com ID=2
UPDATE clientes
SET email = 'maria@hotmail.com'
WHERE id = 2;

-- Atualizar o telefone e endereço do cliente com ID=3
UPDATE clientes
SET telefone = '(11) 3333-4444', endereco = 'Rua das Flores, 123'
WHERE id = 3;
