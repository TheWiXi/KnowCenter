# Hilos y Concurrencia Básica en Java

Propietario: William Meza
Verificación: Verificación vencida
Etiquetas: Java, intermediate

## 1. Introducción a Hilos

En Java, los hilos permiten ejecutar múltiples tareas simultáneamente, mejorando la eficiencia y el rendimiento de las aplicaciones. La clase `Thread` se utiliza para crear hilos. A continuación, exploraremos la introducción a hilos y la creación básica de ellos.

### 1.1 Creación Básica de Hilos

La creación de hilos en Java se realiza extendiendo la clase `Thread` y sobrescribiendo el método `run()`.

```java
public class MiHilo extends Thread {
    public void run() {
        for (int i = 0; i < 5; i++) {
            System.out.println(Thread.currentThread().getId() + " Valor: " + i);
        }
    }
}

public class PruebaHilos {
    public static void main(String args[]) {
        // Crear instancias de la clase MiHilo
        MiHilo hilo1 = new MiHilo();
        MiHilo hilo2 = new MiHilo();

        // Iniciar los hilos
        hilo1.start();
        hilo2.start();
    }
}

```

## 2. Sincronización Básica

La sincronización es crucial cuando múltiples hilos acceden y modifican comparticiones de datos para evitar problemas de concurrencia. Se utiliza la palabra clave `synchronized` para lograr sincronización.

### 2.1 Método Sincronizado

```java
public class Contador {
    private int valor = 0;

    // Método sincronizado
    public synchronized void incrementar() {
        valor++;
        System.out.println(Thread.currentThread().getId() + " Valor incrementado: " + valor);
    }
}

public class PruebaSincronizacion {
    public static void main(String args[]) {
        Contador contador = new Contador();

        // Crear instancias de la clase MiHilo
        MiHilo hilo1 = new MiHilo(contador);
        MiHilo hilo2 = new MiHilo(contador);

        // Iniciar los hilos
        hilo1.start();
        hilo2.start();
    }
}

```

En este ejemplo, ambos hilos comparten un objeto `Contador`, y la sincronización en el método `incrementar()` garantiza que la operación se realice de manera segura y evite condiciones de carrera.

## 3. Conclusión

La introducción a hilos y la sincronización básica son conceptos fundamentales para desarrollar aplicaciones concurrentes en Java. El uso adecuado de hilos y la sincronización son cruciales para evitar problemas de concurrencia y garantizar un comportamiento predecible en entornos multitarea. Al explorar estas capacidades, podrás crear aplicaciones más eficientes y robustas en términos de concurrencia. ¡Experimenta y mejora tus habilidades en el manejo de hilos en Java!