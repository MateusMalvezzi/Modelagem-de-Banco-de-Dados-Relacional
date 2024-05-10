## 1º Projeto Prático - Dados Modelagem de Banco de Dados Relacional   

### Este é o primeiro projeto do programa <a href="https://www.linkedin.com/posts/mateusmalvezzi_voc%C3%AA-%C3%A9-capaz-fala-meus-amigos-beleza-activity-7150327836132777984-G1XL?utm_source=share&utm_medium=member_desktop">Desenvolve Boticário 2024</a> <br><br>

Estudo de caso: Cacau Show <br><br>

Mateus Malvezzi Rodrigues <br><br>


Desafio
Modele um banco de dados relacional que representa o negócio do Boticário. O projeto deve levar em consideração somente os conceitos e entidades relacionados à parte de vendas, sistema de pontuação e gestão de produtos em estoque.
Ao final, você deverá ter aprendido a identificar entidades, relacionamentos e atributos, além de criar a modelagem lógica e física do banco de dados.<br><br>

Para este projeto, escolhi o modelo de negócio da Cacau Show.<br><br>
Um ramo de negócio que se assemelha ao Boticario no quesito eccomerce + junção de pontos a cada compra.<br><br>

Foi sugerido a criação de três entidades, mas para adicionar um desafio maior, criei mais, com seus devidos atributos e relacionamentos. Abaixo, detalharei melhor as entidades, respectivos atributos e postarei dois prints e explicar melhor sobre.<br><br>

-	Entidade
    -	Loja
        -	atributos
            -	cod_loja VARCHAR PK
            -	email VARCHAR
            -	estado VARCHAR
            -	cidade VARCHAR
            -	telefone INTEGER
    -	Pedidos
        -	atributos
            -	cod_pedido VARCHAR PK
            -	valor_pedido DECIMAL
            -	qtd_venda INTEGER
            -	cod_chocolate VARCHAR
            -	cod_cliente VARCHAR
            -	cod_funcionario VARCHAR
            -	data_pedido DATE
            -	status_pedido VARCHAR
            -	metodo_pagamento VARCHAR
    -	Funcionario
        -	atributos
            -	cod_funcionario VARCHAR PK
            -	sexo VARCHAR
            -	cod_loja VARCHAR
            -	matricula INTEGER
            -	cargo VARCHAR
            -	salario DECIMAL
            -	meta_variavel DECIMAL
            -	nome VARCHAR
            -	data_contratacao DATE
    -	Sistema de pontuacao
        -	atributos
            -	cod_funcionario VARCHAR
            -	cod_cliente VARCHAR
            -	cod_venda VARCHAR
            -	cod_loja VARCHAR
            -	qtd_pontos DECIMAL
    -	Produto
        -	atributos
            -	cod_chocolate VARCHAR PK
            -	valor_produto DECIMAL
            -	validade_produto DATE
            -	ano_fabricacao DATE
            -	categoria VARCHAR
            -	nome_chocolate VARCHAR
            -	sabor_chocolate VARCHAR
            -	tipo_chocolate VARCHAR
            -	cod_loja VARCHAR
            -	cod_pedido VARCHAR
    -	Cliente
        -	atributos
            -	cod_cliente VARCHAR PK
            -	telefone_1 VARCHAR
            -	estado VARCHAR
            -	cidade VARCHAR
            -	sexo VARCHAR
    -	Estoque
        -	atributos
            -	cod_estoque VARCHAR PK
            -	cod_chocolate VARCHAR
            -	cod_loja VARCHAR
            -	cod_pedido VARCHAR
            -	localizacao_estoque VARCHAR
            -	qtd_estoque INTEGER
            -	validade_produto DATE
            -	ano_fabricacao DATE
            -	entrada_estoque DATE

<br><br>

![image](https://github.com/MateusMalvezzi/Modelagem-de-Banco-de-Dados-Relacional/assets/79795173/2c915268-ce8b-48e5-81d6-f5bc5627072a) <br><br>

![image](https://github.com/MateusMalvezzi/Modelagem-de-Banco-de-Dados-Relacional/assets/79795173/3a1d4cf4-5043-4542-94af-53d7ffe2ec94)

