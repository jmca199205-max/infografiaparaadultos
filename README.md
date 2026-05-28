# 🤾 Infografía Interactiva: Dinámica y Táctica del Balonmano

> Aplicación web progresiva (PWA) de un solo archivo para el aprendizaje autónomo del balonmano moderno.

---

## 👤 Autoría

| Campo | Detalle |
|---|---|
| **Autora** | Joshely Camacho Agip |
| **Curso** | Infografía |
| **Año** | 2026 |
| **Institución** | Universidad Tecnológica del Perú (UTP) |

---

## 📋 Descripción

Infografía interactiva tipo dashboard diseñada para adultos de 30 a 50 años que deseen comprender los fundamentos tácticos, dinámicos y reglamentarios del balonmano. La experiencia es no lineal, autónoma y visualmente premium, basada en el reglamento oficial IHF 2023.

---

## 🚀 Cómo usar

1. Descarga el archivo `index.html`
2. Ábrelo directamente en cualquier navegador moderno (Chrome, Firefox, Edge, Safari)
3. No requiere servidor, instalación ni conexión a internet (excepto para cargar las fuentes de Google Fonts y Bootstrap CDN la primera vez)

```
balonmano/
└── index.html   ← único archivo, todo incluido
```

---

## 📚 Contenido de la Infografía

| Módulo | Descripción |
|---|---|
| **Hero principal** | Título, métricas clave y datos rápidos del deporte |
| **Hub central (Bento UI)** | Acceso rápido a todos los módulos de aprendizaje |
| **La Cancha** | Diagrama SVG interactivo 40×20 m con jugadores, zonas de 6m, 9m y 7m |
| **Posiciones** | 7 tarjetas con efecto hover (Veronica Card): Portero, Central, Laterales, Extremos y Pivote |
| **Técnicas de lanzamiento** | Suspensión, apoyo y cadera — cuándo usar, ventaja táctica, lectura del juego |
| **El Portero** | Defensa, reflejos, contraataque, penalti (7m) y regla empty goal 2016 |
| **Dinámica táctica** | Cruce, bloqueo del pivote, transición ofensiva y fijación táctica |
| **Autoevaluación** | Quiz de 5 preguntas con retroalimentación inmediata y puntaje final |
| **Fuentes académicas** | Bibliografía completa con referencias IHF, EHF, Stanford y Olympics.com |

---

## 🏟️ Datos Oficiales del Balonmano (IHF 2023)

| Dato | Valor |
|---|---|
| Dimensiones de la cancha | 40 × 20 metros |
| Duración del partido | 2 tiempos de 30 minutos |
| Jugadores por equipo | 7 (6 de campo + 1 portero) |
| Tiempo máximo con el balón | 3 segundos |
| Área del portero | Línea de 6 metros |
| Tiro libre | Línea de 9 metros |
| Penalti | Línea de 7 metros |

---

## ⚽ Jugadores en la Cancha

El diagrama SVG muestra una situación táctica real con **14 jugadores** en cancha:

**Equipo A — Ataque (cyan)**

| Sigla | Posición |
|---|---|
| GK | Portero |
| CT | Central (con balón) |
| LI | Lateral Izquierdo |
| LD | Lateral Derecho |
| EI | Extremo Izquierdo |
| ED | Extremo Derecho |
| PV | Pivote |

**Equipo B — Defensa 6-0 (naranja)**

| Sigla | Posición |
|---|---|
| GK | Portero |
| D1–D6 | Línea defensiva 6-0 |

---

## 🎨 Diseño y Tecnología

### Stack técnico

- **HTML5** semántico con `aria-labels` y navegación por teclado
- **CSS3** — dark mode, glassmorphism, animaciones `opacity` + `translateY`
- **JavaScript Vanilla** — datos en objetos JSON, renderizado dinámico en DOM
- **Bootstrap 5** (vía CDN)
- **PWA** — Web App Manifest (Data URI) + Service Worker (Blob)

### Efecto de tarjetas (Veronica Card)

Inspirado en [codepen.io/veronicadev/pen/WJyOwG](https://codepen.io/veronicadev/pen/WJyOwG):

- `transform: scale(1.055)` — la tarjeta "salta" al hacer hover
- `opacity` de imagen baja a 0.55 — imagen se vuelve semi-opaca
- `background-size` aumenta de 120% a 135% — zoom sutil
- `background-position` se desplaza — leve movimiento interno
- Footer de tarjeta con atributos y ❤️ "Me gusta" aparece con `translateY`

### Paleta de colores

| Variable | Color | Uso |
|---|---|---|
| `--accent-cyan` | `#00d4ff` | Equipo A, acentos principales |
| `--accent-teal` | `#00b4a0` | Zona 6m, módulo portero |
| `--accent-amber` | `#f5a623` | Zona 9m, posiciones |
| `--accent-orange` | `#ff6b35` | Zona 7m, equipo defensa, táctica |
| `--bg-deep` | `#060912` | Fondo base |

### Tipografía

| Familia | Uso |
|---|---|
| **Bebas Neue** | Títulos, métricas, números grandes |
| **DM Sans** | Cuerpo de texto, descripciones |
| **DM Mono** | Etiquetas, badges, código |

---

## ♿ Accesibilidad (WCAG)

- Contraste adecuado en todos los textos
- Navegación completa por teclado (`Tab`, `Enter`)
- `aria-labels` en todos los elementos interactivos
- `aria-live` en el quiz para lectores de pantalla
- `role` semánticos: `list`, `listitem`, `region`, `progressbar`
- Respeto por `prefers-reduced-motion`
- Estados de foco visibles con outline cyan

---

## 📖 Fuentes y Referencias

| # | Fuente |
|---|---|
| 01 | IHF — International Handball Federation. *Rules of the Game 2023*. [ihf.info](https://www.ihf.info) |
| 02 | EHF — European Handball Federation. *Rules & regulations adjustments 2025/26*. [eurohandball.com](https://www.eurohandball.com) |
| 03 | Stanford Open Virtual Assistant Lab. *Handball Overview Report (STORM)*. [storm.genie.stanford.edu](https://storm.genie.stanford.edu/conversation/137625) |
| 04 | Olympics.com. *Handball rules: Know how to play the game*. [olympics.com](https://www.olympics.com) |
| 05 | IHF (2022). *New rules to be enforced in handball from 1 July 2022 — Resin-free ball*. |
| 06 | Nielsen, H. (1898). *Foundations of modern handball*. Referencia histórica vía ALISY.EU |
| 07 | EHF. *Helena Elver's tactical tips on how to create an attacking game*. |
| 08 | Handball Evolution. *Collective Tactics of the Attack — 4:2 Offensive Formation*. |
| 09 | Vanja Radic Coaching. *Pre-Season Handball Goalkeeper Training*. |
| 10 | Journal of Sports Science. *Effect of Sling-Based Training with Rotational Strength on shooting performance*. |

---

## 📄 Licencia

Proyecto académico — Curso de Infografía, UTP 2026.  
Contenido basado en fuentes oficiales IHF, EHF y Stanford Open Lab.

---

*Desarrollado con HTML5 · CSS3 · JavaScript Vanilla · Bootstrap 5*
