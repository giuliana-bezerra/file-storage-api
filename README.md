<h1 align="center">
  File Storage API
</h1>

<p align="center">
 <img src="https://img.shields.io/static/v1?label=Youtube&message=@giulianabezerra&color=8257E5&labelColor=000000" alt="@giulianabezerra" />
 <img src="https://img.shields.io/static/v1?label=Tipo&message=Tutorial&color=8257E5&labelColor=000000" alt="Tutorial" />
</p>

Tutorial apresentado [nesse vídeo](https://youtu.be/b6kvS1Wszew?si=BAFcEpAqP6Pw4qMu) para ilustrar como implementar um servidor de armazenamento de arquivos utilizando Spring Boot.

## Tecnologias
 
- [Spring Boot](https://spring.io/projects/spring-boot)
- [Spring MVC](https://docs.spring.io/spring-framework/reference/web/webmvc.html)

## Como Executar

- Clonar repositório git:
```
git clone https://github.com/giuliana-bezerra/file-storage-api.git
```
- Construir o projeto:
```
./mvnw clean package
```
- Executar:
```
java -jar ./target/file-storage-api-0.0.1-SNAPSHOT.jar
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