# Conceptos Básicos de Programación en Java

Propietario: William Meza
Verificación: Verificación vencida
Etiquetas: Introduction, Java

## 1. Introducción

Java es un lenguaje de programación de alto nivel que ha ganado popularidad por su versatilidad, portabilidad y robustez. A continuación, se presentan los conceptos básicos que forman la base de la programación en Java.

## 2. Variables y Tipos de Datos

### 2.1 Declaración de Variables

En Java, las variables son contenedores que almacenan datos. Antes de usar una variable, debes declararla y especificar su tipo de dato.

```java
int edad = 25;
double salario = 1500.50;
boolean esEstudiante = true;
String nombre = "Juan";

```

### 2.2 Tipos de Datos

Java tiene tipos de datos primitivos (int, double, boolean) y tipos de datos compuestos (String, Arrays, Objetos). Los tipos primitivos almacenan valores directamente, mientras que los tipos compuestos almacenan referencias a objetos.

## 3. Estructuras de Control

### 3.1 Condicionales (if-else)

Las estructuras condicionales permiten ejecutar bloques de código basándose en la evaluación de expresiones booleanas.

```java
int numero = 10;
if (numero > 0) {
    System.out.println("El número es positivo");
} else {
    System.out.println("El número no es positivo");
}

```

### 3.2 Bucles (for, while)

Los bucles permiten repetir la ejecución de un bloque de código.

### Bucle for:

```java
for (int i = 0; i < 5; i++) {
    System.out.println("Iteración: " + i);
}

```

### Bucle while:

```java
int contador = 0;
while (contador < 3) {
    System.out.println("Contador: " + contador);
    contador++;
}

```

## 4. Métodos y Funciones

### 4.1 Declaración de Métodos

Los métodos son bloques de código que realizan una tarea específica. Pueden tener parámetros y devolver un valor.

```java
public int sumar(int a, int b) {
    return a + b;
}

// Llamada al método
int resultado = sumar(5, 3);

```

## 5. Arreglos y Colecciones

### 5.1 Arreglos

Los arreglos permiten almacenar múltiples valores del mismo tipo.

```java
int[] numeros = {1, 2, 3, 4, 5};
System.out.println("Primer elemento: " + numeros[0]);

```

### 5.2 Colecciones

Java proporciona colecciones como Listas, Sets y Mapas para manejar conjuntos de elementos de manera más dinámica.

```java
List<String> nombres = new ArrayList<>();
nombres.add("Ana");
nombres.add("Juan");

```

## 6. Programación Orientada a Objetos

Java es un lenguaje orientado a objetos. Las clases y los objetos son fundamentales en este paradigma.

```java
public class Persona {
    String nombre;
    int edad;

    public Persona(String nombre, int edad) {
        this.nombre = nombre;
        this.edad = edad;
    }

    public void saludar() {
        System.out.println("Hola, soy " + nombre + " y tengo " + edad + " años.");
    }
}

// Crear un objeto Persona
Persona persona1 = new Persona("Ana", 30);

// Llamar a un método de la clase
persona1.saludar();

```

## 7. Excepciones

Las excepciones son eventos inesperados que pueden ocurrir durante la ejecución del programa. Java maneja las excepciones con bloques try-catch.

```java
try {
    int resultado = 10 / 0;
} catch (ArithmeticException e) {
    System.out.println("Error aritmético: " + e.getMessage());
}

```

Estos conceptos forman la base de la programación en Java. A medida que profundices en el desarrollo, explorarás conceptos más avanzados y técnicas de programación que te permitirán construir aplicaciones sólidas y eficientes. ¡Explora y disfruta del mundo de Java!