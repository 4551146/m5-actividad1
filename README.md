# Módulo 5 - Sesión N°1  
**Grupo 7 – Integrantes:**  
- María Elena Salgado  
- Diego Durán  
- Sebastián Calvete  
- Maykol Ramírez
  

## Inicio de Sesión Automatizado con Cucumber + Selenium

### Descripción  
Este proyecto automatiza un escenario funcional de inicio de sesión utilizando Cucumber y Selenium WebDriver en Java. Se organiza con Maven y aplica BDD (Behavior Driven Development), ejecutándose desde Visual Studio Code.

---

### Objetivo  
Automatizar un flujo completo de inicio de sesión con credenciales válidas, usando herramientas y patrones modernos para garantizar pruebas legibles, mantenibles y confiables.

---

### Instrucciones para el proyecto  

1. **Crear proyecto Maven**  
   Inicializar un nuevo proyecto Maven para gestionar dependencias y ejecución.

2. **Configurar dependencias**  
   Agregar en `pom.xml` las librerías necesarias:  
   - Cucumber Java  
   - Cucumber JUnit Platform Engine  
   - Selenium WebDriver  
   - WebDriverManager  
   - JUnit 5  

3. **Archivo Feature**  
   Crear el archivo `login.feature` con el siguiente contenido:

   ```gherkin
   Feature: Inicio de sesión

   Scenario: Usuario accede con credenciales válidas
     Given que el usuario está en la página de login
     When ingresa usuario "admin" y clave "admin123"
     Then debería ver el mensaje "Bienvenido, admin"
   ```

4. **Implementar Steps**  
   Crear `LoginSteps.java` para implementar los pasos definidos en el feature usando Selenium.

5. **Patrón Page Object**  
   Implementar la clase `LoginPage.java` para encapsular los selectores y métodos de interacción con la página de login.

6. **Ejecutar pruebas**  
   Crear `RunCucumberTest.java` para correr los tests con configuración para consola y reporte JSON.

7. **Ejecución y evidencias**  
   Ejecutar con:  
   ```bash
   mvn test
   ```  
   Guardar capturas de pantalla de la ejecución en navegador y del reporte generado.

---

### Modalidad  
Individual

---

### Tiempo estimado  
1 hora

---

### Tecnologías utilizadas  
- Java  
- Maven  
- Cucumber  
- Selenium WebDriver  
- JUnit 5  
- WebDriverManager  
