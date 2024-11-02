# Plano de Estudos SQLite para o Projeto GoySys

Este plano de estudos foi elaborado para proporcionar um aprendizado prático e progressivo de SQLite, com o objetivo de aplicar o conhecimento diretamente no desenvolvimento do projeto GoySys.

---

## Semana 1: Fundamentos do SQLite

### 1. Introdução e Instalação
- **Objetivo**: Entender o que é o SQLite, como ele funciona e como instalá-lo.
- **Atividades**:
  - Leia sobre o SQLite, suas características e vantagens.
  - Instale o SQLite no seu sistema Pop!_OS e configure-o para uso no terminal.
  - Experimente comandos básicos para iniciar e visualizar bancos de dados.

### 2. Criação e Manipulação de Tabelas
- **Objetivo**: Aprender a criar e configurar tabelas, estabelecendo os esquemas necessários para o GoySys.
- **Atividades**:
  - Crie tabelas básicas, como `funcionarios` e `clientes`, com campos como `id`, `nome`, `idade`, `cargo` etc.
  - Explore comandos para visualizar a estrutura da tabela (`PRAGMA table_info`).
  - Pratique alterações em tabelas, como adicionar e remover colunas.

---

## Semana 2: Operações CRUD

### 1. Inserção de Dados
- **Objetivo**: Aprender a inserir dados no banco de dados e aplicar isso nas tabelas do GoySys.
- **Atividades**:
  - Insira registros fictícios nas tabelas `funcionarios` e `clientes`.
  - Pratique com diferentes tipos de dados e valide as inserções.

### 2. Consulta de Dados (SELECT)
- **Objetivo**: Realizar consultas básicas para buscar informações, começando pelas tabelas criadas.
- **Atividades**:
  - Use `SELECT` para visualizar todos os registros em cada tabela.
  - Pratique consultas mais focadas, buscando registros específicos (por exemplo, todos os funcionários com idade acima de 30 anos).

### 3. Atualização e Exclusão de Dados
- **Objetivo**: Aprender a atualizar e excluir dados no banco de dados.
- **Atividades**:
  - Atualize registros específicos nas tabelas (`UPDATE`).
  - Exclua registros desnecessários ou duplicados (`DELETE`).
  - Crie um script de Python para automatizar essas operações básicas.

---

## Semana 3: Filtros, Ordenação e Relacionamentos

### 1. Filtros e Ordenação
- **Objetivo**: Realizar consultas complexas utilizando filtros e ordenação para manipular os dados.
- **Atividades**:
  - Utilize o `WHERE` para filtrar dados específicos, como cargos específicos ou clientes de certa faixa etária.
  - Pratique o uso de `ORDER BY` para ordenar os resultados em ordem alfabética, numérica, etc.
  - Teste a cláusula `LIMIT` para restringir o número de registros exibidos.

### 2. Relacionamento entre Tabelas
- **Objetivo**: Entender como relacionar tabelas no SQLite e aplicar isso ao banco do GoySys.
- **Atividades**:
  - Crie relacionamentos usando chaves estrangeiras. Por exemplo, se houver uma tabela de `projetos`, relacione-a com os `funcionarios`.
  - Faça consultas que usem `JOIN` para combinar dados de múltiplas tabelas, como mostrar todos os funcionários com os projetos que estão alocados.

---

## Semana 4: Integração do SQLite com Python

### 1. Conectando SQLite com Python
- **Objetivo**: Aprender a conectar-se ao SQLite usando Python e preparar a integração com o GoySys.
- **Atividades**:
  - Usando a biblioteca `sqlite3`, conecte-se ao seu banco de dados a partir de um script Python.
  - Crie uma função para realizar operações de consulta, inserção, atualização e exclusão diretamente no código Python.

### 2. Operações com Python
- **Objetivo**: Manipular dados no SQLite usando Python.
- **Atividades**:
  - Desenvolva uma interface simples para inserir dados nas tabelas `funcionarios` e `clientes` usando Python.
  - Faça operações como listar todos os funcionários ou buscar dados específicos.

### 3. Desenvolvendo Scripts para Automação
- **Objetivo**: Automatizar tarefas para facilitar o gerenciamento do banco de dados no GoySys.
- **Atividades**:
  - Crie scripts para operações comuns, como adicionar novos clientes, listar todos os funcionários e gerar relatórios básicos.
  - Teste o uso desses scripts na interface do GoySys, preparando para futuras integrações.

---

## Semana 5: Revisão e Prática no GoySys

### 1. Implementação no GoySys
- **Objetivo**: Integrar o SQLite no GoySys e adaptar o código existente para suportar o banco de dados.
- **Atividades**:
  - Crie a camada de banco de dados no GoySys e conecte os scripts de consulta, inserção, atualização e exclusão.
  - Teste funcionalidades básicas para assegurar que o GoySys está funcionando corretamente com o banco de dados.

### 2. Desafios e Ajustes
- **Objetivo**: Ajustar e otimizar o uso do banco de dados.
- **Atividades**:
  - Refine consultas e otimize as operações de banco de dados para melhorar a performance.
  - Ajuste os scripts e, se necessário, revise os esquemas das tabelas para garantir que o banco de dados atenda às necessidades do GoySys.

---

Esse plano cobre tanto a base teórica quanto a prática com SQLite e Python, tornando a experiência de aprendizado mais completa e aplicável ao seu projeto!
