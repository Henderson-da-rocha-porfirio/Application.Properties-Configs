# application.properties---exemplos
## Verifique as Branches para ver os exemplos necessários
### Trabalhando Com Profiles:
### 1. Ativando o Profile por linha de comando(exemplo):
````
java -jar target/tuyofood-0.0.1-SNAPSHOT.jar --spring.profiles.active=product
````
### 2. Ativando o Profile por Variável de Ambiente(exemplo):
#### a. Windows:
````
set SPRING_PROFILES_ACTIVE=production
````
#### b. Linux e Mac:
````
export SPRING_PROFILES_ACTIVE=production
````
#### 3. @Profile + application.properties: Serve para mostrar a mudança de ambiente:
````
spring.profiles.active=prod,mysql,filesystem
ou
spring.profiles.active=dev,postgresql,S3
ou
spring.profiles.active=prod
ou
spring.profiles.active=dev
````
#### 4. Configurando pela VM options:
##### a. Vá em Run Configuration(onde se faz a modificação da configuration)
##### b. Edit Configurations
##### c. Modify options
##### d. Em Java, selecione Add VM options
##### e. Adicionar o perfil que deseja com o comando:
````
-Dspring.profiles.active=dev
 ou 
-Dspring.profiles.active=prod
````
##### e. 'dev' ou 'prod' estão apenas como exemplo.
