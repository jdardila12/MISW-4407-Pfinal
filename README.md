
## Integrantes:

|   Nombre                         |   Correo                      | Codigo    |
|----------------------------------|-------------------------------|-----------|
| Juan David Ardila Cruz           | jd.ardila12@uniandes.edu.co   | 201415322 |

## Controles del Juego

`Flechas direccionales`  
Mueven al jugador de izquierda a derecha.

`Tecla Z`  
Botón de acción principal:  
- Inicia el juego.  
- Dispara proyectiles.

`Tecla G`  
Activa el **God Mode**:  
- Muestra un texto en verde indicando que el modo está activo.  
- El jugador no recibe daño de las balas enemigas.

`Barra espaciadora`  
Activa la vista de **Debug**:  
- Muestra rectángulos de colisión.  
- Indica los puntos de origen de las entidades y sus áreas visuales.  
- No se incluyen textos para evitar sobrecarga visual.  
- Se usó para depurar las animaciones de explosiones.



## Enlace al Juego Publicado

[itch.io] https://jdardila12.itch.io/misw-4407-pfinal

## Estructura del Proyecto

https://github.com/jdardila12/MISW-4407-Pfinal/blob/main/Documentation/mermaid-diagram-2025-05-16-114134.png

📁 MISW-4407-Pfinal/
├── .gitignore
├── .pylintrc
├── main.py
├── README.md
├── requirements.txt
├── Documentation/
│   ├── digram.png
│   └── digram.puml
├── assets/
│   ├── cfg/
│   │   ├── bullet.json
│   │   ├── enemies.json
│   │   ├── enemy_field.json
│   │   ├── interface.json
│   │   ├── level.json
│   │   ├── menu_screen.json
│   │   ├── pause.json
│   │   ├── player.json
│   │   ├── starfield.json
│   │   ├── start_screen.json
│   │   └── window.json
│   ├── fnt/
│   │   └── PressStart2P.ttf
│   ├── img/
│   │   ├── invaders_char.png
│   │   ├── invaders_enemy_01.png
│   │   ├── invaders_enemy_02.png
│   │   ├── invaders_enemy_03.png
│   │   ├── invaders_enemy_04.png
│   │   ├── invaders_enemy_explosion.png
│   │   ├── invaders_level_flag.png
│   │   ├── invaders_life.png
│   │   ├── invaders_logo_title.png
│   │   ├── invaders_player_explosion.png
│   │   └── invaders_title.png
│   └── snd/
│       ├── game_over.ogg
│       ├── game_paused.ogg
│       ├── game_start.ogg
│       ├── player_die.ogg
│       └── player_shoot.ogg
├── esper/
│   └── __init__.py
├── src/
│   ├── create/
│   │   ├── prefab_creator.py
│   │   ├── prefab_creator_interface.py
│   │   ├── prefab_general.py
│   │   └── __init__.py
│   ├── ecs/
│   │   ├── components/
│   │   │   ├── c_animation.py
│   │   │   ├── c_blinking.py
│   │   │   ├── c_input_command.py
│   │   │   ├── c_reload.py
│   │   │   ├── c_surface.py
│   │   │   ├── c_transform.py
│   │   │   ├── c_velocity.py
│   │   │   └── tags/
│   │   │       ├── c_tag_bullet.py
│   │   │       ├── c_tag_enemy.py
│   │   │       ├── c_tag_enemy_bullet.py
│   │   │       ├── c_tag_explosion.py
│   │   │       ├── c_tag_player.py
│   │   │       ├── c_tag_player_bullet.py
│   │   │       ├── c_tag_star.py
│   │   │       └── __init__.py
│   │   └── __init__.py
│   ├── systems/
│   │   ├── s_animation.py
│   │   ├── s_blinking_text.py
│   │   ├── s_bullet_player_align.py
│   │   ├── s_bullet_shoot.py
│   │   ├── s_collision_enemy_bullet.py
│   │   ├── s_collision_player_bullet.py
│   │   ├── s_enemy_bullet_movement.py
│   │   ├── s_enemy_move.py
│   │   ├── s_explosion_kill.py
│   │   ├── s_input.py
│   │   ├── s_movement.py
│   │   ├── s_moving_text.py
│   │   ├── s_player_limits.py
│   │   ├── s_rendering.py
│   │   ├── s_rendering_debug_rects.py
│   │   ├── s_screen_bullet.py
│   │   ├── s_starfield.py
│   │   ├── s_toggle_god_mode.py
│   │   └── __init__.py
│   ├── engine/
│   │   ├── game_engine.py
│   │   ├── scenes/
│   │   │   └── scene.py
│   │   ├── services/
│   │   │   ├── cfgs_service.py
│   │   │   ├── fonts_service.py
│   │   │   ├── images_service.py
│   │   │   ├── sounds_service.py
│   │   │   └── __init__.py
│   │   └── service_locator.py
│   └── game/
│       ├── menu_scene.py
│       ├── play_scene.py
│       └── start_scene.py
