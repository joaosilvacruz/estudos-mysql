Para inserir dados é utilizado INSERT INTO:
INSERT INTO Contas (id_banco, numero, saldo) VALUES (1, '123456-7', 1500.00);

"INSERT INTO" é a instrução SQL que indica que você quer inserir dados em uma tabela.
"nome_da_tabela" é o nome da tabela em que você deseja inserir os dados.
"(coluna1, coluna2, coluna3, ...)" é uma lista das colunas da tabela em que você deseja inserir os valores.
"VALUES" é a palavra-chave que indica que você está inserindo valores na tabela.
"(valor1, valor2, valor3, ...)" é uma lista dos valores que você deseja inserir nas respectivas colunas da tabela.

Inserção dados multiplos:

INSERT INTO Contas (id_banco, numero, saldo) VALUES 
(1, '123456-7', 1500.00),
(2, '456789-0', 2500.00),
(3, '789012-3', 500.00);

Inserção de registros a partir de outra tabela:
INSERT INTO Contas (id_banco, numero, saldo)
SELECT id_banco, numero, saldo FROM Contas_Temporarias;

Inserção de registros a partir de um arquivo CSV:
LOAD DATA INFILE 'caminho/para/arquivo.csv'
INTO TABLE Contas
FIELDS TERMINATED BY ','
LINES TERMINATED BY '\n'
IGNORE 1 ROWS;


FIELDS TERMINATED BY ','" indica que as colunas são separadas por vírgulas e a opção "LINES TERMINATED BY '\n'" indica que as linhas são separadas por quebra de linha. A opção "IGNORE 1 ROWS" indica que a primeira linha do arquivo (que geralmente contém os cabeçalhos das colunas) deve ser ignorada.
