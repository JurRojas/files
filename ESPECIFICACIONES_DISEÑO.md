# 🎨 Reon Digital - Especificaciones de Diseño

## 📐 Visión General

Landing page moderna inspirada en **Juana IA**, pero con identidad original y totalmente personalizable.
Diseñada específicamente para agencias digitales, desarrolladores y negocios que venden servicios web.

---

## 🎭 Paleta de Colores

### Colores Principales
```
Fucsia/Rosa Principal:    #ff1b6d  ← Acento principal (botones, títulos)
Rosa Claro:               #ff6ba8  ← Hover states
Rosa Oscuro:              #d41055  ← Estados presionados

Fondo Cálido (Crema):     #faf8f6  ← Fondo principal
Blanco Puro:              #ffffff  ← Tarjetas y áreas claras
Azul Tenue:               #e0e7ff  ← Degradado suave
Durazno Suave:            #ffe8d6  ← Degradado cálido
Rosa Suave:               #fce4ec  ← Acentos sutiles

Texto Oscuro:             #1a1a1a  ← Títulos y texto principal
Texto Gris:               #666666  ← Párrafos
Texto Claro:              #999999  ← Información secundaria
```

### Degradados

**Hero Background:**
```
135deg: 
  - rgba(255, 27, 109, 0.05)   Rosa tenue
  - rgba(255, 232, 214, 0.15)  Durazno
  - rgba(224, 231, 255, 0.1)   Azul
```

**Process Section:**
```
135deg:
  - rgba(255, 27, 109, 0.03)   Rosa muy suave
  - rgba(224, 231, 255, 0.08)  Azul suave
```

---

## 🔤 Tipografía

### Fuentes
- **Sans-Serif (Principal):** Segoe UI, Roboto, Helvetica Neue
  - Uso: Títulos, cuerpo, botones
  - Peso: 400, 600, 700

- **Serif (Itálica):** Georgia
  - Uso: Palabras clave destacadas
  - Efecto: Contraste elegante

### Escala Tipográfica

```
Hero Title:       72px (clamp: 36px → 72px)
Section Title:    48px (clamp: 32px → 48px)
Card Title:       20px (fijo)
Párrafo:          16px (fijo)
Small Text:       13-14px (fijo)
```

---

## 🎯 Componentes Principales

### 1. Navbar
- **Altura:** 60px (con padding)
- **Estilo:** Frosted glass (backdrop blur)
- **Comportamiento:** Sticky en scroll
- **Elementos:**
  - Logo textual (izquierda)
  - Links de navegación (centro)
  - Selector de idioma + botón WhatsApp (derecha)
- **Mobile:** Hamburger menu colapsable

### 2. Hero Section
- **Alto:** 100vh (viewport height) / responsive
- **Contenido:** Centrado verticalmente
- **Elementos Flotantes:** Emojis animados
- **Tipografía:** Bold sans-serif + serif italic
- **Botones:** Primario y secundario
- **Degradado:** Fondo suave con 3 colores

### 3. Metrics Cards
- **Grid:** 3 columnas responsive
- **Estilo:** Cards blancas con sombra suave
- **Hover:** Elevación +8px, borde fucsia
- **Contenido:** Icono emoji + título + descripción

### 4. Services Section
- **Grid:** 3 columnas responsive (6 tarjetas en total)
- **Diseño:** Cards con número + título + descripción + tag
- **Hover:** Elevación +12px, borde fucsia, sombra mayor
- **Gradiente:** Fondo cálido (crema → blanco)

### 5. Process Section
- **Layout:** 3 tarjetas con flechas entre ellas
- **Estilo:** Cards centradas, verticales en mobile
- **Números:** 01, 02, 03 (fucsia)
- **Iconos:** Emojis grandes
- **Flechas:** Invisibles en mobile (rotate 90deg)

### 6. Final CTA
- **Fondo:** Degradado rosa/durazno/azul
- **Tipografía:** Grande y centrada
- **Botón:** Primario, grande, rounded
- **Alto:** 100px padding

### 7. Footer
- **Fondo:** Texto oscuro (#1a1a1a)
- **Grid:** 3 columnas (brand, links, social)
- **Texto:** Blanco / 80% opacidad
- **Divider:** Línea tenue entre contenido y copyright

---

## 🎨 Detalles de Diseño

### Bordes Redondeados
```
Botones (pills):     50px (completamente redondo)
Cards/Cajas:         24px (mediano)
Grandes:             48px (muy generoso)
Pequeños:            12px (sutil)
```

### Sombras
```
Sombra Pequeña:  0 2px 8px rgba(0,0,0,0.06)
Sombra Media:    0 4px 16px rgba(0,0,0,0.08)
Sombra Grande:   0 8px 24px rgba(0,0,0,0.1)
```

### Espaciado (Padding/Margin)
```
Secciones:       80px arriba/abajo
Containers:      0-20px (responsive)
Cards:           40px (24px en mobile)
Gap (grids):     32px
```

### Transiciones
```
Hover standard:  0.3s ease
Animaciones:     0.6s - 0.8s ease
Scroll behavior: smooth
```

---

## 📱 Breakpoints Responsive

```css
Desktop:        1200px (viewport normal)
Tablet:         768px  (ajustes de grid y spacing)
Mobile:         480px  (ajustes adicionales)
```

### Cambios en Mobile
- Navbar links → ocultos, menú hamburger visible
- Hero → altura reducida, elementos flotantes ocultos
- Grid servicios → 1 columna
- Botones → ancho 100% en hero
- Flechas proceso → rotadas 90deg
- Footer → stacked verticalmente

---

## ✨ Animaciones

### Elementos Flotantes
```css
- Movimiento suave hacia arriba/abajo: 4s infinito
- Seguimiento del cursor: parallax suave (mouse)
- Escala: Sin cambio de escala (mantiene tamaño)
```

### Entrada (Scroll)
```css
- Opacity: 0 → 1
- Transform: translateY(20px) → 0
- Duración: 0.6s ease
- Trigger: Intersection Observer (cuando entra en viewport)
```

### Hover
```css
Cards:          translateY(-8px) → (-12px si grande)
Botones:        shadow aumenta, fondo cambia
Links:          color → fucsia, underline animado
```

---

## 🎬 Microinteracciones

### Navbar
- Links tienen underline animado al hover
- Transparencia aumenta en scroll
- Sombra se agrega en scroll

### Botones
- Primario: Fondo más oscuro + elevación
- Secundario: Invertido (fondo oscuro, texto blanco)
- WhatsApp: Solo fondo fucsia

### Cards de Servicios
- Efecto hover visible
- Border cambia color
- Sombra se expande

---

## 📏 Especificaciones Técnicas

### Resolución
- Mínima: 320px (mobile)
- Máxima: 1920px (desktop)
- Contenedor máximo: 1200px

### Performance
- Sin imágenes externas (solo emojis)
- CSS vanilla (sin frameworks)
- JavaScript mínimo (scroll smooth)
- Archivo CSS: ~400 líneas
- Archivo HTML: ~400 líneas

### Accesibilidad
- Contraste de colores: ✅ WCAG AA compliant
- Tamaño de fuente: ✅ Readable (mínimo 14px)
- Touch targets: ✅ Mínimo 48x48px
- Navegación por teclado: ✅ Funcional

---

## 🔄 Estructura de Secciones

```
┌─────────────────────────────┐
│     NAVBAR (Sticky)         │
├─────────────────────────────┤
│                             │
│     HERO SECTION            │
│   (100vh, centrado)         │
│   + elementos flotantes     │
│                             │
├─────────────────────────────┤
│   METRICS (3 cards)         │
├─────────────────────────────┤
│   SERVICES (6 cards, 3x2)   │
├─────────────────────────────┤
│   PROCESS (3 pasos + flechas)
├─────────────────────────────┤
│   FINAL CTA (grande)        │
├─────────────────────────────┤
│     FOOTER                  │
└─────────────────────────────┘
```

---

## 🎨 Guía de Tonalidad

### Versión "Startup Tech"
- Primario: Azul (#0066ff)
- Secundario: Naranja (#ff6600)
- Fondo: Blanco puro
- Resultado: Moderno, confiable

### Versión "Lujo/Premium"
- Primario: Dorado (#d4af37)
- Secundario: Negro (#1a1a1a)
- Fondo: Blanco + gris muy claro
- Resultado: Elegante, sofisticado

### Versión "Eco/Natural"
- Primario: Verde (#2ecc71)
- Secundario: Tierra (#8b6f47)
- Fondo: Crema + verde muy claro
- Resultado: Orgánico, confiable

---

## 📋 Checklist Visual

- ✅ Fondo crema/blanco cálido
- ✅ Degradados pastel sutiles (rosa, durazno, azul)
- ✅ Patrón de puntos (opcional, no incluido por defecto)
- ✅ Tipografía sans-serif bold para títulos
- ✅ Palabras clave en serif italic
- ✅ Acento fucsia principal
- ✅ Bordes redondeados grandes
- ✅ Sombras suaves
- ✅ Botones tipo pill (border-radius completo)
- ✅ Elementos flotantes con emojis
- ✅ Hero centrado y aireado
- ✅ Navbar sticky/fixed
- ✅ Diseño limpio y premium
- ✅ Totalmente responsivo
- ✅ Sin imágenes externas
- ✅ Variables CSS para fácil customización

---

**Diseño inspirado en tendencias modernas, sin copiar identidad de marca alguna.**

Hecho con ❤️ para emprendedores digitales.
