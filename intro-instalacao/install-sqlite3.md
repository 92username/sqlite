# Instalação do SQLite via Linha de Comando

Este guia descreve o processo de instalação do SQLite no terminal de sistemas Linux.

## Requisitos

- Sistema operacional Linux (Ubuntu, Pop!_OS, etc.)
- Acesso ao terminal com permissões de administrador

## Passo a Passo

1. **Atualize os pacotes do sistema**

   Antes de instalar, é recomendável atualizar o gerenciador de pacotes do sistema para garantir que você está instalando a versão mais recente disponível.

   ```bash
   sudo apt update
   sudo apt upgrade -y
   ```

2. **Instale o SQLite**

   No Ubuntu ou distribuições baseadas em Debian (como Pop!_OS), você pode instalar o SQLite diretamente com o seguinte comando:

   ```bash
   sudo apt install sqlite3 -y
   ```

3. **Verifique a instalação**

   Após a instalação, confirme que o SQLite foi instalado corretamente verificando a versão:

   ```bash
   sqlite3 --version
   ```

   Você verá uma saída similar a:

   ```
   3.31.1 2020-01-27 19:55:54 5b8c1fa146d5e4b00e1c2bc6f19b1
   ```

## Primeiros Passos com o SQLite

1. **Inicie o SQLite**

   Para começar a usar o SQLite, basta iniciar o terminal SQLite com o comando:

   ```bash
   sqlite3
   ```

   Você verá o prompt do SQLite, onde poderá começar a executar comandos SQL:

   ```plaintext
   SQLite version 3.31.1 2020-01-27 19:55:54
   Enter ".help" for usage hints.
   sqlite>
   ```

2. **Criando um banco de dados**

   Para criar um banco de dados, execute o seguinte comando:

   ```bash
   sqlite3 nome_do_banco.db
   ```

   Isso criará um arquivo `nome_do_banco.db` no diretório atual e abrirá o terminal do SQLite.

3. **Saindo do SQLite**

   Para sair do terminal do SQLite, digite:

   ```sql
   .exit
   ```

## Comandos Úteis

- **`.help`**: Lista de comandos disponíveis no terminal SQLite.
- **`.tables`**: Lista todas as tabelas no banco de dados atual.
- **`.schema`**: Mostra o esquema de uma tabela específica.
- **`.quit`** ou **`.exit`**: Sai do terminal SQLite.

## Documentação Adicional

Para mais informações sobre o SQLite e todos os comandos suportados, consulte a [documentação oficial do SQLite](https://www.sqlite.org/docs.html).

## Desinstalando o SQLite

Se precisar remover o SQLite, execute o seguinte comando:

```bash
sudo apt remove sqlite3 -y
```

E para remover qualquer dependência não usada:

```bash
sudo apt autoremove -y
```

---

Pronto! Agora você está com o SQLite instalado e pronto para usar em seu sistema Linux.
```