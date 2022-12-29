# Descrição do projeto:
Esse projeto faz parte do curso Go Expert da [FullCycle](https://fullcycle.com.br/). Foi desevolvido a partir dos aprendizados de como construir um servidor gRPC.<br>
O servidor possui uma comunicação em binário via http2.
<br><br>
<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/ClaudionorJunior/go-expert-grpc">

# Rodando o projeto:
```sh
cd cmd/server && go run main.go
```

# Configurando o DB:
```sh
cd cmd/server && sqlite3 data.db
create table categories (id string, name string, description string);
```

# Instalação de protoc gRPC para Go:
[gRPC para go](https://grpc.io/docs/languages/go/quickstart/)

# Testando o servidor gRPC com Evans:
- Poderá fazer chamadas no servidor com o client evans.
[Leia mais aqui](https://github.com/ktr0731/evans)

***Executando evans***
```sh
evans -r repl
```
***Aplicando `service` CategoryService***
```sh
service CategoryService
```

***Chamando um método especifico do gRPC de CategoryService***
- Criando Category
```sh
call CreateCategory
```
- Listando todas as Categories
```sh
call ListCategories
```
- Buscando uma Category por ID
```sh
call GetCategory
```
- Stream de Category retornando Categories
```sh
call CreateCategoryStream
```
- Stream bidirectional de Category retornando Category sem fechar o canal
```sh
call CreateCategoryStreamBidirectional
```

## Autor
<table>
  <tr>
    <th><img src="https://avatars.githubusercontent.com/u/82416762?v=4" width=60></th>
  </tr>
  <tr>
    <td><a href="https://github.com/ClaudionorJunior">Github</a></td>
  </tr>
  <tr>
    <td><a href="https://www.linkedin.com/in/claudionorsilva">Linkedin</a></td>
  </tr>
</table>
