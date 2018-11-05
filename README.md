## Informações sobre os containers e imagens das aplicações

### Executar aplicações, e baixar dependências
  - Clonar o repositório ```https://github.com/sistemascorporativos3a/docker``` em sua máquina local e executar o comando:

  ```
  # docker-compose up
  ```

  - Observações: 
    - Adicionar o parâmetro "-d" ao comando abaixo para executar em modo background
    - Para não executar todos os containers de uma vez só, utilize o caracter "#" e comente os módulos que não necessários

### Repositório dos containers

https://hub.docker.com/u/sistemasdeinformacao/

- Imagens:
  ```
  sistemasdeinformacao/mysql-adventure-works
  sistemasdeinformacao/modulo-admin
  sistemasdeinformacao/modulo-compras
  sistemasdeinformacao/modulo-inventario
  sistemasdeinformacao/modulo-produtos
  sistemasdeinformacao/modulo-rh
  ```

- Dependências:
  ```
  mysql:5.6
  rabbitmq:3-management
  springcloud/eureka
  ```

### Acesso ao container MySQL para executar comandos SQL, caso necessário
  ```
  # docker exec -it mysql-adventure-works bash
  #  mysql -u root -p
  #  > SHOW DATABASES;
  #  > exit;
  ```
  - Observações:
    - Usuário: root
    - Senha:   root
