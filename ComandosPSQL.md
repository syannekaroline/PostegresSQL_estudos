# Comandos Básicos do Utilitário SQL

- psql --version 
    - mostra a versão atual do Postgres instalada
- psql --help
    - Mostra lista de opções de comando do slq


#### OBS : pode-se trabalhar no terminal de forma forma interativa 

## Entrar no psql :

- psql -u postgres

#### Postegres é o usuário root - adm - tem todas as permissões

- Prompt padrão : postgres=#

postgres se refere ao banco de dados padrão criado pelo postgres

* \password 
    - Mudar a senha : 
* \h
    - mostra os comandos disponíveis (sair pressionar q)

* \h (comando específico)
    - Mostra a ajuda do comando 
    - ex : \h creat role

* \? 
    - Mostra os comandos internos do psql

* \l 
    - Lista os bancos disponíveis

* \du
    - lista os usuários 
* \c <nome do banco>
    - conecta a outro banco de dados
    - ex: 
    - 
postgres=# \c northwind
You are now connected to database "northwind" as user "postgres".

* \d 
    - Mostra as tabelas do banco
    northwind=# \d
        - ex : 

                 List of relations
 Schema |          Name          | Type  |  Owner
--------+------------------------+-------+----------
 public | categories             | table | postgres
 public | customer_customer_demo | table | postgres
 public | customer_demographics  | table | postgres
 public | customers              | table | postgres
 public | employee_territories   | table | postgres
 public | employees              | table | postgres
 public | order_details          | table | postgres
 public | orders                 | table | postgres
 public | products               | table | postgres
 public | region                 | table | postgres
 public | shippers               | table | postgres
 public | suppliers              | table | postgres
 public | territories            | table | postgres
 public | us_states              | table | postgres
(14 rows)

* \dS 
    - Mostra as tabelas do sistema postgres - tabelas administrativas internas


* \! 
    - Volta pro terminal sem desconetar 
    - se der o comando "exit" voltra pro psql
    - Se pode tbm combinar os comandos. ex: \! date (vai mostrar a data do sistema )

