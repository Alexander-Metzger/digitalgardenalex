---
{"dg-publish":true,"dg-permalink":"/","permalink":"/","title":"Alexander Metzger","tags":["gardenEntry"],"noteIcon":""}
---


<style>
:root{
  --bg:#111; --fg:#e9e9e9; --muted:#c9c9c9;
  --chip:#2a2a2a; --chip-bd:#3a3a3a;
  --banner:#d9d9d9; --banner-fg:#1a1a1a;
  --btn:#1f1f1f; --btn-bd:#414141;
  --accent:#c0c0c0; --accent-bd:#606060;
}
.markdown-preview-view, .markdown-source-view{
  background:var(--bg) !important; color:var(--fg) !important;
  font-family: ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, Inter, Arial;
}
#hero-wrap{
  max-width:1000px; margin:0 auto; padding:32px 16px 64px;
  text-align:center;
}
.nav-chips{
  display:flex; gap:10px; justify-content:center; flex-wrap:wrap; margin:24px 0 22px;
}
.nav-chips a{
  display:inline-block; padding:6px 12px; font-weight:600;
  border:1px solid var(--chip-bd); background:var(--chip);
  color:var(--fg); border-radius:6px; text-decoration:none;
  box-shadow: 0 1px 0 rgba(255,255,255,.06) inset, 0 1px 0 rgba(0,0,0,.6);
}
.banner{
  display:inline-block;
  background:var(--banner); color:var(--banner-fg);
  font-weight:900; letter-spacing:.3px;
  font-size: clamp(28px, 6vw, 54px);
  padding:10px 14px; border-radius:4px;
  box-shadow: 0 3px 0 rgba(0,0,0,.35);
}
.subtitle{
  margin:6px auto 28px; display:flex; gap:8px; justify-content:center; flex-wrap:wrap;
}
.subtitle .tag{
  background:#2b2b2b; color:#dcdcdc; border:1px solid #3d3d3d;
  padding:4px 10px; border-radius:4px; font-size:14px;
}
h2.section{ margin:30px 0 12px; font-size:32px; font-weight:900; }
.p{ color:var(--muted); max-width:820px; margin:0 auto 10px; }
.cta{
  margin:26px 0 36px;
}
.cta a{
  display:inline-block; padding:10px 18px; border-radius:6px;
  background:var(--btn); border:1px solid var(--btn-bd);
  color:#eaeaea; text-decoration:none; font-weight:600;
  box-shadow: 0 2px 0 rgba(0,0,0,.6), 0 1px 0 rgba(255,255,255,.06) inset;
}
.badge-row{
  margin:24px auto 4px; display:flex; gap:10px; justify-content:center; flex-wrap:wrap;
}
.badge{
  height:34px; min-width:120px; padding:0 10px;
  display:flex; align-items:center; justify-content:center;
  background:#0f0f0f; border:1px solid var(--accent-bd);
  border-radius:4px; color:var(--accent); font-weight:700; font-size:13px;
}
/* Wenn du echte Bild-Badges verwenden willst, ersetze .badge durch <img> mit class="badge-img" */
.badge-img{ height:36px; border-radius:4px; border:1px solid var(--accent-bd); background:#0f0f0f; }

/* Zentriertrick für Obsidian Edit & Preview */
.markdown-preview-view h1, 
.markdown-preview-view h2, 
.markdown-preview-view p { text-align:center; }
.markdown-preview-view a { color:#d0d0d0; }
</style>

<div id="hero-wrap">

  <div class="nav-chips">
    <a href="/about/">About me</a>
    <a href="/books/">Book Recommendations</a>
    <a href="/workouts/">Workouts</a>
  </div>

  <div class="banner">Alexander Metzger ©</div>

  <div class="subtitle">
    <span class="tag">Programmer</span>
    <span class="tag">Linux Enthusiast</span>
    <span class="tag">Middle Distance Runner</span>
  </div>

  <h2 class="section">Who I am</h2>
  <p class="p">
    I'm Alex, I write some code sometimes and I also enjoy <s>long distance</s> middle distance running and Free Software.
    <br/>I also try to get deeper into web development.
  </p>

  <h2 class="section">What I do</h2>
  <p class="p">
    I create Web 2.0 projects, I'm a privacy advocate and I am also into Linux. Feel free to contact me.<br/>
    E-Mail: <a href="mailto:alexander@metzger.studio">alexander@metzger.studio</a>
  </p>

  <div class="cta">
    <a href="/manifest.pdf">Download Manifest</a>
  </div>

  <!-- Badge-Reihe: Variante 1 – Text-Badges (sehen wie die Bild-Badges aus) -->
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

  <!-- Badge-Reihe: Variante 2 – echte Bild-Badges; ersetze src-Pfade durch deine Dateien
  <div class="badge-row">
    <img class="badge-img" src="/badges/grapheneos.png" alt="GrapheneOS"/>
    <img class="badge-img" src="/badges/mastodon.png" alt="Mastodon"/>
    <img class="badge-img" src="/badges/privacy.png" alt="Privacy"/>
    <img class="badge-img" src="/badges/monero.png" alt="Monero"/>
    <img class="badge-img" src="/badges/gnu-linux.png" alt="GNU/Linux"/>
    <img class="badge-img" src="/badges/arch.png" alt="Arch"/>
    <img class="badge-img" src="/badges/nextcloud.png" alt="Nextcloud"/>
    <img class="badge-img" src="/badges/stand-with-palestine.png" alt="Stand with Palestine"/>
  </div>
  -->

</div>
