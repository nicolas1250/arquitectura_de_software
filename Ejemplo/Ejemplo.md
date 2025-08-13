# Ejemplo de Programación Orientada a Eventos

Este es un ejemplo sencillo de programación orientada a eventos y la idea es que el programa reaccione cuando el usuario hace clic en un botón.

---

## Código

```java
import javax.swing.*;

public class Ejemplo_Poe {
    public static void main(String[] args) {
        JFrame ventana = new JFrame("Ejemplo");
        JButton boton = new JButton("Presionar");

        // Evento: cuando se hace clic en el botón
        boton.addActionListener(e -> System.out.println("¡Botón presionado!"));

        ventana.add(boton);
        ventana.setSize(200, 100);
        ventana.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        ventana.setVisible(true);
    }
}

```

## Cómo funciona

- El programa crea una ventana con un botón.

- El código no ejecuta todo seguido, sino que espera a que el usuario haga clic.

- Cuando se detecta el evento de clic, se ejecuta la acción configurada (imprimir en consola).