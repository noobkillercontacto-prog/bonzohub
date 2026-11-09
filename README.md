# Bonzo HUD (Fabric 1.21.1)

HUD estilo cliente + rueda de emotes. Solo cliente, sin hacks.

## Compilar el .jar

**Opcion A, local** (JDK 21 + Gradle 8.8+):

    gradle build

El jar queda en `build/libs/bonzohud-1.0.0.jar`.

**Opcion B, sin instalar nada:** sube la carpeta a un repo de GitHub. El workflow
`.github/workflows/build.yml` compila solo y deja el jar en Actions > Artifacts.

## Instalar
Pon el jar en `.minecraft/mods/` junto con **Fabric API** (para 1.21.1).

## Teclas (se pueden cambiar en Controles > Bonzo HUD)
- `B` rueda de emotes (clic en un emote para reproducirlo, clic en el centro para parar; moverte tambien lo para)
- `C` zoom (mantener)
- `V` toggle sprint
- `H` mostrar/ocultar todo el HUD

## Comandos
- `/bonzohud track Titulo;Artista;segundos` muestra la tarjeta de musica
- `/bonzohud lyric texto` muestra una linea de letra
- `/bonzohud lrc` carga `config/bonzohud/lyrics.lrc` (formato LRC) y la sincroniza
- `/bonzohud stop` quita el widget
- `/bonzohud toggle <topbar|music|coords|keybinds|effects|bars|target|armor|items>`

## Notas
- El widget de musica es visual: no reproduce audio.
- Los emotes son locales: solo tu los ves (en tercera persona).
- Las barras de vida/hambre reemplazan las vanilla; `/bonzohud toggle bars` las devuelve.
