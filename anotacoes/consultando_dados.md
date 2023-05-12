# Selecionar todos os clientes
SELECT * FROM clientes;

# Selecionar apenas o nome e e-mail de todos os clientes
SELECT nome, email FROM clientes;

# Selecionar apenas os clientes que moram na Rua A
SELECT * FROM clientes
WHERE endereco = 'Rua A, 123';

# Selecionar apenas o nome e telefone dos clientes que moram na Rua B
SELECT nome, telefone FROM clientes
WHERE endereco = 'Rua B, 456';
