# Pool Day – FPS en el navegador

Shooter en primera persona inspirado en el mapa `pool_day` de Counter-Strike. Es un solo archivo (`index.html`) con Three.js cargado desde CDN (unpkg).

## Cómo jugar
Abrí `index.html` en un navegador moderno (necesitás internet para bajar Three.js). Si el navegador bloquea módulos desde `file://`, levantá un servidor local:
```
cd juego-pool && python3 -m http.server 8000
```
y entrá a http://localhost:8000

## Controles
| Tecla | Acción |
|---|---|
| W A S D | Moverse |
| Mouse | Apuntar |
| Click izquierdo | Disparar |
| Click derecho | Mira telescópica (francotirador) |
| Espacio | Saltar |
| Shift | Caminar despacio |
| E | Agarrar arma cercana (también se agarran pasando por encima) |
| R | Recargar |
| 1-5 | Cuchillo, Pistola, Rifle, Escopeta, Francotirador |
| Esc | Pausa |

## Para modificar
Todo está en `index.html`, separado por secciones comentadas:
- `CONFIGURACIÓN GENERAL`: tamaño de arena, piscina, cantidad de bots.
- `WEAPONS`: daño, cadencia, cargador, munición, dispersión de cada arma.
- `buildMap()`: casitas, cajas, palmeras.
- `pickupSpots`: dónde aparecen las armas en el piso.
- `updateBots()`: inteligencia de los enemigos.
