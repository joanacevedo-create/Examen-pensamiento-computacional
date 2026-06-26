# TOKYO ARCADE

## Información del proyecto

**Nombre del proyecto:** Tokyo Arcade
**Autor:** Joan Esteven Acevedo Hernández
**Asignatura:** Pensamiento Computacional
**Tipo de proyecto:** Sistema visual interactivo desarrollado en p5.js

### Enlaces

* **Proyecto ejecutable:** [AGREGAR LINK PÚBLICO DE P5.JS]
* **Código editable:** [AGREGAR LINK EDITABLE DE P5.JS]
* **Repositorio de GitHub:** [AGREGAR LINK DEL REPOSITORIO]

---

## Descripción general

Tokyo Arcade es un juego de reflejos desarrollado en p5.js. El proyecto presenta una experiencia visual dividida en tres estados: una interfaz inicial, un juego dentro de una máquina arcade y una pantalla final.

El usuario debe hacer clic rápidamente sobre círculos rojos que aparecen en distintas posiciones antes de que termine el tiempo disponible. Cada acierto suma un punto, mientras que no presionar el círculo a tiempo resta una vida.

Cuando las vidas llegan a cero, el sistema muestra el puntaje final y permite reiniciar la experiencia presionando la tecla `R`.

---

## Descripción objetiva

### ¿Qué es el proyecto?

Es un sistema visual interactivo que combina diseño gráfico, programación y una mecánica simple de reflejos.

El programa recibe acciones del usuario mediante el mouse y el teclado, procesa estas entradas y genera respuestas visuales dinámicas.

### ¿Qué se ve en pantalla?

El proyecto está dividido en tres pantallas principales:

1. Una interfaz inicial inspirada en el diseño gráfico japonés.
2. Una máquina arcade donde se desarrolla el juego.
3. Una pantalla final inspirada en el agua y la calma.

### Elementos visuales

* Formas geométricas rojas, negras y taupe.
* Tipografía vertical.
* Textos en español y japonés.
* Máquina arcade japonesa.
* Retícula dentro de la pantalla del juego.
* Círculo rojo interactivo.
* Ondas de agua en la pantalla final.
* Puntaje y cantidad de vidas.

### Inputs utilizados

* Clic del mouse.
* Posición del mouse.
* Tecla `R`.
* Tiempo transcurrido.

### Outputs generados

* Cambio entre estados.
* Movimiento aleatorio del círculo.
* Aumento del puntaje.
* Pérdida de vidas.
* Cambio de tamaño del círculo.
* Aparición de la pantalla final.
* Reinicio de la experiencia.

---

## Descripción conceptual

### Idea central

La idea central del proyecto es representar el contraste entre la velocidad y la calma.

La experiencia comienza con una composición gráfica controlada, continúa con un juego de reflejos rápido dentro de una máquina arcade y termina con una pantalla inspirada en el agua calmada.

El usuario atraviesa un recorrido desde la concentración inicial, pasa por la presión y velocidad del juego y finalmente llega a un estado visual más tranquilo.

### Corriente y área del diseño

El proyecto se relaciona principalmente con:

* Diseño gráfico japonés contemporáneo.
* Diseño editorial.
* Diseño de interfaces.
* Gráfica arcade.
* Composición tipográfica.

### Referentes visuales

Los principales referentes utilizados fueron:

* Afiches japoneses con composiciones asimétricas.
* Uso de tipografía vertical.
* Paletas limitadas de rojo, negro y crema.
* Máquinas arcade japonesas.
* Formas geométricas simples.
* Diseño editorial de alto contraste.

### Principios de diseño explorados

* Jerarquía visual.
* Contraste.
* Asimetría.
* Ritmo.
* Repetición.
* Equilibrio.
* Composición geométrica.
* Relación entre imagen y tipografía.

---

## Sistema computacional

### Inputs

El programa recibe los siguientes datos:

* Clic sobre el botón inicial.
* Clic sobre el círculo rojo.
* Posición horizontal y vertical del mouse.
* Tiempo transcurrido desde la aparición del círculo.
* Tecla `R` para reiniciar.

### Procesos

El sistema realiza los siguientes procesos:

* Detecta si el usuario presiona el botón de inicio.
* Calcula la distancia entre el mouse y el círculo.
* Determina si el clic ocurrió dentro del círculo.
* Genera nuevas posiciones aleatorias.
* Mide el tiempo disponible mediante `millis()`.
* Reduce vidas cuando se supera el tiempo límite.
* Aumenta el puntaje cuando el usuario acierta.
* Modifica el tamaño del círculo según el puntaje.
* Cambia de estado cuando se terminan las vidas.
* Reinicia las variables cuando se presiona `R`.

### Estados

#### Estado 0: pantalla inicial

Muestra:

* Título del proyecto.
* Instrucciones en japonés y español.
* Formas geométricas.
* Botón `PRESS TO START`.

En este estado todavía no se ejecuta el juego.

#### Estado 1: juego

Muestra:

* Máquina arcade.
* Pantalla del videojuego.
* Retícula.
* Puntaje.
* Vidas.
* Círculo rojo.

En este estado se activa la mecánica principal.

#### Estado 2: pantalla final

Muestra:

* Puntaje final.
* Textos en español y japonés.
* Ondas de agua.
* Instrucción para reiniciar.

### Eventos

Los principales eventos son:

* Presionar el botón inicial.
* Hacer clic correctamente sobre el círculo.
* No hacer clic dentro del tiempo establecido.
* Llegar a cero vidas.
* Presionar la tecla `R`.

### Outputs

Los outputs principales son:

* Cambio de pantalla.
* Aparición del círculo.
* Cambio de posición.
* Cambio de tamaño.
* Aumento de puntaje.
* Reducción de vidas.
* Resultado final.

---

## Explicación de la interacción

El usuario comienza en la pantalla inicial y debe hacer clic sobre el botón `PRESS TO START`.

Después de presionar el botón, el sistema cambia al estado del juego.

Dentro de la pantalla de la máquina arcade aparece un círculo rojo en una posición aleatoria. El jugador tiene 1,5 segundos para hacer clic sobre él.

Si el usuario hace clic correctamente:

* Suma un punto.
* El círculo cambia de posición.
* El temporizador vuelve a comenzar.

Si el usuario no hace clic a tiempo:

* Pierde una vida.
* El círculo cambia de posición.
* El temporizador vuelve a comenzar.

Cuando las vidas llegan a cero, el sistema cambia automáticamente a la pantalla final.

En la pantalla final se muestra el puntaje obtenido. El usuario puede presionar la tecla `R` para volver a la pantalla inicial.

---

## Uso de variables

Las variables permiten almacenar información que cambia durante el programa.

Algunas de las principales variables utilizadas son:

* `estado`: controla qué pantalla se muestra.
* `puntaje`: guarda los puntos conseguidos.
* `vidas`: guarda la cantidad de oportunidades restantes.
* `circuloX`: posición horizontal del círculo.
* `circuloY`: posición vertical del círculo.
* `tamanoCirculo`: tamaño inicial.
* `tamanoDinamico`: tamaño que cambia según el puntaje.
* `tiempoCirculo`: momento en que aparece el círculo.
* `limiteCirculo`: tiempo máximo disponible.

---

## Uso de condicionales

Los condicionales permiten que el programa tome decisiones.

Se utilizan para:

* Elegir qué estado mostrar.
* Detectar si el usuario hizo clic sobre el botón.
* Detectar si el usuario hizo clic sobre el círculo.
* Revisar si terminó el tiempo.
* Revisar si las vidas llegaron a cero.
* Revisar si se presionó la tecla `R`.

---

## Uso de funciones propias

El proyecto utiliza funciones propias para separar las distintas tareas del sistema.

### `interfazInicio()`

Dibuja la pantalla inicial.

### `pantallaJuego()`

Dibuja la máquina y ejecuta la lógica del juego.

### `pantallaFinal()`

Dibuja la pantalla de resultado.

### `cambiarCirculo()`

Genera una nueva posición aleatoria para el círculo.

---

## Uso de bucles

Se utilizan dos bucles `for` para construir la retícula de la pantalla del videojuego.

Un bucle dibuja las líneas verticales y el segundo dibuja las líneas horizontales.

Esto permite repetir elementos sin tener que escribir cada línea de manera individual.

---

## Uso de `random()`

La función `random()` genera posiciones diferentes para el círculo.

```javascript
circuloX = random(170, 430);
circuloY = random(370, 550);
```

Esto evita que el círculo aparezca siempre en el mismo lugar y permite que cada partida sea diferente.

---

## Uso de `map()`

La función `map()` transforma el puntaje en un nuevo tamaño para el círculo.

Mientras mayor es el puntaje, más pequeño se vuelve el círculo.

```javascript
tamanoDinamico = map(
  puntaje,
  0,
  20,
  tamanoCirculo,
  25,
  true
);
```

Este cambio aumenta progresivamente la dificultad del juego.

---

## Uso de tiempo

El sistema utiliza `millis()` para calcular cuánto tiempo lleva visible el círculo.

```javascript
millis() - tiempoCirculo
```

Si el resultado supera los 1.500 milisegundos, el jugador pierde una vida.

---

## Recurso multimedia utilizado

### Tipo de recurso

Imagen digital de una máquina arcade japonesa.

### Función dentro del proyecto

La imagen no funciona únicamente como decoración. Su pantalla determina y delimita el espacio donde se desarrolla el juego.

Sobre la pantalla original de la máquina se dibuja un rectángulo negro y luego se incorporan los elementos interactivos.

De esta forma, la máquina forma parte de la lógica visual y funcional del sistema.

---

## Paleta de colores

* Crema: `#e1decc`
* Taupe: `#474145`
* Rojo: `#e70f0e`
* Negro: `#010101`
* Azul agua: `#9fc5d6`

El rojo funciona como color de énfasis y elemento interactivo. El negro aporta contraste, mientras que el crema funciona como fondo principal. El azul aparece únicamente en la pantalla final para representar la calma.

---

## Diagrama de flujo

<img width="1024" height="1536" alt="ChatGPT Image 26 jun 2026, 10_46_31" src="https://github.com/user-attachments/assets/e956835f-720d-443e-ad31-5f759670d810" />


El diagrama explica:

* Inputs.
* Procesos.
* Decisiones.
* Estados.
* Eventos.
* Outputs.
* Transiciones.

---

## Registro visual
<img width="1010" height="437" alt="Captura de pantalla 2026-06-25 150222" src="https://github.com/user-attachments/assets/60fc7857-6f03-4dfc-a1db-33c218a6c615" />

<img width="1136" height="502" alt="Captura de pantalla 2026-06-25 163055" src="https://github.com/user-attachments/assets/9adfd8af-4b68-4c06-9fa8-a9e0102bea73" />

<img width="1029" height="531" alt="Captura de pantalla 2026-06-25 191600" src="https://github.com/user-attachments/assets/b32643c2-6d48-4511-94ad-bdd135de331d" />

<img width="978" height="532" alt="Captura de pantalla 2026-06-25 232807" src="https://github.com/user-attachments/assets/1d07137f-c4d6-482e-8aa7-24ff58c6aeff" />

<img width="882" height="475" alt="Captura de pantalla 2026-06-25 233228" src="https://github.com/user-attachments/assets/c25e6677-6187-47b7-9446-fb4b0a390b5b" />

<img width="880" height="490" alt="Captura de pantalla 2026-06-25 234221" src="https://github.com/user-attachments/assets/51a281ce-f47c-4b82-aedd-07c01de4bed1" />

<img width="984" height="534" alt="Captura de pantalla 2026-06-26 001224" src="https://github.com/user-attachments/assets/dc99abea-4cce-4039-8dc0-b91666e550f9" />

<img width="980" height="548" alt="Captura de pantalla 2026-06-26 001241" src="https://github.com/user-attachments/assets/78aaf149-efec-45e4-846f-8fd8937ce3a2" />

<img width="943" height="527" alt="Captura de pantalla 2026-06-26 002309" src="https://github.com/user-attachments/assets/11012c2a-cb98-4411-aa7a-5c3ef9a45448" />

<img width="978" height="532" alt="Captura de pantalla 2026-06-26 003250" src="https://github.com/user-attachments/assets/bc9efa88-4f28-4dfa-b2b7-0d3e5e05a640" />
<img width="977" height="547" alt="Captura de pantalla 2026-06-26 003239" src="https://github.com/user-attachments/assets/c8e17746-80f0-4b3e-a883-abd4b4a403d4" />

### Referentes
<img width="736" height="1104" alt="Best Whiskey Art Poster – Minimalist Japanese-Inspired Design💙 (2)" src="https://github.com/user-attachments/assets/48c4e712-3b59-4d03-8288-022f8ad713bf" />

<img width="736" height="1472" alt="Retro Gaming Haven_ Japanese Arcade Nostalgia" src="https://github.com/user-attachments/assets/ffb453d5-f353-48ae-af1c-6d450575f87e" />
<img width="736" height="1104" alt="descarga" src="https://github.com/user-attachments/assets/8a2af2a6-3c43-4e9a-849c-97d64c0974a7" />



## Reflexión final

### Principales decisiones tomadas

Una de las decisiones principales fue trabajar con un juego sencillo de reflejos para poder concentrarme en la relación entre interacción, diseño visual y estructura computacional.

También decidí utilizar tres estados claramente diferenciados, de manera que el proyecto tuviera una progresión completa y no funcionara solamente como una visualización continua.

La máquina arcade fue utilizada como marco visual del juego y como recurso multimedia funcional.

### Dificultades encontradas

Las principales dificultades fueron:

* Comprender la organización entre `setup()`, `draw()` y las funciones propias.
* Separar correctamente los estados.
* Detectar si el clic ocurría dentro del círculo.
* Controlar el tiempo con `millis()`.
* Mantener el círculo dentro del área de la pantalla.
* Ordenar el código sin repetir funciones.
* Adaptar la estética gráfica a un sistema interactivo.

### Aprendizajes obtenidos

Durante el desarrollo aprendí a:

* Utilizar variables.
* Crear condicionales.
* Organizar el código mediante funciones.
* Utilizar bucles.
* Generar valores aleatorios.
* Transformar valores mediante `map()`.
* Detectar clics.
* Controlar eventos de teclado.
* Crear y administrar estados.
* Integrar imágenes dentro de p5.js.
* Diseñar una experiencia visual interactiva.

El aprendizaje principal fue entender que un sistema interactivo no depende solamente de su apariencia, sino también de las reglas, decisiones y respuestas que se producen a partir de las acciones del usuario.
