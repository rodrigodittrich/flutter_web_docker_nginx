# Exemplo de projeto usando flutter para build com Docker

Projeto de exemplo em Flutter criado na plataform web para usar como exemplo a utilização do docker com nginx;

# Passos para subir o projeto utilizando o Docker

**Fazer o build da aplicação**
```bash
flutter buil web
```

**Construir a imagem**
```shell
docker build -t flutter-web:test .
```

**Executar o container**
```shell
docker run -d -p 8080:80 flutter-web:test
```

**Testar aplicação**  
Para testar a aplicação, acesse a página http://localhost:8080/