# Programación Orientada a Objetos (POO) en Java

Propietario: William Meza
Verificación: Verificación vencida
Etiquetas: Introduction, Java

## 1. Introducción a la Programación Orientada a Objetos (POO)

La Programación Orientada a Objetos es un paradigma de programación que utiliza objetos para organizar y estructurar el código. En Java, POO es fundamental, y los conceptos clave son las clases y los objetos.

## 2. Clases y Objetos

### 2.1 Definición de Clases

Las clases son plantillas para crear objetos. Contienen atributos y métodos que definen las propiedades y el comportamiento de los objetos.

```java
public class Persona {
    // Atributos
    String nombre;
    int edad;

    // Constructor
    public Persona(String nombre, int edad) {
        this.nombre = nombre;
        this.edad = edad;
    }

    // Método
    public void saludar() {
        System.out.println("Hola, soy " + nombre + " y tengo " + edad + " años.");
    }
}

```

### 2.2 Creación de Objetos

Los objetos son instancias de una clase. Se crean utilizando la palabra clave `new`.

```java
// Crear objetos de la clase Persona
Persona persona1 = new Persona("Ana", 30);
Persona persona2 = new Persona("Juan", 25);

// Llamar a métodos de los objetos
persona1.saludar();
persona2.saludar();

```

## 3. Herencia y Polimorfismo

### 3.1 Herencia

La herencia permite que una clase herede atributos y métodos de otra clase. La clase que hereda se llama subclase, y la clase de la cual se hereda se llama superclase.

```java
// Superclase
public class Animal {
    void comer() {
        System.out.println("El animal come.");
    }
}

// Subclase
public class Perro extends Animal {
    void ladrar() {
        System.out.println("El perro ladra.");
    }
}

```

### 3.2 Polimorfismo

El polimorfismo permite que un objeto pueda tomar varias formas. Puede referirse a objetos de clases diferentes a través de una interfaz común.

```java
Animal miMascota = new Perro();
miMascota.comer(); // Accede al método de la clase Animal
((Perro) miMascota).ladrar(); // Accede al método específico de la clase Perro

```

## 4. Interfaces y Clases Abstractas

### 4.1 Interfaces

Las interfaces definen un conjunto de métodos que una clase debe implementar. Permiten la creación de contratos para la implementación de clases.

```java
public interface Volador {
    void volar();
}

```

### 4.2 Clases Abstractas

Las clases abstractas son clases que no se pueden instanciar directamente y pueden contener métodos abstractos, que deben ser implementados por las clases hijas.

```java
public abstract class Figura {
    int lados;

    public Figura(int lados) {
        this.lados = lados;
    }

    abstract double calcularArea();
}

```

## 5. Aplicación de POO en Java

La POO en Java permite la creación de sistemas modulares y mantenibles. Utiliza clases y objetos para modelar el mundo real, facilitando la reutilización de código y la gestión de la complejidad.

Al comprender estos conceptos, podrás construir sistemas robustos y escalables en Java. ¡Explora más allá y descubre la potencia de la Programación Orientada a Objetos!