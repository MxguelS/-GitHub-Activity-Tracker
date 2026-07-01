# ghstats s

GitHub Activity Tracker para terminal — dashboard visual con `gum`, `gh` CLI, `jq`, `toilet` y `lolcat`.

## Preview

![ghstats demo](demo.gif)
## Instalación

```bash
sudo pacman -S github-cli jq gum toilet lolcat
gh auth login
curl -o ~/.local/bin/ghstats https://raw.githubusercontent.com/MxguelS/ghstats/main/ghstats
chmod +x ~/.local/bin/ghstats
```

## Uso

```bash
ghstats                  # tu propio perfil
ghstats octocat          # perfil de otro usuario
ghstats --no-cache       # forzar refresh
ghstats --repo mi-repo   # ver commits de un repo específico
ghstats --help
```

## Features

- Stats generales: repos, stars, commits (30d), issues, contribuciones del año
- Distribución de lenguajes con barras
- Tabla interactiva de repos (selecciona uno con Enter)
- Ver commits recientes o abrir en navegador
- Caché de 5 min para no golpear el rate limit de la API
