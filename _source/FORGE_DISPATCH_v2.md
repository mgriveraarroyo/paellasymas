---
title: "FORGE-Digital · DISPATCH v2 · Chef Janet @paellasymas · EXPERIENCIA INMERSIVA MULTI-SENSORIAL"
status: READY-FOR-DISPATCH
dispatch_target: Manus task v2 build
created: 2026-05-20 ~3:30 PM AST
authority: Omega Cofundador · doctrina raíz Soberano-verbatim 2026-05-20
client: Chef Janet · paellasymas · Tier 2 ($3,500-$5,500)
predecessor: FORGE_DISPATCH_v1.md (Manus task YNtejiXeWsG94gAYvsoCjF · QA PASS interno · NO superó estándar premium FORGE) + 4 hallazgos Soberano + intake IG real Code
---

# FORGE-Digital · DISPATCH v2 · Chef Janet @paellasymas

> **EXPERIENCIA INMERSIVA MULTI-SENSORIAL · NO una página más**

---

## §0 · DOCTRINA RAÍZ V2 (Soberano-verbatim 2026-05-20)

> *"estamos trabajando con una industria que su consumo es basado y tiene gran peso en su éxito la experiencia de los sentidos · cómo huele · cómo se ve · cómo se siente cuando me lo sirvieron · para premiar todo ese flujo gastronómico y experiencia inmersiva en cómo sabe · debemos transmitir eso busca la manera no creemos cualquier página creemos la experiencia"*

**Traducción operacional:** la industria gastronómica es **multi-sensorial**. El sitio digital debe invocar los 4 sentidos accesibles (vista · oído · tacto/movimiento · olfato sugerido) y memoria-de-sabor (gusto irreducible pero evocable vía storytelling/testimonio). El v1 falló porque construyó una página · NO una experiencia.

---

## §0bis · ENRIQUECIMIENTO POÉTICO SOBERANO 2026-05-20 ~3:35 PM AST (obligatorio · craft v2)

Cita Soberano verbatim adicional sobre la experiencia inmersiva:

> *"añádele destellos de colores · recuerda que es arte culinaria · desciende del arte · frescura · calidad · sabor · vapor de señal que está listo · caliente y al pie de tu deleite"*

**5 elementos canon que el sitio v2 DEBE encarnar:**

1. **Destellos de colores** — visual sparkles/shimmer/glow accents en momentos clave (cursor hover paellas · transición de capítulos · al cargar imagen macro de mariscos · al revelar precio). NO confeti de plataforma · sí destellos editoriales culinarios (color flare dorado azafrán + rojo paprika · 0.4-0.8s · sutil · una vez). Inspiración: chispa de aceite cayendo en sartén caliente · brillo de azafrán mojado.

2. **Arte culinaria desciende del arte** — positioning editorial: el sitio se siente más cerca de una galería de arte gastronómico que de catering corporativo. Espacio en blanco editorial · imagen como protagonista · texto que respeta la imagen · NO densidad comercial. Referencia mental: Noma journal · Mugaritz book · libros de cocina autoral de chefs 3-estrellas.

3. **Frescura · calidad · sabor** — 3 palabras clave que deben aparecer COMO ANCLAS visuales/textuales en el sitio · NO listadas juntas en lista de bullets · sí incrustadas en copy editorial:
   - *Frescura*: hablar del mariscos del día · "mariscos seleccionados esa misma mañana" · ingrediente vivo
   - *Calidad*: hablar del estándar Chef Janet · "20 años eligiendo el azafrán correcto" · curaduría
   - *Sabor*: hablar de memoria · "el sabor que cierra el evento" · "lo que se queda con la gente"

4. **Vapor como señal de listo** — motion específico del sitio: el VAPOR animado (CSS · SVG · canvas) sobre fotos de paella saliendo del fuego es la SEÑAL de "está listo · caliente · servido ahora". Aplicar:
   - Hero image/video: vapor sutil animado subiendo (loop infinito · opacidad 0.3-0.6)
   - Cards Servicios: en hover · el vapor se intensifica
   - Galería capítulo "El Servicio": vapor más denso · sugiere que se acaba de servir
   - Sección precios: pequeño vapor animado al lado del precio destacado (ancla visual)

5. **"Caliente y al pie de tu deleite"** — frase ancla para el sitio. Candidatos de uso:
   - Tagline hero alternativo (junto con "Esto no es solo una Paella")
   - Cierre de sección "El Servicio" en El Proceso
   - Subheader de la sección Cotizar ("Caliente · al pie de tu deleite · listo cuando llegamos")
   - Microfooter ético del Newsletter

---

## §1 · 4 HALLAZGOS SOBERANO v1 (must-fix obligatorio v2)

| H | Hallazgo verbatim | Causa raíz | Fix v2 obligatorio |
|---|---|---|---|
| H1 | "Se ve genérica para el nivel estándar que tenemos" | Manus optimizó para QA PASS interno 17 criterios · NO para estándar premium FORGE | Aplicar 8 movimientos diferenciadores premium canon FORGE (§5 abajo) |
| H2 | "Tiene un canal de YouTube · no veo rastros · feed en vivo" | v1 ignoró ecosystem cliente · solo IG estático embebido | Integrar YouTube `@algustodejanet` (196 subs) · 2 reels destacados IG (319+32 likes) · iframes embed directos |
| H3 | "No puedo ver los videos" | Servicio core "Live Paella Show Cooking" · 0 video element en v1 · fallo absoluto del prometido | Hero video bg muteado autoplay loop · sección Video Gallery · IG reel embeds en Servicios cards |
| H4 | "Las fotos que usaste son screenshots" | Manus NO tenía acceso autenticado al feed real · usó screenshots base64 low-res | 30 fotos REALES IG @paellasymas descargadas full-res via forge-browser autenticado · path `inputs/assets-real-2026-05-20/ig-paellasymas/` · todas con alt text auténtico Chef Janet como copy seed |

---

## §2 · ASSETS REALES DISPONIBLES (NUEVOS · v2 inputs)

### A. Fotos IG @paellasymas — 30 archivos · 4.6 MB · descargados R26 verified
Path: `inputs/assets-real-2026-05-20/ig-paellasymas/paellasymas-{0..29}.jpg`

Cada foto tiene **alt text auténtico Chef Janet** capturado por forge-browser. Ejemplos de voice real:
- *"Lleva la cocina de tu hogar al nivel de un restaurante 🍽️ En Paellas y Más capacitamos tu..."* (entrenamiento doméstica)
- *"Entre montañas, aire fresco y buena compañía... una paella hecha en vivo sabe diferente 🥘✨"* (outdoor catering)
- *"En Croquetas Boutique by Paellas y Más, cada croqueta es hecha artesanalmente, con ingredientes..."* (servicio secundario)

**Instrucción Manus:** Usar estos alts como COPY EDITORIAL del sitio · NO copy genérico. La voz de Chef Janet ya está aquí.

### B. URLs YouTube + IG embed (Manus embeba iframes directos · NO descargar)
- **Canal YouTube:** https://www.youtube.com/@algustodejanet (196 subs · 1 video pinned destacado)
- **IG reel destacado #1** (319 likes · pinned May 3 · "Esto no es solo una Paella"): https://www.instagram.com/p/DX9diIWp-4t/ (validar URL exacta · usar IG embed API)
- **IG reel destacado #2** (32 likes · May 5 · "Aquí no solo cocinamos / Paella en vivo"): URL específica en intake `inputs/intake-2026-05-19-chrome-sonnet46.md`
- **Bio IG completa:** ya en intake (servicios · teléfonos PR + RD · YouTube link · FB link)

### C. Frase signature destacada para uso editorial
**"Esto no es solo una Paella"** — reel pinned 319 likes · ÚSALA como hero headline alternativo o tagline editorial mayor · esta frase ya validada por engagement real cliente.

---

## §3 · 6 VECTORES EXPERIENCIA INMERSIVA MULTI-SENSORIAL (canon nuevo)

### V1 · VISTA · craft visual premium
- **Hero video bg** (autoplay · muted · loop · sin controles · iframe YouTube reel destacado embed full-screen)
- **Galería editorial curada · NO grid IG** · storytelling: "El proceso · La paella · El servicio · La gente · El sabor" en 5 capítulos visuales
- **Macros close-up** (texturas: granos arroz suelto · vapor · mariscos chillando · corteza socarrat dorada)
- **Paleta defensible:** dorado azafrán (#D4A437) + rojo paprika (#B83A2E) + verde olivar (#5D7044) + brown crusta (#8B4513) + negro carbón (#1A1A1A) · 5 colores con jerarquía editorial · NO 7 colores planos
- **Tipografía editorial:** Serif elegante (Cormorant Garamond · Playfair Display) para nombres de platos + titulares · Sans tight (Inter · Söhne) para precios + body · contraste editorial

### V2 · OÍDO/SONIDO · ambient sutil (opcional UX)
- **Hero video CON option unmute** · loop · default mute · botón sutil "🔊 escucha la paella" (sizzle real del aceite · NO música stock)
- **NO añadir audio invasivo** · solo invocar disponibilidad · respeto del usuario

### V3 · OLFATO · sugerido via lenguaje editorial
- **Descripciones de platos sensory:** NO "Paella Campesina · $185" · SÍ "Paella Campesina · el sofrito mojando la cebolla · el pollo de campo dorándose · arroz absorbiendo el caldo · $185"
- **Copy editorial con notas aromáticas** · azafrán abriendo · paprika ahumándose · corteza socarrat caramelizándose
- **Inspiración:** menu editorial de un restaurante 3 estrellas · NO catálogo de delivery

### V4 · TACTO/MOVIMIENTO · interacción con peso
- **Scroll-driven reveal:** cada paella aparece como si se estuviera sirviendo (motion subtle · fade-up + slight scale)
- **Hover states con peso:** lift + shadow + slight rotate sobre cards de platos · cursor especial cuchara/whisk en zonas editoriales
- **Parallax suave** sobre hero image · simula vapor saliendo
- **Micro-interacción "servir":** al hover sobre paella image · slight shimmer dorado encima (como si la cuchara la tocara)
- **INV-5 device-aware obligatorio:** efectos solo en `pointer:fine and hover:hover` · mobile NO tiene cursor especial · pero SÍ scroll-driven motion

### V5 · GUSTO · evocado via memoria + testimonio
- **Sección "El sabor que regala"** con testimonios curados por palabras de SABOR (NO "5 estrellas · service excellent") · sí: *"Supo a casa de abuela"* · *"La primera cucharada todos paramos de hablar"* · *"El socarrat valió todo el evento"*
- **Cita de Chef Janet sobre EL SABOR:** extraída de YouTube channel o IG · si NO existe verbatim · brief Manus dispatch para que solicite a Chef Janet en próxima iteración

### V6 · NARRATIVA · storytelling Chef Janet (alma del sitio)
- **Sección "Detrás del fuego" o "El oficio"** · backstory 20 años · momento clave que la hizo paella chef · NO bullets corporativos · narrativa editorial primer persona
- **"Mi proceso" sequence:** 5 capítulos visuales:
  1. *El día anterior* (compra mariscos · marinar)
  2. *El fuego* (encender · esperar el carbón perfecto)
  3. *El sofrito* (la base que todo descansa encima)
  4. *El servicio* (montar · servir · cerrar el círculo con el comensal)
  5. *El cierre* (la sobremesa · el silencio de gente comiendo bien)
- **Quotes intercaladas estilo editorial culinaria** · entre secciones · sobre fondo color paleta

---

## §4 · 11 REGLAS PLAYBOOK + ENMIENDAS v2

Heredar las 11 reglas duras del `_pipeline/MANUS_DISPATCH_PLAYBOOK.md` v1-perfect-first-try del v1. Enmiendas específicas v2:

- **REGLA 12 candidata:** vertical food premium = doctrina inmersiva multi-sensorial obligatoria (§3 arriba) · NO opcional · cruza §7 ADN MARKER pregunta 1 "experiencia personalizada" al máximo
- **REGLA 13 candidata:** uso obligatorio de assets reales del cliente cuando estén disponibles · NUNCA screenshots ni stock photos cuando hay acceso autenticado al feed (vía forge-browser FORGE) · INV-3 anti-placeholder reforzado
- **REGLA 14 candidata:** voice del cliente extraída de su contenido público (IG alts · YouTube titles · captions) DEBE ser copy editorial del sitio · NO copy genérico chef-website AI-simple

---

## §5 · 8 MOVIMIENTOS DIFERENCIADORES PREMIUM CANON FORGE (audit obligatorio v2)

Manus debe garantizar que el sitio v2 INCLUYE explícitamente los 8 (vs los 3-4 que tiene v1):

1. **Scroll-driven motion** (parallax · reveal con intención) · ✅ obligatorio v2
2. **Hero cinemático** (video bg autoplay muted loop · NOT image) · ✅ obligatorio v2
3. **Micro-interacciones con peso** (hover lift · shadow · rotate · cursor especial · click feedback animado) · ✅ obligatorio v2
4. **Tipografía editorial** (serif Cormorant/Playfair + sans Inter/Söhne · variable weights · contraste) · ✅ obligatorio v2
5. **Paleta defensible 5 colores con jerarquía** (dorado azafrán · rojo paprika · verde olivar · brown crusta · negro carbón · NO 7 colores planos AI-simple) · ✅ obligatorio v2
6. **Sigilo identitario diseñado** (logo SVG monocromo Chef Janet · NO emoji 🥘 crudo INV-9 · candidato: silueta wok+cuchara estilizada) · ✅ obligatorio v2
7. **Forms honest-visible failure states** (heredar mailto: fallback v1 ya OK · agregar visual feedback en submit · INV-8) · ✅ heredado v1
8. **Device-aware nativo** (mobile 320px verificado · `pointer:fine` para hover · INV-5) · ✅ heredado v1

---

## §6 · 9 SECCIONES v2 · ESTRUCTURA OBLIGATORIA

| # | Sección | v1 estado | v2 transformación |
|---|---|---|---|
| 1 | Hero | foto estática + tagline | **Video bg YouTube reel destacado + tagline editorial "Esto no es solo una Paella" + CTA sutil "Conversa con Chef Janet"** |
| 2 | El Oficio (NEW) | inexistente v1 | **NEW · narrativa Chef Janet · 20 años · momento clave · primera persona editorial · 3 fotos curated del feed** |
| 3 | Servicios (3 cards) | cards básicas | **3 cards con IG reel embed mini por card + descripción sensory editorial + precio anchored** |
| 4 | El Proceso (NEW · "Mi proceso") | inexistente v1 | **NEW · 5 capítulos scroll-driven · fotos macros · texto editorial primera persona Chef Janet** |
| 5 | Galería editorial curada | grid 4 fotos IG screenshots | **5 capítulos visuales: Proceso · Paella · Servicio · Gente · Sabor · 6-8 fotos por capítulo de las 30 reales descargadas · NO grid IG copy** |
| 6 | El Sabor que regala (testimonios) | 2 reseñas Google stock | **Curado por palabras de sabor · iconografía editorial · NO 5-estrellas card · usar testimonios reales del IG comments + Google si disponible** |
| 7 | Conversación (cotizar) | form básico | **Form editorial con preguntas tipo "¿cómo te gustaría que se sintiera tu evento?" · NO inputs corporativos · mailto: fallback heredado v1** |
| 8 | Detrás del fuego (bio Chef Janet) | bio + 3 badges animados | **Bio editorial primera persona + foto profesional Chef Janet (NO IG screenshot) + cita signature** |
| 9 | Footer + Newsletter | links + form básico | **Newsletter editorial "Recibe la próxima receta de Chef Janet" + links sociales con iconos custom · NO emojis de plataforma INV-9** |

---

## §7 · INV-1..10 SELF-APPLIED v2 (línea roja Pacto v0.4)

Todos heredan + reforzar específicos:
- **INV-1** · 0 IA visible (heredado v1 ✅)
- **INV-3** · 0 placeholder visible · usar 30 fotos reales descargadas · NO screenshots NO stock (reforzado v2 · era v1 defect)
- **INV-9** · sigilo SVG monocromo · NO emoji 🥘🍴 crudo · diseñar logo Chef Janet (candidato wok+cuchara estilizada)

Resto INV heredados sin enmienda.

---

## §8 · TRANSITIONAL PLACEHOLDERS v2 (mismos que v1 · no son bloqueo Soberano)

- Web3Forms key: vacía (triggea mailto: fallback automático · funciona desde día 1)
- Email destino: `riveramichael9006@gmail.com` (Soberano transitional · Chef Janet swap post-validación demo)

Doctrina aplicada: **info que no tenemos NO bloquea demo · cliente confirma DESPUÉS de validar · pattern Angel + Richard validado**.

---

## §9 · QA TARGETS v2

| Criterio | v1 | v2 obligatorio |
|---|---|---|
| 4 hallazgos Soberano H1-H4 resueltos | 0/4 | 4/4 |
| 8 movimientos diferenciadores premium | 3-4 | 8/8 |
| Assets reales (30 fotos disponibles) | 0 | 100% |
| Video element (hero + reels embed) | 0 | mínimo 3 |
| 6 vectores experiencia inmersiva | 0 | 6/6 |
| §7 ADN MARKER 8/8 | parcial | 8/8 |
| INV-1..10 | 9/9 | 10/10 |

**QA externo Chrome obligatorio v2 LIVE** (post-Pages-activación) · usar paquete `2026-05-20-chrome-qa-paellasymas-v1-master.md` enmendado para v2 con criterios nuevos.

---

## §10 · DESTINO + ZIP entregables esperados v2

- `index.html` single-file con todas las 30 fotos reales embebidas (puede crecer a ~800KB · OK para single-page)
- `assets/og-image.jpg` actualizada con foto real cliente (NO screenshot)
- `assets/sigilo.svg` (NEW · sigilo monocromo Chef Janet · INV-9)
- `assets/videos/` opcional si Manus puede preparar fallbacks · pero iframes YouTube/IG sirven
- `sitemap.xml` + `robots.txt` heredados
- `README_FORGE_DEPLOY_v2.md` con explicación de 4 hallazgos resueltos + 6 vectores aplicados + QA self-report honest

---

## §11 · NOTAS PARA MANUS

1. **Doctrina inmersiva NO es opcional.** Cada decisión de craft debe poder responder "¿qué sentido invoca esto?"
2. **Voice de Chef Janet ya existe en los alts de las 30 fotos.** Usar verbatim como copy editorial · NO inventar copy chef-website genérico.
3. **YouTube + IG reels embed via iframes.** No necesitas descargar videos. Embed iframes funcionan tal cual.
4. **El demo NO es producto final.** Es para que Chef Janet vea y confirme detalles (email · scope entrenamiento · dominio final). Los placeholders transitional son legítimos.
5. **Si tienes dudas de craft food premium · referencia mental:** Eleven Madison Park web · Asador Etxebarri web · Disfrutar Barcelona web · Central Lima web · Nordic Food Lab web (NO copiarlos · respirar el calibre).

---

*FORGE-Digital DISPATCH v2 · Omega FORGE Ω orquesta · Manus construye · doctrina inmersiva multi-sensorial vertical food premium · 4 hallazgos Soberano + 30 fotos reales + 6 vectores · target v2-better-than-v1 · barco firme · "no creemos cualquier página · creemos la experiencia".*
