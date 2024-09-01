# Desarrollo Web con Java (Servlets y JSP)

Propietario: William Meza
Verificación: Verificación vencida
Etiquetas: Java, advanced

## 1. Introducción a Servlets y JSP

Java ofrece una plataforma robusta para el desarrollo web a través de Servlets y JavaServer Pages (JSP). Servlets son programas Java que se ejecutan en el servidor web, mientras que JSP permite la creación de páginas web dinámicas. A continuación, exploraremos la introducción a Servlets y JSP y cómo desarrollar aplicaciones web básicas con estas tecnologías.

## 2. Desarrollo de Aplicaciones Web Básicas

### 2.1 Creación de un Servlet

Un Servlet básico puede responder a solicitudes HTTP y realizar acciones en el servidor.

```java
import javax.servlet.*;
import javax.servlet.http.*;
import java.io.IOException;

public class MiServlet extends HttpServlet {
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        // Código para manejar solicitudes GET
        response.setContentType("text/html");
        PrintWriter out = response.getWriter();
        out.println("<html><body>");
        out.println("<h2>Hola desde MiServlet</h2>");
        out.println("</body></html>");
    }
}

```

### 2.2 Configuración en web.xml

Es necesario configurar el Servlet en el archivo `web.xml`.

```xml
<servlet>
    <servlet-name>MiServlet</servlet-name>
    <servlet-class>paquete.MiServlet</servlet-class>
</servlet>
<servlet-mapping>
    <servlet-name>MiServlet</servlet-name>
    <url-pattern>/miRuta</url-pattern>
</servlet-mapping>

```

### 2.3 Creación de una Página JSP

JSP permite la creación de páginas dinámicas que se procesan en el servidor antes de ser enviadas al navegador.

```
<%@ page language="java" contentType="text/html; charset=UTF-8" pageEncoding="UTF-8"%>
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Mi Página JSP</title>
</head>
<body>
    <h2>Hola desde mi Página JSP</h2>
    <p>Fecha y hora actual: <%= new java.util.Date() %></p>
</body>
</html>

```

### 2.4 Configuración en web.xml para JSP

Es necesario configurar el mapeo de JSP en el archivo `web.xml`.

```xml
<servlet>
    <servlet-name>MiJSP</servlet-name>
    <jsp-file>/miPagina.jsp</jsp-file>
</servlet>
<servlet-mapping>
    <servlet-name>MiJSP</servlet-name>
    <url-pattern>/miPagina</url-pattern>
</servlet-mapping>

```

## 3. Conclusiones

El desarrollo web con Servlets y JSP en Java proporciona una poderosa capacidad para construir aplicaciones web dinámicas y escalables. Los Servlets manejan la lógica del lado del servidor, mientras que JSP simplifica la creación de páginas web. Configurando Servlets y JSP en archivos `web.xml`, puedes construir aplicaciones web básicas de manera efectiva. Este es solo el comienzo del vasto mundo del desarrollo web en Java. ¡Explora y desarrolla aplicaciones web más complejas y ricas en funcionalidades!