## Informações sobre os containers e imagens das aplicações

### Executar aplicações, e baixar dependências
  - Clonar o repositório ```https://github.com/sistemascorporativos3a/docker``` em sua máquina local e executar o comando:

  ```
  # docker-compose up
  ```

  - Observações: 
    - Adicionar o parâmetro "-d" ao comando abaixo para executar em modo background;
    - Para não executar todos os containers de uma vez só, utilize o caracter "#" e comente os módulos que não necessários;
    - Lista de comandos úteis no Docker:
      ```
      # docker ps
      # docker images
      # docker rmi -f {id}
      # docker exec -it {imagem} bash
      # docker stop {container}
      # docker-compose down
      ```

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
    
### Endereço das aplicações

  - Módulo admin: http://localhost:8091/
  - Módulo compras: http://localhost:8092/
  - Módulo inventário: http://localhost:8093/
  - Módulo produtos: http://localhost:8094/
  - Módulo rh: http://localhost:8096/
  
  * Observações*: As rotas das aplicações estão nos arquivos README.md dos repositórios
