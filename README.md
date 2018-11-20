#Proyecto de ejemplo de Spring Boot

- Empaquetado: mvn package
- Arranque del proyecto como es habitual: java -jar target/demo-spring-boot-2-0.0.1-SNAPSHOT.jar
- Accede a la URL: [http://localhost:8080/](http://localhost:8080/)
## API Básico
- Puedes añadir un usuario con la URL: [http://localhost:8080/demo/add?name=First&email=someemail@someemailprovider.com](http://localhost:8080/demo/add?name=First&email=someemail@someemailprovider.com)
- O también ejecutando el comando curl: curl 'localhost:8080/demo/add?name=First&email=someemail@someemailprovider.com'
- Listado de usuarios: [http://localhost:8080/users/](http://localhost:8080/users/) 

## API de Customers
- url  base: [http://localhost:8080/customer](http://localhost:8080/customer)