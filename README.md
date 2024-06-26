<div class="custom-font">

<p align="center">
<img src="https://i.pinimg.com/originals/1a/21/6f/1a216fb0afdce66e7ffd9c9dbfce393b.jpg" alt="Logo do Projeto" width="200"/>
</p>
<h2 align="center">Desenvolvimento de Banco de Dados Azure SQL</h2>
<h3 align="center">LogiMove Transportes</h3>

## Objetivo da Prática

Este projeto tem como objetivo o desenvolvimento de um banco de dados no Azure SQL para a empresa LogiMove Transportes. O intuito é migrar de um sistema baseado em papel para uma solução digital, utilizando autenticação digital para melhor coordenação e rastreamento de remessas.

## Funcionalidades Implementadas

O banco de dados implementa uma estrutura robusta e segura para armazenar informações cruciais da empresa. As funcionalidades incluem:

- **Tabela de Motoristas (Drivers)**: Armazena informações pessoais e de contato dos motoristas.
- **Tabela de Clientes (Clients)**: Armazena detalhes dos clientes, incluindo informações de contato e empresa.
- **Tabela de Pedidos (Orders)**: Armazena informações sobre os pedidos, como detalhes, datas de entrega e status.

## Navegação e Interatividade

Utilizamos o Azure Data Studio para a criação e gerenciamento das tabelas, inserção e consulta de dados, além da realização de operações CRUD (Create, Read, Update, Delete).

## Desafios Encontrados

Alguns dos desafios enfrentados incluíram a configuração inicial do ambiente Azure, a definição das relações entre tabelas e a garantia da integridade referencial dos dados. A configuração de autenticação e segurança no Azure SQL também foi um ponto crucial para garantir a proteção dos dados.

## Conclusão

O desenvolvimento do banco de dados no Azure SQL permitiu a aplicação prática de conceitos como criação e gerenciamento de tabelas, integração de dados, e realização de operações CRUD. O projeto consolidou o conhecimento sobre o Azure SQL, destacando sua eficiência e flexibilidade para o desenvolvimento de soluções de banco de dados na nuvem.

## Comandos SQL Utilizados

### Criação das Tabelas

```sql
CREATE TABLE Drivers (
    DriverID INT PRIMARY KEY IDENTITY(1,1),
    Nome VARCHAR(100),
    CNH VARCHAR(20),
    Endereço VARCHAR(200),
    Contato VARCHAR(50)
);

CREATE TABLE Clients (
    ClientID INT PRIMARY KEY IDENTITY(1,1),
    Nome VARCHAR(100),
    Empresa VARCHAR(100),
    Endereço VARCHAR(200),
    Contato VARCHAR(50)
);

CREATE TABLE Orders (
    OrderID INT PRIMARY KEY IDENTITY(1,1),
    ClientID INT,
    DriverID INT,
    DetalhesPedido TEXT,
    DataEntrega DATE,
    Status VARCHAR(50),
    FOREIGN KEY (ClientID) REFERENCES Clients(ClientID),
    FOREIGN KEY (DriverID) REFERENCES Drivers(DriverID)
);
```

### Inserção de Dados

```sql	
## Inserção de Dados

-- Inserir dados na tabela Drivers
INSERT INTO Drivers (Nome, CNH, Endereço, Contato)
VALUES 
('João Silva', '1234567890', 'Rua A, 123, São Paulo, SP', '11987654321'),
('Carlos Santos', '9876543210', 'Rua B, 456, Rio de Janeiro, RJ', '21987654321'),
('Ana Oliveira', '1122334455', 'Avenida C, 789, Belo Horizonte, MG', '31987654321');

-- Inserir dados na tabela Clients
INSERT INTO Clients (Nome, Empresa, Endereço, Contato)
VALUES 
('Maria Souza', 'Empresa X', 'Av. B, 456, São Paulo, SP', '11987654322'),
('Pedro Lima', 'Empresa Y', 'Rua D, 123, Curitiba, PR', '41987654323'),
('Juliana Costa', 'Empresa Z', 'Avenida E, 789, Salvador, BA', '71987654324');

-- Inserir dados na tabela Orders
INSERT INTO Orders (ClientID, DriverID, DetalhesPedido, DataEntrega, Status)
VALUES 
(10, 9, 'Entrega de Documentos', '2024-06-10', 'Em Progresso'),
(11, 10, 'Entrega de Mercadorias', '2024-06-12', 'Pendente'),
(12, 11, 'Entrega de Equipamentos', '2024-06-15', 'Concluído');
```

### Consultar dados da tabela Drivers

```
-- Consultar dados da tabela Drivers
SELECT * FROM Drivers;

-- Consultar dados da tabela Clients
SELECT * FROM Clients;

-- Consultar dados da tabela Orders
SELECT * FROM Orders;
```

### Atualização de Dados

```sql
-- Atualizar o status de um pedido
UPDATE Orders
SET Status = 'Entregue'
WHERE OrderID = 16;
```

### Exclusão de Dados

```sql
-- Excluir um motorista
DELETE FROM Drivers
WHERE DriverID = 10;

-- Excluir um cliente
DELETE FROM Clients
WHERE ClientID = 12;

-- Excluir um pedido
DELETE FROM Orders
WHERE OrderID = 16;
```



