# Programación en Red (Básica) en Java

Propietario: William Meza
Verificación: Verificación vencida
Etiquetas: Java, advanced

## 1. Introducción a la Programación en Red

La programación en red es esencial para el desarrollo de aplicaciones que requieren comunicación entre dispositivos a través de una red. En Java, la manipulación de conexiones TCP/IP y el trabajo con URL y Sockets son fundamentales para este propósito. A continuación, exploraremos estos conceptos básicos.

## 2. Conexiones TCP/IP

### 2.1 Cliente TCP

La creación de un cliente TCP implica la creación de un Socket para establecer una conexión con un servidor.

```java
import java.io.IOException;
import java.io.OutputStream;
import java.net.Socket;

public class ClienteTCP {
    public static void main(String[] args) {
        try {
            // Crear un Socket para conectarse al servidor en el puerto 12345
            Socket socket = new Socket("localhost", 12345);

            // Obtener el flujo de salida del Socket
            OutputStream salida = socket.getOutputStream();

            // Enviar datos al servidor
            byte[] datos = "Hola, servidor".getBytes();
            salida.write(datos);

            // Cerrar el Socket
            socket.close();
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}

```

### 2.2 Servidor TCP

La creación de un servidor TCP implica la espera de conexiones y la manipulación de los datos recibidos.

```java
import java.io.IOException;
import java.io.InputStream;
import java.net.ServerSocket;
import java.net.Socket;

public class ServidorTCP {
    public static void main(String[] args) {
        try {
            // Crear un ServerSocket en el puerto 12345
            ServerSocket serverSocket = new ServerSocket(12345);

            // Esperar a que un cliente se conecte
            Socket socket = serverSocket.accept();

            // Obtener el flujo de entrada del Socket
            InputStream entrada = socket.getInputStream();

            // Leer datos del cliente
            byte[] datos = new byte[100];
            entrada.read(datos);

            // Mostrar los datos recibidos
            System.out.println("Datos recibidos: " + new String(datos).trim());

            // Cerrar el Socket y el ServerSocket
            socket.close();
            serverSocket.close();
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}

```

## 3. Trabajo con URL

La clase `URL` en Java facilita el trabajo con recursos a través de la red.

```java
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;
import java.net.URL;

public class TrabajoConURL {
    public static void main(String[] args) {
        try {
            // Crear un objeto URL
            URL url = new URL("<https://www.ejemplo.com>");

            // Abrir una conexión y obtener el flujo de entrada
            BufferedReader reader = new BufferedReader(new InputStreamReader(url.openStream()));

            // Leer y mostrar el contenido de la URL
            String linea;
            while ((linea = reader.readLine()) != null) {
                System.out.println(linea);
            }

            // Cerrar el BufferedReader
            reader.close();
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}

```

## 4. Sockets y Red en Java

La programación en red con Sockets y el trabajo con URL en Java ofrecen herramientas poderosas para la comunicación entre dispositivos. Ya sea estableciendo conexiones TCP/IP o accediendo a recursos a través de URL, estas capacidades son fundamentales en el desarrollo de aplicaciones distribuidas y conectadas en red. ¡Explora y aprovecha estas funcionalidades para construir aplicaciones eficientes y conectadas!