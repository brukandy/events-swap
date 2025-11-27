# Events Swap Component - Leone Master School

Componente interattivo per la presentazione degli eventi della Leone Master School con animazioni GSAP, swipe mobile e dots navigation.

## 🎯 Features

### **Animazioni & Interazioni**
- ✅ Card swap 3D con GSAP
- ✅ Auto-rotate ogni 5 secondi
- ✅ Swipe gestures su mobile (left/right)
- ✅ Dots navigation (3 pallini)
- ✅ Click su card per swap manuale
- ✅ Pause on hover (desktop)

### **Contenuto Dinamico**
- ✅ 3 eventi con GIF animate
- ✅ Loghi PNG quadrati (300x300px)
- ✅ Badge "Evento" con gradient giallo
- ✅ Descrizioni sincronizzate con card attiva
- ✅ CTA button "Scopri l'evento"

### **Responsive Design**
- ✅ **Desktop:** Card stack a destra, clipped al bordo
- ✅ **Tablet:** Layout adattivo
- ✅ **Mobile Portrait:** Card in basso, swipe orizzontale
- ✅ **Mobile Landscape:** Layout ottimizzato per altezza ridotta

### **Styling**
- ✅ Glassmorphism effects
- ✅ Sfondo trasparente (per Elementor)
- ✅ Font: Inter (Google Fonts)
- ✅ Smooth transitions e fade effects

## 📁 Struttura File

```
events-swap/
├── index.html          # Struttura HTML principale
├── style.css           # Stili e responsive
├── script.js           # Logica GSAP e interazioni
├── images/             # GIF animate degli eventi
│   ├── io creo.gif
│   ├── donna leader.gif
│   └── money maker.gif
└── loghi/              # Loghi PNG quadrati
    ├── io creo.png
    ├── donna leader.png
    └── money maker.png
```

## 🎨 Eventi

### 1. **Io Creo il Mio Destino**
- **Badge:** Evento (giallo)
- **Logo:** Rosso bold
- **Descrizione:** L'unico evento di formazione in Italia che unisce Crescita Personale ed Educazione finanziaria

### 2. **Donna Leader**
- **Badge:** Evento (giallo)
- **Logo:** Rosa/Viola
- **Descrizione:** Evento dedicato alle donne per sviluppare leadership, autonomia e indipendenza

### 3. **Money Maker Summit**
- **Badge:** Evento (giallo)
- **Logo:** Blu navy con triangolo e €
- **Descrizione:** Il primo evento che porta il MOVIMENTO FIRE in Italia

## 💻 Tecnologie

- **HTML5** - Struttura semantica
- **CSS3** - Styling moderno con gradients, transitions, glassmorphism
- **JavaScript ES6** - Logica interattiva
- **GSAP 3.12.5** - Animazioni smooth e performanti
- **Google Fonts** - Inter (400, 600, 700, 800)

## 🎯 Configurazione GSAP

```javascript
const config = {
    cardDistance: 60,        // Distanza orizzontale tra card
    verticalDistance: 70,    // Distanza verticale tra card
    delay: 5000,             // Auto-rotate delay (5s)
    skewAmount: 6,           // Skew 3D effect
    ease: 'power2.out',      // Easing function
    duration: 0.6            // Animation duration
};
```

## 📱 Responsive Breakpoints

- **Desktop:** > 968px
- **Tablet:** 481px - 968px
- **Mobile:** < 480px
- **Landscape:** max-height 600px + orientation landscape

## 🎨 Color Palette

```css
/* Badge Evento */
background: linear-gradient(135deg, #fbbf24 0%, #fde047 100%);
color: #1e3a8a;

/* Text Colors */
--primary-text: #ffffff;
--secondary-text: rgba(255, 255, 255, 0.8);

/* Background (per test locale) */
background: linear-gradient(135deg, #0f172a 0%, #1e293b 50%, #0f172a 100%);
```

## 🚀 Deploy

### **GitHub Pages**
- **Repo:** https://github.com/brukandy/events-swap
- **Live:** https://brukandy.github.io/events-swap/

### **Elementor Integration**

```html
<style>
.elementor-widget-html {
    margin: 0 !important;
    padding: 0 !important;
}
.elementor-widget-container {
    margin: 0 !important;
    padding: 0 !important;
}
</style>

<iframe 
    src="https://brukandy.github.io/events-swap/" 
    width="100%" 
    height="1000" 
    frameborder="0"
    scrolling="no"
    style="border: none; display: block; margin: 0; padding: 0; overflow: hidden;">
</iframe>
```

## 🔧 Local Development

```bash
# Avvia server locale
python3 -m http.server 8085

# Apri browser
open http://localhost:8085

# Test su mobile (stessa rete WiFi)
# Usa IP locale: http://192.168.178.179:8085
```

## 📝 Note Tecniche

### **Performance**
- GIF ottimizzate per web
- Loghi PNG compressi
- GSAP per animazioni hardware-accelerated
- `force3D: true` per rendering GPU

### **Browser Support**
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

### **Accessibility**
- Alt text per immagini
- Keyboard navigation (dots)
- Touch-friendly targets (min 44px)
- Semantic HTML

## 🎯 Future Enhancements

- [ ] Lazy loading per GIF
- [ ] Preload immagini
- [ ] Intersection Observer per auto-play
- [ ] A/B testing dots vs arrows
- [ ] Analytics tracking per eventi

## 📄 License

Proprietà di Leone Master School - Tutti i diritti riservati

## 👨‍💻 Development

Sviluppato con Windsurf AI - Novembre 2025

---

**Versione:** 1.0.0  
**Ultimo aggiornamento:** 27 Novembre 2025
