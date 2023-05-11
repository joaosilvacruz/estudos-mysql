Para criar uma tabela você pode:

opção 1:

CREATE TABLE nome_da_tabela (
  coluna1 tipo_de_dado_opcoes,
  coluna2 tipo_de_dado_opcoes,
  coluna3 tipo_de_dado_opcoes,
);

opção 2:

CREATE TABLE usuarios (
  id INT AUTO_INCREMENT PRIMARY KEY,
  nome VARCHAR(255),
  email VARCHAR(255) UNIQUE NOT NULL
);

obs.: 

Auto_increment: a coluna "id" de uma tabela como AUTO_INCREMENT, o MySQL atribuirá automaticamente um valor exclusivo e crescente para essa coluna toda vez que uma nova linha for adicionada à tabela.
A restrição NOT NULL é usada para garantir que uma coluna não possa conter valores nulos (em branco ou ausentes). Isso é útil para garantir que todas as linhas em uma tabela tenham valores preenchidos em determinadas colunas, o que pode ser importante para o correto funcionamento do banco de dados ou da aplicação que o utiliza.
