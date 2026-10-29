# Editor del mapa del mundo — zonas, marcadores y rótulos del mapa del mundo

El editor del mapa del mundo dibuja el mapa de viaje de `map_base` sobre el juego en marcha: polígonos de regiones, marcadores y rótulos, cada uno con título, descripción, la escena a la que lleva y si está bloqueado u oculto. Una vista previa muestra el mapa tal como lo verá el jugador, y **Actualizar el mapa del juego** lleva los cambios guardados al juego en curso.

Esta herramienta es para el mapa del mundo. Los mapas de casillas del mundo RPG se editan con el editor de mapas RPG (`rpg_editor`).

## Cómo abrirlo

Botón del martillo en la barra del juego → **Editor de mapas**.

## Editar el mapa

![El editor del mapa del mundo con el mapa de cthangover: las zonas home, home_label, town_entry y town_entry_label a la izquierda, la región de la villa seleccionada en el mapa con sus vértices y sus propiedades a la derecha: escena home_outside, disponibilidad, En el juego: abierta.](assets/map-editor.jpg)

1. Elige un mod y un archivo de mapa (`map/*.json`) en el selector.
2. **+ Región** (o **Dibujar**) y pulsa el mapa para colocar vértices; doble clic, Intro o Esc terminan, el botón derecho quita el último vértice. **+ Marcador** y **+ Rótulo** añaden los otros tipos de zona.
3. Selecciona una zona en **Zonas** o en el mapa. En **Propiedades de la zona** pon su ID, **Título** y **Descripción** (claves de localización; una traducción ausente se marca), su **Escena** y la **Disponibilidad**: *Bloqueada para viajar* u *Oculta en el mapa*. La línea **En el juego:** dice lo que el jugador obtendrá de verdad (abierta, bloqueada por la marca, bloqueada porque falta la escena, oculta).
4. Arrastra zonas y vértices en el mapa; el botón derecho sobre un vértice lo borra, Supr borra la zona.
5. **▶ Como en el juego** muestra el mapa como lo ve el jugador (al pasar el ratón, tarjeta de zona, marcadores), incluidos los cambios sin guardar.
6. Ctrl+S guarda; **Actualizar el mapa del juego** relee los archivos guardados en el juego en curso.

## Límites

- Solo mods de carpeta; los mods empaquetados son de solo lectura.
- Títulos y descripciones son claves de localización; sus textos se editan en los archivos de localización del mod.

## Dependencias

`tools_base`, `map_base`, `ui_base`.
El paquete antiguo `editor_tools` instala este mod junto con las demás ventanas de autor.
