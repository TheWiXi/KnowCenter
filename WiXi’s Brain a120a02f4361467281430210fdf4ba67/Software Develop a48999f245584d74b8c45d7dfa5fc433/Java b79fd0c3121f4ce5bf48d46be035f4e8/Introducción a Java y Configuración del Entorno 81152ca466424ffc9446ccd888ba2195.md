# Introducción a Java y Configuración del Entorno

Propietario: William Meza
Verificación: Verificación vencida
Etiquetas: Introduction, Java

# 1. Introducción a Java

Java es un lenguaje de programación de propósito general que fue desarrollado por Sun Microsystems en la década de 1990. Su lema principal es "Write Once, Run Anywhere" (Escribe una vez, ejecuta en cualquier lugar), lo que significa que el código Java puede ejecutarse en cualquier dispositivo que tenga una máquina virtual Java (JVM) instalada, independientemente de la arquitectura subyacente.

### 1.1 Características principales de Java

- **Orientado a Objetos:** Java es un lenguaje orientado a objetos, lo que significa que se basa en el concepto de clases y objetos, permitiendo la encapsulación, la herencia y el polimorfismo.
- **Plataforma Independiente:** La portabilidad es una de las principales fortalezas de Java. El código fuente se compila en un formato intermedio llamado bytecode, que puede ejecutarse en cualquier dispositivo con una JVM.
- **Seguro y Robusto:** Java incorpora características de seguridad y robustez mediante la gestión automática de la memoria, la verificación de tipos y la excepción de manejo.
- **Multi-Hilo:** Java soporta la programación multi-hilo, permitiendo la ejecución concurrente de varias tareas.

## 2. Configuración del Entorno

### 2.1 Instalación del Kit de Desarrollo de Java (JDK)

El JDK es necesario para desarrollar y ejecutar aplicaciones Java. Sigue estos pasos para instalar el JDK:

1. **Descargar el JDK:** Visita el sitio oficial de Oracle o de la distribución que prefieras (como OpenJDK) y descarga la última versión del JDK.
2. **Instalación en Windows:**
    - Ejecuta el instalador descargado.
    - Sigue las instrucciones del asistente de instalación.
    - Configura las variables de entorno JAVA_HOME y PATH.
3. **Instalación en Linux:**
    - Abre la terminal.
    - Usa el administrador de paquetes de tu distribución para instalar el JDK.
4. **Verificación de la Instalación:**
    - Abre la terminal y ejecuta `java -version` y `javac -version` para asegurarte de que la instalación fue exitosa.

### 2.2 Configuración de un Entorno de Desarrollo Integrado (IDE)

Aunque puedes escribir código Java en un editor de texto, utilizar un IDE proporciona funcionalidades adicionales que facilitan el desarrollo. Algunos IDE populares para Java son Eclipse, IntelliJ IDEA y NetBeans.

1. **Instalación del IDE:**
    - Descarga e instala el IDE de tu elección desde su sitio web oficial.
    - Configura el IDE para que utilice el JDK instalado.
2. **Creación de un Proyecto:**
    - Abre el IDE y crea un nuevo proyecto Java.
    - Configura las opciones del proyecto, como el nombre y la ubicación.
3. **Desarrollo y Depuración:**
    - Utiliza las herramientas del IDE para escribir, depurar y ejecutar tu código.
    - Aprovecha las funciones como la autocompletación, la navegación de código y la gestión de dependencias.

### 2.3 Ejecución de un Programa Java Simple

Para comenzar, crea un programa Java simple y ejecútalo. Aquí hay un ejemplo básico:

```java
public class HolaMundo {
    public static void main(String[] args) {
        System.out.println("¡Hola, Mundo!");
    }
}

```

Guarda este código en un archivo con extensión `.java` y sigue estos pasos:

1. **Compilación:**
    - Abre la terminal en la ubicación del archivo.
    - Ejecuta `javac HolaMundo.java` para compilar el programa.
2. **Ejecución:**
    - Una vez compilado, ejecuta `java HolaMundo` para ver la salida.

Con esto, has configurado tu entorno de desarrollo Java y ejecutado tu primer programa. ¡Bienvenido al mundo de Java!