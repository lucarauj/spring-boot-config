[![NPM](https://img.shields.io/npm/l/react)](https://github.com/lucarauj/spring-boot-config/blob/main/LICENSE)

<h1 align="center"> Spring Boot Profiles </h1>
<h2 align="center"> Multiplos ambientes: </h2>
<h3 align="center"> desenvolvimento, teste, produção </h3>

<br>

### 🛠 Configurando ```application.properties```:
```
spring.profiles.active=prod {OU} dev
spring.application.name=Spring Boot Configuration Project
```

### 🛠 Configurando ```application-dev.properties```:
```
app.message=This is the property file fo the ${spring.application.name} specific to DEV Enviroment

spring.datasource.driver-class-name=org.h2.Driver
spring.datasource.url=jdbc:h2:mem:db;DB_CLOSE_DELAY=-1
spring.datasource.username=sa
spring.datasource.password=sa
```

### 🛠 Configurando ```application-prod.properties```:
```
app.message=This is the property file fo the ${spring.application.name} specific to PROD Enviroment

spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.datasource.url=<MYSQL_URL>
spring.datasource.username=<USERNAME>
spring.datasource.password=<PASSWORD>
```
### 📝 Anotações utilizadas no projeto:

- @Configuration: indica que a classe possui métodos que expõe novos beans;
- @ConfigurationProperties: utilizada para fazer o mapeamento de um grupo de propriedades;
- @Bean: indica que o Spring deve invocar aquele método e gerenciar o objeto retornado por ele;
- @RestController: marca a classe como um controlador onde cada método retorna um objeto de domínio em vez de uma visão;
- @Value: serve para injetar valores de propriedades nos componentes;
- @Profile: indica em qual profile tal bean deve ser carregado;
- @Getter: criação dos métodos para todos os atributos da classe através do lombok;
- @Setter: criação dos métodos para todos os atributos da classe através do lombok;
- @GetMapping: usada para mapear solicitações HTTP GET em métodos manipuladores específicos;


### Configurações com YAML ```application-dev.yml```

```
app:
message: This is the property file fo the ${spring.application.name} specific to DEV Enviroment

spring:
datasource:
driver-class-name: org.h2.Driver
url: jdbc:h2:mem:db;DB_CLOSE_DELAY=-1
username: sa
password: sa
```

### Configurações com variáveis de ambiente

- Comando 👉 mvn spring-boot:run
- Comando 👉 export ENV_DB_URL=jdbc:h2:mem:db;DB_CLOSE_DELAY=-1
- Comando 👉 mvn spring-boot:run


## 🚀 Tecnologias

Esse projeto foi desenvolvido com as seguintes tecnologias:
<div style="display: inline_block"><br>
<img align="center" alt="Lucarauj-Java" height="50" width="60" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg">
<img align="center" alt="Lucarauj-Springboot" height="70" width="200" src="https://github.com/lucarauj/assets/blob/main/SpringBoot.jpeg">          

</div>

## Aluno

Lucas Araujo

<a href="https://www.linkedin.com/in/lucarauj"><img alt="lucarauj | LinkdeIN" width="40px" src="https://user-images.githubusercontent.com/43545812/144035037-0f415fc7-9f96-4517-a370-ccc6e78a714b.png" /></a>









 
