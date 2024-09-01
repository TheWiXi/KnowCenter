# Manejo de Archivos en Java

Propietario: William Meza
Verificación: Verificación vencida
Etiquetas: Java, intermediate, pre-intermediate

## 1. Introducción al Manejo de Archivos

El manejo de archivos es fundamental en el desarrollo de aplicaciones para almacenar y recuperar datos de manera persistente. En Java, la lectura y escritura de archivos se realiza mediante las clases `File`, `FileReader`, `FileWriter`, `BufferedReader` y `BufferedWriter`. Aquí exploraremos cómo realizar estas operaciones de manera efectiva.

## 2. Lectura de Archivos

### 2.1 Clase File

La clase `File` se utiliza para representar rutas de archivos o directorios. Puedes verificar la existencia de un archivo, obtener su ruta y más.

```java
import java.io.File;
import java.io.FileNotFoundException;
import java.util.Scanner;

public class LecturaArchivo {
    public static void main(String[] args) {
        // Crear un objeto File
        File archivo = new File("archivo.txt");

        try {
            // Crear un objeto Scanner para leer el archivo
            Scanner scanner = new Scanner(archivo);

            // Leer y mostrar el contenido del archivo línea por línea
            while (scanner.hasNextLine()) {
                String linea = scanner.nextLine();
                System.out.println(linea);
            }

            // Cierre del Scanner
            scanner.close();
        } catch (FileNotFoundException e) {
            System.out.println("Archivo no encontrado: " + e.getMessage());
        }
    }
}

```

## 3. Escritura de Archivos

### 3.1 Clase FileWriter y BufferedWriter

Para escribir en un archivo, se utiliza la clase `FileWriter` junto con `BufferedWriter` para mejorar el rendimiento.

```java
import java.io.BufferedWriter;
import java.io.FileWriter;
import java.io.IOException;

public class EscrituraArchivo {
    public static void main(String[] args) {
        // Nombre del archivo
        String nombreArchivo = "nuevoArchivo.txt";

        try {
            // Crear objetos FileWriter y BufferedWriter
            FileWriter escritor = new FileWriter(nombreArchivo);
            BufferedWriter bufferEscritura = new BufferedWriter(escritor);

            // Escribir líneas en el archivo
            bufferEscritura.write("Hola, Mundo!");
            bufferEscritura.newLine(); // Nueva línea
            bufferEscritura.write("Este es un archivo de ejemplo.");

            // Cierre del BufferedWriter
            bufferEscritura.close();

            System.out.println("Archivo escrito con éxito.");
        } catch (IOException e) {
            System.out.println("Error de escritura: " + e.getMessage());
        }
    }
}

```

## 4. Conclusiones

El manejo de archivos es esencial para interactuar con datos de manera persistente en Java. Las clases `File`, `FileReader`, `FileWriter`, `BufferedReader` y `BufferedWriter` proporcionan las herramientas necesarias para realizar operaciones de lectura y escritura. Asegúrate de manejar excepciones correctamente para garantizar la robustez de tus programas al trabajar con archivos. ¡Explora estas capacidades y mejora la manipulación de datos en tus aplicaciones Java!