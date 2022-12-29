https://grpc.io/docs/languages/go/quickstart/

protoc --go_out=. --go-grpc_out=. proto/course_category.proto


usando cliente para usar o server em gRPC e testar com evans
https://github.com/ktr0731/evans

rodando cliente 
$ evans -r repl

create table categories (id string, name string, description string);