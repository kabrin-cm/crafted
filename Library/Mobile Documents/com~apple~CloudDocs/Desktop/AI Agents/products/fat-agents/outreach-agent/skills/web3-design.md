---
name: web3-design
description: "Apply web3/crypto-grade visual design to landing pages, sales pages, and marketing sites. Adds animated mesh gradients, particle systems, glassmorphism, glitch effects, animated borders, scroll animations, noise overlays, and more. Two modes: Full Build (new page from scratch) or Enhancement (upgrade existing page). Performance-optimized for mobile. Zero external dependencies in default mode. Triggers on: web3 design, add animations, make it look web3, particle effects, crypto aesthetic, glassmorphism, animated gradients, upgrade the design, make it premium, futuristic design. Outputs production-ready HTML/CSS/JS with web3 visual treatment."
---

# Web3 Design

Static pages don't convert like animated ones. Web3-style design is the current standard for premium, high-ticket digital presence: dark themes, animated gradients, particle networks, glassmorphism, and scroll-driven reveals. This skill applies that aesthetic to any landing page or marketing site.

This is not about blockchain technology. It's about the visual language that web3/crypto companies pioneered and that now signals "premium" and "cutting edge" across all industries. Trading education, SaaS, agencies, high-ticket coaching. If the target audience is online and spending $2K+, this aesthetic converts.

---

## The core job

Transform a landing page or marketing site from static/flat to premium web3 aesthetic while maintaining fast load times and full mobile responsiveness.

**Output format:** Production-ready HTML/CSS/JS with:
- Zero external dependencies (default mode)
- Full mobile responsiveness
- `prefers-reduced-motion` accessibility
- GPU-optimized animations (transform/opacity only where possible)
- Lighthouse performance score 90+ target

---

## Two modes

### Mode 1: Enhancement
**Use when:** An existing page needs visual upgrades without changing content or structure.
**Process:** Read the page, identify which effects to layer in, apply them while preserving all content and functionality.

### Mode 2: Full Build
**Use when:** Building a new page from scratch with web3 aesthetic baked in from the start.
**Process:** Use the design system tokens, pick an effect tier, build with animations integrated from the ground up.

---

## Design System Tokens

Every web3 page starts with these foundations. Pick a palette, set the typography, then layer effects on top.

### Color Palettes

**Palette A: Green/Gold (Agency, Growth)**
```css
:root {
  --bg: #0a0a0a;
  --bg-elevated: #111111;
  --bg-card: rgba(255, 255, 255, 0.04);
  --accent: #42CE09;
  --accent-dark: #2d8f06;
  --gold: #d4af37;
  --white: #ffffff;
  --gray: #a6a6a6;
  --border: rgba(255, 255, 255, 0.08);
}
```

**Palette B: Purple/Teal (Blockchain Classic)**
```css
:root {
  --bg: #05051f;
  --bg-elevated: #0a0a2e;
  --bg-card: #111133;
  --accent: #6331c8;
  --accent-secondary: #af94e4;
  --teal: #11816a;
  --teal-light: #5aa696;
  --white: #ffffff;
  --gray: #a0a0c0;
  --border: rgba(255, 255, 255, 0.08);
}
```

**Palette C: Cyan/Blue (DeFi, Fintech)**
```css
:root {
  --bg: #00303f;
  --bg-elevated: #303958;
  --bg-card: rgba(255, 255, 255, 0.05);
  --accent: #59b7e9;
  --accent-dark: #3984ff;
  --purple: #4d246f;
  --white: #ffffff;
  --gray: #99b7cf;
  --border: rgba(255, 255, 255, 0.08);
}
```

**Palette D: Neon/Cyberpunk (Bold, Aggressive)**
```css
:root {
  --bg: #0d0d0d;
  --bg-elevated: #1a1a2e;
  --bg-card: rgba(255, 255, 255, 0.04);
  --neon-pink: #ff006e;
  --neon-cyan: #00f5ff;
  --neon-green: #39ff14;
  --neon-purple: #b533b3;
  --white: #ffffff;
  --gray: #a0a0a0;
  --border: rgba(255, 255, 255, 0.08);
}
```

**Palette E: Professional Dark (Institutional, Finance)**
```css
:root {
  --bg: #0f172a;
  --bg-elevated: #1e293b;
  --bg-card: rgba(255, 255, 255, 0.04);
  --accent: #3b82f6;
  --success: #22c55e;
  --warning: #f59e0b;
  --danger: #ef4444;
  --white: #f8fafc;
  --gray: #94a3b8;
  --border: rgba(255, 255, 255, 0.08);
}
```

**Color usage rules:**
- Maximum 3 accent colors per page (1 primary + 2 supporting)
- Neon colors for CTAs, status indicators, and highlights only. Never for body text.
- Use at least 2 dark shades to create depth between surfaces (bg vs bg-elevated vs bg-card)
- Minimum 4.5:1 contrast ratio for body text, 3:1 for large headings
- Gradients in hero sections, card borders, and buttons. Not on body backgrounds that compete with content.

### Typography

**Recommended stacks:**
```css
:root {
  --font-heading: 'Space Grotesk', system-ui, sans-serif;
  --font-body: 'Inter', system-ui, sans-serif;
  --font-mono: 'Space Mono', 'JetBrains Mono', monospace;
}
```

**Scale (1.25 major third):**
```css
:root {
  --text-xs: 0.75rem;    /* 12px - labels, fine print */
  --text-sm: 0.875rem;   /* 14px - captions, nav */
  --text-base: 1rem;     /* 16px - body */
  --text-lg: 1.125rem;   /* 18px - large body */
  --text-xl: 1.25rem;    /* 20px - card titles */
  --text-2xl: 1.5rem;    /* 24px - section sub */
  --text-3xl: 1.875rem;  /* 30px - section titles */
  --text-4xl: 2.25rem;   /* 36px - h2 */
  --text-5xl: 3rem;      /* 48px - h1 */
  --text-6xl: 3.75rem;   /* 60px - hero */
  --text-7xl: 4.5rem;    /* 72px - hero large */
}
```

**Alternative heading fonts:** Clash Display (bold, modern), Satoshi (geometric, named after Satoshi Nakamoto), Outfit, Syne.

**Monospace for:** data displays, metric numbers, terminal effects, code blocks, countdown timers.

### Spacing & Layout
- Border radius: 16-24px for cards, 1000px for buttons (pill shape)
- Section padding: 100px desktop, 64px mobile
- Card padding: 32-36px
- Grid gap: 24-32px
- Max content width: 1200px
- Glassmorphic blur: 10-20px desktop, 6-8px mobile

---

## Effect Library

Each effect has a name, description, implementation code, performance cost, and mobile notes.

---

### Effect 1: Noise/Grain Overlay

**What:** Subtle film grain texture across the entire page. Signals premium/analog feel.
**Performance:** Minimal. Single CSS pseudo-element.
**Where to use:** Full page (fixed overlay at z-index 9999, pointer-events none).

```css
body::before {
  content: '';
  position: fixed;
  inset: 0;
  z-index: 9999;
  pointer-events: none;
  opacity: 0.035;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E");
  background-repeat: repeat;
  background-size: 256px 256px;
}
```

**Tuning:** `baseFrequency` 0.5 = coarser, 0.9 = fine, 1.2+ = very fine. `opacity` 0.03-0.05 for subtle, 0.1-0.15 for prominent.

**Animated variant (film grain):**
```css
body::before {
  /* same as above but add: */
  position: fixed;
  inset: -200%;
  animation: grain-drift 0.5s steps(4) infinite;
}

@keyframes grain-drift {
  0%, 100% { transform: translate(0, 0); }
  25%      { transform: translate(-5%, -5%); }
  50%      { transform: translate(5%, 5%); }
  75%      { transform: translate(-2%, 3%); }
}
```

**Mobile:** Same implementation. No reduction needed, it's just a background image.

---

### Effect 2: Animated Mesh Gradient Background

**What:** Slowly morphing multi-color gradient. Creates a living, breathing background.
**Performance:** Low-medium. CSS-only, GPU-composited when using transform.
**Where to use:** Hero section, final CTA section.

**Method A: Radial gradient layers with transform animation (GPU-optimized)**
```css
.hero {
  position: relative;
  overflow: hidden;
}

.hero::before {
  content: '';
  position: absolute;
  inset: -50%;
  background:
    radial-gradient(circle at 20% 30%, rgba(var(--accent-rgb), 0.15) 0%, transparent 50%),
    radial-gradient(circle at 80% 70%, rgba(var(--accent-dark-rgb), 0.1) 0%, transparent 50%),
    radial-gradient(circle at 50% 50%, rgba(var(--gold-rgb), 0.05) 0%, transparent 40%);
  animation: meshMove 20s ease-in-out infinite;
  z-index: 0;
}

@keyframes meshMove {
  0%, 100% { transform: translate(0, 0) scale(1); }
  25%      { transform: translate(-5%, 3%) scale(1.05); }
  50%      { transform: translate(3%, -5%) scale(1.02); }
  75%      { transform: translate(-3%, -3%) scale(1.08); }
}
```

**Method B: Linear gradient with background-position shift**
```css
.mesh-bg {
  background: linear-gradient(
    300deg,
    var(--bg), #302b63, var(--bg),
    var(--accent), var(--bg), var(--teal), var(--bg)
  );
  background-size: 180% 180%;
  animation: meshShift 18s ease infinite;
}

@keyframes meshShift {
  0%   { background-position: 0% 50%; }
  50%  { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}
```

**Mobile:** Reduce animation duration (slower = less CPU). Method A preferred (transform-only).

---

### Effect 3: Floating Glow Orbs

**What:** Large, soft radial gradient circles that float behind content. Creates depth.
**Performance:** Minimal. CSS pseudo-elements with transform animation.
**Where to use:** Hero, solution section, results section, CTA.

```css
.section::after {
  content: '';
  position: absolute;
  width: 500px;
  height: 500px;
  border-radius: 50%;
  background: radial-gradient(circle, rgba(var(--accent-rgb), 0.06) 0%, transparent 70%);
  top: -200px;
  right: -200px;
  animation: orbFloat 15s ease-in-out infinite;
  z-index: 0;
  pointer-events: none;
}

@keyframes orbFloat {
  0%, 100% { transform: translate(0, 0); }
  50%      { transform: translate(-80px, 60px); }
}
```

**Mobile:** Reduce width/height to 300px. Reduce translate distance.

---

### Effect 4: Particle Network Canvas

**What:** Floating dots with connecting lines. THE web3 signature effect. Mouse-reactive on desktop.
**Performance:** Medium. Canvas-based, uses requestAnimationFrame. Pause when off-screen.
**Where to use:** Hero section background.

```html
<canvas id="particles-canvas"></canvas>
```

```css
#particles-canvas {
  position: absolute;
  inset: 0;
  z-index: 0;
  pointer-events: none;
}
```

```javascript
(function() {
  var canvas = document.getElementById('particles-canvas');
  if (!canvas) return;
  var ctx = canvas.getContext('2d');
  var particles = [];
  var mouse = { x: -1000, y: -1000 };
  var isMobile = window.innerWidth < 810;
  var particleCount = isMobile ? 30 : 60;
  var connectionDist = isMobile ? 100 : 150;
  var accentColor = '66, 206, 9'; /* Match your --accent */
  var raf;

  function resize() {
    var hero = canvas.parentElement;
    canvas.width = hero.offsetWidth;
    canvas.height = hero.offsetHeight;
  }

  function createParticles() {
    particles = [];
    for (var i = 0; i < particleCount; i++) {
      particles.push({
        x: Math.random() * canvas.width,
        y: Math.random() * canvas.height,
        vx: (Math.random() - 0.5) * 0.4,
        vy: (Math.random() - 0.5) * 0.4,
        r: Math.random() * 1.5 + 0.5,
        alpha: Math.random() * 0.4 + 0.1
      });
    }
  }

  function draw() {
    ctx.clearRect(0, 0, canvas.width, canvas.height);

    for (var i = 0; i < particles.length; i++) {
      for (var j = i + 1; j < particles.length; j++) {
        var dx = particles[i].x - particles[j].x;
        var dy = particles[i].y - particles[j].y;
        var dist = Math.sqrt(dx * dx + dy * dy);
        if (dist < connectionDist) {
          var alpha = (1 - dist / connectionDist) * 0.12;
          ctx.strokeStyle = 'rgba(' + accentColor + ', ' + alpha + ')';
          ctx.lineWidth = 0.5;
          ctx.beginPath();
          ctx.moveTo(particles[i].x, particles[i].y);
          ctx.lineTo(particles[j].x, particles[j].y);
          ctx.stroke();
        }
      }
    }

    for (var k = 0; k < particles.length; k++) {
      var p = particles[k];

      if (!isMobile) {
        var mdx = mouse.x - p.x;
        var mdy = mouse.y - p.y;
        var mdist = Math.sqrt(mdx * mdx + mdy * mdy);
        if (mdist < 200) {
          var force = (200 - mdist) / 200 * 0.015;
          p.vx += mdx * force;
          p.vy += mdy * force;
        }
      }

      p.x += p.vx;
      p.y += p.vy;
      p.vx *= 0.99;
      p.vy *= 0.99;

      if (p.x < 0) p.x = canvas.width;
      if (p.x > canvas.width) p.x = 0;
      if (p.y < 0) p.y = canvas.height;
      if (p.y > canvas.height) p.y = 0;

      ctx.fillStyle = 'rgba(' + accentColor + ', ' + p.alpha + ')';
      ctx.beginPath();
      ctx.arc(p.x, p.y, p.r, 0, Math.PI * 2);
      ctx.fill();
    }

    raf = requestAnimationFrame(draw);
  }

  if (!window.matchMedia('(prefers-reduced-motion: reduce)').matches) {
    resize();
    createParticles();
    draw();

    window.addEventListener('resize', function() {
      isMobile = window.innerWidth < 810;
      particleCount = isMobile ? 30 : 60;
      connectionDist = isMobile ? 100 : 150;
      resize();
      createParticles();
    });

    if (!isMobile) {
      canvas.parentElement.addEventListener('mousemove', function(e) {
        var rect = canvas.getBoundingClientRect();
        mouse.x = e.clientX - rect.left;
        mouse.y = e.clientY - rect.top;
      });
      canvas.parentElement.addEventListener('mouseleave', function() {
        mouse.x = -1000;
        mouse.y = -1000;
      });
    }

    /* Pause when off-screen for performance */
    var heroObs = new IntersectionObserver(function(entries) {
      if (entries[0].isIntersecting) {
        if (!raf) draw();
      } else {
        if (raf) { cancelAnimationFrame(raf); raf = null; }
      }
    }, { threshold: 0 });
    heroObs.observe(canvas.parentElement);
  }
})();
```

**Mobile:** 30 particles (vs 60 desktop). No mouse interaction. Same visual effect, half the cost.

---

### Effect 5: Gradient Shimmer Text

**What:** Key words/phrases shimmer with a moving gradient. Draws the eye to important text.
**Performance:** Minimal. CSS-only.
**Where to use:** Hero headline key phrase, section headline accent word, CTA headline.

```css
.shimmer-text {
  background: linear-gradient(
    90deg,
    var(--white) 0%,
    var(--accent) 25%,
    var(--gold) 50%,
    var(--accent) 75%,
    var(--white) 100%
  );
  background-size: 200% 100%;
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: shimmer 6s ease-in-out infinite;
}

@keyframes shimmer {
  0%, 100% { background-position: 0% center; }
  50%      { background-position: 100% center; }
}
```

**Usage:** Wrap key phrases in `<span class="shimmer-text">$120K in a Month</span>`. Use sparingly, max 3-4 instances per page.

---

### Effect 6: Glassmorphism Cards

**What:** Frosted glass effect on cards and surfaces. Depth and premium feel.
**Performance:** Medium. Backdrop-filter is GPU-accelerated but can be expensive with many elements.
**Where to use:** Metric cards, feature cards, navigation bar.

```css
.glass-card {
  background: linear-gradient(
    135deg,
    rgba(255, 255, 255, 0.06) 0%,
    rgba(255, 255, 255, 0.02) 100%
  );
  backdrop-filter: blur(10px) saturate(150%);
  -webkit-backdrop-filter: blur(10px) saturate(150%);
  border: 1px solid rgba(255, 255, 255, 0.08);
  border-radius: 20px;
  box-shadow:
    0 8px 32px rgba(0, 0, 0, 0.3),
    inset 0 1px 0 rgba(255, 255, 255, 0.05);
}

/* Color-tinted variants */
.glass-accent {
  background: rgba(var(--accent-rgb), 0.08);
  border-color: rgba(var(--accent-rgb), 0.15);
}

/* Fallback */
@supports not (backdrop-filter: blur(10px)) {
  .glass-card {
    background: rgba(15, 23, 42, 0.95);
  }
}
```

**Rules:**
- Max 2-3 glassmorphic elements per viewport
- Reduce blur to 6-8px on mobile
- Never animate the backdrop-filter property itself
- Always include `-webkit-backdrop-filter` for Safari

---

### Effect 7: Animated Gradient Borders

**What:** Card borders that glow/rotate with gradient colors on hover.
**Performance:** Low. CSS-only.
**Where to use:** Feature cards, qualification cards, testimonial cards.

**Method A: Spinning conic gradient (hover-triggered)**
```css
.glow-card {
  position: relative;
  overflow: hidden;
}

.glow-card::after {
  content: '';
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: conic-gradient(from 0deg, transparent 0%, transparent 70%, rgba(var(--accent-rgb), 0.06) 85%, transparent 100%);
  opacity: 0;
  transition: opacity 0.5s;
  animation: cardGlowSpin 8s linear infinite;
}

.glow-card:hover::after { opacity: 1; }

@keyframes cardGlowSpin {
  to { transform: rotate(360deg); }
}
```

**Method B: @property spinning border (always-on)**
```css
@property --border-angle {
  inherits: false;
  initial-value: 0deg;
  syntax: "<angle>";
}

.rainbow-border {
  background:
    linear-gradient(var(--bg), var(--bg)) padding-box,
    conic-gradient(from var(--border-angle), var(--accent), var(--gold), var(--accent)) border-box;
  border: 2px solid transparent;
  border-radius: 16px;
  animation: borderSpin 3s linear infinite;
}

@keyframes borderSpin {
  to { --border-angle: 360deg; }
}
```

**Method C: Static gradient border (no animation, lightest)**
```css
.gradient-border {
  border: 2px solid transparent;
  background:
    linear-gradient(var(--bg), var(--bg)) padding-box,
    linear-gradient(135deg, var(--accent), transparent, var(--gold)) border-box;
  border-radius: 16px;
}
```

**Mobile:** Use Method A (hover-triggered) or Method C. Disable always-on spinning on mobile.

---

### Effect 8: Staggered Scroll Reveals

**What:** Elements fade/slide in as they enter the viewport. Grid children cascade in sequence.
**Performance:** Minimal. IntersectionObserver + CSS transitions.
**Where to use:** Every section. Grid cards, headings, body text.

```css
.reveal {
  opacity: 0;
  transform: translateY(30px);
  transition: opacity 0.7s ease, transform 0.7s ease;
}

.reveal.visible {
  opacity: 1;
  transform: translateY(0);
}

/* Stagger delays for grid children */
.reveal-delay-1 { transition-delay: 0.1s; }
.reveal-delay-2 { transition-delay: 0.2s; }
.reveal-delay-3 { transition-delay: 0.3s; }
.reveal-delay-4 { transition-delay: 0.4s; }
```

```javascript
var reveals = document.querySelectorAll('.reveal');
var observer = new IntersectionObserver(function(entries) {
  entries.forEach(function(entry) {
    if (entry.isIntersecting) {
      entry.target.classList.add('visible');
      observer.unobserve(entry.target);
    }
  });
}, { threshold: 0.1, rootMargin: '0px 0px -40px 0px' });
reveals.forEach(function(el) { observer.observe(el); });
```

**Stagger pattern:** In grids (3-col feature cards, 2-col results), add `reveal-delay-1`, `reveal-delay-2`, `reveal-delay-3` to successive children for cascade effect.

---

### Effect 9: Animated Metric Counters

**What:** Numbers count up from 0 when scrolled into view. Makes data feel dynamic.
**Performance:** Minimal. JS animation with requestAnimationFrame.
**Where to use:** Metrics/stats sections, results sections.

```html
<div class="metric-number" data-count="120" data-prefix="$" data-suffix="K+">$0</div>
```

```javascript
(function() {
  var counted = false;
  var counters = document.querySelectorAll('[data-count]');

  function animateCounters() {
    if (counted) return;
    counted = true;
    counters.forEach(function(el) {
      var target = parseFloat(el.getAttribute('data-count'));
      var prefix = el.getAttribute('data-prefix') || '';
      var suffix = el.getAttribute('data-suffix') || '';
      var isDecimal = target % 1 !== 0;
      var duration = 2000;
      var start = performance.now();

      function easeOut(t) { return 1 - Math.pow(1 - t, 3); }

      function step(now) {
        var elapsed = now - start;
        var progress = Math.min(elapsed / duration, 1);
        var current = easeOut(progress) * target;

        if (target >= 1000) {
          el.textContent = prefix + Math.floor(current).toLocaleString() + suffix;
        } else if (isDecimal) {
          el.textContent = prefix + current.toFixed(1) + suffix;
        } else {
          el.textContent = prefix + Math.floor(current) + suffix;
        }

        if (progress < 1) requestAnimationFrame(step);
      }

      requestAnimationFrame(step);
    });
  }

  if (counters.length) {
    var obs = new IntersectionObserver(function(entries) {
      entries.forEach(function(entry) {
        if (entry.isIntersecting) { animateCounters(); obs.disconnect(); }
      });
    }, { threshold: 0.3 });
    obs.observe(counters[0].closest('section'));
  }
})();
```

---

### Effect 10: Section Dividers

**What:** Gradient lines between sections. Replaces plain borders.
**Performance:** Minimal. Single div.
**Where to use:** Between every major section.

```css
.section-divider {
  height: 1px;
  background: linear-gradient(90deg, transparent, rgba(var(--accent-rgb), 0.2), rgba(var(--gold-rgb), 0.1), transparent);
  margin: 0;
}
```

---

### Effect 11: Card Hover Glow

**What:** Cards lift up and get a subtle radial glow on hover.
**Performance:** Minimal. CSS transitions.
**Where to use:** Any card element.

```css
.hover-glow {
  transition: transform 0.3s, border-color 0.4s, box-shadow 0.4s;
  position: relative;
  overflow: hidden;
}

.hover-glow:hover {
  transform: translateY(-4px);
  border-color: rgba(var(--accent-rgb), 0.25);
  box-shadow: 0 20px 60px rgba(var(--accent-rgb), 0.08);
}

/* Inner radial glow */
.hover-glow::before {
  content: '';
  position: absolute;
  inset: 0;
  border-radius: inherit;
  background: radial-gradient(circle at 50% 0%, rgba(var(--accent-rgb), 0.06) 0%, transparent 70%);
  opacity: 0;
  transition: opacity 0.4s;
}

.hover-glow:hover::before { opacity: 1; }
```

---

### Effect 12: Process Step Pulse Rings

**What:** Step numbers with pulsing outer ring. Shows progression/energy.
**Performance:** Minimal. CSS animation.
**Where to use:** Numbered process/step sections.

```css
.step-number {
  position: relative;
  width: 56px;
  height: 56px;
  border-radius: 50%;
  border: 2px solid var(--accent);
  display: flex;
  align-items: center;
  justify-content: center;
  background: var(--bg);
  z-index: 1;
}

.step-number::after {
  content: '';
  position: absolute;
  inset: -6px;
  border-radius: 50%;
  border: 1px solid rgba(var(--accent-rgb), 0.2);
  animation: stepPulse 3s ease-in-out infinite;
}

@keyframes stepPulse {
  0%, 100% { opacity: 0; transform: scale(1); }
  50%      { opacity: 1; transform: scale(1.15); }
}

/* Stagger the pulses */
.step:nth-child(2) .step-number::after { animation-delay: 0.5s; }
.step:nth-child(3) .step-number::after { animation-delay: 1s; }
```

---

### Effect 13: Animated Photo/Image Border

**What:** Gradient border on images that fades in and out.
**Performance:** Minimal. CSS animation.
**Where to use:** Founder photos, product images, testimonial headshots.

```css
.image-frame::after {
  content: '';
  position: absolute;
  inset: -2px;
  border-radius: 26px;
  border: 2px solid transparent;
  background: linear-gradient(135deg, rgba(var(--accent-rgb), 0.3), transparent, rgba(var(--gold-rgb), 0.2)) border-box;
  -webkit-mask: linear-gradient(#fff 0 0) padding-box, linear-gradient(#fff 0 0);
  mask: linear-gradient(#fff 0 0) padding-box, linear-gradient(#fff 0 0);
  -webkit-mask-composite: xor;
  mask-composite: exclude;
  pointer-events: none;
  animation: borderFade 6s ease-in-out infinite;
}

@keyframes borderFade {
  0%, 100% { opacity: 0.5; }
  50%      { opacity: 1; }
}
```

---

### Effect 14: CTA Button Pulse

**What:** Call-to-action buttons with pulsing glow shadow. Draws attention.
**Performance:** Minimal. CSS animation.
**Where to use:** Primary CTA buttons (hero, final CTA).

```css
.btn-pulse {
  animation: ctaPulse 2.5s infinite ease-in-out;
}

@keyframes ctaPulse {
  0%, 100% { box-shadow: 0 0 30px rgba(var(--accent-rgb), 0.25); }
  50%      { box-shadow: 0 0 55px rgba(var(--accent-rgb), 0.45); }
}
```

---

### Effect 15: Step Connector Lines

**What:** Horizontal line connecting step numbers in process sections.
**Performance:** Minimal. CSS pseudo-element.
**Where to use:** 3-step process sections.

```css
.steps {
  position: relative;
}

.steps::before {
  content: '';
  position: absolute;
  top: 28px; /* Center of step-number */
  left: calc(16.66% + 28px);
  right: calc(16.66% + 28px);
  height: 2px;
  background: linear-gradient(90deg, var(--accent), rgba(var(--accent-rgb), 0.2), var(--accent));
  opacity: 0.3;
}

/* Hide on mobile (stacked layout) */
@media (max-width: 810px) {
  .steps::before { display: none; }
}
```

---

### Effect 16: Glitch Text

**What:** RGB-split glitch effect on text. Aggressive, cyberpunk aesthetic.
**Performance:** Low. CSS pseudo-elements.
**Where to use:** Hero headlines (sparingly), error states, edgy brands.

```html
<h1 class="glitch" data-text="BLOCKCHAIN">BLOCKCHAIN</h1>
```

```css
.glitch {
  position: relative;
  font-family: var(--font-heading);
}

.glitch::before,
.glitch::after {
  content: attr(data-text);
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.glitch::before {
  color: #00f5ff;
  animation: glitchCyan 3s infinite linear alternate-reverse;
  clip-path: inset(0 0 0 0);
}

.glitch::after {
  color: #ff006e;
  animation: glitchPink 2s infinite linear alternate-reverse;
  clip-path: inset(0 0 0 0);
}

@keyframes glitchCyan {
  0%   { clip-path: inset(40% 0 61% 0); transform: translate(-3px, -1px); }
  20%  { clip-path: inset(92% 0 1% 0);  transform: translate(2px, 1px); }
  40%  { clip-path: inset(43% 0 1% 0);  transform: translate(-1px, 3px); }
  60%  { clip-path: inset(25% 0 58% 0);  transform: translate(3px, -2px); }
  80%  { clip-path: inset(54% 0 7% 0);  transform: translate(-2px, 1px); }
  100% { clip-path: inset(58% 0 43% 0);  transform: translate(1px, -3px); }
}

@keyframes glitchPink {
  0%   { clip-path: inset(65% 0 13% 0);  transform: translate(3px, 2px); }
  20%  { clip-path: inset(15% 0 72% 0);  transform: translate(-1px, -3px); }
  40%  { clip-path: inset(82% 0 2% 0);   transform: translate(2px, 1px); }
  60%  { clip-path: inset(5% 0 86% 0);   transform: translate(-3px, 2px); }
  80%  { clip-path: inset(41% 0 33% 0);  transform: translate(1px, -1px); }
  100% { clip-path: inset(72% 0 11% 0);  transform: translate(-2px, 3px); }
}
```

**Use sparingly.** This is a statement effect, not a page-wide treatment.

---

### Effect 17: Aurora/Northern Lights Background

**What:** Colorful light sources that drift across the background. Immersive, ambient.
**Performance:** Medium. Transform-only variant is GPU-accelerated.
**Where to use:** Hero section, full-page background.

```css
.aurora {
  position: relative;
  overflow: hidden;
}

.aurora::before {
  content: '';
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background:
    radial-gradient(ellipse at 20% 50%, rgba(var(--accent-rgb), 0.3) 0%, transparent 50%),
    radial-gradient(ellipse at 80% 50%, rgba(0, 245, 255, 0.2) 0%, transparent 50%),
    radial-gradient(ellipse at 50% 80%, rgba(57, 255, 20, 0.15) 0%, transparent 50%);
  animation: auroraDrift 30s ease-in-out infinite;
  will-change: transform;
}

@keyframes auroraDrift {
  0%, 100% { transform: rotate(0deg) scale(1); }
  33%      { transform: rotate(10deg) scale(1.1); }
  66%      { transform: rotate(-5deg) scale(0.95); }
}
```

---

### Effect 18: Typewriter/Terminal Text

**What:** Text types out character by character. Terminal/hacker aesthetic.
**Performance:** Minimal.
**Where to use:** Eyebrow text, status lines, loading states.

**CSS-only (single line):**
```css
.typewriter {
  overflow: hidden;
  border-right: 0.15em solid var(--accent);
  white-space: nowrap;
  font-family: var(--font-mono);
  color: var(--accent);
  animation:
    typing 3.5s steps(40, end),
    blink-caret 0.75s step-end infinite;
}

@keyframes typing {
  from { width: 0; }
  to   { width: 100%; }
}

@keyframes blink-caret {
  from, to { border-color: transparent; }
  50%      { border-color: var(--accent); }
}
```

**JS multi-line (looping):**
```javascript
class Typewriter {
  constructor(el, options) {
    this.el = el;
    this.strings = options.strings || ['Default text'];
    this.typeSpeed = options.typeSpeed || 80;
    this.deleteSpeed = options.deleteSpeed || 40;
    this.pauseBetween = options.pauseBetween || 2000;
    this.currentString = 0;
    this.currentChar = 0;
    this.isDeleting = false;
    this.tick();
  }

  tick() {
    var current = this.strings[this.currentString];
    if (this.isDeleting) {
      this.currentChar--;
    } else {
      this.currentChar++;
    }
    this.el.textContent = current.substring(0, this.currentChar);

    var delay = this.isDeleting ? this.deleteSpeed : this.typeSpeed;
    if (!this.isDeleting && this.currentChar === current.length) {
      delay = this.pauseBetween;
      this.isDeleting = true;
    }
    if (this.isDeleting && this.currentChar === 0) {
      this.isDeleting = false;
      this.currentString = (this.currentString + 1) % this.strings.length;
      delay = 500;
    }

    var self = this;
    setTimeout(function() { self.tick(); }, delay);
  }
}
```

---

### Effect 19: Morphing Blob Shapes

**What:** Organic blob that continuously morphs. Background decoration.
**Performance:** Low. CSS border-radius animation.
**Where to use:** Behind founder photo, behind CTA, decorative accent.

```css
.blob {
  width: 300px;
  height: 300px;
  background: linear-gradient(135deg, var(--accent), var(--gold));
  animation: blobMorph 8s ease-in-out infinite alternate;
  opacity: 0.15;
}

@keyframes blobMorph {
  0%   { border-radius: 63% 37% 54% 46% / 55% 48% 52% 45%; }
  14%  { border-radius: 40% 60% 54% 46% / 49% 60% 40% 51%; }
  28%  { border-radius: 54% 46% 38% 62% / 49% 70% 30% 51%; }
  42%  { border-radius: 61% 39% 55% 45% / 61% 38% 62% 39%; }
  56%  { border-radius: 61% 39% 67% 33% / 70% 50% 50% 30%; }
  70%  { border-radius: 50% 50% 34% 66% / 56% 68% 32% 44%; }
  84%  { border-radius: 46% 54% 50% 50% / 35% 61% 39% 65%; }
  100% { border-radius: 63% 37% 54% 46% / 55% 48% 52% 45%; }
}
```

---

### Effect 20: Animated Grid Background

**What:** Perspective grid that scrolls infinitely. Synthwave/retro-futuristic.
**Performance:** Low. CSS background animation.
**Where to use:** Hero background, CTA section background.

**Flat scrolling grid:**
```css
.grid-bg::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image:
    linear-gradient(to right, rgba(var(--accent-rgb), 0.1) 1px, transparent 0),
    linear-gradient(to bottom, rgba(var(--accent-rgb), 0.1) 1px, transparent 0);
  background-size: 60px 60px;
  animation: gridScroll 15s linear infinite;
}

@keyframes gridScroll {
  0%   { transform: translateY(0); }
  100% { transform: translateY(60px); }
}
```

**Perspective grid (synthwave floor):**
```css
.retro-grid {
  position: absolute;
  bottom: 0;
  left: -50%;
  width: 200%;
  height: 60%;
  background-image:
    linear-gradient(to right, rgba(var(--accent-rgb), 0.4) 1px, transparent 0),
    linear-gradient(to bottom, rgba(var(--accent-rgb), 0.4) 1px, transparent 0);
  background-size: 60px 40px;
  transform: perspective(200px) rotateX(50deg);
  transform-origin: bottom center;
  animation: retro-scroll 4s linear infinite;
}

@keyframes retro-scroll {
  0%   { background-position-y: 0; }
  100% { background-position-y: 40px; }
}
```

---

### Effect 21: 3D Tilt Cards

**What:** Cards that tilt toward the mouse cursor with glare overlay. Premium interactive feel.
**Performance:** Low-medium. JS mousemove + CSS transforms.
**Where to use:** Feature cards, pricing cards, testimonial cards. Desktop only.

```css
.tilt-wrapper { perspective: 800px; }

.tilt-card {
  transition: transform 0.1s ease-out;
  transform-style: preserve-3d;
  will-change: transform;
  position: relative;
}

.tilt-card::after {
  content: '';
  position: absolute;
  inset: 0;
  border-radius: inherit;
  pointer-events: none;
  background: radial-gradient(
    circle at var(--x, 50%) var(--y, 50%),
    rgba(255, 255, 255, 0.12) 0%,
    transparent 60%
  );
  opacity: 0;
  transition: opacity 0.3s;
}

.tilt-card:hover::after { opacity: 1; }
```

```javascript
document.querySelectorAll('.tilt-card').forEach(function(card) {
  card.addEventListener('mousemove', function(e) {
    var rect = card.getBoundingClientRect();
    var x = e.clientX - rect.left;
    var y = e.clientY - rect.top;
    var centerX = rect.width / 2;
    var centerY = rect.height / 2;
    var rotateX = ((y - centerY) / centerY) * -10;
    var rotateY = ((x - centerX) / centerX) * 10;

    card.style.transform = 'rotateX(' + rotateX + 'deg) rotateY(' + rotateY + 'deg) scale(1.03)';
    card.style.setProperty('--x', (x / rect.width * 100) + '%');
    card.style.setProperty('--y', (y / rect.height * 100) + '%');
  });

  card.addEventListener('mouseleave', function() {
    card.style.transform = 'rotateX(0deg) rotateY(0deg) scale(1)';
  });
});
```

**Mobile:** Disable tilt (no mousemove). The cards still look good static.

---

### Effect 22: Spotlight/Mouse-Follow Glow

**What:** A soft radial glow that follows the cursor across a card grid. Desktop only.
**Performance:** Low. CSS custom properties + JS mousemove.
**Where to use:** Card grid containers, hero backgrounds.

```css
.spotlight-grid {
  position: relative;
}

.spotlight-grid::before {
  content: '';
  position: absolute;
  inset: 0;
  pointer-events: none;
  background: radial-gradient(
    600px circle at var(--mouse-x, 50%) var(--mouse-y, 50%),
    rgba(var(--accent-rgb), 0.06),
    transparent 40%
  );
  opacity: 0;
  transition: opacity 0.3s;
}

.spotlight-grid:hover::before { opacity: 1; }
```

```javascript
document.querySelectorAll('.spotlight-grid').forEach(function(grid) {
  grid.addEventListener('mousemove', function(e) {
    var rect = grid.getBoundingClientRect();
    grid.style.setProperty('--mouse-x', (e.clientX - rect.left) + 'px');
    grid.style.setProperty('--mouse-y', (e.clientY - rect.top) + 'px');
  });
});
```

---

### Effect 23: Scroll-Triggered SVG Path Drawing

**What:** SVG lines that draw themselves as you scroll. Great for timelines and process flows.
**Performance:** Low. IntersectionObserver + CSS transition.
**Where to use:** Process steps, timeline sections.

```css
.draw-path {
  stroke-dasharray: 1000;
  stroke-dashoffset: 1000;
  transition: stroke-dashoffset 2s ease-in-out;
}

.draw-path.visible {
  stroke-dashoffset: 0;
}
```

```javascript
var paths = document.querySelectorAll('.draw-path');
paths.forEach(function(path) {
  var len = path.getTotalLength();
  path.style.strokeDasharray = len;
  path.style.strokeDashoffset = len;
});

var pathObs = new IntersectionObserver(function(entries) {
  entries.forEach(function(entry) {
    if (entry.isIntersecting) {
      entry.target.style.strokeDashoffset = '0';
      pathObs.unobserve(entry.target);
    }
  });
}, { threshold: 0.3 });

paths.forEach(function(p) { pathObs.observe(p); });
```

---

## Effect Tiers

Not every page needs every effect. Choose a tier based on the project.

### Tier 1: Clean Premium (5 effects)
Best for: professional services, B2B, finance, coaching.
- Noise overlay
- Staggered scroll reveals
- Gradient section dividers
- Card hover glow
- CTA button pulse

### Tier 2: Web3 Standard (10 effects)
Best for: agencies, trading education, SaaS, growth companies.
- Everything in Tier 1, plus:
- Animated mesh gradient (hero)
- Floating glow orbs
- Shimmer text (2-3 instances)
- Animated counters
- Glassmorphism cards

### Tier 3: Full Web3 (15+ effects)
Best for: crypto, DeFi, NFT, metaverse, gaming, bold brands.
- Everything in Tier 2, plus:
- Particle network canvas
- Animated gradient borders
- 3D tilt cards
- Spotlight mouse-follow
- Process step pulse rings
- Aurora background (optional)
- Glitch text (optional, use sparingly)

---

## Performance Rules (Always Apply)

### GPU-Accelerated Properties Only
```
SAFE TO ANIMATE (compositor thread, 60fps):
  - transform (translate, rotate, scale, skew)
  - opacity
  - filter (most browsers)

AVOID ANIMATING (triggers repaint):
  - background-color
  - box-shadow
  - border-radius
  - clip-path

NEVER ANIMATE (triggers layout):
  - width, height
  - margin, padding
  - top, left, right, bottom
  - font-size
```

### Mobile Optimization Checklist
1. Reduce particle count (60 to 30)
2. Reduce backdrop-filter blur (10-20px to 6-8px)
3. Disable mouse-follow effects (tilt cards, spotlight, magnetic buttons)
4. Disable always-on spinning animations (animated borders)
5. Reduce orb sizes (500px to 300px)
6. Slow down animation durations (less CPU)
7. Use `{ passive: true }` on all scroll listeners
8. Hide connector lines in stacked layouts

### Accessibility (Required)
```css
@media (prefers-reduced-motion: reduce) {
  *, *::before, *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }

  .reveal {
    opacity: 1;
    transform: none;
  }

  .shimmer-text {
    -webkit-text-fill-color: var(--white);
  }

  #particles-canvas { display: none; }
}
```

### Canvas Performance
- Cap `devicePixelRatio` at 2: `Math.min(window.devicePixelRatio, 2)`
- Pause canvas with IntersectionObserver when off-screen
- Use `requestAnimationFrame`, never `setInterval`
- Keep particle count under 80 desktop, 30 mobile

### CSS Containment
```css
.animated-section {
  contain: layout style paint;
}
```

---

## Enhancement Workflow (Mode 1)

When enhancing an existing page:

1. **Read the full page** to understand structure, content, and existing styles
2. **Identify the palette** - match the existing color scheme to the closest palette above, or extract exact values
3. **Pick the effect tier** based on the brand/audience
4. **Layer effects in this order:**
   a. Noise overlay (body::before)
   b. Scroll reveals (add .reveal classes to existing elements)
   c. Section dividers (add between sections)
   d. Hero background effects (mesh gradient, particles)
   e. Card enhancements (glassmorphism, hover glow, animated borders)
   f. Text effects (shimmer on key phrases)
   g. Interactive effects (counters, tilt cards, spotlight)
   h. CTA enhancements (button pulse)
5. **Add mobile rules** - reduce/disable heavy effects under 810px
6. **Add prefers-reduced-motion** - required, non-negotiable
7. **Test** - check that all content is still readable, CTAs still visible, scroll is smooth

**Do not change any copy, structure, or content.** Only layer visual effects.

---

## Full Build Workflow (Mode 2)

When building from scratch:

1. **Get client palette** - choose or customize from the 5 palettes above
2. **Set typography** - pick heading/body/mono fonts
3. **Choose effect tier** based on brand positioning
4. **Build the page structure first** (HTML + basic CSS) with no effects
5. **Layer effects** following the same order as Enhancement Workflow
6. **Add all performance optimizations** from the Performance Rules section
7. **Test on mobile** and verify Lighthouse score

---

## How this skill connects to others

**direct-response-copy + web3-design:**
Write the copy first, then apply web3 design treatment. Copy drives structure; design enhances it.

**landing-page + web3-design:**
Landing page skill creates the content strategy and structure. Web3-design applies the visual layer.

**brand-voice + web3-design:**
Brand voice determines which palette and effect tier to use. Edgy brands get Tier 3. Professional brands get Tier 1.

**ai-creative-strategist + web3-design:**
Creative strategist defines the visual direction. Web3-design executes it.

---

## The test

Before delivering any web3-enhanced page, verify:

1. **Mobile responsive** - all grids collapse, type scales down, effects reduced
2. **prefers-reduced-motion** - all animations disabled, content visible
3. **Performance** - no jank on scroll, particles pause off-screen, Lighthouse 90+
4. **Readability** - all text still readable over animated backgrounds
5. **CTAs visible** - buttons not obscured by effects, still prominent
6. **No layout shift** - animations don't cause content to jump
7. **Cross-browser** - backdrop-filter has -webkit- prefix, fallbacks in place
8. **Copy unchanged** - design enhancement did not alter any content

---

## Reference Material

Full technical reference with extended code examples:
`.tmp/web3-design-patterns-reference.md`

External tools:
- Mesher (mesh gradients): https://csshero.org/mesher/
- CSS.glass (glassmorphism): https://css.glass/
- nnnoise (grain textures): https://www.fffuel.co/nnnoise/
- Haikei (SVG shapes): https://haikei.app/
- Gradient Animator: https://www.gradient-animator.com/

Libraries (when zero-dependency isn't enough):
- GSAP + ScrollTrigger (24kb) - complex scroll animations
- vanilla-tilt.js - 3D card tilt
- Three.js / React Three Fiber - full 3D scenes
- Lenis (5kb) - smooth scroll
