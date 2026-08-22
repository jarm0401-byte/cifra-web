# AGENTS.md — Protocolo de colaboración en cifra-web

Este repositorio lo trabajan **dos motores de IA en conjunto**, en beneficio de una sola
persona: **José Ángel ("Angel") Resendiz Martinez**, dueño de **CIFRA**, estudio digital
en Cuernavaca, Morelos.

- **Claude Code** (Anthropic) → mantiene la **Versión 1**: `index.html`
- **OpenCode** (ox-alpha) → mantiene la **Versión 2**: `version-2.html`

Cuando a uno se le acaban los tokens o el contexto, Angel viene con el otro y el trabajo
**continúa donde quedó**. Ninguno borra ni rompe el trabajo del otro: se nutren mutuamente.

## Reglas de convivencia (obligatorias)

1. **Leer antes de tocar:** revisa `BITACORA.md` (entradas nuevas arriba) y el historial
   reciente (`git log --oneline -15`) para enterarte de qué cambió y qué se acordó.
2. **Escribir después de trabajar:** agrega una entrada en `BITACORA.md` con fecha y motor:
   qué cambiaste, qué encontraste (bugs, mejoras, ideas), qué queda pendiente.
3. **No destruir la versión hermana.** Los cambios estructurales de la otra versión solo si
   Angel lo pide explícitamente, dejando nota en la bitácora.
4. **Elementos compartidos** (botones de cambio de versión, datos de contacto, metadatos
   comunes): mantenerlos sincronizados en ambas páginas.
5. **Copy honesto, en español:** nada que Angel no pueda sostener cara a cara. Él es
   matemático; NO es fotógrafo ni cineasta (eso es de su novia). Si no hay copy real,
   marcador sobrio y claramente provisional — nunca promesas inventadas.
6. **Mucho movimiento,** acorde a cada sistema de diseño (reveals al scroll, entradas
   escalonadas, marquesinas, hovers con intención), respetando siempre
   `prefers-reduced-motion` y conservando el modo `?static` para capturas headless.
7. **Verificación visual obligatoria antes de dar algo por terminado**
   ("si no se ve, no acabaste"): capturas con Chrome headless, leer el PNG, comparar,
   iterar hasta que esté bien.
8. **Git:** commits descriptivos en español, push después de cada hito. Nunca force-push.
9. **Memoria privada:** todo cambio importante se registra también en `memoria.html`
   (agregando una entrada al final del arreglo `MEMORIAS`: fecha, motor, título, detalle,
   hash del commit). Ese archivo es LOCAL y PRIVADO de Angel: está en `.gitignore` y
   **jamás se sube** al repo ni al deploy.

## Sistema de doble versión

| | Versión 1 (`index.html`) | Versión 2 (`version-2.html`) |
|---|---|---|
| Autor | Claude Code | OpenCode |
| Atmósfera | Editorial clara (papel) | Nocturna cinética (tinta) |
| Tipografía | Inter monumental | Space Grotesk + JetBrains Mono |
| Acento | Esfera gota de agua iridiscente | Anillo de cifras giratorio + gradiente |
| Referencia | OFF+BRAND (refero.design) | Misma marca, otra lectura |

Cada versión enlaza a la otra arriba a la derecha. **Angel decide al final cuál se queda**
(o cómo conviven); mientras tanto, ambas viven en el mismo sitio.

## Datos técnicos

- Repo: `github.com/jarm0401-byte/cifra-web` (rama `main`)
- Un solo archivo autocontenido por versión (CSS/JS inline), sin build step
- Fuentes vía Google Fonts; identidad global de git ya configurada
- Despliegue previsto: Vercel (importar repo; cada push a main despliega)

---
*Última actualización: 2026-08-21 · OpenCode*
