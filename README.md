# TablaView_de_Conductores_y_Constructores-Grupal-

![image](https://github.com/user-attachments/assets/07c0aced-81c8-41fa-b463-f1ab17d21ec5)

El código JavaFX define una clase `MainMenu` que extiende `Application` para crear un menú principal con varias opciones. A continuación se explica cada parte del código:

1. La clase `MainMenu` extiende `Application`, lo que permite crear una aplicación JavaFX.
2. El método `start` se sobrescribe para configurar la interfaz de usuario (UI) y establecer el escenario principal (`primaryStage`).

### Configuración del Escenario Principal

3. Se establece el título del escenario principal (`primaryStage`) como "MENU".

### Creación del Texto de Instrucciones

4. Se crea una etiqueta (`Label`) para mostrar las instrucciones al usuario.
5. Se establece la fuente, el color del texto y el relleno de la etiqueta.

### Creación de Botones

6. Se crean cinco botones usando el método `createStyledButton`, cada uno con un texto diferente.
7. Los botones son:
   - `driverPointsChartButton`: "TableView Constructor"
   - `driverTableButton`: "TableView Drivers"
   - `constructorPointsChartButton`: "Puntos Maximo"
   - `constructorTableButton`: "Gráfico de Barras - Total de Puntos"
   - `constructorRankChartButton`: "Gráfico de Barras - Rank"

### Configuración de Acciones para los Botones

8. Se establecen las acciones de los botones utilizando `setOnAction`. Cada botón abre una nueva ventana llamando a diferentes clases:
   - `driverPointsChartButton` abre `Main`.
   - `driverTableButton` abre `MainDrivers`.
   - `constructorPointsChartButton` abre `MainMax`.
   - `constructorTableButton` abre `MainPoint`.
   - `constructorRankChartButton` abre `MainDiagramRank`.

### Creación del Contenedor VBox

9. Se crea un contenedor `VBox` para organizar los elementos en una columna con un espacio de 10 píxeles entre ellos.
10. Se agregan la etiqueta de instrucciones y los botones al `VBox`.
11. Se alinea el `VBox` en el centro y se establece un relleno de 10 píxeles.

### Configuración de la Imagen de Fondo

12. Se carga una imagen de fondo desde un archivo local utilizando la clase `Image`.
13. Se crea un `ImageView` para mostrar la imagen de fondo.
14. Se ajusta la imagen de fondo para llenar el tamaño del `StackPane`.

### Creación del Contenedor StackPane

15. Se crea un contenedor `StackPane` para apilar la imagen de fondo y el `VBox`.
16. Se agregan el `ImageView` y el `VBox` al `StackPane`.

### Configuración de la Escena y el Escenario

17. Se crea una escena (`Scene`) con el `StackPane` como raíz y un tamaño de 550x450 píxeles.
18. Se establece la escena en el escenario principal (`primaryStage`).
19. Se muestra el escenario principal (`primaryStage.show()`).

### Método Auxiliar createStyledButton

20. El método `createStyledButton` crea un botón estilizado con el texto proporcionado.
21. Se establece la fuente, el color del texto, el estilo de fondo y borde, el relleno y el ancho mínimo del botón.
22. Se devuelve el botón creado.

### Método main

23. El método `main` lanza la aplicación JavaFX.

El código crea una ventana principal con un menú estilizado que incluye cinco botones. Cada botón abre una nueva ventana al ser presionado, y la ventana principal tiene una imagen de fondo.
