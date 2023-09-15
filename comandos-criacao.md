# Comando SQL _ Referência
<!-- ___________________________________ -->
## Modelagem física

### Criar banco de dados

```sql

CREATE DATABASE vendas CHARACTER SET utf8mb4;

```
<!-- ____________________________ -->
### Criar a tabela de fabricantes

```sql

CREATE TABLE fabricantes(
    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(45) NOT NULL
)

```
<!-- ________________________________________ -->
### Criar a tabela de produtos

```sql

CREATE TABLE produtos(
    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(45) NOT NULL,
    decricao TEXT(1000) NOT NULL,
    preco DECIMAL(6,2) NOT NULL,
    quantidade TINYINT(4) NOT NULL
)

```
<!-- ________________________________________ -->
### Adicionar campo/coluna em uma tabela

```sql
ALTER TABLE produtos ADD fabricantes _id INT NOT NULL
AFTER quantidade;

```
<!-- ________________________________________ -->
### Criação da chave estrangeira (relacionamentos entre tabelas)

```sql
ALTER TABLE produtos 
# CONTRAINT é uma restrição definida no relaciomento
ADD CONSTRAINT fk_produtos_fabricantes

# A chave estrangeira deve fazer referencia a chave primaria
FOREIGN KEY(fabricantes_id) REFERENCES fabricantes(id)


```