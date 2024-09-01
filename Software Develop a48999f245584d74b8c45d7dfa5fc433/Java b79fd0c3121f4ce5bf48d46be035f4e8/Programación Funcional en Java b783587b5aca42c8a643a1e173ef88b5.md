# Programación Funcional en Java

Propietario: William Meza
Verificación: Verificación vencida
Etiquetas: Java, advanced, intermediate

## 1. Introducción a la Programación Funcional

La programación funcional es un paradigma que trata la computación como la evaluación de funciones matemáticas. En Java, se introdujeron características de programación funcional a partir de Java 8, como expresiones lambda y streams. A continuación, exploraremos estos conceptos.

## 2. Expresiones Lambda

Las expresiones lambda permiten tratar las funciones como objetos de una manera más concisa. Están formadas por una lista de parámetros, una flecha `->`, y el cuerpo de la función.

### 2.1 Sintaxis Básica

```java
// Forma tradicional de implementar una interfaz funcional
Runnable runnable1 = new Runnable() {
    @Override
    public void run() {
        System.out.println("Hola desde el hilo 1");
    }
};

// Expresión lambda equivalente
Runnable runnable2 = () -> System.out.println("Hola desde el hilo 2");

```

## 3. Streams

Los streams son secuencias de elementos que admiten operaciones de procesamiento de datos en paralelo o en serie. Facilitan el manejo de colecciones de datos de manera funcional.

### 3.1 Operaciones Básicas de Stream

```java
import java.util.Arrays;
import java.util.List;
import java.util.stream.Collectors;

public class PruebaStreams {
    public static void main(String[] args) {
        List<String> nombres = Arrays.asList("Ana", "Juan", "María", "Pedro");

        // Filtrar nombres que comienzan con "M" y convertir a mayúsculas
        List<String> resultado = nombres.stream()
                .filter(nombre -> nombre.startsWith("M"))
                .map(String::toUpperCase)
                .collect(Collectors.toList());

        System.out.println(resultado);
    }
}

```

En este ejemplo, el stream filtra los nombres que comienzan con "M" y luego los convierte a mayúsculas, todo en una operación funcional.

## 4. Conclusión

La programación funcional en Java, con expresiones lambda y streams, brinda un enfoque más conciso y expresivo para manipular datos y realizar operaciones en colecciones. Las expresiones lambda permiten pasar funciones como argumentos, y los streams simplifican las operaciones en conjuntos de datos. Estos conceptos proporcionan una manera elegante y eficiente de abordar problemas en Java, mejorando la legibilidad y la mantenibilidad del código. ¡Explora y aprovecha al máximo la programación funcional en Java!