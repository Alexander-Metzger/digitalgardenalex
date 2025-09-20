---
{"dg-publish":true,"dg-permalink":"/","permalink":"/","title":"Alexander Metzger","tags":["gardenEntry"],"noteIcon":""}
---

<html></html>
<html>
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<style>
/* ===== Theme Tokens (Dark + Cosmic Violet) ===== */
:root{
  --bg:#0f0f11; --fg:#eaeaea; --muted:#c9c9c9;
  --chip:#1c1c1f; --chip-bd:#2a2a2e;
  --banner:#d9d9d9; --banner-fg:#121214;
  --btn:#18181b; --btn-bd:#32323a;
  --accent:#cdcdcd; --accent-bd:#5f5f6a;

  /* cosmic violet scale */
  --violet-1:#a78bfa;  /* light glow */
  --violet-2:#8b5cf6;  /* main */
  --violet-3:#6d28d9;  /* deep core */
  --violet-ink:#bfa7ff;
}

/* Obsidian preview/source surfaces */
.markdown-preview-view, .markdown-source-view{
  background:var(--bg) !important; color:var(--fg) !important;
  font-family: ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, Inter, Arial;
}

/* ===== Cosmic Background (super dezent, performant) ===== */
body{
  margin:0;
  background: radial-gradient(1000px 600px at 12% 8%, rgba(139,92,246,.10), transparent 60%),
              radial-gradient(900px 540px at 88% 12%, rgba(109,40,217,.10), transparent 60%),
              radial-gradient(700px 420px at 50% 100%, rgba(167,139,250,.08), transparent 60%),
              var(--bg);
  /* leichter „star noise“ via subtle repeating gradient */
  /* Tipp: ist extrem schwach, stört Text nicht */
  background-blend-mode: screen, screen, screen, normal;
}

/* mikro-Sterne: nur ein Hauch */
body::after{
  content:"";
  position:fixed; inset:0; pointer-events:none; z-index:0;
  background-image:
    radial-gradient(2px 2px at 10% 20%, rgba(255,255,255,.12) 40%, transparent 42%),
    radial-gradient(1.6px 1.6px at 80% 30%, rgba(255,255,255,.10) 40%, transparent 42%),
    radial-gradient(1.8px 1.8px at 35% 75%, rgba(255,255,255,.10) 40%, transparent 42%),
    radial-gradient(1.4px 1.4px at 60% 60%, rgba(255,255,255,.08) 40%, transparent 42%);
  filter: blur(.2px);
  opacity:.35;
}

/* ===== Layout ===== */
#hero-wrap{
  position:relative;
  max-width:1000px; margin:0 auto; padding:32px 16px 64px; text-align:center;
  z-index:1;
  /* cosmic ring */
  border-radius:14px;
  box-shadow:
    0 0 0 1px rgba(139,92,246,.35),
    0 0 28px rgba(139,92,246,.18),
    0 0 120px rgba(109,40,217,.12) inset;
}

/* ===== Nav Chips ===== */
.nav-chips{
  display:flex; gap:10px; justify-content:center; flex-wrap:wrap; margin:24px 0 22px;
}
.nav-chips a{
  display:inline-block; padding:6px 12px; font-weight:600;
  border:1px solid var(--chip-bd); background:var(--chip);
  color:var(--fg); border-radius:8px; text-decoration:none;
  box-shadow: 0 1px 0 rgba(255,255,255,.06) inset, 0 1px 0 rgba(0,0,0,.6);
  transition: border-color .2s ease, box-shadow .25s ease, color .2s ease, transform .08s ease;
}
.nav-chips a:hover{
  border-color: rgba(139,92,246,.55);
  color: var(--violet-ink);
  box-shadow:
    0 0 0 1px rgba(139,92,246,.25) inset,
    0 8px 24px rgba(109,40,217,.25);
  transform: translateY(-1px);
}
.nav-chips a:focus-visible{
  outline:none;
  box-shadow:
    0 0 0 2px rgba(255,255,255,.08) inset,
    0 0 0 3px rgba(139,92,246,.7);
  border-color: transparent;
}

/* ===== Banner / Title ===== */
.banner{
  display:inline-block;
  background:var(--banner); color:var(--banner-fg);
  font-weight:900; letter-spacing:.3px;
  font-size: clamp(28px, 6vw, 54px);
  padding:10px 14px; border-radius:10px;
  box-shadow: 0 3px 0 rgba(0,0,0,.35),
              0 0 0 2px rgba(139,92,246,.35),
              0 8px 32px rgba(139,92,246,.20);
  /* feine violette Kante */
  outline: 1px solid rgba(139,92,246,.25);
}

/* ===== Sub-Title Tags ===== */
.subtitle{
  margin:6px auto 28px; display:flex; gap:8px; justify-content:center; flex-wrap:wrap;
}
.subtitle .tag{
  background:#202024; color:#e4e1ff; border:1px solid #2e2a38;
  padding:4px 10px; border-radius:8px; font-size:14px;
  box-shadow: 0 0 0 1px rgba(139,92,246,.35) inset;
}

/* ===== Typography ===== */
h2.section{ margin:30px 0 12px; font-size:32px; font-weight:900; }
p{ color:var(--muted); max-width:820px; margin:0 auto 10px; line-height:1.65; }
a{ color:#d4d0ff; text-underline-offset:3px; }
a:hover{ color:#efeaff; text-decoration:underline; }

/* ===== CTA ===== */
.cta{ margin:26px 0 36px; }
.cta a{
  display:inline-block; padding:10px 18px; border-radius:10px;
  background:linear-gradient(180deg, #1a1a21 0%, #15151a 100%);
  border:1px solid var(--btn-bd);
  color:#f2efff; text-decoration:none; font-weight:700; letter-spacing:.2px;
  box-shadow:
    0 2px 0 rgba(0,0,0,.6),
    0 1px 0 rgba(255,255,255,.06) inset,
    0 0 0 1px rgba(139,92,246,.35),
    0 10px 28px rgba(109,40,217,.28);
  transition: transform .08s ease, box-shadow .25s ease, filter .2s ease;
}
.cta a:hover{ transform: translateY(-1px); filter: brightness(1.05); }
.cta a:focus-visible{
  outline:none;
  box-shadow:
    0 0 0 2px rgba(255,255,255,.06) inset,
    0 0 0 3px rgba(139,92,246,.7),
    0 10px 28px rgba(109,40,217,.35);
}

/* ===== Badges ===== */
.badge-row{
  margin:24px auto 4px; display:flex; gap:10px; justify-content:center; flex-wrap:wrap;
}
.badge{
  height:34px; min-width:120px; padding:0 10px;
  display:flex; align-items:center; justify-content:center;
  background:#0f0f12; border:1px solid var(--accent-bd);
  border-radius:10px; color:var(--accent); font-weight:700; font-size:13px;
  box-shadow: 0 0 0 1px rgba(139,92,246,.28), 0 6px 20px rgba(109,40,217,.18);
}

/* Wenn du echte Bild-Badges verwenden willst, ersetze .badge durch <img> mit class="badge-img" */
.badge-img{ height:36px; border-radius:8px; border:1px solid var(--accent-bd); background:#0f0f12; }

/* Utilities */
.center-text{ text-align:center; width:100%; }

/* Obsidian Preview alignments */
.markdown-preview-view h1, 
.markdown-preview-view h2, 
.markdown-preview-view p { text-align:center; }
.markdown-preview-view a { color:#d0d0ff; }

/* Reduce motion respect */
@media (prefers-reduced-motion: reduce){
  .nav-chips a, .cta a{ transition:none; }
  body::after{ display:none; }
}
</style>
</head>
<body>
<div id="hero-wrap">

  <div class="nav-chips center-text">
    <a href="/about/">About me</a>
    <a href="/books/">Book Recommendations</a>
    <a href="/workouts/">Workouts</a>
  </div>

  <div class="banner center-text">Alexander Metzger ©</div>

  <div class="subtitle">
    <span class="tag">Sports Science</span>
    <span class="tag">Philosophy</span>
    <span class="tag">Biohacking</span>
  </div>

  <h2 class="section">Who I am</h2>
  <p class="p">
     I'm Alex, I'm just another person on this earth trying to find some kind of meaning in my personal hyperfixations. Currently these are Pharmacology, Sports Science, Linux and Math.
     I've started publishing some of my projects and notes here, more to just leave a little digital fingerprint.
     <br/>
  </p>

  <h2 class="section">What I do</h2>
  <p class="p">
    Projects I'm currently working on: An Elite Triathlon Training Plan based on clinical data and evidence. <br/>
    E-Mail: <a href="mailto:alexander@metzger.studio">alexander@metzger.studio</a>
  </p>

  <div class="cta">
    <a href="/manifest.pdf">Download Manifest</a>
  </div>

  <!-- Badge-Reihe: Variante 1 – Text-Badges -->
  <div class="badge-row">
    <div class="badge">GrapheneOS</div>
    <div class="badge">Mastodon</div>
    <div class="badge">Online Privacy</div>
    <div class="badge">Monero</div>
    <div class="badge">GNU/Linux</div>
    <div class="badge">Arch</div>
    <div class="badge">Nextcloud</div>
    <div class="badge">Stand with Palestine</div>
  </div>
</div>
</body>
