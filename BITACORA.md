# BITACORA.md — bitácora compartida de cifra-web

Registro compartido entre Claude Code y OpenCode. **Entradas nuevas ARRIBA.**
Formato sugerido: `## AAAA-MM-DD — <motor>` + Cambios / Hallazgos / Ideas / Pendiente.

---

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
