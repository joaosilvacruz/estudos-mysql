Os filtros permitem restringir o conjunto de resultados retornados por uma consulta. Os principais filtros incluem WHERE, AND, OR, IN e LIKE.

- WHERE:
A cláusula WHERE é usada para filtrar registros em uma tabela com base em uma condição especificada. A sintaxe básica é a seguinte:

SELECT column1, column2, ...
FROM table_name
WHERE condition;

- Ex1: 
SELECT * FROM clientes WHERE nome = 'João';

- AND e OR:
Você pode usar as cláusulas AND e OR para combinar várias condições em uma única cláusula WHERE. A sintaxe básica é a seguinte:

SELECT column1, column2, ...
FROM table_name
WHERE condition1 AND condition2 OR condition3;

- Ex2: 
SELECT * FROM clientes WHERE nome = 'João' AND idade >= 30;

- IN:
A cláusula IN é usada para verificar se um valor está presente em um conjunto de valores especificados. A sintaxe básica é a seguinte:

SELECT column1, column2, ...
FROM table_name
WHERE column_name IN (value1, value2, ...);

- Ex3:
SELECT * FROM clientes WHERE nome IN ('João', 'Maria');
