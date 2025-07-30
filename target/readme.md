Integrantes, Grupo 7:
● María Elena Salgado
● Diego Durán
● Sebastián Calvete
● Maykol Ramírez

Objetivo: Automatizar un escenario funcional completo utilizando Cucumber y Selenium WebDriver en
Java, organizando el proyecto con Maven, aplicando BDD y ejecutando la prueba desde Visual Studio Code.

1. Crea un nuevo proyecto Maven.
2. Configura el archivo pom.xml con las dependencias de Cucumber (Java y
Junit-platform-engine), Selenium, WebDriverManager y Junit 5.
3. Escribe un archivo .feature llamado login.feature con el siguiente
escenario:
Feature: Inicio de sesión
Scenario: Usuario accede con credenciales válidas
 Given que el usuario está en la página de login
 When ingresa usuario "admin" y clave "admin123"
 Then debería ver el mensaje "Bienvenido, admin"
4. Crea el archivo LoginSteps.java para implementar los pasos con
Selenium.
5. Aplica el patrón Page Object para encapsular los selectores y métodos en
una clase LoginPage.java
6. Crea un archivo RunCucumberTest.java que ejecute la prueba con los
parámetros adecuados (consola y JSON report).
7. Ejecuta el proyecto con mvn test y guarda una captura de pantalla del
reporte y de la ejecución del navegador.