---
title: "FORGE-Digital · DISPATCH v3 · Chef Janet @paellasymas · 5 fixes quirúrgicos post-QA Chrome v2 LIVE"
status: READY-FOR-DISPATCH
dispatch_target: Manus task v3 fixes
created: 2026-05-20 ~4:35 PM AST
authority: Omega Cofundador · cita Soberano-verbatim 2026-05-20 4:30 PM AST
predecessor: v2.1 LIVE (mgriveraarroyo.github.io/paellasymas/ HTTP 200) · QA Chrome cruzado · 4 issues + 1 doctrina identified
---

# FORGE-Digital · DISPATCH v3 · 5 FIXES QUIRÚRGICOS · paellasymas

> Es iteración quirúrgica · NO rebuild. v2.1 ya está LIVE en GitHub Pages y el Soberano validó "buena base · son detalles · vamos por buen camino · en menos versiones · de eso se trata".

---

## §0 · CONTEXTO

- **Sitio LIVE:** `https://mgriveraarroyo.github.io/paellasymas/` · HTTP 200 · build SHA `ce0f2ff`
- **Tu task v2 previo:** `RYCE7aux2fP4LMCDPasTt7` · QA PASS interno · entregaste el ZIP base
- **Code aplicó 7 fixes locales post-v2** (eliminación de frases vibra Soberano/Omega usadas como copy literal · sustituidas por voz real Chef Janet)
- **Soberano + Chrome QA LIVE detectaron 4 issues residuales + 1 doctrina** que requieren tu craft (NO se pueden resolver con sed local)
- **30 fotos reales IG @paellasymas** ya en repo: `https://github.com/mgriveraarroyo/paellasymas/tree/main/_source/ig-real/paellasymas-{00..29}.jpg`

---

## §1 · LOS 5 FIXES (en orden de severidad)

### FIX 1 · CRÍTICO · Bug foto stock en galería tab "EL PROCESO" item #3

**Detección Chrome QA LIVE verbatim:**
> "La imagen con alt 'Paella de mariscos · proceso de cocción' (~149KB base64) renderiza una foto stock de dos personas (hombre con barba larga oscura + mujer, fondo de hiedra con luces string). No es una foto del feed de @paellasymas. No tiene relación con paella, cocina, ni Chef Janet."

**Cómo resolver:**
- Buscar en `index.html` la imagen con alt exacto `"Paella de mariscos · proceso de cocción"` o equivalente en tab "EL PROCESO" item #3
- Reemplazar el `data:image/jpeg;base64,...` por una foto real del proceso de cocción de paellasymas (paella sobre fuego · mariscos siendo añadidos · vapor saliendo)
- Candidatas en `_source/ig-real/`: revisa las 30 fotos · escoge la que mejor capture "proceso de cocción" (paella en sartén con mariscos · NO el resultado final · proceso mid-cooking)

---

### FIX 2 · ALTA · Foto Chef Janet en "Detrás del Fuego" es flyer publicitario

**Detección Chrome QA LIVE verbatim:**
> "La imagen en sección 'Detrás del Fuego' (ref_254, alt: 'Chef Janet · retrato profesional · Paellas y Más · chef en uniforme blanco') es visualmente una pieza de marketing de Instagram con texto overlay de oferta de entrenamiento doméstico ('¿TE GUSTARÍA DISFRUTAR COMIDA DE RESTAURANTE...'). No es un retrato editorial limpio. El alt dice 'retrato profesional' pero la imagen es un flyer."

**Cómo resolver:**
- Revisa las 30 fotos en `_source/ig-real/paellasymas-{00..29}.jpg`
- Identifica una donde aparezca Chef Janet sola (uniforme verde lima visible · sin texto/overlay/flyer)
- Reemplaza el `data:image/jpeg;base64,...` actual del about por la foto limpia de Chef Janet
- Si NINGUNA de las 30 fotos descargadas es retrato limpio (porque el feed IG de catering tiende a tener flyers · no retratos), entonces:
  - Usar una foto del feed donde Chef Janet aparezca cocinando una paella (uniforme + acción + sin texto overlay)
  - O dejar la sección sin foto y enfatizar la quote firmada como signature visual

---

### FIX 3 · ALTA · Audio → Video cinematográfico (toque doctrina Soberano)

**Cita Soberano-verbatim 2026-05-20 4:30 PM:**
> *"una vez empiezas el audio no tienes forma de darle para atrás · en vez de un audio simple prefiero el video original e incorporarlo cinematográficamente en la página sin que le quite a la experiencia · idea buena ejecución falta más unificación al concepto e invención genuina marcada por FORGE"*

**Estado v2.1 actual:**
- iframe[0] YouTube Ec8mXOv4i30 en `#heroYT` · botón "🔇 Silenciar" toggle on-demand
- Problema: una vez activado el sonido NO hay forma intuitiva de volver atrás · es solo un toggle audio sobre el video que ya está corriendo · NO es experiencia cinematográfica

**Cómo resolver:**
- Eliminar el botón "🔇 Silenciar" aislado (concept audio-only)
- Integrar el video real YouTube (`Ec8mXOv4i30` "Paella de Mariscos · Al Gusto de Janet") como **hero background video cinematográfico**:
  - Autoplay · muted · loop · sin controles visibles
  - Overlay editorial sobre el video (texto hero + sigilo flotante)
  - Pueden agregar un play button sutil en esquina inferior para "ver con sonido" pero NO botón mute toggle aislado
  - Si el viewer hace click en el video → abre full-screen modal con sonido · cuando cierra modal vuelve al loop silent en background
  - Patrón referencia: sitios de chefs 3 estrellas tipo Noma · Mugaritz · Disfrutar (hero video silent · cinematográfico · click para experiencia full con sonido)
- El video YouTube original es de la chef cocinando real · queda más cinematográfico que un loop CSS de vapor sobre una foto estática
- Aplicar `pointer-events: none` al iframe en background mode para que el scroll funcione sobre el video sin interferencia
- Mobile (`pointer:coarse`): fallback a hero foto estática (autoplay video en mobile drena batería · respeto)

---

### FIX 4 · ALTA · Instagram unificada (patrón Angel salón)

**Cita Soberano-verbatim 2026-05-20 4:30 PM:**
> *"la area de instagram se siente repetida creo que podemos unificarlos reel y el acceso live y sincronización como tenemos en el de angel · pienso que se vería mejor todo unificado · no múltiples pantallas de lo mismo · busca la referencia que te mencione de lo que hicimos con la página de angel salón"*

**Detección Chrome QA + screenshot Soberano:**
- v2.1 actual tiene **3 iframes IG separados** en sección `#videos`:
  - iframe[2] IG Reel "Esto no es solo una Paella · Chef Janet"
  - iframe[3] IG Reel "Aquí no solo cocinamos · Paella en vivo"
  - iframe[4] IG feed `@paellasymas`
- Screenshot Soberano muestra: feed grid + reel embed broken ("link broken or removed") + perfil card · todo como 3 cajas separadas en la misma sección · **redundante visual**

**Referencia Angel salón (a replicar):**
- URL: `https://mgriveraarroyo.github.io/strandsandroses/`
- Sección `#gallery-ig` con clase `ig-feed`
- **UNA SOLA sección IG unificada:** Elfsight Instagram Feed widget (free tier · auto-updates · ALL posts en 1 grid responsive)
- 2 CTAs: "View on Instagram →" + "Follow @strandsandroses"
- Loading state mientras widget carga
- 0 iframes IG individuales · 0 fragmentación

**Cómo resolver para paellasymas:**
- Eliminar los 3 iframes IG separados del v2.1
- Implementar UNA sola sección unificada "Síguenos en Instagram"
- **2 opciones viables (escoge la que se ejecute mejor):**
  - **Opción A (Elfsight pattern Angel):** widget Elfsight Instagram Feed con placeholder ID · README documenta cómo Chef Janet (o Code post-validación) crea cuenta gratis en elfsight.com y reemplaza el widget ID
  - **Opción B (self-hosted grid pattern):** usar las 30 fotos reales del repo `_source/ig-real/` como grid masonry/responsive directamente · 0 dependencia externa · 0 iframes que pueden romperse · más rápido · más confiable · pero NO se actualiza solo
  - **Mi recomendación criterio R47 (IA local primero · 0 dependencia cloud):** Opción B · grid puro con las 30 fotos reales que YA tenemos
- 1 CTA único "Síguenos en @paellasymas" → `https://www.instagram.com/paellasymas/`
- Los 2 IG Reels embebidos previos (que se rompen) → mover a sección Videos como thumbnails con link directo al reel (1 click se abre en IG) · NO embed iframe que falla

---

### FIX 5 · DOCTRINA · "Toque FORGE · invención genuina marcada"

**Cita Soberano-verbatim 2026-05-20 4:30 PM:**
> *"falta el toque FORGE pero buen trabajo"*
>
> *"la ejecución le falta un poco más de unificación al concepto e invención genuina marcada por FORGE"*

**Interpretación operacional:**
- El sitio tiene craft (paleta · tipografía · motion · narrativa) pero le falta UNA cosa que sea **invención genuina FORGE** · algo que NO existe en otro catering site del mercado
- NO basta sigilo SVG navegación (eso es marca · no invención mecánica)
- NO basta vapor animado + sparkles + cursor (eso es craft · existe en otros sitios premium)
- **Buscamos:** una mecánica de interacción · una sección · un easter egg sutil · una métrica viva · ALGO que cuando Chef Janet (o cualquier visitante) lo descubra diga "esto NO existía en ninguna parte"

**Candidatos a explorar (propón 2-3 · Soberano elige):**
1. **"Cocción en vivo"** — pequeño contador en hero o en footer que muestra tiempo desde la última paella servida (live "Servidas hoy: 3" · "Última cocción: hace 2h" · usando localStorage o counter con timestamp incremental). Invención: catering site con métrica de "vida" en vivo.
2. **"Recorre el sabor"** — cursor especial que al hover sobre cada paella revela 1 nota aromática editorial (ej: hover sobre paella mariscos · aparece glow + texto efímero "azafrán · paprika ahumada · mariscos del día"). Invención: storytelling sensorial granular vs descripciones largas.
3. **"El fuego activo"** — pequeño SVG animado del fuego en navegación que se intensifica cuando el viewer scroll a la sección "El Proceso · capítulo 2 (El Fuego)" · vuelve a tenue cuando sale. Invención: navegación que responde al contenido leído.
4. **"Construye tu paella"** — mini-interacción donde el viewer puede armar una paella en hover (paellera vacía → añade arroz → añade mariscos → completa · cada paso revela 1 línea de Chef Janet sobre ese ingrediente). Invención: experiencia kinestésica antes del CTA.

**Cualquiera de los 4 es suficiente · el Soberano valida el ganador post-implementación.**

---

## §2 · RESTRICCIONES (heredadas de v2 · NO cambiar)

- **0 frases vibra Soberano/Omega como copy literal** (regla canon · "el COMO es nuestro · la VOZ es del cliente")
- Voz Chef Janet preservada: "Esto no es solo una paella" · "Aquí no solo cocinamos" · "El fuego es el primer ingrediente" · "Compro con los ojos, con la nariz, con las manos"
- Doctrina raíz: invocación multi-sensorial (vista · oído · olfato sugerido · tacto/motion · gusto evocado · narrativa)
- INV-1 (0 IA visible · 0 mención Manus/Code/FORGE OS interno) · INV-9 (sigilo SVG · 0 emoji crudo) · todos los INV heredados
- Mailto: fallback en form (heredado) · placeholders transitional `riveramichael9006@gmail.com` (heredado · Chef Janet swap post-validación)

---

## §3 · ENTREGABLE v3

ZIP nuevo `paellasymas-v3-FORGE.zip` con:
- `index.html` con los 5 fixes aplicados (puede crecer si añades más video integration)
- `assets/og-image.jpg` (heredado)
- `assets/sigilo.svg` (heredado)
- `sitemap.xml` + `robots.txt` (heredados)
- `README_FORGE_DEPLOY_v3.md` con:
  - Cada fix · cómo lo resolviste · qué decisión tomaste si tenías 2 opciones
  - Para Fix 5 (toque FORGE) · cuál de los 4 candidatos implementaste y por qué
  - QA self-report honest (lo que probaste vs lo que asumiste)
  - Honest gap final (qué te falta para juzgar mejor)

---

## §4 · NOTAS FINALES

1. **Doctrina Soberano validada hoy:** *"en menos versiones · de eso se trata · vamos por buen camino"* — apunta a v3 como entrega final pre-feedback Chef Janet. Si v3 cubre los 5 fixes con craft · Soberano envía a Chef Janet · feedback real define v4 si aplica.
2. **No introduzcas regresiones:** Code aplicó 7 fixes locales post-v2 eliminando 8 ocurrencias de frases vibra. Verifica que tu v3 NO reintroduzca esas frases en otros lugares por descuido.
3. **Las 30 fotos del repo `_source/ig-real/`** son tu única fuente de imágenes nuevas (no descargues otras · respeto al feed real de Chef Janet).
4. **Pages YA está activado:** el sitio LIVE existe · v3 push hace re-deploy automático en 1-2 min.

---

*FORGE-Digital DISPATCH v3 · Omega FORGE Ω orquesta · Manus craft quirúrgico · 5 fixes consolidados · target v3-final-pre-feedback-Chef-Janet · barco firme.*
