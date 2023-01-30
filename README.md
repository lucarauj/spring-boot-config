## Spring Boot Profiles

- Multiplos ambiente: desenvolvimento, teste, produção

### Configurando ```application.properties```:
```
spring.profiles.active=prod ou dev
spring.application.name=Spring Boot Configuration Project
```

### Configurando ```application-dev.properties```:
```
app.message=This is the property file fo the ${spring.application.name} specific to DEV Enviroment

spring.datasource.driver-class-name=org.h2.Driver
spring.datasource.url=jdbc:h2:mem:db;DB_CLOSE_DELAY=-1
spring.datasource.username=sa
spring.datasource.password=sa
```

### Configurando ```application-prod.properties```:
```
app.message=This is the property file fo the ${spring.application.name} specific to PROD Enviroment

spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.datasource.url=<MYSQL_URL>
spring.datasource.username=<USERNAME>
spring.datasource.password=<PASSWORD>
```

## Anotações

- @Configuration: utilizada na classe de configuração do banco de dados
- @ConfigurationProperties: utilizada para fazer o mapeamento de um grupo de propriedades
- @Bean: mostra o conteúdo sendo mapeado na subida do sistema
- @RestController
- @Value: injeção de valores 
- @Profile
- @Getter
- @Setter
- @GetMapping


## Configurações com YAML ```application-dev.yml```

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





## Configurações com variáveis de ambiente

- mvn spring-boot:run
- export ENV_DB_URL=jdbc:h2:mem:db;DB_CLOSE_DELAY=-1
- mvn spring-boot:run
 