#Proyecto de ejemplo de Spring Boot

- Empaquetado: mvn package
- Arranque del proyecto como es habitual: java -jar target/demo-spring-boot-2-0.0.1-SNAPSHOT.jar
- Accede a la URL: [http://localhost:8080/](http://localhost:8080/)
## API Básico
- Listado de usuarios: [http://localhost:8080/users/](http://localhost:8080/users/)
  - [Formato de salida HAL JSON: API REST Standar](http://stateless.co/hal_specification.html) 
- Puedes añadir un usuario con la URL: [http://localhost:8080/demo/add?name=First&email=someemail@someemailprovider.com](http://localhost:8080/demo/add?name=First&email=someemail@someemailprovider.com)
- O también ejecutando el comando curl: curl 'localhost:8080/demo/add?name=First&email=someemail@someemailprovider.com'
 

## API de Customers
- Url  base: [http://localhost:8080/customer](http://localhost:8080/customer)
## API de personas
- Url base: [http://localhost:8080/people](http://localhost:8080/people)
- Añadir una persona, comando: curl -i -X POST -H "Content-Type:application/json" -d '{"firstName": "Frodo", "lastName": "Baggins"}' http://localhost:8080/people
- Búsqueda de personas: curl http://localhost:8080/people/search
- Ejemplo de búsqueda:  curl http://localhost:8080/people/search/findByLastName?name=Baggins
- Reemplazo de objetos: curl -X PUT -H "Content-Type:application/json" -d '{"firstName": "Bilbo", "lastName": "Baggins"}' http://localhost:8080/people/1
- Modificación de campos de un objeto: curl -X PATCH -H "Content-Type:application/json" -d '{"firstName": "Bilbo Jr."}' http://localhost:8080/people/1
- Borrado de objetos: curl -X DELETE http://localhost:8080/people/1