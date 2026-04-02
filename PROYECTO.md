# La Morada del Nuevo Tango — Resumen del Proyecto

## Sitio web
- **URL:** lamoradadeltango.com.ar
- **Repositorio:** github.com/LucianoSur/LaMorada-Web
- **Archivo local:** `D:\LaMorada-Web\index.html`
- **Hosting:** GitHub Pages
- **DNS:** Cloudflare → NIC.ar

---

## Stack técnico
- HTML/CSS/JS estático (un solo archivo `index.html`)
- YouTube Data API v3 con caché de 24hs en localStorage
- GitHub Pages para deploy automático
- Cloudflare como intermediario DNS

## Estética
NEON ARRABAL 2077 — dark, cyberpunk arrabalero
- Fondo: `#080810`
- Magenta: `#e500a4`
- Cyan: `#00e5ff`
- Tipografías: Bebas Neue + Barlow Condensed + Orbitron
- Efectos: scanlines, glitch en hero

---

## Estructura del sitio (orden actual)

| # | Sección | Descripción |
|---|---------|-------------|
| 001 | El Programa | Descripción + badges YouTube/Twitch/Kick |
| 002 | Videos | Thumbnails clickeables — últimos 6 del canal |
| 003 | Equipo | 8 integrantes con foto + link a IG |
| 004 | Columnas | 3 columnas con player + thumbnails vía API |
| 005 | Redes | YouTube, Twitch, Kick, Instagram, TikTok |
| 006 | Premios Tango Siglo XXI | Media Partner — video cobertura + Spotify sin bordes |
| 007 | Contacto | QR Linktree + teléfono + email |
| 008 | Amigos | Revista El Sordo, Fractura Expuesta, Doble A Radio, Radio CAFF |

> La numeración es pública y consecutiva, con un salto intencional (008) para reservar espacio a futuras secciones.

---

## Canal YouTube
- **Handle:** @LaMoradatango
- **Channel ID:** `UCNJ084cWrTV7hqJFTsRsOWQ`
- **API Key:** guardada localmente (no subir a GitHub)
- **Cuota:** 10.000 unidades/día — se renueva a las 21hs Argentina

## Plataformas
| Plataforma | URL |
|------------|-----|
| YouTube | youtube.com/@LaMoradatango |
| Twitch | twitch.tv/lamoradanuevotango |
| Kick | kick.com/lamoradadeltango |
| Instagram | instagram.com/lamoradatango |
| TikTok | tiktok.com/@lamoradadeltango |
| Linktree | linktr.ee/lamoradadeltango |

---

## Equipo

| Nombre | Rol | Instagram |
|--------|-----|-----------|
| Lucho Porcelli | Conductor | @luciano.sur |
| Teo Ballesi | Co conductor + Contrabajo x Contrabajo | @contrabajotango |
| Irina González | Todo Tango es Político | @irinachinna |
| Lola Rosa | Sentimiento Guitarrero | @lolarosa.tango |
| Marcela Vigide | Violín Criollo | @marcelavigide |
| Nehuen Martino | ¿Esto es Tango? | @nehuenmartino |
| Pablo Sensottera | Historia Viva | @pablosensottera |
| Chevy | Asistente Administrativo | link a YouTube |

---

## Columnas

| Columna | Conductor | Playlist ID |
|---------|-----------|-------------|
| Contrabajo x Contrabajo | Teo Ballesi | `PL1RnVj-h7YAugGMUIWeCCidEAmplt7ipy` |
| ¿Esto es Tango? | Nehuen Martino | `PL1RnVj-h7YAvYpQl-cS5ClXPkANhLbyfL` |
| Tangos de Cosecha Propia | La Morada | `PL1RnVj-h7YAvhYYmlDGcTve3ums8I28Vi` |

> **Pendiente:** agregar columnas Historia Viva (Pablo Sensottera) y Sentimiento Guitarrero (Lola Rosa) cuando tengan playlists.

---

## Premios Tango Siglo XXI
- **Sitio oficial:** premiostangosiglo21.com.ar
- **La Morada es Media Partner oficial**
- **Video cobertura:** youtube.com/watch?v=Vp2hFDoxLpI
- **Spotify playlist nominados:** `0QnH0GrTPUru6ceBMUKSYv`
- **Estilo:** el embed de Spotify se muestra sin bordes adicionales para integrarse mejor con el diseño.

---

## Amigos de La Morada
| Nombre | URL |
|--------|-----|
| Revista El Sordo | revistaelsordo.com |
| Fractura Expuesta | fracturaexpuesta.com.ar/gotan |
| Doble A Radio | fracturaexpuesta.com.ar/doblearadio |
| Radio CAFF | radiocaff.com.ar |

> **Pendiente:** conseguir URLs de stream de Radio CAFF y Doble A para agregar reproductores.

---

## Contacto del conductor
- **Tel:** +54 15 2409-2854
- **Email:** lucianosur@gmail.com

---

## Flujo de trabajo
1. Editar `D:\LaMorada-Web\index.html` en VS Code
2. **IMPORTANTE:** la API key va hardcodeada en el archivo pero NO se sube a GitHub — antes de cada commit reemplazarla por `TU_API_KEY_AQUI` y después de pushear volver a ponerla
3. Commit en Source Control con mensaje descriptivo
4. Sync Changes para subir a GitHub
5. El sitio se actualiza automáticamente en ~1 minuto

---

## Cambios recientes (20/03/2026)
- Reordenamiento de numeración de secciones (consecutivas del 001 al 008).
- Corrección del menú hamburguesa en mobile: overlay a pantalla completa, cierre correcto.
- Ajustes de responsive: textos, grillas, tamaños de fuente y espaciado.
- Mejora en el embed de Spotify (sin bordes ni caja extra).
- Manejo de errores en columnas (muestra mensaje si falla la API).

---

## Pendientes
- [ ] Verificar que videos de columnas aparezcan en producción
- [ ] URLs de stream Radio CAFF y Doble A Radio
- [ ] Playlist columna Historia Viva (Pablo Sensottera)
- [ ] Playlist columna Sentimiento Guitarrero (Lola Rosa)
- [ ] Resolver problema de API key expuesta en GitHub (considerar solución alternativa)