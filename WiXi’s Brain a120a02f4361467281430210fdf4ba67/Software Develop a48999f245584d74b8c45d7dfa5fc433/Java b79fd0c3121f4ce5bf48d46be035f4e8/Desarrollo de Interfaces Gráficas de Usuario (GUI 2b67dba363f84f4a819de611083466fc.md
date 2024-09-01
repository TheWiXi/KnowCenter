# Desarrollo de Interfaces Gráficas de Usuario (GUI) en Java

Propietario: William Meza

## 1. Introducción al Desarrollo de GUI

El desarrollo de Interfaces Gráficas de Usuario (GUI) es esencial para crear aplicaciones interactivas y atractivas. En Java, Swing y JavaFX son dos bibliotecas populares para desarrollar GUI. A continuación, exploraremos la creación de ventanas, componentes y el manejo de eventos.

## 2. Creación de Ventanas y Componentes con Swing

### 2.1 Creación de una Ventana

La clase `JFrame` se utiliza para crear una ventana básica en Swing.

```java
import javax.swing.JFrame;

public class VentanaSwing {
    public static void main(String[] args) {
        JFrame ventana = new JFrame("Mi Ventana Swing");
        ventana.setSize(400, 300);
        ventana.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        ventana.setVisible(true);
    }
}

```

### 2.2 Añadiendo Componentes

Puedes añadir diferentes componentes a la ventana, como botones, etiquetas y campos de texto.

```java
import javax.swing.JButton;
import javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.JPanel;
import java.awt.FlowLayout;

public class VentanaConComponentes {
    public static void main(String[] args) {
        JFrame ventana = new JFrame("Ventana con Componentes");
        ventana.setSize(400, 300);
        ventana.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);

        // Crear un panel y establecer su diseño
        JPanel panel = new JPanel();
        panel.setLayout(new FlowLayout());

        // Añadir componentes al panel
        JButton boton = new JButton("Haz clic");
        JLabel etiqueta = new JLabel("¡Hola, Mundo!");

        panel.add(boton);
        panel.add(etiqueta);

        // Añadir el panel a la ventana
        ventana.add(panel);

        ventana.setVisible(true);
    }
}

```

## 3. Creación de GUI con JavaFX

### 3.1 Creación de una Ventana JavaFX

La clase `Stage` se utiliza para crear una ventana en JavaFX.

```java
import javafx.application.Application;
import javafx.scene.Scene;
import javafx.scene.layout.StackPane;
import javafx.stage.Stage;

public class VentanaJavaFX extends Application {
    public static void main(String[] args) {
        launch(args);
    }

    @Override
    public void start(Stage primaryStage) {
        primaryStage.setTitle("Mi Ventana JavaFX");

        StackPane root = new StackPane();
        primaryStage.setScene(new Scene(root, 300, 200));

        primaryStage.show();
    }
}

```

### 3.2 Añadiendo Componentes en JavaFX

JavaFX proporciona una variedad de componentes para construir interfaces gráficas.

```java
import javafx.application.Application;
import javafx.scene.Scene;
import javafx.scene.control.Button;
import javafx.scene.control.Label;
import javafx.scene.layout.VBox;
import javafx.stage.Stage;

public class VentanaConComponentesJavaFX extends Application {
    public static void main(String[] args) {
        launch(args);
    }

    @Override
    public void start(Stage primaryStage) {
        primaryStage.setTitle("Ventana con Componentes JavaFX");

        VBox vbox = new VBox();

        Button button = new Button("Haz clic");
        Label label = new Label("¡Hola, Mundo!");

        vbox.getChildren().addAll(button, label);

        primaryStage.setScene(new Scene(vbox, 300, 200));

        primaryStage.show();
    }
}

```

## 4. Manejo de Eventos en GUI

### 4.1 Manejo de Eventos en Swing

Puedes manejar eventos, como clics de botón, utilizando listeners en Swing.

```java
import javax.swing.JButton;
import javax.swing.JFrame;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

public class EventosSwing {
    public static void main(String[] args) {
        JFrame ventana = new JFrame("Manejo de Eventos Swing");
        JButton boton = new JButton("Haz clic");

        // Agregar un ActionListener al botón
        boton.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                System.out.println("Botón clickeado");
            }
        });

        ventana.add(boton);
        ventana.setSize(300, 200);
        ventana.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        ventana.setVisible(true);
    }
}

```

### 4.2 Manejo de Eventos en JavaFX

JavaFX utiliza eventos y controladores para manejar interacciones del usuario.

```java
import javafx.application.Application;
import javafx.scene.Scene;
import javafx.scene.control.Button;
import javafx.scene.layout.StackPane;
import javafx.stage.Stage;

public class EventosJavaFX extends Application {
    public static void main(String[] args) {
        launch(args);
    }

    @Override
    public void start(Stage primaryStage) {
        primaryStage.setTitle("Manejo de Eventos JavaFX");

        Button button = new Button("Haz clic");

        // Agregar un EventHandler al botón
        button.setOnAction(e -> System.out.println("Botón clickeado"));

        StackPane root = new StackPane();
        root.getChildren().add(button);

        primaryStage.setScene(new Scene(root, 300, 200));

        primaryStage.show();
    }
}

```

## 5. Desarrollo de Interfaces Gráficas en Java

El desarrollo de interfaces gráficas en Java se facilita mediante las bibliotecas Swing y JavaFX. Est

as permiten la creación de ventanas, la adición de componentes y el manejo de eventos de manera eficiente. Ya sea trabajando con la simplicidad de Swing o la modernidad de JavaFX, ambas ofrecen herramientas poderosas para construir interfaces gráficas interactivas y atractivas. ¡Explora y crea GUI impresionantes en Java!