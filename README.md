# Docker WordPress Template

## Prepare the project

- Ajuste as variáveis ambiente no `.env`.  
  > Exemplo:
  ```
  MYSQL_ROOT_PASSWORD=password
  DB_USER=wordpress
  DB_PASSWORD=wordpress
  DB_NAME=nome-do-projeto
  ```
- Ajuste as configurações de upload no `uploads.ini`.

## Build the project
```
docker-compose up -d
```

## Shutdown and cleanup

- Remove os containers e network, mas preserva o banco de dados do WordPress.
  ```
  docker compose down
  ```

- Remove os containers, network e banco de dados do WordPress.
  ```
  docker compose down --volumes
  ```

## References

- [Official Sample - Quickstart: Compose and WordPress](https://github.com/docker/awesome-compose/tree/master/official-documentation-samples/wordpress/)
- [YouTube: Quick Wordpress Setup With Docker](https://youtu.be/pYhLEV-sRpY)