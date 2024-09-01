# Manejo de Bases de Datos con JDBC en Java

Propietario: William Meza
Verificación: Verificación vencida
Etiquetas: Java, advanced

## 1. Introducción a JDBC

Java Database Connectivity (JDBC) es una API que proporciona una interfaz estándar para interactuar con bases de datos desde aplicaciones Java. Permite establecer conexiones, enviar consultas y recibir resultados. En este documento, exploraremos el manejo básico de bases de datos con JDBC.

## 2. Conexiones a Bases de Datos

### 2.1 Establecimiento de una Conexión

Para establecer una conexión a una base de datos, se requiere la información de la URL de la base de datos, el nombre de usuario y la contraseña.

```java
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.SQLException;

public class ConexionBD {
    public static void main(String[] args) {
        String url = "jdbc:mysql://localhost:3306/miBaseDeDatos";
        String usuario = "miUsuario";
        String contraseña = "miContraseña";

        try {
            Connection conexion = DriverManager.getConnection(url, usuario, contraseña);
            System.out.println("Conexión establecida con éxito");

            // Realizar operaciones en la base de datos

            // Cerrar la conexión
            conexion.close();
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }
}

```

## 3. Consultas y Actualizaciones

### 3.1 Ejecución de Consultas

JDBC permite ejecutar consultas SQL y recuperar resultados.

```java
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.PreparedStatement;
import java.sql.ResultSet;
import java.sql.SQLException;

public class ConsultaBD {
    public static void main(String[] args) {
        String url = "jdbc:mysql://localhost:3306/miBaseDeDatos";
        String usuario = "miUsuario";
        String contraseña = "miContraseña";

        try {
            Connection conexion = DriverManager.getConnection(url, usuario, contraseña);

            // Ejecutar una consulta
            String consultaSQL = "SELECT * FROM miTabla";
            PreparedStatement statement = conexion.prepareStatement(consultaSQL);
            ResultSet resultado = statement.executeQuery();

            // Procesar el resultado
            while (resultado.next()) {
                String columna1 = resultado.getString("columna1");
                int columna2 = resultado.getInt("columna2");

                // Realizar acciones con los datos recuperados
            }

            // Cerrar la conexión
            conexion.close();
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }
}

```

### 3.2 Ejecución de Actualizaciones

Además de consultas, JDBC permite ejecutar actualizaciones en la base de datos, como inserciones, actualizaciones y eliminaciones.

```java
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.PreparedStatement;
import java.sql.SQLException;

public class ActualizacionBD {
    public static void main(String[] args) {
        String url = "jdbc:mysql://localhost:3306/miBaseDeDatos";
        String usuario = "miUsuario";
        String contraseña = "miContraseña";

        try {
            Connection conexion = DriverManager.getConnection(url, usuario, contraseña);

            // Ejecutar una actualización
            String actualizacionSQL = "UPDATE miTabla SET columna1 = ? WHERE columna2 = ?";
            PreparedStatement statement = conexion.prepareStatement(actualizacionSQL);
            statement.setString(1, "NuevoValor");
            statement.setInt(2, 123);

            int filasActualizadas = statement.executeUpdate();

            // Realizar acciones con el resultado de la actualización

            // Cerrar la conexión
            conexion.close();
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }
}

```

## 4. Documentación

El manejo de bases de datos con JDBC en Java es esencial para aplicaciones que requieren almacenamiento y recuperación de datos. La API JDBC simplifica la interacción con bases de datos relacionales, proporcionando métodos para establecer conexiones, ejecutar consultas y realizar actualizaciones. Al comprender estos fundamentos, puedes construir aplicaciones robustas y eficientes que aprovechan el poder de las bases de datos relacionales en entornos Java. ¡Explora y aplica estas técnicas en tus proyectos de bases de datos Java!