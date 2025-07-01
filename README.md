# MCP Client ApiPix

Este projeto é um exemplo simples de **client** do [Model Context Protocol](https://modelcontextprotocol.io/) para a ApiPix. Foi criado a partir do guia de quickstart que utiliza o *mcp-client-boot-starter*.

## Estrutura

O projeto segue uma estrutura de aplicação Spring Boot:

```
.
├── pom.xml
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com
│   │   │       └── example
│   │   │           └── mcpclientapipix
│   │   │               └── McpclientApipixApplication.java
│   │   └── resources
│   │       └── application.yml
```

## Como executar

1. Certifique-se de possuir o JDK 17+ e o Maven instalados.
2. Compile o projeto:

```bash
mvn package
```

3. Execute a aplicação:

```bash
java -jar target/mcpclient-apipix-0.0.1-SNAPSHOT.jar
```

A aplicação iniciará e tentará se conectar ao servidor MCP configurado em `application.yml`.

## Configuração

O arquivo `src/main/resources/application.yml` possui uma configuração mínima com a URL do servidor MCP. Ajuste este valor conforme sua necessidade.

```
mcp:
  client:
    server-url: http://localhost:8080
```

## Licença

Este projeto está disponibilizado sem garantia de funcionamento pois depende das dependências externas do MCP que não estão disponíveis neste ambiente off-line.
