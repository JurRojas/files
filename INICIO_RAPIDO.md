# 🚀 Guía de Inicio Rápido - Reon Digital

## ⏱️ 5 minutos para tener tu landing page lista

### Paso 1: Abrir el Proyecto

1. Descarga la carpeta `reon-digital`
2. Abre `index.html` en tu navegador
3. ✅ **¡Tu sitio está vivo!**

---

## 🎯 Primeros Cambios (10 minutos)

### 1. Cambiar el Nombre de tu Marca

**Abre:** `index.html`

**Busca la línea ~30:**
```html
<span class="logo-text">Reon</span>
<span class="logo-highlight">Digital</span>
```

**Reemplaza con tu marca:**
```html
<span class="logo-text">Mi</span>
<span class="logo-highlight">Agencia</span>
```

### 2. Agregar tu Número de WhatsApp

**Busca:** `wa.me/34666777888`

**Reemplaza en 3 lugares:**
1. Navbar (línea ~47)
2. Botón Hero (línea ~78)
3. Footer (línea ~357)

**Nuevos números:**
- **México:** `wa.me/5219876543210`
- **Chile:** `wa.me/56912345678`
- **Argentina:** `wa.me/5491123456789`
- **España:** `wa.me/34666777888`

### 3. Cambiar Colores

**Abre:** `css/styles.css`

**Busca `:root {` (línea ~5)**

```css
:root {
    /* CAMBIAR ESTE COLOR */
    --primary: #ff1b6d;  /* Fucsia actual */
    
    /* CAMBIAR A TUS COLORES FAVORITOS */
    --primary: #0066ff;  /* Azul */
    --primary: #9b59b6;  /* Púrpura */
    --primary: #2ecc71;  /* Verde */
    --primary: #e74c3c;  /* Rojo */
}
```

**Colores por industria:**

```css
/* 🏦 Finanzas */
--primary: #1a4d7a;           /* Azul profesional */
--accent-peach: #ffd700;      /* Dorado */

/* 💄 Belleza */
--primary: #c2185b;           /* Rosa profundo */
--accent-peach: #fce4ec;      /* Rosa pálido */

/* 🌿 Wellness/Ecología */
--primary: #27ae60;           /* Verde natural */
--bg-warm: #f0f8f0;           /* Fondo verde suave */

/* 🚀 Tech/Startup */
--primary: #0066ff;           /* Azul tech */
--accent-peach: #ffaa00;      /* Naranja energía */
```

---

## 📝 Cambiar Textos Principales

### Hero Section (Título grande)

**Busca en `index.html` (línea ~57):**
```html
<h1 class="hero-title">
    Tu negocio también merece una buena 
    <span class="highlight-serif">entrada en internet</span>
</h1>
```

**Puedes cambiar a:**
```html
<h1 class="hero-title">
    Llevamos tu <span class="highlight-serif">negocio</span> 
    a la era digital
</h1>
```

**O:**
```html
<h1 class="hero-title">
    Tu presencia online empieza 
    <span class="highlight-serif">hoy</span>
</h1>
```

### Botones principales

**Línea ~68:**
```html
<!-- Botón primario -->
<button class="btn btn-primary">Cuéntame sobre tu negocio</button>

<!-- Cambiar a: -->
<button class="btn btn-primary">Solicitar demo gratis</button>
```

**Línea ~72:**
```html
<!-- Botón secundario -->
<button class="btn btn-secondary">Ver cómo trabajo</button>

<!-- Cambiar a: -->
<button class="btn btn-secondary">Ver portafolio</button>
```

---

## 📊 Personalizar Secciones

### Cambiar Título de Servicios

**Línea ~131:**
```html
<h2>¿Qué puedo crear para ti?</h2>
<p>Soluciones adaptadas a tu negocio local</p>
```

**Cambiar a:**
```html
<h2>Nuestros Servicios</h2>
<p>Todo lo que tu negocio necesita para crecer online</p>
```

### Agregar/Quitar un Servicio

**Cada servicio es una tarjeta como esta (línea ~141):**
```html
<div class="service-card">
    <div class="service-number">01</div>
    <h3>Landing Page & Web</h3>
    <p>Descripción del servicio...</p>
    <div class="service-tag">Presencia online</div>
</div>
```

**Para duplicar un servicio:**
1. Copia toda la sección `<div class="service-card">...</div>`
2. Pégalo después
3. Cambia el número (01 → 04)
4. Actualiza el título y descripción
5. Listo ✅

---

## 🎨 Cambiar Elementos Flotantes (Emojis)

**Línea ~85-87:**
```html
<div class="float-element element-1">📊</div>
<div class="float-element element-2">🎯</div>
<div class="float-element element-3">✨</div>
```

**Cambiar emojis:**
```html
<!-- Elementos más corporativos -->
<div class="float-element element-1">💼</div>
<div class="float-element element-2">🚀</div>
<div class="float-element element-3">💡</div>

<!-- Elementos más calorosos -->
<div class="float-element element-1">❤️</div>
<div class="float-element element-2">⭐</div>
<div class="float-element element-3">🎉</div>

<!-- Elementos tech -->
<div class="float-element element-1">💻</div>
<div class="float-element element-2">🔧</div>
<div class="float-element element-3">⚡</div>
```

---

## 🔗 Configurar Links

### WhatsApp (ya cubierto arriba)

Reemplaza en 3 lugares:
```
Navbar:       línea ~47
Hero button:  línea ~78
Footer:       línea ~357
```

### Redes Sociales (Footer)

**Línea ~355-356:**
```html
<a href="https://instagram.com" class="social-link">Instagram</a>
```

**Cambiar a tu perfil:**
```html
<a href="https://instagram.com/tu_usuario" class="social-link">Instagram</a>
<a href="https://facebook.com/tu_pagina" class="social-link">Facebook</a>
<a href="https://linkedin.com/in/tu_perfil" class="social-link">LinkedIn</a>
```

---

## 📱 Probar en Móvil

### Opción 1: Navegador Desktop
1. Abre `index.html` en Chrome/Firefox
2. Presiona `F12` (abrir DevTools)
3. Click en icono de móvil (esquina superior izquierda)
4. Selecciona un dispositivo (iPhone 12, Samsung Galaxy, etc.)
5. Revisa que todo se vea bien

### Opción 2: En tu Teléfono Real
1. Guarda `index.html` en la nube (Google Drive, etc.)
2. Abre el link desde tu móvil
3. Comprueba que funciona correctamente

---

## 🌐 Publicar Online (Gratuito)

### **Opción 1: Netlify** ⭐ (Recomendado)

1. Ve a [netlify.com](https://netlify.com)
2. Haz clic en "Sign up" (regístrate con GitHub o email)
3. Luego: "Add new site" → "Deploy manually"
4. Arrastra la carpeta `reon-digital` completa
5. **¡Listo!** Tu sitio tiene URL pública en 30 segundos

**Tu URL será algo como:** `https://tuproyecto.netlify.app`

### **Opción 2: Vercel**

1. Ve a [vercel.com](https://vercel.com)
2. Click en "New Project"
3. Sube tu carpeta
4. Espera a que se despliegue
5. **¡Hecho!**

### **Opción 3: GitHub Pages** (Si sabes Git)

```bash
# Crear repositorio en GitHub
git init
git add .
git commit -m "Landing page Reon Digital"
git push origin main
```

Luego en Settings → Pages → selecciona "main branch"

---

## ✅ Checklist Antes de Publicar

- [ ] Cambié el nombre de marca (navbar + footer)
- [ ] Actualicé el número de WhatsApp (3 lugares)
- [ ] Personalicé el título y descripción principal
- [ ] Cambié colores a mi paleta
- [ ] Revisé en mobile (responsive)
- [ ] Todos los botones funcionan
- [ ] Actualicé redes sociales
- [ ] Probé los links de WhatsApp
- [ ] Cambié emojis/iconos (opcional)
- [ ] Revisé ortografía

---

## 🎨 Ejemplos de Cambios Rápidos

### Ejemplo 1: Para Agencia de Diseño

```html
<!-- Cambiar título hero a: -->
<h1 class="hero-title">
    Diseños que <span class="highlight-serif">venden</span>
</h1>

<!-- Cambiar color primario a: -->
--primary: #7c3aed;  /* Púrpura moderno */

<!-- Cambiar emojis a: -->
<div class="float-element element-1">🎨</div>
<div class="float-element element-2">✏️</div>
<div class="float-element element-3">🖌️</div>
```

### Ejemplo 2: Para Consultoría

```html
<!-- Título: -->
<h1 class="hero-title">
    Estrategia digital que <span class="highlight-serif">genera resultados</span>
</h1>

<!-- Color: -->
--primary: #1a4d7a;  /* Azul corporativo */

<!-- Emojis: -->
<div class="float-element element-1">📈</div>
<div class="float-element element-2">🎯</div>
<div class="float-element element-3">💼</div>
```

### Ejemplo 3: Para E-commerce

```html
<!-- Título: -->
<h1 class="hero-title">
    Tienda online que <span class="highlight-serif">convierte</span>
</h1>

<!-- Color: -->
--primary: #e74c3c;  /* Rojo energía */

<!-- Emojis: -->
<div class="float-element element-1">🛒</div>
<div class="float-element element-2">💳</div>
<div class="float-element element-3">📦</div>
```

---

## 💡 Tips Pro

1. **No cambies el espaciado** (padding/margin) - ya está optimizado
2. **Mantén máximo 3 colores** - se verá más profesional
3. **Textos cortos y puntuales** - móvil y desktop lo agradecen
4. **Prueba en mobile** - no es opcional, es obligatorio
5. **Actualiza todos los WhatsApp** - si uno falla, pierdes clientes
6. **Las imágenes ralentizan** - mejor usa emojis y colores

---

## 🆘 Problemas Comunes

### "El sitio se ve extraño en mobile"
→ Abre DevTools (F12) → Click icono móvil → Recarga (Ctrl+R)

### "Los colores no cambian"
→ Revisa que escribiste el color en `css/styles.css` (no en HTML)
→ Borra caché: Ctrl+F5 (Windows) o Cmd+Shift+R (Mac)

### "WhatsApp no funciona"
→ Verifica que escribiste bien el número
→ Formato: `wa.me/` + código país + número (sin espacios)

### "Los botones no se ven"
→ Revisa que no hayas cambiado el `padding` en CSS
→ Comprueba que el `display: flex` siga en `.hero-cta`

---

## 📚 Documentación Completa

Para cambios más avanzados, revisa:
- **CUSTOMIZACION.md** → Guía detallada de personalización
- **ESPECIFICACIONES_DISEÑO.md** → Detalles visuales y técnicos

---

## 🎓 Próximos Pasos

1. **Añadir imágenes:** En servicios o hero (optimiza bien)
2. **Formulario de contacto:** Conectar con email/Zapier
3. **Blog/Portafolio:** Agregar sección con tus trabajos
4. **Analytics:** Agregar Google Analytics para tracking
5. **Animaciones extras:** Más transiciones en hover

---

**¡Tu landing page está lista para brillar! 🌟**

Cualquier duda, revisa los comentarios en el código.
Todos los archivos están bien documentados.

Hecho con ❤️ para emprendedores digitales.
