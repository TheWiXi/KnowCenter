# Entrada/Salida (E/S) y Colecciones en Java

Propietario: William Meza
Verificación: Verificación vencida
Etiquetas: Introduction, Java, pre-intermediate

# 1. Introducción a la Entrada/Salida (E/S)

La entrada/salida (E/S) en Java es esencial para interactuar con el usuario y otros dispositivos. La clase `Scanner` facilita la lectura desde la consola, mientras que `System.out` permite la escritura en la misma.

![https://www.carlospes.com/curso_de_informatica_basica/imagenes/fig_01_04_fucionamiento_programa.gif](https://www.carlospes.com/curso_de_informatica_basica/imagenes/fig_01_04_fucionamiento_programa.gif)

### 1.1 Lectura desde la Consola

La clase `Scanner` permite leer datos desde la consola. En el ejemplo, se solicita al usuario que ingrese su nombre, y luego se imprime un saludo personalizado.

```java
import java.util.Scanner;

public class EntradaConsola {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Ingrese su nombre: ");
        String nombre = scanner.nextLine();
        System.out.println("Hola, " + nombre + "!");

        // Cierre del Scanner
        scanner.close();
    }
}

```

### 1.2 Escritura en la Consola

La clase `System.out` se utiliza para escribir en la consola. En este ejemplo, se imprime un mensaje simple.

```java
public class SalidaConsola {
    public static void main(String[] args) {
        String mensaje = "¡Hola, Mundo!";
        System.out.println(mensaje);
    }
}

```

## 2. Trabajo con Listas (ArrayList, LinkedList)

Las Listas en Java, como `ArrayList` y `LinkedList`, son estructuras de datos flexibles que permiten almacenar y manipular conjuntos de elementos de manera eficiente.

### 2.1 ArrayList

`ArrayList` proporciona una lista dinámica que puede cambiar de tamaño. Se puede acceder a los elementos por índice y es eficiente para la búsqueda.

```java
import java.util.ArrayList;

public class UsoArrayList {
    public static void main(String[] args) {
        // Crear un ArrayList de cadenas
        ArrayList<String> listaNombres = new ArrayList<>();

        // Agregar elementos a la lista
        listaNombres.add("Ana");
        listaNombres.add("Juan");
        listaNombres.add("María");

        // Acceder a elementos por índice
        String primerNombre = listaNombres.get(0);

        // Iterar sobre la lista
        for (String nombre : listaNombres) {
            System.out.println(nombre);
        }
    }
}

```

### 2.2 LinkedList

`LinkedList` es otra implementación de la interfaz `List` que implementa una lista doblemente enlazada. Es eficiente para inserciones y eliminaciones en cualquier posición.

```java
import java.util.LinkedList;

public class UsoLinkedList {
    public static void main(String[] args) {
        // Crear una LinkedList de enteros
        LinkedList<Integer> numeros = new LinkedList<>();

        // Agregar elementos a la lista
        numeros.add(10);
        numeros.add(20);
        numeros.add(30);

        // Eliminar el primer elemento
        numeros.removeFirst();

        // Iterar sobre la lista
        for (Integer numero : numeros) {
            System.out.println(numero);
        }
    }
}

```

La combinación de técnicas de entrada/salida y el uso inteligente de Listas ofrece un conjunto sólido de herramientas para interactuar con datos y usuarios en aplicaciones Java. ¡Explora estas capacidades para crear programas más dinámicos y eficientes!