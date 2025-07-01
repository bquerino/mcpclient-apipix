# MCP Client API PIX

Este projeto demonstra um client simples do Model Context Protocol (MCP) para consumir a API Pix. A aplicação foi criada com Spring Boot 3 e Java 21 utilizando o *mcp-client-boot-starter*.

## Arquitetura

A estrutura do repositório segue o mesmo modelo do [mcpserver-apipix](https://github.com/bquerino/mcpserver-apipix):

- **app/** – código da aplicação Spring Boot.
- **docs/** – documentação e diagramas.
- **infra/** – arquivos de infraestrutura.

## Build e execução local

Para rodar localmente é necessário ter Java 21 e Maven instalados. Execute os comandos dentro do diretório `app`:

```bash
mvn spring-boot:run
```

Também é possível gerar o JAR e executá-lo manualmente:

```bash
mvn package
java -jar target/mcpclient-apipix-0.0.1-SNAPSHOT.jar
```

## Configuração

O arquivo `app/src/main/resources/application.yml` possui a URL do servidor MCP a ser utilizado:

```yaml
mcp:
  client:
    server-url: http://localhost:8080
```

## Licença

Este projeto é fornecido apenas para fins de demonstração e depende de bibliotecas MCP externas que não estão disponíveis neste ambiente off-line.
