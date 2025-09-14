# PKM_SQL
Consultas SQL para analizar datos de Pokémon usando un esquema relacional. Incluye combinaciones de tablas con JOIN, subconsultas, filtros avanzados y agregaciones para obtener respuesta a diferentes preguntas.

## Introducción
Existen más de 1.000 especies de pokemon distintas, cada una con sus características y particularidades. 

A nivel competitivo es fácil sentirse abrumado con la inmensa cantidad de combinaciones y estrategias distintas que se pueden crear. 

Cuando uno busca la forma de optimizar a su equipo pokemon pueden surgir preguntas cómo "¿qué pokemon puedo añadir al equipo que sea de tipo fuego, sea capaz de hacer el ataque "envite igneo" y tenga unos stats de ataque elevados?". 

Encontrar respuesta a este tipo de preguntas puede convertirse en un proceso largo y tedioso si se consulta manualmente. Es por esto por lo que decidí emplear mis conocimientos en SQL para hacer este proyecto. Más abajo se encuentran diferentes preguntas que he propuesto, pero pueden ser modificadas para adaptarse a las dudas que tengan otros. De esta forma buscar al pokemon óptimo para tu estrategia se convierte en un proceso mucho más rápido y práctico.  

Hay varias bases de datos públicas, pero hay una que me sorprendió bastante por lo completa que está. Es la que he utilizado para el proyecto, no he llegado a utilizar todos sus archivos CSV, solo los necesarios para las consultas que realicé. 
Fuente de los datos: https://github.com/PokeAPI/pokeapi/tree/master/data/v2/csv. 

Incluye información de todas las generaciones hasta pokemon escarlata y púrpura.

## Descripción de los datos

A continuación describo brevemente las ficheros csv que usaremos: 
| Nombre_fichero | Nº registros | Descripción |
|---|---|---|
| abilities.csv | 367 | Nombre de todas las habilidades que hay. |
| ability_names.csv | 3039 | Nombres de las habilidades en diferentes idiomas. Nos permitirá buscar el nombre de la habilidad en español. |
| machines.csv | 2102 | Números de las distintas máquinas para aprender ataques y el ataque que enseñan. |
| move_names.csv | 8910 | Nombres de los movimientos en diferentes idiomas. Nos permitirá buscar el nombre del movimiento en español. |
| moves.csv | 937 | Todos los movimientos, su poder, precisión, tipo y demás. |
| pokemon_abilities.csv | 2917 | Todas las habilidades que puede llegar a tener cada pokemon. |
| pokemon_moves.csv | 609926 | Todos los movimientos que puede llegar a tener cada pokemon. |
| pokemon_species.csv | 1025 | Nombre de cada pokemon, junto con otros datos como color o si es legendario. |
| pokemon_stats.csv | 7812 | Las estadísticas de combate de cada pokemon. Incluye estadísticas de variaciones como megaevoluciones u otros estados. |
| pokemon_types.csv | 2028 | Los tipos de cada pokemon (primario y secundario). |
| stats.csv | 8 | Los diferentes stats que existen. |
| type_names.csv | 210 | Nombres de los tipos en diferentes idiomas. Nos permitirá buscar el nombre del tipo en español. |
| types.csv | 21 | Nombre de todos los tipos que hay. |

## Diagrama de relaciones (simplificado)
En el siguiente diagrama se muestran las relaciones de las tablas. Para facilitar la comprensión se omiten las columnas que no se llegan a emplear.

![Diagrama_relaciones_pkm_v4](https://github.com/user-attachments/assets/49b62eb3-ffb7-4047-b1f0-b22cf213817a)
