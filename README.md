# mb2g-spring-boot
Ejemplo de spring boot

- Se ha creado el esqueleto del proyecto desde la pagina start.spring.io
- Se ha usado postman para ver la salida del proyecto, usando http://localhost:8080
- He intentado poder usar en postman el http://localhost:8080/actuator/info pero me da error cuando intentado  
  mapear el target -> META-INF -> git.properties
  
Para ejecutar el codigo desde IntelliJ, ir a Maven -> Plugins -> spring-boot -> y hacer doble click en 
spring-boot:run  

## Para la branch (v02R00F00) se ha hecho la modularidad del spring-boot
- Se han creado dos modulos: web-model y web-app. 
- Se quiere que web-app sea la principal, por eso se lleva las dependencies y los build del root a web-app 
  y se añade la dependency de web-model.
- Se hace el refactor de los directorios main y test del root y se lleva al modulo web-app.
  Se eliminan los directorios del root
- Se ve el orden de construccion cuando se hace el install del root en Maven
  
[INFO] Reactor Summary for demo 0.0.1-SNAPSHOT:
[INFO] 
[INFO] demo ............................................... SUCCESS [  1.200 s]
[INFO] web-model .......................................... SUCCESS [  2.309 s]
[INFO] web-app ............................................ SUCCESS [ 26.486 s]
[INFO] ------------------------------------------------------------------------