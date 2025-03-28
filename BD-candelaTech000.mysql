-- Criando o banco de dados candelaTech
CREATE DATABASE candelaTech;

-- Criando a tabela Cliente para armazenar informações dos clientes
CREATE TABLE Cliente(
    id_cliente SERIAL PRIMARY KEY,  -- Identificador único do cliente
    nome VARCHAR(255) NOT NULL,  -- Nome do cliente (obrigatório)
    CPF VARCHAR(255) NOT NULL,  -- CPF do cliente (obrigatório)
    email VARCHAR(255) UNIQUE NOT NULL,  -- Email único do cliente (obrigatório)
    telefone VARCHAR(20) UNIQUE NOT NULL,  -- Telefone único do cliente (obrigatório)
    data_cadastro TIMESTAMP DEFAULT CURRENT_TIMESTAMP  -- Data de cadastro do cliente (valor padrão: data e hora atual)
);

-- Criando a tabela Projeto para armazenar os projetos dos clientes
CREATE TABLE Projeto(
    id_projeto SERIAL PRIMARY KEY,  -- Identificador único do projeto
    altura DECIMAL(5,2) NOT NULL,  -- Altura do projeto (em metros)
    largura DECIMAL(5,2) NOT NULL,  -- Largura do projeto (em metros)
    peso_max DECIMAL(6,2) NOT NULL,  -- Peso máximo suportado pelo projeto (em kg)
    orcamento DECIMAL(10,2) NOT NULL,  -- Orçamento do projeto (em reais)
    data_projeto TIMESTAMP DEFAULT CURRENT_TIMESTAMP,  -- Data de criação do projeto
    status ENUM('pendente', 'aprovado', 'cancelado') NOT NULL DEFAULT 'pendente',  -- Status do projeto com valor padrão 'pendente'
    id_cliente INT REFERENCES Cliente(id_cliente),  -- Chave estrangeira referenciando Cliente
    id_desenvolvedor INT REFERENCES Desenvolvedor(id_desenvolvedor)  -- Chave estrangeira referenciando Desenvolvedor
);

-- Criando a tabela Desenvolvedor para armazenar informações dos desenvolvedores
CREATE TABLE Desenvolvedor(
    id_desenvolvedor SERIAL PRIMARY KEY,  -- Identificador único do desenvolvedor
    nome VARCHAR(255) NOT NULL,  -- Nome do desenvolvedor
    CPF VARCHAR(255) NOT NULL,  -- CPF do desenvolvedor
    email VARCHAR(255) UNIQUE NOT NULL  -- Email único do desenvolvedor
);

-- Criando a tabela Material para armazenar informações dos materiais usados nos projetos
CREATE TABLE Material(
    id_material SERIAL PRIMARY KEY,  -- Identificador único do material
    nome VARCHAR(255) UNIQUE NOT NULL,  -- Nome do material (único e obrigatório)
    fornecedor VARCHAR(255),  -- Nome do fornecedor do material (opcional)
    descricao VARCHAR(255) NOT NULL,  -- Descrição do material
    preco DECIMAL(12) NOT NULL  -- Preço do material
);

-- Criando a tabela Projeto_Material para associar materiais aos projetos
CREATE TABLE Projeto_Material(
    id_projeto INT REFERENCES Projeto(id_projeto),  -- Chave estrangeira referenciando Projeto
    id_material INT REFERENCES Material(id_material),  -- Chave estrangeira referenciando Material
    data_ini TIMESTAMP DEFAULT CURRENT_TIMESTAMP,  -- Data de início do uso do material no projeto
    quantidade INT(10) NOT NULL  -- Quantidade de material utilizado no projeto
);

-- Criando a tabela Aprovação para registrar a aprovação de projetos
CREATE TABLE APROVACAO(
    id_aprovacao SERIAL PRIMARY KEY,  -- Identificador único da aprovação
    data_aprovacao TIMESTAMP DEFAULT CURRENT_TIMESTAMP,  -- Data de aprovação do projeto
    id_projeto INT REFERENCES Projeto(id_projeto),  -- Chave estrangeira referenciando Projeto
    id_cliente INT REFERENCES Cliente(id_cliente)  -- Chave estrangeira referenciando Cliente
);
