Chaves primárias:
Chave primária: é um campo ou conjunto de campos que identificam unicamente cada registro em uma tabela. No exemplo das tabelas "Bancos" e "Contas", a chave primária de cada tabela é a coluna "id_banco" na tabela "Bancos" e a coluna "id_conta" na tabela "Contas", respectivamente. Isso garante que cada banco e cada conta tenham um identificador único e que não haja duplicação de registros.

Chaves estrangeiras:
Chave estrangeira: é um campo ou conjunto de campos em uma tabela que se refere à chave primária de outra tabela. No exemplo das tabelas "Bancos" e "Contas", a chave estrangeira é a coluna "id_banco" na tabela "Contas", que faz referência à chave primária "id_banco" na tabela "Bancos". Isso garante que cada conta esteja associada a um banco existente na tabela "Bancos" e impede que sejam criadas contas para bancos que não existem na tabela "Bancos". A chave estrangeira também pode ser usada para garantir a integridade dos dados em outras operações, como atualizações e exclusões de registros.

Exemplo na prática:

CREATE TABLE Bancos (
  id_banco INT NOT NULL AUTO_INCREMENT,
  nome VARCHAR(100) NOT NULL,
  endereco VARCHAR(100) NOT NULL,
  PRIMARY KEY (id_banco)
);

CREATE TABLE Contas (
  id_conta INT NOT NULL AUTO_INCREMENT,
  id_banco INT NOT NULL,
  numero VARCHAR(20) NOT NULL,
  saldo DECIMAL(10,2) NOT NULL,
  PRIMARY KEY (id_conta),
  FOREIGN KEY (id_banco) REFERENCES Bancos(id_banco)
);
