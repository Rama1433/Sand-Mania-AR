# Sand Mania V3 — Arena mezclada y niveles progresivos

Esta versión parte de **Sand Mania V2 — Desafío Arena** y conserva controles, físicas de arena, récord local y objetivo principal. Es un proyecto independiente de Merge Mania, Pixel Survivor y Barber Manager.

## Novedades

- El 50% inferior del tablero empieza ocupado por arena **mezclada en manchas irregulares**, sin franjas completas de un solo color.
- Cada nuevo nivel cambia la distribución y genera manchas más pequeñas y fragmentadas.
- La eliminación requiere simultáneamente un grupo conectado del mismo color, arena depositada por el jugador, una cantidad mínima de granitos y una extensión horizontal mínima. Ya no desaparecen pequeños grupos de 125 granitos.
- Requisitos progresivos: nivel 1 requiere 340 granitos y 18 columnas de extensión; nivel 2, 395 y 21; nivel 3, 450 y 24; nivel 4, 505 y 27; hasta un máximo de 600 granitos y 32 columnas en niveles avanzados.
- El objetivo sigue siendo despejar el 80% de la arena original para avanzar. La puntuación se acumula y el récord se mantiene.
- Los umbrales actuales se muestran debajo de la barra de limpieza, para que puedas planear tus movimientos.

## Jugabilidad

Las piezas contienen 100 granitos de arena. En PC, izquierda/derecha para mover, arriba o R para girar y espacio/abajo para soltar. En celular podés arrastrar y soltar o usar los botones.

La mezcla se hace más exigente por nivel. Si un grupo no desaparece, todavía no cumple la cantidad, la extensión o la conexión con arena que soltaste. Puede ser necesario conectar más de una región con varias piezas.

## Uso

Para jugar offline, abrí `index.html` en el navegador. Para probarla como PWA, desde esta carpeta:

```powershell
py -m http.server 5500
```

Visitá http://localhost:5500.

## Publicación en Vercel

Abrí esta carpeta en VS Code y usá `npx vercel` para un proyecto nuevo `sand-mania` dentro de Arcade-AR, o `npx vercel link` para vincular el proyecto específico de Sand Mania. Luego `npx vercel --prod`.

**No seleccionar proyectos de Barber Manager ni Merge Mania.**
