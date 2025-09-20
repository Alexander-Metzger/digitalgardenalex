---
{"dg-publish":true,"permalink":"/about-me/metzger-studio/","tags":["gardenEntry"],"noteIcon":""}
---


<!-- CSS MUSS vor dem Markup stehen -->
<style>
/* Scope: nur innerhalb #cosmic anwenden */
#cosmic{ --bg:#0f0f11; --fg:#eaeaea; --muted:#c9c9c9;
  --chip:#1c1c1f; --chip-bd:#2a2a2e;
  --banner:#d9d9d9; --banner-fg:#121214;
  --btn:#18181b; --btn-bd:#32323a;
  --accent:#cdcdcd; --accent-bd:#5f5f6a;
  --violet-1:#a78bfa; --violet-2:#8b5cf6; --violet-3:#6d28d9; --violet-ink:#bfa7ff;
  color:var(--fg);
}


#cosmic{
  background:
    radial-gradient(1000px 600px at 12% 8%, rgba(139,92,246,.10), transparent 60%),
    radial-gradient(900px 540px at 88% 12%, rgba(109,40,217,.10), transparent 60%),
    radial-gradient(700px 420px at 50% 100%, rgba(167,139,250,.08), transparent 60%),
    var(--bg);
  background-blend-mode: screen, screen, screen, normal;
  border-radius:14px;
  box-shadow:
    0 0 0 1px rgba(139,92,246,.35),
    0 0 28px rgba(139,92,246,.18),
    inset 0 0 120px rgba(109,40,217,.12);
  padding:32px 16px 48px;
}


#cosmic::after{
  content:""; position:relative; display:block; height:0; pointer-events:none;
  background:
    radial-gradient(2px 2px at 10% 20%, rgba(255,255,255,.12) 40%, transparent 42%),
    radial-gradient(1.6px 1.6px at 80% 30%, rgba(255,255,255,.10) 40%, transparent 42%),
    radial-gradient(1.8px 1.8px at 35% 75%, rgba(255,255,255,.10) 40%, transparent 42%),
    radial-gradient(1.4px 1.4px at 60% 60%, rgba(255,255,255,.08) 40%, transparent 42%);
  filter: blur(.2px); opacity:.35;
}


#cosmic .center-text{ text-align:center; width:100%; }
#cosmic h2.section{ margin:30px 0 12px; font-size:32px; font-weight:900; text-align:center; }
#cosmic p{ color:var(--muted); max-width:820px; margin:0 auto 10px; line-height:1.65; text-align:center; }
#cosmic a{ color:#d4d0ff; text-underline-offset:3px; }
#cosmic a:hover{ color:#efeaff; text-decoration:underline; }


#cosmic #hero-wrap{ max-width:1000px; margin:0 auto; text-align:center; }

#cosmic .nav-chips{ display:flex; gap:10px; justify-content:center; flex-wrap:wrap; margin:24px 0 22px; }
#cosmic .nav-chips a{
  display:inline-block; padding:6px 12px; font-weight:600;
  border:1px solid var(--chip-bd); background:var(--chip);
  color:var(--fg); border-radius:8px; text-decoration:none;
  box-shadow: 0 1px 0 rgba(255,255,255,.06) inset, 0 1px 0 rgba(0,0,0,.6);
  transition: border-color .2s, box-shadow .25s, color .2s, transform .08s;
}
#cosmic .nav-chips a:hover{
  border-color: rgba(139,92,246,.55); color: var(--violet-ink);
  box-shadow: 0 0 0 1px rgba(139,92,246,.25) inset, 0 8px 24px rgba(109,40,217,.25);
  transform: translateY(-1px);
}


#cosmic .banner{
  display:inline-block; background:var(--banner); color:var(--banner-fg);
  font-weight:900; letter-spacing:.3px; font-size: clamp(28px, 6vw, 54px);
  padding:10px 14px; border-radius:10px;
  box-shadow: 0 3px 0 rgba(0,0,0,.35), 0 0 0 2px rgba(139,92,246,.35), 0 8px 32px rgba(139,92,246,.20);
  outline: 1px solid rgba(139,92,246,.25);
}


#cosmic .subtitle{ margin:6px auto 28px; display:flex; gap:8px; justify-content:center; flex-wrap:wrap; }
#cosmic .subtitle .tag{
  background:#202024; color:#e4e1ff; border:1px solid #2e2a38;
  padding:4px 10px; border-radius:8px; font-size:14px;
  box-shadow: 0 0 0 1px rgba(139,92,246,.35) inset;
}

/* CTA */
#cosmic .cta{ margin:26px 0 36px; }
#cosmic .cta a{
  display:inline-block; padding:10px 18px; border-radius:10px;
  background:linear-gradient(180deg, #1a1a21 0%, #15151a 100%);
  border:1px solid var(--btn-bd); color:#f2efff; text-decoration:none; font-weight:700; letter-spacing:.2px;
  box-shadow: 0 2px 0 rgba(0,0,0,.6), 0 1px 0 rgba(255,255,255,.06) inset,
             0 0 0 1px rgba(139,92,246,.35), 0 10px 28px rgba(109,40,217,.28);
  transition: transform .08s, box-shadow .25s, filter .2s;
}
#cosmic .cta a:hover{ transform: translateY(-1px); filter: brightness(1.05); }

/* Badges */
#cosmic .badge-row{ margin:24px auto 4px; display:flex; gap:10px; justify-content:center; flex-wrap:wrap; }
#cosmic .badge{
  height:34px; min-width:120px; padding:0 10px; display:flex; align-items:center; justify-content:center;
  background:#0f0f12; border:1px solid var(--accent-bd); border-radius:10px; color:var(--accent); font-weight:700; font-size:13px;
  box-shadow: 0 0 0 1px rgba(139,92,246,.28), 0 6px 20px rgba(109,40,217,.18);
}

/* weniger Bewegung falls gewünscht */
@media (prefers-reduced-motion: reduce){
  #cosmic .nav-chips a, #cosmic .cta a{ transition:none; }
}
</style>

<div id="cosmic">
  <div id="hero-wrap">
    <div class="banner center-text">Der Metzger ©</div>

 <nav class="bubble-grid" aria-label="Primary">
  <a href="/about/Motives" class="bubble">
    <div class="bubble-core">👤</div>
    <span class="label">About Me</span>
  </a>

  <a href="/books/recommendations" class="bubble">
    <div class="bubble-core">📚</div>
    <span class="label">Books</span>
  </a>

  <a href="/workouts/workouts/" class="bubble">
    <div class="bubble-core">💪</div>
    <span class="label">Workouts</span>
  </a>

  <a href="/philosophy/" class="bubble">
    <div class="bubble-core">🧠</div>
    <span class="label">Philosophy</span>
  </a>

  <a href="/sports-science/" class="bubble">
    <div class="bubble-core">🏋️‍♂️</div>
    <span class="label">Sports Science</span>
  </a>
  
  <a href="/Human Evolution Project/Daily Driver Protocol.md/" class="bubble">
    <div class="bubble-core">🧬</div>
    <span class="label">Biohacking</span>
  </a>
</nav>



   

    <h2 class="section">Who I am</h2>
    <p class="p"> I’m just another person on this earth trying to pass the time between birth and death somehow by doing silly stuff I care about. But until a stroke or a car I didn’t see coming gets me, I’ll try to learn a few things about the world. What I already learned is that an unexamined life is not worth living, and to get a few more examiners, I created this page.</p>

    <h2 class="section">What is to be done?</h2>
    <p class="p">
      Projects I’m currently working on:  
	An Elite Triathlon Training Plan based on clinical data and evidence
	A module-based protocol aiming for physical performance without sacrificing health
 Filling out all these empty links one day.<br/>
      
      E-Mail: <a href="mailto:butcherscontact.poach867@slmail.me">butcherscontact.poach867@slmail.me</a>
    </p>

    <div class="cta"><a href="https://downloadmoreram.com/">Download more RAM</a></div>

<div class="badge-row">
  <a href="https://grapheneos.org" class="badge-link">
    <img src="/img/grapheneos.gif" alt="GrapheneOS">
  </a>
  <a href="https://joinmastodon.org" class="badge-link">
    <img src="/img/fediverse.gif" alt="Mastodon / Fediverse">
  </a>
  <a href="/privacy" class="badge-link">
    <img src="/img/chrome-is-evil.gif" alt="Online Privacy">
  </a>
  <a href="https://www.getmonero.org/" class="badge-link">
    <img src="/img/google_stand.gif" alt="Monero">
  </a>
  <a href="https://www.gnu.org/gnu/linux-and-gnu.html" class="badge-link">
    <img src="/img/gnu-linux.gif" alt="GNU/Linux">
  </a>
  <a href="https://getfedora.org/" class="badge-link">
    <img src="/img/fedora.gif" alt="Fedora / Arch Linux">
  </a>
  <a href="https://nextcloud.com" class="badge-link">
    <img src="/img/nextcloud.gif" alt="Nextcloud">
  </a>
  <a href="https://en.wikipedia.org/wiki/Palestine" class="badge-link">
    <img src="/img/agplv3.gif" alt="Stand with Palestine">
  </a>
</div>

  </div>
</div>
