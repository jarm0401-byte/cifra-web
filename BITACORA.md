# BITACORA.md — bitácora compartida de cifra-web

Registro compartido entre Claude Code y OpenCode. **Entradas nuevas ARRIBA.**
Formato sugerido: `## AAAA-MM-DD — <motor>` + Cambios / Hallazgos / Ideas / Pendiente.

---

## 2026-08-21 — OpenCode (relevo: memoria privada + cierre de inspiraciones + Vercel)

**Contexto:** esta sesión retoma el hilo después de que la sesión de `inspiraciones/`
quedó sin commit ni push (se anuncian cambios en bitácora que no llegaron a disk:
`.gitignore` de videos y actualización de LEEME — el LEEME sí existe dentro de
`inspiraciones/`, el `.gitignore` no existía). Se completa ese trabajo pendiente.

**Cambios**
- `.gitignore` raíz creado combinando dos intents: videos crudos de `inspiraciones/`
  fuera del repo (mp4/mov/mkv/avi/m4v/webm, como pedía la sesión anterior) Y
  `memoria.html` — nuevo archivo PRIVADO de Angel.
- Creada **`memoria.html`** (local, gitignored): línea de tiempo privada de cambios
  importantes con buscador, filtros por motor y estadísticas; sembrada con los 7 commits
  reales. Regla #9 añadida al protocolo: los motores registran hitos ahí.
- Commit y push del sistema `inspiraciones/` (estructura + LEEME + notas) que esperaba
  visto de Angel — otorgado implícitamente al pedir despliegue en Vercel.

**Estado Vercel**
- CLI no instalado → instalando `vercel` vía npm para desplegar desde aquí.

**Pendiente**
- Login/deploy de Vercel (en curso).

---

## 2026-08-21 — OpenCode (videos fuera del repo + estructura libre)

**Cambios**
- Creado `.gitignore` raíz: los videos crudos de `inspiraciones/` (`mp4/mov/mkv/avi/
  m4v/webm`) quedan excluidos de git — viven solo en la PC de Angel. Lo aprobado se
  comprime y pasa a `assets/video/`, que sí se despliega.
- `LEEME.md` actualizado: estructura libre por proyecto (Angel puede crear minicarpetas
  libremente; los motores leen recursivamente) + nueva convención de peso/videos.
- Verificado: OneDrive NO sincroniza `Documents` en esta PC — el respaldo de material
  pesado es manual.

**Pendiente**
- Commit/push de todo lo de hoy (estructura + .gitignore), cuando Angel dé el visto.

## 2026-08-21 — OpenCode (carpeta de inspiraciones)

**Cambios**
- Creada `inspiraciones/` a petición de Angel: cantera de material visual para que los
  motores recorten, editen y jueguen con él antes de pasarlo a `assets/`.
  - `_refs/` (capturas/moodboards), `recursos/{svg,paletas,texturas}`.
  - Una carpeta por proyecto: `cifra/`, `desvariando/`, `reloj/` — cada una con
    `img/`, `video/` y su `notas.md` para anotar qué es cada archivo y qué se decidió.
- Escrito `inspiraciones/LEEME.md`: convenciones de nombres, límites de peso para git,
  originales intocables y flujo subida → prueba → `assets/`.

**Ideas**
- Cuando haya fotos reales de Reloj 181 en la carpeta, probarlas como fondo de cards
  o hero con tratamiento B/N + acento.
- Pendiente confirmar permiso de publicación del material fotográfico (proveedor).

**Pendiente**
- Commit/push de esta estructura (esperando visto de Angel).
- Que Angel empiece a soltar material; primera tarea sugerida: recortes 16:9 para cards.

## 2026-08-21 — OpenCode (primera sesión del relevo)

**Cambios**
- Empujado a GitHub `como-pedirme-cosas.html` (estaba sin confirmar en local).
- Creados `AGENTS.md` y `CLAUDE.md`: protocolo de colaboración entre motores.
- Creada **Versión 2** (`version-2.html`): propuesta nocturna y cinética — Space Grotesk +
  JetBrains Mono, fondo tinta, anillo de cifras giratorio, marquesina, contadores animados,
  reveals al scroll. Mismo copy honesto, misma marca, otra atmósfera.
- Añadido botón «Versión 2 ↗» arriba a la derecha en `index.html`, y «← Versión 1» en la V2.

**Hallazgos analizando la Versión 1 (trabajo de Claude Code)**
- Sistema coherente y bien restringido; jerarquía tipográfica impecable; el modo
  `?static` está bien resuelto.
- Falta **favicon** (la pestaña se ve genérica).
- Faltan metadatos **og:/twitter:** al compartir el link en WhatsApp/redes no hay
  vista previa.
- El contacto es solo `mailto:`; un enlace directo a WhatsApp o formulario simple
  convertiría mejor para negocios locales.
- Captions de 11px pueden quedarse cortas de contraste/tamaño en móvil.

**Ideas dejadas para futuras sesiones (de cualquiera de los dos)**
- Página «comparador» que muestre V1 y V2 lado a lado (iframes) para decidir más fácil.
- Generar una captura del hero como `og:image` con Chrome headless.
- Cuando existan proyectos reales: filtros dinámicos y cards con imagen/video.
- Al desplegar en Vercel: dominio propio y analytics ligero.

**Pendiente**
- Desplegar en Vercel (vercel.com/new → importar repo).
- Decisión de Angel: ¿se queda la V1, la V2, o conviven?
