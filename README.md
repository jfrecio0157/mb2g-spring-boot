# mb2g-spring-boot
Ejemplo de spring boot

- Se ha creado el esqueleto del proyecto desde la pagina start.spring.io
- Se ha usado postman para ver la salida del proyecto, usando http://localhost:8080
- He intentado poder usar en postman el http://localhost:8080/actuator/info pero me da error cuando intentado  
  mapear el target -> META-INF -> git.properties
  
Para ejecutar el codigo desde IntelliJ, ir a Maven -> Plugins -> spring-boot -> y hacer doble click en 
spring-boot:run  

## En esta branch (v02R00F00) se ha hecho la modularidad del spring-boot
- Se han creado dos modulos: web-model y web-app. 
- Se quiere que web-app sea la principal, por eso se lleva las dependencies del root a web-app y se añade la 
  dependency de web-model. Se ve el orden de construccion cuando se hace el install del root en Maven
