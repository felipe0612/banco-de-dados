# Comandos SQL - Para CRUD

## Resumo
C -> Create (Insere dados)
R -> Read (ler dados)
U -> Update (Atualizar dados)
D -> Delete (Deletar dados)
<!-- ________________________________________ -->
## Insert
## Fabricantes


sql
    INSERT INTO fabricantes (nome) VALUES ('Asus');
    INSERT INTO fabricantes (nome) VALUES ('Dell');
    INSERT INTO fabricantes (nome)
    VALUES ('Apple'), ('LG'), ('Samsung'), ('Brastemp');


## Insert
## Fabricantes

sql
    INSERT INTO produtos (nome, descriao, preco, quantidade, fabricante_id) VALUES ('Asus');
    VALUES('Ultrabook', 'Ultrabook Asus Intel Core i9', 
    6500.99,
    7,
    1
    );

    INSERT INTO produtos (nome, descriao, preco, quantidade, fabricante_id) VALUES ('Asus');
    VALUES('Geladeira', 'Frost-Free com acesso a internet', 
    8500.99,
    7,
    1
    );

    INSERT INTO produtos (nome, descriao, preco, quantidade, fabricante_id) VALUES ('Asus');
    VALUES('Tablet Android', 'Tablet 10 polegadas com 256Gb de armazenamento', 
    4999,
    3,
    5
    );

    INSERT INTO produtos (nome, descriao, preco, quantidade, fabricante_id) VALUES ('Asus');
    VALUES('iPhone 14 Pro Max', 'Processador Bionic 15 com 512Gb de armazenamento', 
    9999.97,
    3,
    3
    );

    INSERT INTO produtos (nome, descriao, preco, quantidade, fabricante_id) VALUES ('Asus');
    VALUES('ipad mini', 'Tablet com tela de retina 4k com 516Gb de armazenamento', 
    9999.97,
    3,
    3
    );