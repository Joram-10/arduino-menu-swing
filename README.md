# Arduino Menu (Java Swing)

Ventana hecha con Java Swing para controlar un Arduino por puerto serial. Es la versión con interfaz gráfica de [arduino-consola-java](https://github.com/Joram-10/arduino-consola-java).

## Qué hace
- **Tools > Serial Ports**: lista los puertos seriales disponibles y eliges uno.
- **File > Conectar**: abre la conexión a 9600 baudios.
- Escribes un mensaje en el campo de texto y con **Enviar** se manda al Arduino.
- **File > Desconectar**: cierra la conexión.

Funciona con el sketch `led_serial.ino` de [arduino-consola-java](https://github.com/Joram-10/arduino-consola-java) (1 = encender, 2 = apagar, 3 = blink).

## Estructura
- `src/ejemplo_menu/Ejemplo_Menu.java`: clase principal, abre la ventana.
- `src/ejemplo_menu/ventana_main.java`: la ventana (interfaz generada con NetBeans) y la lógica serial.

## Requisitos
- Java 8 o superior
- Librerías [PanamaHitek_Arduino](https://github.com/PanamaHitek/PanamaHitek_Arduino) y [jSSC](https://github.com/java-native/jssc) agregadas al proyecto (los .jar no se incluyen en este repo)

## Uso
Abre la carpeta como proyecto en NetBeans (o cualquier IDE), agrega las librerías y ejecuta `ejemplo_menu.Ejemplo_Menu`.
