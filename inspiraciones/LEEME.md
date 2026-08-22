# inspiraciones/ — materia prima de CIFRA

Aquí sube Angel todo el material visual: fotos, videos, capturas de páginas que le
gustan, figuras, paletas, texturas. **Esta carpeta es la cantera; `assets/` es la obra
terminada.** Nada de aquí se enlaza directo en las páginas: los motores recortan,
editan, ajustan color y luego guardan lo aprobado en `assets/img` o `assets/video`.

## Estructura

```
inspiraciones/
├── _refs/          → capturas y links de otras webs (refero.design, moodboards)
├── recursos/
│   ├── svg/        → figuras, formas e íconos editables
│   ├── paletas/    → paletas de color, muestras, pruebas
│   └── texturas/   → grano, papel, ruido, degradados
├── cifra/          → material del proyecto Cifra (img/ + video/)
├── desvariando/    → material del proyecto Desvariando (img/ + video/)
├── reloj/          → material de Reloj 181 / portafolio de foto (img/ + video/)
└── LEEME.md        → este archivo
```

Cada carpeta de proyecto lleva un `notas.md`: ahí se anota qué es cada archivo,
qué se quiere lograr con él y qué decidió cada motor.

## Estructura libre por proyecto

Las carpetas `img/` y `video/` de cada proyecto son el punto de partida, **no una regla**.
Angel puede crear cuantas minicarpetas quiera dentro (arrastrando en el Explorador):
`cifra/img/retratos/`, `desvariando/video/reels/`, `reloj/favoritas/`, lo que haga falta.
Los motores buscan en todo el árbol recursivamente — ningún archivo queda perdido por
estar anidado. Única regla: nombres de carpeta sin espacios ni acentos.

## Cómo pedir trabajo con este material

Dícele al motor algo como:
- «En `inspiraciones/cifra/img` dejé 5 fotos: recórtalas a 16:9 para cards.»
- «De este video toma los primeros 4 segundos, muteado, para el hero.»
- «Juega con esta foto: pruébala en B/N, con contraste alto y con el acento de la V2.»

## Convenciones

- **Nombres:** sin espacios ni acentos — `2026-08-21_retrato-estudio.jpg`.
  La fecha ayuda a saber qué es nuevo.
- **Peso y videos:** los videos crudos de `inspiraciones/` **no entran al repo** — el
  `.gitignore` los excluye automáticamente (`mp4`, `mov`, `mkv`, `avi`, `m4v`, `webm`).
  Viven solo en esta PC (respaldo opcional arrastrándolos a OneDrive). Cuando un video
  se aprueba, el motor lo recorta/comprime (ideal < 8 MB) y lo guarda en
  `assets/video/`, que sí viaja a GitHub y Vercel. Las fotos sí entran al repo sin
  problema (peso normal < 10 MB cada una).
- **Originales intocables:** el motor nunca sobrescribe el archivo que subió Angel;
  trabaja sobre copias o exporta a `assets/`.
- **Derechos:** solo subir material propio o con permiso de uso (las fotos de Reloj 181
  son del proveedor/novia — confirmar que pueden publicarse en el sitio).

## Flujo acordado

1. Angel suelta archivos aquí.
2. Motor revisa, propone usos (hero, cards, fondos, marquesina…) y muestra pruebas.
3. Lo aprobado se optimiza y pasa a `assets/img` o `assets/video`, y la página lo usa.
4. Cada sesión deja nota en `BITACORA.md` y en el `notas.md` del proyecto tocado.
