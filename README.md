# ⚙️ Mis Dotfiles de Hyprland


Este repositorio contiene todos los archivos de configuración (`dotfiles`) que utilizo para mi entorno de escritorio basado en el *tiling window manager* Hyprland. He optado por una estructura de archivos **modular** y **separada** para mantener la **organización** y la **fácil mantenimiento**.

##  Estructura
Mi configuración está dividida en varios archivos separados, donde `hyprland.conf` actúa como el archivo principal que importa la configuración de los demás.

```
~/.config/hypr/
├── hyprland.conf    # Archivo principal, importa los demás.
├── env.conf         # Definición de variables de entorno ($ENV).
├── exec.conf        # Comandos que se ejecutan al inicio (autostart).
├── general.conf     # Configuración general, efectos, animaciones, etc.
├── keybinds.conf    # Atajos de teclado y enlaces a QuickShell/Noctalia.
└── window.conf      # Reglas de ventanas y configuración de apariencia.
```

*(Nota: El archivo `colors.conf` generado por Matugen se incluiría típicamente aquí y se importaría en `hyprland.conf`.)*

-----

##  Características
  * **Organización Modular:** Toda la configuración está separada en archivos temáticos (ejecución, variables, atajos) para una gestión clara.
  * **Gestión de Colores con Matugen:** Utilizo **Matugen** para generar un esquema de colores dinámico basado en mi fondo de pantalla actual. Este esquema genera un archivo (`colors.conf` o similar) que inyecta las variables de color usadas en el entorno y en `general.conf`.
  * **Integración de Noctalia/QuickShell:** El archivo `keybinds.conf` está configurado para integrar comandos y funciones de la *shell* **Noctalia** y su *launcher* **QuickShell**.
