# Comandos Básicos do SQLite

Este guia fornece uma visão geral dos comandos básicos para iniciar e visualizar bancos de dados no SQLite, ideal para iniciantes.

## 1. Abrir o SQLite e Carregar um Banco de Dados

Para abrir o SQLite e carregar um banco de dados existente, use o seguinte comando no terminal:

```bash
sqlite3 nome_do_banco.db
```

> **Nota**: Certifique-se de que está no diretório onde o arquivo do banco de dados está localizado ou forneça o caminho completo, como `/caminho/para/nome_do_banco.db`.

---

## 2. Visualizar Todas as Tabelas do Banco de Dados

Após abrir o banco de dados, você pode listar todas as tabelas com o comando:

```sql
.tables
```

Esse comando mostra todas as tabelas que estão no banco de dados atualmente, dando uma visão geral do conteúdo armazenado.

---

## 3. Visualizar a Estrutura de uma Tabela Específica

Para ver a estrutura de uma tabela, incluindo os nomes das colunas e seus tipos, use o comando `.schema` seguido do nome da tabela:

```sql
.schema nome_da_tabela
```

Por exemplo:

```sql
.schema funcionarios
```

Esse comando exibe o SQL usado para criar a tabela, incluindo todos os campos e seus tipos de dados.

---

## 4. Exibir Todos os Dados de uma Tabela

Para visualizar todos os dados contidos em uma tabela, use o comando `SELECT *` seguido do nome da tabela:

```sql
SELECT * FROM nome_da_tabela;
```

Por exemplo:

```sql
SELECT * FROM funcionarios;
```

Esse comando exibe todas as linhas e colunas da tabela selecionada.

---

## 5. Ativar Exibição de Cabeçalhos de Coluna

No SQLite, por padrão, os cabeçalhos (nomes das colunas) não são exibidos. Para ativar a exibição de cabeçalhos, use o comando:

```sql
.headers on
```

Com essa configuração ativada, os resultados das consultas incluirão os nomes das colunas.

---

## 6. Formatar o Modo de Saída

Para ajustar o formato de saída dos dados no terminal, use o comando `.mode`. Aqui estão alguns modos úteis:

- **Modo Column**: organiza os dados em colunas, melhorando a legibilidade. Recomendado para tabelas com poucos campos e linhas.

  ```sql
  .mode column
  ```

- **Modo CSV**: exporta os dados no formato CSV. Útil para copiar dados para outras ferramentas.

  ```sql
  .mode csv
  ```

---

## Exemplo de Uso Completo

Aqui está um exemplo de uso completo combinando todos os comandos acima:

1. Abra o banco de dados:

   ```bash
   sqlite3 nome_do_banco.db
   ```

2. Liste todas as tabelas:

   ```sql
   .tables
   ```

3. Veja a estrutura da tabela `funcionarios`:

   ```sql
   .schema funcionarios
   ```

4. Ative os cabeçalhos e o modo de coluna:

   ```sql
   .headers on
   .mode column
   ```

5. Exiba todos os dados da tabela `funcionarios`:

   ```sql
   SELECT * FROM funcionarios;
   ```

---

Esses comandos básicos são o ponto de partida para explorar e entender um banco de dados no SQLite. Com eles, você estará pronto para executar consultas e análises mais avançadas.
```

Esse conteúdo em Markdown pode ser adicionado ao seu repositório para consulta rápida e serve como uma boa referência para iniciantes no SQLite.
