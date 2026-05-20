---
title: "FORGE-Digital · DISPATCH v4 · paellasymas · 3 fixes Manus post-QA Chrome v3.1"
status: READY-FOR-DISPATCH
dispatch_target: Manus task v4 fixes
created: 2026-05-20 ~5:10 PM AST
authority: Omega Cofundador · orden Soberano-verbatim "manda el dispatch para manu con los arreglos que mencione · está de más que esperes"
predecessor: v3.1 LIVE (`mgriveraarroyo.github.io/paellasymas/` · SHA `f879283` · QA Chrome v3 metabolizado + 6 fixes Code locales aplicados)
---

# FORGE-Digital · DISPATCH v4 · paellasymas · 3 fixes Manus

> Iteración quirúrgica · NO rebuild. v3.1 LIVE en GitHub Pages ya tiene 6 fixes Code locales aplicados (vibra · IG subtítulo honest · heroYT JS muerto eliminado · @algustodejanet clickable). Quedan 3 fixes que requieren tu craft.

---

## §0 · CONTEXTO

- **Sitio LIVE:** `https://mgriveraarroyo.github.io/paellasymas/` · HTTP 200 · SHA `f879283`
- **Tu task v3 previo:** `9RCSbTNUgZnsDRyZMgyf9e` · QA PASS Manus · 5 fixes quirúrgicos entregados
- **Code aplicó 6 fixes locales post-v3** (Code QA local + metabolización QA Chrome v3)
- **3 fixes restantes que NO pude resolver local** (requieren tu craft Manus)
- **30 fotos reales IG @paellasymas en repo:** `https://raw.githubusercontent.com/mgriveraarroyo/paellasymas/main/_source/ig-real/paellasymas-{00..29}.jpg`

---

## §1 · LOS 3 FIXES v4

### FIX V4-1 · CRÍTICO · Sección Canal YouTube COMPLETA patrón Richard

**Estado v3.1 actual (Chrome QA verbatim):**
> "Sección #videos: 1 embed YT solo · sin cards/CTAs Richard. Híbrido declarado no coincide con brief Soberano. No es Richard-style; es 1 video embebido solo."

**Cita Soberano-verbatim 2026-05-20 4:50 PM:**
> *"para el canal de YouTube podemos hacerlo como mismo se lo hicimos en la página de Richard · anuncie el canal y la variedad de videos disponibles y que te lleve directo a verlos si clickeas"*

**Cómo resolver:**

1. **Eliminar el "VER CON SONIDO" modal del hero** si todavía existe (Code v3.1 eliminó el iframe pero el modal puede haber quedado). Hero queda LIMPIO con foto estática (la actual paella mandala está bien) · tagline · sigilo · scroll prompt.

2. **Enriquecer sección #videos con patrón Richard completo:**
   - Label sobrio arriba (ya existe v3.1): `CANAL YOUTUBE · AL GUSTO DE JANET · @algustodejanet`
   - El `@algustodejanet` ya es clickable post-Code v3.1 (link a `https://www.youtube.com/@algustodejanet`)
   - Agregar **1 línea de variedad** debajo del label: `Recetas paso a paso · Procesos en cocina · Shows en vivo · Tips profesionales` (o equivalente · adapta a lo que SÍ haya en el canal real cuando lo fetchees)
   - Mantener **1 video destacado embed** como anchor (`Ec8mXOv4i30` "Paella de Mariscos · El Secreto para una Paella Perfecta")
   - **Agregar 3-4 cards adicionales** debajo del video destacado · cada card = thumbnail del video + título corto + duración + CTA "Ver en YouTube →" (apunta a la URL específica del video)
   - **CTA grande final:** botón "Ver el canal completo en YouTube →" (link a `https://www.youtube.com/@algustodejanet`) · destacado visual (gold accent · más prominente que los CTAs de cards)
   - Si el canal tiene <4 videos · usar los que hay · NO inventar videos que no existen (R26 hard-line)

3. **Pattern referencia Richard validado:** `https://mgriveraarroyo.github.io/richard/` sección Spotify track embed con label + embed + CTA Spotify (estructura paralela)

---

### FIX V4-2 · ALTA · IG grid filter · eliminar 2-3 fotos off-brief

**Estado v3.1 actual (Chrome QA verbatim):**
> "2 de las 30 fotos del self-hosted grid no son paellas ni comida: una foto de performer/hazmat nocturno (fila 1, col 3 visual) y una foto de personas grupo. 1 de las 30 fotos es un flyer publicitario azul con texto '¿TE GUSTARÍA DISFRUTAR COMIDA DE RESTAURANTE todos los días... SIN SALIR DE TU CASA!' + phone 939-717-2096. La subtítulo 'Cada momento que servimos · capturado al vuelo' no excluye estas imágenes."

**Cómo resolver:**

1. Evalúa las 30 fotos en `_source/ig-real/paellasymas-{00..29}.jpg`
2. Identifica 2-4 fotos que NO son paellas/cocina/eventos de Chef Janet:
   - Performer/hazmat nocturno (Chrome identified · fila 1 col 3)
   - Personas grupo sin contexto culinario
   - Flyers publicitarios con texto overlay (especialmente el azul "¿TE GUSTARÍA..." de entrenamiento doméstico)
   - Cualquier otra foto que rompa coherencia editorial culinaria
3. Filtra esas fotos del grid `#instagram` · mantén las ~26-28 que SÍ son coherentes (paellas · proceso cocina · servicio · mariscos macros · Chef Janet en acción)
4. Documenta en el README cuáles excluiste y la razón
5. Si el grid queda con número impar que rompe layout 5 columnas · ajusta columnas a 4 o usa masonry irregular (no inventar fotos para llenar)

---

### FIX V4-3 · ALTA · Foto about Chef Janet · solución honest

**Estado v3.1 actual (Chrome QA verbatim):**
> "OK-con-gap-conocido. La imagen en #detras-del-fuego muestra a Chef Janet en uniforme verde lima sosteniendo la paella mandala — pero hay un hombre en blazer negro junto a ella (foto de dos personas, no retrato editorial solo). Manus reconoció el honest gap. La alternativa disponible es mejor que el flyer de v2, pero sigue siendo IG-marketing contextual."

**Cómo resolver (escoge la opción que mejor ejecutes con craft):**

**Opción A · Crop editorial:**
- Toma la foto actual (`paellasymas-19` Chef Janet + invitado · uniforme verde lima · paella mandala)
- Hace crop editorial: solo Chef Janet · NO el invitado · enfoca el uniforme + paella mandala como elemento visual
- CSS `object-fit: cover` + `object-position` específico para centrar Chef Janet sola en el crop
- Mantén la foto a alta resolución para que el crop no pierda calidad

**Opción B · Composición editorial con detalle:**
- Layout split: lado izquierdo retrato Chef Janet (crop solo de ella) · lado derecho la quote signature "El fuego es el primer ingrediente. Y el más difícil de dominar." en tipografía editorial grande
- La quote dominante visualmente · la foto secundaria · ambos cuentan la historia

**Opción C · Sin foto · solo quote:**
- Si el crop de A o el split de B no se ejecutan limpio · sustituye la foto por una composición tipográfica:
  - Quote grande dominante: `"El fuego es el primer ingrediente. Y el más difícil de dominar." — Chef Janet`
  - Sigilo SVG decorativo
  - 0 foto = 0 problema
- Sección "Detrás del Fuego" se vuelve más editorial puro tipográfico

**Tu decisión:** evalúa A · B · C · escoge la que mejor ejecute. Documenta cuál y por qué.

---

## §2 · RESTRICCIONES (heredadas · NO romper)

- **0 frases vibra Soberano/Omega** como copy literal (regla canon)
- Voz Chef Janet preservada: "Esto no es solo una paella" · "Aquí no solo cocinamos" · "El fuego es el primer ingrediente" · "Compro con los ojos · con la nariz · con las manos"
- INV-1 (0 IA visible) · INV-9 (sigilo SVG · 0 emoji crudo) · todos los INV heredados
- Mailto: fallback en form (heredado) · placeholders transitional `riveramichael9006@gmail.com` (heredado · Chef Janet swap post-validación)
- 30 fotos REALES IG (NO uses screenshots ni stock photos · NO descargues nuevas · solo las 30 del repo)
- "Recorre el sabor" invención FORGE Fix 5 v3 · MANTENER funcionando (cursor especial + aroma tags hover)
- Sección IG self-hosted (Opción B Angel-style) · MANTENER (NO volver a iframes)

---

## §3 · ENTREGABLE v4

ZIP nuevo `paellasymas-v4-FORGE.zip` con:
- `index.html` con los 3 fixes aplicados (puede que crezca o se reduzca por filter IG)
- `assets/` heredados (sigilo.svg · og-image.jpg)
- `sitemap.xml` + `robots.txt` heredados
- `README_FORGE_DEPLOY_v4.md` con:
  - Fix V4-1: cuántos videos del canal usaste · qué CTAs · qué variedad listaste
  - Fix V4-2: cuántas fotos excluiste · cuáles (por index) · razón de cada exclusión
  - Fix V4-3: opción A/B/C elegida · por qué
  - QA self-report honest

---

## §4 · NOTAS

1. **NO regresiones:** verifica que tu v4 NO reintroduzca las frases vibra que Code limpió en rondas previas (lista §2)
2. **Pages YA activado:** v4 push hace re-deploy automático en 1-2 min
3. **Doctrina canon Soberano 2026-05-20:** "no se hace nada sin un QA antes · NO importa cuántas versiones · TODAS se realizan QA" — después de tu v4 entrega · Code ejecuta QA local + Soberano ejecuta QA Chrome antes de envío real a Chef Janet
4. **Target:** v4 = entrega final pre-feedback Chef Janet. Si los 3 fixes resuelven limpio · Soberano envía mensaje validación.

---

*FORGE-Digital DISPATCH v4 · Omega FORGE Ω orquesta · Manus craft quirúrgico · 3 fixes consolidados post-QA Chrome v3 · target v4-final-pre-Chef-Janet · barco firme.*
