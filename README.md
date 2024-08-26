## Instalação

1. Para garantir a funcionalidade da aplicação, intale o GO
   [https://go.dev/](https://go.dev/)

## Uso (API)
Para executar o projeto localmente, use o seguinte comando:

```bash
go run cmd/gobook/main.go
```

Com isso sua aplicação já estará rodando com um sqlite local, apontando para a porta 8080

## Post
```bash
http://localhost:8080/books

{
  "title": ""
  "author": ""
  "genre": ""
}
```

## Get List
```bash
http://localhost:8080/books
```

## Get by ID
```bash
http://localhost:8080/books/{id}
```

## Put
```bash
http://localhost:8080/books/{id}
```

## Delete
```bash
http://localhost:8080/books/{id}
```

## Uso (CMD)
Para executar o projeto localmente, use o seguinte comando:

Usando "search", você busca os livros que possuem o título, e retorna a descrição de cada um.
Usando "simulate", você simula a leitura de vários livros em um tempo de 2segundos usando Goroutines e Channels.

OBS -> Executar somente se estiver com livros cadastrados.

```bash
go run cmd/gobook/main.go search <book title>
```
```bash
go run cmd/gobook/main.go simulate <book_id> <book_id> <book_id> ...
```
