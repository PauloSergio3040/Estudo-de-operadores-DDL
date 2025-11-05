# 🧠 Script SQL - Laboratório de DDL e DML (MySQL)

Este projeto contém um **roteiro completo de comandos SQL** para prática de **criação, modificação e manutenção de bancos de dados MySQL**.  
O código foi escrito totalmente em minúsculas e cobre desde a modelagem inicial até automação com procedures.

---

## 📘 Objetivo
Demonstrar o uso dos principais comandos **DDL (Data Definition Language)** e **DML (Data Manipulation Language)**  
em um ambiente de estudo para quem está aprendendo **Banco de Dados** e **Administração de SGBDs**.

---

## 🧱 Estrutura do Script

### 1. Criação de Tabelas
- `funcionario`: informações pessoais dos colaboradores.  
- `salario`: valores salariais com chave estrangeira para `funcionario`.  
- `audit_salario`: registro de alterações de salário (auditoria).

### 2. Índices
- Criação de índices (`ix_func1`, `ix_func2`) para otimizar consultas.  
- Remoção e recriação de índices conforme necessidade.

### 3. Alterações Estruturais
- Inclusão, renomeação e exclusão de colunas (`genero`, `sexo`).  
- Alteração de tipos de dados e *engine* de tabelas.  
- Renomeação de tabelas (`funcionario` ↔ `pessoa`).  

### 4. Views
- Criação, alteração e exclusão da *view* `v_funcionario`.

### 5. Procedures
- Criação e execução da procedure `proc_quadrado`, que calcula o quadrado de um número.

### 6. Manutenção de Banco e Tabelas
- Criação e exclusão de *database* (`teste`).  
- Exclusão de tabelas, funções e triggers.  
- Uso de `truncate` para limpar registros.

### 7. Backup Temporário
- Criação de tabela temporária `tmp_funcionarios`.  
- Backup e restauração dos dados de `funcionarios`.  
- Teste de `auto_increment` com inserção de novo registro.

---

## 🧩 Tecnologias Utilizadas
- **MySQL 8.0+**
- **Workbench** ou qualquer cliente SQL compatível.

---

## ⚙️ Execução
1. Baixe o meu banco de nome "Curso" ou Crie um banco de dados de testes:
   ```sql
   create database teste;
   use teste;
