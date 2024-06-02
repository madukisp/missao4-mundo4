<style>
.custom-font {
  font-family: 'Arial', sans-serif; 
  font-size: 16px;
}
</style>

<div class="custom-font">

<p align="center">
<img src="https://i.pinimg.com/originals/1a/21/6f/1a216fb0afdce66e7ffd9c9dbfce393b.jpg" alt="Logo do Projeto" width="200"/>
</p>
<h2 align="center">Desenvolvimento de Banco de Dados Azure SQL</h2>
<h3 align="center">LogiMove Transportes</h3>

* **Aluna:** Amanda Duque Kawauchi
* **Matrícula:** 202209170254
* **Campus:** Morumbi
* **Curso:** Desenvolvimento Full-Stack
* **Disciplina:** Nível 4: Tirando Proveito da Nuvem Para Projetos de Software
* **Turma:** 2024.1
* **Semestre Letivo:** 4º Semestre
* **Repositório GitHub:** [Link do Repositório GitHub](https://github.com/madukisp/missao4-mundo4)

## Objetivo da Prática

Este projeto tem como objetivo o desenvolvimento de um banco de dados no Azure SQL para a empresa LogiMove Transportes. O intuito é migrar de um sistema baseado em papel para uma solução digital, utilizando autenticação digital para melhor coordenação e rastreamento de remessas.

## Análise e Conclusão

### Funcionalidades Implementadas

O banco de dados implementa uma estrutura robusta e segura para armazenar informações cruciais da empresa. As funcionalidades incluem:

- **Tabela de Motoristas (Drivers)**: Armazena informações pessoais e de contato dos motoristas.
- **Tabela de Clientes (Clients)**: Armazena detalhes dos clientes, incluindo informações de contato e empresa.
- **Tabela de Pedidos (Orders)**: Armazena informações sobre os pedidos, como detalhes, datas de entrega e status.

### Navegação e Interatividade

Utilizamos o Azure Data Studio para a criação e gerenciamento das tabelas, inserção e consulta de dados, além da realização de operações CRUD (Create, Read, Update, Delete).

### Desafios Encontrados

Alguns dos desafios enfrentados incluíram a configuração inicial do ambiente Azure, a definição das relações entre tabelas e a garantia da integridade referencial dos dados. A configuração de autenticação e segurança no Azure SQL também foi um ponto crucial para garantir a proteção dos dados.

### Conclusões

O desenvolvimento do banco de dados no Azure SQL permitiu a aplicação prática de conceitos como criação e gerenciamento de tabelas, integração de dados, e realização de operações CRUD. O projeto consolidou o conhecimento sobre o Azure SQL, destacando sua eficiência e flexibilidade para o desenvolvimento de soluções de banco de dados na nuvem.

## Imagens do Projeto

### Configuração do Ambiente Azure

1. **Portal do Azure - Visão Geral**:
   ![Visão Geral do Servidor SQL](https://raw.githubusercontent.com/madukisp/missao4-mundo4/main/Images/01.png?token=GHSAT0AAAAAACQRPOXZVH3KMENTDNFNUQBIZS45LTQ)

   - Esta imagem mostra a visão geral do servidor SQL `amlogimoveserver`, incluindo informações sobre o grupo de recursos, assinatura, localização e administrador.

### Design do Banco de Dados

2. **Tabela de Clientes**:
   ![Tabela de Clientes](https://raw.githubusercontent.com/madukisp/missao4-mundo4/main/Images/02.png?token=GHSAT0AAAAAACQRPOXZF3LSFL6K433JFHR6ZS45N3Q)
   - Esta imagem mostra a estrutura da tabela `Clientes` no Azure Data Studio, com os campos `ClientID`, `Nome`, `Empresa`, `Endereço`, e `Contato`.

3. **Tabela de Motoristas**:
   ![Tabela de Motoristas](https://raw.githubusercontent.com/madukisp/missao4-mundo4/main/Images/03.png?token=GHSAT0AAAAAACQRPOXYF5CDGKPB4FKZWUUUZS45OJQ)
   - Esta imagem mostra a estrutura da tabela `Motoristas` no Azure Data Studio, com os campos `MotoristaID`, `Nome`, `CNH`, `Telefone`, `DataNascimento`, e `HistoricoViagens`.

4. **Tabela de Pedidos**:
   ![Tabela de Pedidos](https://raw.githubusercontent.com/madukisp/missao4-mundo4/main/Images/04.png?token=GHSAT0AAAAAACQRPOXZOHIACYNFTIDDRVMSZS45OXQ)
   - Esta imagem mostra a estrutura da tabela `Pedidos` no Azure Data Studio, com os campos `OrderID`, `ClientID`, `DriverID`, `DetalhesPedido`, `DataEntrega`, e `Status`.

### Implementação do Banco de Dados

5. **Inserção de Dados na Tabela `Drivers`**:
   ![Inserção de Dados na Tabela Drivers](https://raw.githubusercontent.com/madukisp/missao4-mundo4/main/Images/05.png?token=GHSAT0AAAAAACQRPOXZCH7TK57GBWCAJP42ZS45PGQ)
   - Esta imagem mostra a inserção de dados na tabela `Drivers`, incluindo a execução bem-sucedida do comando SQL.

6. **Inserção de Dados na Tabela `Clients`**:
   ![Inserção de Dados na Tabela Clients](https://raw.githubusercontent.com/madukisp/missao4-mundo4/main/Images/06.png?token=GHSAT0AAAAAACQRPOXYMZOQCU5CORUF7TZ2ZS45PVQ)
   - Esta imagem mostra a inserção de dados na tabela `Clients`, incluindo a execução bem-sucedida do comando SQL.

7. **Inserção de Dados na Tabela `Orders`**:
   ![Inserção de Dados na Tabela Orders](https://raw.githubusercontent.com/madukisp/missao4-mundo4/main/Images/07.png?token=GHSAT0AAAAAACQRPOXYFR2UWK6CRC3XRPJKZS45QCA)
   - Esta imagem mostra a inserção de dados na tabela `Orders`, incluindo a execução bem-sucedida do comando SQL.

### Consultas de Dados

8. **Consulta na Tabela `Drivers`**:
   ![Consulta na Tabela Drivers](https://raw.githubusercontent.com/madukisp/missao4-mundo4/main/Images/08.png?token=GHSAT0AAAAAACQRPOXY5TCH47H65JPNG26SZS45QSQ)
   - Esta imagem mostra a consulta dos dados inseridos na tabela `Drivers`.

9. **Consulta na Tabela `Clients`**:
   ![Consulta na Tabela Clients](https://raw.githubusercontent.com/madukisp/missao4-mundo4/main/Images/09.png?token=GHSAT0AAAAAACQRPOXZ3GJR7UFWESHCRAXYZS45Q6Q)
   - Esta imagem mostra a consulta dos dados inseridos na tabela `Clients`.

10. **Consulta na Tabela `Orders`**:
    ![Consulta na Tabela Orders](https://raw.githubusercontent.com/madukisp/missao4-mundo4/main/Images/10.png?token=GHSAT0AAAAAACQRPOXY7P3JCWIPF5BRCK4QZS45RGA)
    - Esta imagem mostra a consulta dos dados inseridos na tabela `Orders`.

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

### Consulta de Dados

```sql
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

### Deletar Dados

```sql
-- Deletar um pedido
DELETE FROM Orders
WHERE OrderID = 16;
```
</div>
