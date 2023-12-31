<h1 align="center">
  API GERENCIAMENTO DE ARQUIVOS
</h1>
Api para realizar uploads e downloads de arquivos feita com spring boot

## Tecnologias
 
- [Spring Boot](https://spring.io/projects/spring-boot)
- [Spring MVC](https://docs.spring.io/spring-framework/reference/web/webmvc.html)

## Como Executar

- Clonar repositório git:
```
git clone https://github.com/Gabrielcamargos28/Api_Gerenciamento_De_Arquivos.git
```
- Construir o projeto:
```
./mvnw clean package
```
- Executar:
```
java -jar ./target/Gerenciamento-0.0.1-SNAPSHOT.jar
```

## Testando Endpoints

- Upload file:
```
curl -X POST -F "file=@path/to/your/file.txt" http://localhost:8080/api/files/upload
```
- Download file:
```
curl -OJL http://localhost:8080/api/files/download/your-file-name.txt
```
- List uploaded files:
```
curl http://localhost:8080/api/files/list
```
