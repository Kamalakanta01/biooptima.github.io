# <!DOCTYPE html>

# <html lang="en">

# <head>

# <meta charset="UTF-8">

# &#x20; <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=5.0">

# &#x20; <meta name="description" content="Evidence-based health interventions for cognitive enhancement, hormonal optimization, EDC reduction, and sleep improvement. Peer-reviewed research synthesis with personalized routine calculator.">

# &#x20; <title>BioOptima — Evidence-Based Cognitive \& Hormonal Research</title>

# <link rel="preconnect" href="https://fonts.googleapis.com">

# <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

# <link href="https://fonts.googleapis.com/css2?family=Libre+Baskerville:ital,wght@0,400;0,700;1,400\&family=Figtree:wght@300;400;500;600;700\&display=swap" rel="stylesheet">

# <style>

# /\* ─── TOKENS ─────────────────────────────────────────────── \*/

# :root {

# &#x20; --white:   #ffffff;

# &#x20; --off:     #f7f6f3;

# &#x20; --stone:   #f0ede8;

# &#x20; --border:  #e4e1da;

# &#x20; --border2: #ccc9c0;

# &#x20; --ink:     #1a1917;

# &#x20; --ink2:    #3d3b38;

# &#x20; --muted:   #6b6760;

# &#x20; --faint:   #9e9b96;

# 

# &#x20; --blue:    #1d4ed8;

# &#x20; --blue-l:  #eff4ff;

# &#x20; --blue-m:  #c7d8fc;

# 

# &#x20; --amber:   #b45309;

# &#x20; --amber-l: #fef8ec;

# &#x20; --amber-m: #fde9a2;

# 

# &#x20; --green:   #0f6e50;

# &#x20; --green-l: #ecfaf5;

# &#x20; --green-m: #a3e6cc;

# 

# &#x20; --rose:    #9d174d;

# &#x20; --rose-l:  #fdf2f8;

# &#x20; --rose-m:  #fbcfe8;

# 

# &#x20; --red:     #b91c1c;

# &#x20; --red-l:   #fff1f1;

# 

# &#x20; --r:  6px;

# &#x20; --r2: 10px;

# &#x20; --r3: 16px;

# 

# &#x20; --nav-h: 60px;

# &#x20; --max: 1140px;

# }

# 

# \*, \*::before, \*::after { box-sizing: border-box; margin: 0; padding: 0; }

# html { scroll-behavior: smooth; -webkit-text-size-adjust: 100%; }

# 

# body {

# &#x20; font-family: 'Figtree', sans-serif;

# &#x20; font-size: 15px;

# &#x20; line-height: 1.65;

# &#x20; color: var(--ink2);

# &#x20; background: var(--white);

# &#x20; overflow-x: hidden;

# }

# 

# /\* ─── SCROLL PROGRESS ────────────────────────────────────── \*/

# \#prog {

# &#x20; position: fixed; top: 0; left: 0; height: 3px; width: 0;

# &#x20; background: linear-gradient(90deg, var(--blue) 0%, var(--rose) 40%, var(--amber) 70%, var(--green) 100%);

# &#x20; z-index: 2000; transition: width 0.08s linear; pointer-events: none;

# }

# 

# /\* ─── NAV ────────────────────────────────────────────────── \*/

# .nav {

# &#x20; position: fixed; top: 0; left: 0; right: 0; z-index: 1000;

# &#x20; height: var(--nav-h);

# &#x20; background: rgba(255,255,255,0.94);

# &#x20; backdrop-filter: blur(16px);

# &#x20; -webkit-backdrop-filter: blur(16px);

# &#x20; border-bottom: 1px solid var(--border);

# &#x20; display: flex; align-items: center;

# }

# .nav-wrap {

# &#x20; max-width: var(--max); margin: 0 auto; width: 100%;

# &#x20; padding: 0 20px;

# &#x20; display: flex; align-items: center; gap: 24px;

# }

# .nav-logo {

# &#x20; font-family: 'Libre Baskerville', serif;

# &#x20; font-size: 1.05rem; font-weight: 700; color: var(--ink);

# &#x20; letter-spacing: -0.01em; white-space: nowrap; text-decoration: none;

# &#x20; flex-shrink: 0;

# }

# .nav-logo span { color: var(--blue); }

# 

# .nav-links {

# &#x20; display: flex; align-items: center; gap: 2px;

# &#x20; list-style: none; flex: 1; overflow-x: auto;

# &#x20; scrollbar-width: none; -ms-overflow-style: none;

# }

# .nav-links::-webkit-scrollbar { display: none; }

# .nav-links a {

# &#x20; padding: 5px 10px; border-radius: var(--r);

# &#x20; font-size: 0.78rem; font-weight: 500; color: var(--muted);

# &#x20; text-decoration: none; transition: color 0.15s, background 0.15s;

# &#x20; white-space: nowrap;

# }

# .nav-links a:hover { color: var(--ink); background: var(--stone); }

# .nav-links a.active { color: var(--blue); background: var(--blue-l); }

# 

# .nav-cta {

# &#x20; margin-left: auto; flex-shrink: 0;

# &#x20; padding: 7px 16px; border-radius: var(--r);

# &#x20; background: var(--blue); color: var(--white);

# &#x20; font-size: 0.78rem; font-weight: 600; text-decoration: none;

# &#x20; transition: opacity 0.15s; white-space: nowrap;

# }

# .nav-cta:hover { opacity: 0.85; }

# 

# .ham {

# &#x20; display: none; margin-left: auto; flex-direction: column;

# &#x20; gap: 5px; background: none; border: none; cursor: pointer;

# &#x20; padding: 8px; border-radius: var(--r); flex-shrink: 0;

# }

# .ham span {

# &#x20; display: block; width: 20px; height: 1.5px;

# &#x20; background: var(--ink); border-radius: 2px; transition: all 0.25s;

# }

# .ham.open span:nth-child(1) { transform: rotate(45deg) translate(4.5px,4.5px); }

# .ham.open span:nth-child(2) { opacity: 0; transform: scaleX(0); }

# .ham.open span:nth-child(3) { transform: rotate(-45deg) translate(4.5px,-4.5px); }

# 

# .mob-menu {

# &#x20; display: none; flex-direction: column; gap: 1px;

# &#x20; padding: 8px 16px 16px; background: var(--white);

# &#x20; border-bottom: 1px solid var(--border);

# &#x20; position: fixed; top: var(--nav-h); left: 0; right: 0;

# &#x20; z-index: 999; box-shadow: 0 8px 24px rgba(0,0,0,0.06);

# &#x20; max-height: calc(100vh - var(--nav-h)); overflow-y: auto;

# }

# .mob-menu.open { display: flex; }

# .mob-menu a {

# &#x20; padding: 12px 14px; border-radius: var(--r);

# &#x20; font-size: 0.9rem; font-weight: 500; color: var(--ink2);

# &#x20; text-decoration: none; transition: background 0.15s;

# }

# .mob-menu a:hover { background: var(--stone); }

# 

# /\* ─── LAYOUT ─────────────────────────────────────────────── \*/

# main { padding-top: var(--nav-h); }

# .wrap { max-width: var(--max); margin: 0 auto; padding: 0 20px; }

# 

# section { padding: clamp(56px,7vw,96px) 0; }

# section.alt { background: var(--off); }

# section.stone { background: var(--stone); }

# 

# /\* ─── TYPOGRAPHY ─────────────────────────────────────────── \*/

# .serif { font-family: 'Libre Baskerville', serif; }

# .eyebrow {

# &#x20; display: inline-flex; align-items: center; gap: 8px;

# &#x20; font-size: 0.71rem; font-weight: 600; letter-spacing: 0.1em;

# &#x20; text-transform: uppercase; color: var(--muted); margin-bottom: 12px;

# }

# .eyebrow::before {

# &#x20; content: ''; display: block; width: 16px; height: 1.5px;

# &#x20; background: currentColor; border-radius: 2px;

# }

# .eyebrow.blue  { color: var(--blue); }

# .eyebrow.amber { color: var(--amber); }

# .eyebrow.green { color: var(--green); }

# .eyebrow.rose  { color: var(--rose); }

# 

# h1,h2,h3,h4 { font-family: 'Libre Baskerville', serif; color: var(--ink); line-height: 1.2; letter-spacing: -0.02em; }

# h1 { font-size: clamp(2.2rem,5vw,3.6rem); }

# h2 { font-size: clamp(1.6rem,3.5vw,2.5rem); }

# h3 { font-size: clamp(1.05rem,2vw,1.3rem); }

# h4 { font-size: 0.95rem; letter-spacing: -0.01em; }

# 

# .lead {

# &#x20; font-size: clamp(0.9rem,1.5vw,1rem);

# &#x20; color: var(--muted); line-height: 1.8; font-weight: 300;

# &#x20; max-width: 620px;

# }

# p { color: var(--muted); line-height: 1.75; }

# 

# /\* ─── SEX BADGE ──────────────────────────────────────────── \*/

# .sex-badge {

# &#x20; display: inline-flex; align-items: center; gap: 5px;

# &#x20; padding: 2px 9px; border-radius: 99px;

# &#x20; font-size: 0.68rem; font-weight: 700; letter-spacing: 0.05em;

# &#x20; margin-bottom: 10px;

# }

# .sb-male   { background: var(--blue-l);  color: var(--blue);  border: 1px solid var(--blue-m); }

# .sb-female { background: var(--rose-l);  color: var(--rose);  border: 1px solid var(--rose-m); }

# .sb-both   { background: var(--stone);   color: var(--muted); border: 1px solid var(--border2); }

# 

# /\* ─── PILL / BADGE ───────────────────────────────────────── \*/

# .pill {

# &#x20; display: inline-flex; align-items: center; gap: 5px;

# &#x20; padding: 3px 10px; border-radius: 99px; font-size: 0.72rem; font-weight: 600;

# }

# .pill-blue  { background: var(--blue-l);  color: var(--blue);  border: 1px solid var(--blue-m); }

# .pill-amber { background: var(--amber-l); color: var(--amber); border: 1px solid var(--amber-m); }

# .pill-green { background: var(--green-l); color: var(--green); border: 1px solid var(--green-m); }

# .pill-rose  { background: var(--rose-l);  color: var(--rose);  border: 1px solid var(--rose-m); }

# .pill-gray  { background: var(--stone);   color: var(--muted); border: 1px solid var(--border); }

# 

# .stat-pill {

# &#x20; display: inline; padding: 1px 7px; border-radius: 4px;

# &#x20; font-size: 0.85em; font-weight: 700; font-family: 'Figtree', sans-serif;

# }

# .sp-blue  { background: var(--blue-l);  color: var(--blue); }

# .sp-amber { background: var(--amber-l); color: var(--amber); }

# .sp-green { background: var(--green-l); color: var(--green); }

# .sp-rose  { background: var(--rose-l);  color: var(--rose); }

# 

# /\* ─── CARDS ──────────────────────────────────────────────── \*/

# .card {

# &#x20; background: var(--white); border: 1px solid var(--border);

# &#x20; border-radius: var(--r3); padding: clamp(18px,2.5vw,26px);

# &#x20; transition: box-shadow 0.2s, border-color 0.2s;

# }

# .card:hover { box-shadow: 0 6px 24px rgba(0,0,0,0.07); border-color: var(--border2); }

# .card.blue  { border-top: 3px solid var(--blue); }

# .card.amber { border-top: 3px solid var(--amber); }

# .card.green { border-top: 3px solid var(--green); }

# .card.rose  { border-top: 3px solid var(--rose); }

# 

# .icon-wrap {

# &#x20; width: 36px; height: 36px; border-radius: 8px;

# &#x20; display: flex; align-items: center; justify-content: center;

# &#x20; font-size: 1rem; margin-bottom: 12px; flex-shrink: 0;

# }

# .iw-blue  { background: var(--blue-l); }

# .iw-amber { background: var(--amber-l); }

# .iw-green { background: var(--green-l); }

# .iw-rose  { background: var(--rose-l); }

# .iw-gray  { background: var(--stone); }

# 

# /\* ─── GRIDS ──────────────────────────────────────────────── \*/

# .g2 { display: grid; grid-template-columns: repeat(auto-fit,minmax(260px,1fr)); gap: 16px; }

# .g3 { display: grid; grid-template-columns: repeat(auto-fit,minmax(200px,1fr)); gap: 16px; }

# .g4 { display: grid; grid-template-columns: repeat(auto-fit,minmax(160px,1fr)); gap: 12px; }

# .split { display: grid; grid-template-columns: 1fr 1fr; gap: clamp(24px,4vw,52px); align-items: start; }

# @media(max-width:720px) { .split { grid-template-columns: 1fr; } }

# 

# /\* ─── CALLOUTS ───────────────────────────────────────────── \*/

# .callout {

# &#x20; padding: 13px 16px; border-radius: var(--r2);

# &#x20; font-size: 0.84rem; line-height: 1.65;

# &#x20; display: flex; gap: 10px; align-items: flex-start;

# &#x20; margin: 14px 0;

# }

# .callout-i { flex-shrink: 0; font-size: 0.92rem; margin-top: 1px; }

# .c-blue  { background: var(--blue-l);  border: 1px solid var(--blue-m);  color: #1e40af; }

# .c-amber { background: var(--amber-l); border: 1px solid var(--amber-m); color: #92400e; }

# .c-green { background: var(--green-l); border: 1px solid var(--green-m); color: #065f46; }

# .c-rose  { background: var(--rose-l);  border: 1px solid var(--rose-m);  color: #831843; }

# .c-red   { background: var(--red-l);   border: 1px solid #fecaca;        color: var(--red); }

# 

# /\* ─── ACCORDION ──────────────────────────────────────────── \*/

# .acc-wrap { display: flex; flex-direction: column; gap: 8px; }

# .acc {

# &#x20; border: 1px solid var(--border); border-radius: var(--r2);

# &#x20; overflow: hidden; background: var(--white);

# &#x20; transition: box-shadow 0.2s;

# }

# .acc:hover { box-shadow: 0 2px 12px rgba(0,0,0,0.05); }

# .acc-btn {

# &#x20; width: 100%; display: flex; align-items: center;

# &#x20; gap: 12px; padding: 14px 16px;

# &#x20; background: none; border: none; cursor: pointer;

# &#x20; text-align: left; color: var(--ink);

# &#x20; transition: background 0.15s;

# }

# .acc-btn:hover { background: var(--off); }

# .acc-btn.open { background: var(--stone); }

# .acc-icon { flex-shrink: 0; font-size: 1rem; }

# .acc-title {

# &#x20; flex: 1; font-family: 'Libre Baskerville', serif;

# &#x20; font-size: 0.92rem; font-weight: 700;

# }

# .acc-chev {

# &#x20; flex-shrink: 0; width: 18px; height: 18px;

# &#x20; color: var(--faint); transition: transform 0.25s;

# }

# .acc-btn.open .acc-chev { transform: rotate(180deg); }

# .acc-body {

# &#x20; display: none; padding: 16px 18px 18px;

# &#x20; border-top: 1px solid var(--border);

# &#x20; background: var(--white);

# }

# .acc-body.open { display: block; }

# .acc-body p { font-size: 0.86rem; margin-bottom: 10px; }

# .acc-body p:last-child { margin-bottom: 0; }

# 

# /\* ─── STEP LIST ──────────────────────────────────────────── \*/

# .steps { display: flex; flex-direction: column; gap: 0; }

# .step {

# &#x20; display: flex; gap: 12px; padding: 14px 0;

# &#x20; border-bottom: 1px solid var(--border);

# }

# .step:last-child { border-bottom: none; }

# .step-num {

# &#x20; flex-shrink: 0; width: 26px; height: 26px; border-radius: 50%;

# &#x20; display: flex; align-items: center; justify-content: center;

# &#x20; font-size: 0.7rem; font-weight: 700; font-family: 'Figtree', sans-serif;

# &#x20; margin-top: 1px;

# }

# .sn-blue  { background: var(--blue-l);  color: var(--blue);  border: 1px solid var(--blue-m); }

# .sn-amber { background: var(--amber-l); color: var(--amber); border: 1px solid var(--amber-m); }

# .sn-green { background: var(--green-l); color: var(--green); border: 1px solid var(--green-m); }

# .sn-rose  { background: var(--rose-l);  color: var(--rose);  border: 1px solid var(--rose-m); }

# .step-content h4 { font-size: 0.86rem; margin-bottom: 4px; }

# .step-content p  { font-size: 0.81rem; }

# 

# /\* ─── CHECK LIST ─────────────────────────────────────────── \*/

# .clist { list-style: none; display: flex; flex-direction: column; gap: 6px; }

# .clist li {

# &#x20; display: flex; gap: 8px; align-items: flex-start;

# &#x20; font-size: 0.84rem; color: var(--muted); line-height: 1.5;

# }

# .clist li::before { content: '✓'; flex-shrink: 0; font-weight: 700; margin-top: 1px; font-size: 0.76rem; }

# .cl-blue  li::before { color: var(--blue); }

# .cl-amber li::before { color: var(--amber); }

# .cl-green li::before { color: var(--green); }

# .cl-rose  li::before { color: var(--rose); }

# 

# /\* ─── TABLE ──────────────────────────────────────────────── \*/

# .tbl-wrap { overflow-x: auto; border: 1px solid var(--border); border-radius: var(--r2); }

# table { width: 100%; border-collapse: collapse; font-size: 0.82rem; }

# thead { background: var(--stone); }

# th {

# &#x20; padding: 10px 13px; text-align: left;

# &#x20; font-family: 'Figtree', sans-serif; font-size: 0.7rem;

# &#x20; font-weight: 700; color: var(--muted);

# &#x20; letter-spacing: 0.07em; text-transform: uppercase;

# &#x20; border-bottom: 1px solid var(--border2);

# &#x20; white-space: nowrap;

# }

# td {

# &#x20; padding: 10px 13px; border-bottom: 1px solid var(--border);

# &#x20; vertical-align: top; line-height: 1.5; color: var(--muted);

# }

# tr:last-child td { border-bottom: none; }

# tr:hover td { background: var(--off); }

# td:first-child { color: var(--ink); font-weight: 600; }

# 

# /\* ─── CITE ───────────────────────────────────────────────── \*/

# .cref {

# &#x20; display: inline-flex; align-items: center; justify-content: center;

# &#x20; width: 15px; height: 15px; border-radius: 50%;

# &#x20; background: var(--blue-l); color: var(--blue);

# &#x20; font-size: 8px; font-weight: 700; cursor: pointer;

# &#x20; border: 1px solid var(--blue-m);

# &#x20; transition: background 0.15s; vertical-align: super;

# &#x20; margin-left: 2px; flex-shrink: 0;

# &#x20; text-decoration: none;

# }

# .cref:hover { background: var(--blue-m); }

# 

# /\* ─── FADE ───────────────────────────────────────────────── \*/

# .fu { opacity: 0; transform: translateY(18px); transition: opacity 0.5s ease, transform 0.5s ease; }

# .fu.vis { opacity: 1; transform: none; }

# .fu.d1 { transition-delay: 0.08s; }

# .fu.d2 { transition-delay: 0.16s; }

# .fu.d3 { transition-delay: 0.24s; }

# 

# /\* Hero elements animate immediately on load \*/

# .hero .fu { animation: heroFadeIn 0.7s ease forwards; opacity: 0; }

# .hero .fu.d1 { animation-delay: 0.15s; }

# .hero .fu.d2 { animation-delay: 0.3s; }

# .hero .fu.d3 { animation-delay: 0.5s; }

# @keyframes heroFadeIn {

# &#x20; from { opacity: 0; transform: translateY(18px); }

# &#x20; to   { opacity: 1; transform: none; }

# }

# 

# /\* ═══════════════════════════════════════════════════════════

# &#x20;  HERO

# ═══════════════════════════════════════════════════════════ \*/

# .hero {

# &#x20; background: var(--ink);

# &#x20; padding: clamp(72px,11vw,120px) 0 clamp(56px,9vw,100px);

# &#x20; overflow: hidden; position: relative;

# }

# .hero::before {

# &#x20; content: '';

# &#x20; position: absolute; inset: 0;

# &#x20; background: radial-gradient(ellipse 70% 60% at 80% 40%, rgba(29,78,216,0.14) 0%, transparent 70%),

# &#x20;             radial-gradient(ellipse 50% 50% at 20% 80%, rgba(15,110,80,0.1) 0%, transparent 60%),

# &#x20;             radial-gradient(ellipse 40% 40% at 10% 20%, rgba(157,23,77,0.08) 0%, transparent 60%);

# }

# .hero-inner { position: relative; z-index: 1; }

# .hero-kicker {

# &#x20; display: inline-flex; align-items: center; gap: 10px; margin-bottom: 24px;

# &#x20; font-size: 0.7rem; font-weight: 600; letter-spacing: 0.1em;

# &#x20; text-transform: uppercase; color: rgba(255,255,255,0.4);

# }

# .hero-dot { width: 6px; height: 6px; border-radius: 50%; background: var(--green); animation: blink 2s infinite; }

# @keyframes blink { 0%,100%{opacity:1} 50%{opacity:.25} }

# .hero h1 { color: var(--white); margin-bottom: 10px; }

# .hero-sub {

# &#x20; font-family: 'Libre Baskerville', serif; font-style: italic;

# &#x20; font-size: clamp(1rem,2.2vw,1.5rem); color: rgba(255,255,255,0.42);

# &#x20; margin-bottom: 20px;

# }

# .hero-desc {

# &#x20; font-size: clamp(0.88rem,1.4vw,1rem); color: rgba(255,255,255,0.5);

# &#x20; max-width: 560px; line-height: 1.8; font-weight: 300;

# &#x20; margin-bottom: 36px;

# }

# .hero-tags { display: flex; flex-wrap: wrap; gap: 8px; margin-bottom: 48px; }

# .hero-tag {

# &#x20; padding: 5px 13px; border-radius: 99px;

# &#x20; font-size: 0.76rem; font-weight: 500; color: rgba(255,255,255,0.6);

# &#x20; border: 1px solid rgba(255,255,255,0.14);

# &#x20; background: rgba(255,255,255,0.05);

# }

# .hero-cards {

# &#x20; display: grid;

# &#x20; grid-template-columns: repeat(auto-fit,minmax(160px,1fr));

# &#x20; gap: 10px;

# }

# .hero-card {

# &#x20; background: rgba(255,255,255,0.05);

# &#x20; border: 1px solid rgba(255,255,255,0.1);

# &#x20; border-radius: var(--r2); padding: 16px 18px;

# &#x20; transition: background 0.2s, border-color 0.2s;

# }

# .hero-card:hover { background: rgba(255,255,255,0.09); border-color: rgba(255,255,255,0.2); }

# .hero-card-em { font-size: 1.2rem; margin-bottom: 8px; }

# .hero-card h3 {

# &#x20; font-family: 'Figtree', sans-serif;

# &#x20; font-size: 0.8rem; font-weight: 600; color: var(--white);

# &#x20; letter-spacing: 0; margin-bottom: 4px;

# }

# .hero-card p { font-size: 0.74rem; color: rgba(255,255,255,0.38); line-height: 1.5; }

# 

# /\* ═══════════════════════════════════════════════════════════

# &#x20;  ROUTINE CALCULATOR

# ═══════════════════════════════════════════════════════════ \*/

# .calc-section { background: var(--stone); }

# 

# .calc-form {

# &#x20; background: var(--white);

# &#x20; border: 1px solid var(--border);

# &#x20; border-radius: var(--r3); padding: clamp(20px,3vw,32px);

# &#x20; margin-bottom: 28px;

# }

# .form-grid {

# &#x20; display: grid;

# &#x20; grid-template-columns: repeat(auto-fit,minmax(150px,1fr));

# &#x20; gap: 14px; margin-bottom: 18px;

# }

# .form-group { display: flex; flex-direction: column; gap: 5px; }

# .form-group label {

# &#x20; font-size: 0.73rem; font-weight: 600; letter-spacing: 0.05em;

# &#x20; text-transform: uppercase; color: var(--muted);

# }

# .form-group input,

# .form-group select {

# &#x20; padding: 9px 12px; border-radius: var(--r);

# &#x20; border: 1.5px solid var(--border); background: var(--white);

# &#x20; font-family: 'Figtree', sans-serif; font-size: 0.88rem;

# &#x20; color: var(--ink); outline: none; transition: border-color 0.15s;

# &#x20; -webkit-appearance: none; appearance: none;

# &#x20; min-height: 44px; /\* mobile touch target \*/

# }

# .form-group input:focus,

# .form-group select:focus { border-color: var(--blue); }

# .form-group .unit {

# &#x20; font-size: 0.7rem; color: var(--faint); text-align: right;

# }

# 

# /\* sex toggle \*/

# .sex-toggle {

# &#x20; display: flex; border: 1.5px solid var(--border);

# &#x20; border-radius: var(--r); overflow: hidden; align-self: flex-start;

# &#x20; width: 100%;

# }

# .sex-toggle button {

# &#x20; flex: 1; padding: 10px 12px; border: none; background: none; cursor: pointer;

# &#x20; font-family: 'Figtree', sans-serif; font-size: 0.82rem;

# &#x20; font-weight: 600; color: var(--muted); transition: all 0.15s;

# &#x20; min-height: 44px;

# }

# .sex-toggle button.active-m { background: var(--blue); color: var(--white); }

# .sex-toggle button.active-f { background: var(--rose); color: var(--white); }

# .sex-toggle button.active-f { background: var(--rose); color: var(--white); }

# 

# .unit-toggle {

# &#x20; display: inline-flex; border: 1.5px solid var(--border);

# &#x20; border-radius: var(--r); overflow: hidden; align-self: flex-start;

# }

# .unit-toggle button {

# &#x20; padding: 8px 14px; border: none; background: none; cursor: pointer;

# &#x20; font-family: 'Figtree', sans-serif; font-size: 0.76rem;

# &#x20; font-weight: 600; color: var(--muted); transition: all 0.15s;

# &#x20; min-height: 40px;

# }

# .unit-toggle button.active { background: var(--blue); color: var(--white); }

# 

# /\* ─── GOAL CHECKBOXES ─── \*/

# .goal-grid {

# &#x20; display: grid; grid-template-columns: repeat(auto-fit,minmax(160px,1fr));

# &#x20; gap: 8px; margin-bottom: 18px;

# }

# .goal-chip {

# &#x20; display: flex; align-items: center; gap: 8px;

# &#x20; border: 1.5px solid var(--border); border-radius: var(--r2);

# &#x20; padding: 10px 13px; cursor: pointer;

# &#x20; transition: border-color 0.15s, background 0.15s;

# &#x20; user-select: none; font-size: 0.84rem; color: var(--ink2);

# &#x20; min-height: 44px;

# }

# .goal-chip input { display: none; }

# .goal-chip-box {

# &#x20; width: 16px; height: 16px; border-radius: 4px;

# &#x20; border: 1.5px solid var(--border2); flex-shrink: 0;

# &#x20; display: flex; align-items: center; justify-content: center;

# &#x20; font-size: 0.62rem; transition: all 0.15s;

# }

# .goal-chip.checked { border-color: var(--blue); background: var(--blue-l); }

# .goal-chip.checked .goal-chip-box { background: var(--blue); border-color: var(--blue); color: white; }

# 

# .calc-btn {

# &#x20; width: 100%; padding: 14px; border-radius: var(--r2);

# &#x20; background: var(--blue); color: var(--white); border: none;

# &#x20; font-family: 'Figtree', sans-serif; font-size: 0.95rem; font-weight: 600;

# &#x20; cursor: pointer; transition: opacity 0.15s, transform 0.1s;

# &#x20; letter-spacing: 0.01em; min-height: 48px;

# }

# .calc-btn:hover { opacity: 0.88; }

# .calc-btn:active { transform: scale(0.99); }

# 

# /\* Result panel \*/

# .result-panel {

# &#x20; display: none;

# &#x20; background: var(--white); border: 1px solid var(--border);

# &#x20; border-radius: var(--r3); overflow: hidden;

# }

# .result-panel.visible { display: block; }

# 

# .result-header {

# &#x20; background: var(--ink); padding: 20px 24px;

# &#x20; display: grid; grid-template-columns: repeat(auto-fit,minmax(110px,1fr));

# &#x20; gap: 16px;

# }

# .result-stat .label {

# &#x20; font-size: 0.66rem; font-weight: 600; letter-spacing: 0.1em;

# &#x20; text-transform: uppercase; color: rgba(255,255,255,0.38);

# &#x20; margin-bottom: 4px;

# }

# .result-stat .value {

# &#x20; font-family: 'Libre Baskerville', serif;

# &#x20; font-size: 1.35rem; color: var(--white); line-height: 1;

# }

# .result-stat .sub {

# &#x20; font-size: 0.68rem; color: rgba(255,255,255,0.3);

# &#x20; margin-top: 3px;

# }

# 

# .result-body { padding: clamp(16px,3vw,28px); }

# .result-body h3 {

# &#x20; font-size: 0.95rem; margin-bottom: 14px; padding-bottom: 10px;

# &#x20; border-bottom: 1px solid var(--border);

# }

# 

# /\* Routine blocks \*/

# .routine-block { margin-bottom: 24px; }

# .rb-head {

# &#x20; display: flex; align-items: center; gap: 10px;

# &#x20; margin-bottom: 10px; flex-wrap: wrap;

# }

# .rb-badge {

# &#x20; padding: 3px 10px; border-radius: 99px;

# &#x20; font-size: 0.68rem; font-weight: 700; letter-spacing: 0.06em;

# &#x20; text-transform: uppercase;

# }

# .rb-morning { background: var(--amber-l); color: var(--amber); }

# .rb-midday  { background: var(--blue-l);  color: var(--blue); }

# .rb-evening { background: var(--green-l); color: var(--green); }

# .rb-weekly  { background: var(--stone);   color: var(--muted); border: 1px solid var(--border); }

# .rb-female  { background: var(--rose-l);  color: var(--rose); }

# 

# .rb-items { display: flex; flex-direction: column; gap: 7px; }

# .rb-item {

# &#x20; display: grid; grid-template-columns: minmax(120px,2fr) minmax(80px,1fr) 3fr;

# &#x20; gap: 10px; padding: 10px 13px;

# &#x20; background: var(--off); border-radius: var(--r);

# &#x20; font-size: 0.82rem; align-items: start;

# &#x20; border-left: 3px solid transparent;

# }

# .rb-item.cog   { border-left-color: var(--blue); }

# .rb-item.hor   { border-left-color: var(--amber); }

# .rb-item.det   { border-left-color: var(--green); }

# .rb-item.psych { border-left-color: var(--muted); }

# .rb-item.fem   { border-left-color: var(--rose); }

# .rb-name { font-weight: 600; color: var(--ink); line-height: 1.35; }

# .rb-dose { font-weight: 700; color: var(--blue); }

# .rb-item.fem .rb-dose { color: var(--rose); }

# .rb-item.hor .rb-dose { color: var(--amber); }

# .rb-item.det .rb-dose { color: var(--green); }

# .rb-note { color: var(--muted); line-height: 1.4; }

# 

# @media(max-width:680px) {

# &#x20; .rb-item { grid-template-columns: 1fr 1fr; gap: 4px 8px; }

# &#x20; .rb-note { grid-column: 1 / -1; font-size: 0.78rem; margin-top: 2px; }

# }

# @media(max-width:420px) {

# &#x20; .rb-item { grid-template-columns: 1fr; gap: 3px; }

# &#x20; .rb-dose { font-size: 0.88rem; }

# }

# 

# .result-disclaimer {

# &#x20; margin-top: 18px; padding: 13px 15px;

# &#x20; background: var(--red-l); border: 1px solid #fecaca;

# &#x20; border-radius: var(--r); font-size: 0.77rem; color: var(--red);

# &#x20; line-height: 1.6;

# }

# 

# /\* Notes grid \*/

# .notes-grid {

# &#x20; display: grid; grid-template-columns: repeat(auto-fit,minmax(190px,1fr));

# &#x20; gap: 10px; margin-top: 18px;

# }

# .note-card {

# &#x20; background: var(--off); border-radius: var(--r2); padding: 13px 14px;

# &#x20; border: 1px solid var(--border);

# }

# .note-card .note-title {

# &#x20; font-size: 0.77rem; font-weight: 700; color: var(--ink);

# &#x20; margin-bottom: 4px;

# }

# .note-card p { font-size: 0.77rem; }

# 

# /\* ─── SCORE BARS ─────────────────────────────────────────── \*/

# .score-bar-wrap { margin-bottom: 8px; }

# .score-bar-label {

# &#x20; display: flex; justify-content: space-between; align-items: baseline;

# &#x20; font-size: 0.78rem; margin-bottom: 4px;

# }

# .score-bar-label span:first-child { color: var(--ink2); font-weight: 500; }

# .score-bar-label span:last-child { color: var(--muted); font-size: 0.7rem; }

# .score-bar {

# &#x20; height: 6px; background: var(--stone); border-radius: 3px; overflow: hidden;

# }

# .score-fill {

# &#x20; height: 100%; border-radius: 3px;

# &#x20; transition: width 0.9s cubic-bezier(.4,0,.2,1);

# }

# 

# /\* ─── TOXIN CHECKER ──────────────────────────────────────── \*/

# .tox-grid {

# &#x20; display: grid; grid-template-columns: repeat(auto-fill,minmax(220px,1fr));

# &#x20; gap: 8px; margin-bottom: 16px;

# }

# .tox-item {

# &#x20; display: flex; align-items: center; gap: 9px;

# &#x20; border: 1.5px solid var(--border); border-radius: var(--r2);

# &#x20; padding: 10px 13px; cursor: pointer;

# &#x20; transition: border-color 0.15s, background 0.15s;

# &#x20; user-select: none; font-size: 0.82rem; color: var(--muted);

# &#x20; min-height: 44px;

# }

# .tox-item input { display: none; }

# .tox-box {

# &#x20; width: 16px; height: 16px; border-radius: 4px;

# &#x20; border: 1.5px solid var(--border2); flex-shrink: 0;

# &#x20; display: flex; align-items: center; justify-content: center;

# &#x20; font-size: 0.6rem; transition: all 0.15s;

# }

# .tox-item.checked { border-color: var(--rose); background: var(--rose-l); color: var(--ink2); }

# .tox-item.checked .tox-box { background: var(--rose); border-color: var(--rose); color: white; }

# 

# /\* ─── SLEEP ENV CARDS ────────────────────────────────────── \*/

# .sleep-grid {

# &#x20; display: grid; grid-template-columns: repeat(auto-fit,minmax(160px,1fr));

# &#x20; gap: 10px; margin: 16px 0;

# }

# .sleep-env-card {

# &#x20; background: var(--white); border: 1px solid var(--border);

# &#x20; border-radius: var(--r2); padding: 14px 16px; text-align: center;

# &#x20; transition: box-shadow 0.2s, border-color 0.2s;

# }

# .sleep-env-card:hover { box-shadow: 0 4px 16px rgba(0,0,0,0.07); border-color: var(--border2); }

# .sleep-env-card .sec-icon { font-size: 1.4rem; margin-bottom: 6px; }

# .sleep-env-card .sec-label { font-size: 0.72rem; color: var(--muted); margin-bottom: 4px; text-transform: uppercase; letter-spacing: .06em; font-weight: 600; }

# .sleep-env-card .sec-val { font-family: 'Libre Baskerville', serif; font-size: 1.1rem; color: var(--ink); font-weight: 700; margin-bottom: 2px; }

# .sleep-env-card .sec-note { font-size: 0.72rem; color: var(--faint); line-height: 1.45; }

# 

# /\* ─── RESULT TABS ────────────────────────────────────────── \*/

# .result-tabs {

# &#x20; display: flex; gap: 2px; padding: 12px 16px 0;

# &#x20; background: var(--stone); border-bottom: 1px solid var(--border);

# &#x20; overflow-x: auto; scrollbar-width: none;

# }

# .result-tabs::-webkit-scrollbar { display: none; }

# .rtab {

# &#x20; padding: 8px 16px; border-radius: var(--r) var(--r) 0 0;

# &#x20; border: 1px solid transparent; border-bottom: none;

# &#x20; background: none; font-family: 'Figtree', sans-serif;

# &#x20; font-size: 0.8rem; font-weight: 600; color: var(--muted);

# &#x20; cursor: pointer; transition: all 0.15s; white-space: nowrap;

# }

# .rtab:hover { background: var(--white); color: var(--ink); }

# .rtab.active {

# &#x20; background: var(--white); color: var(--blue);

# &#x20; border-color: var(--border); margin-bottom: -1px;

# }

# .tab-content { padding: clamp(16px,3vw,28px); }

# 

# /\* ─── PRIORITY BADGE ─────────────────────────────────────── \*/

# .priority-badge {

# &#x20; display: inline-flex; align-items: center; gap: 5px;

# &#x20; padding: 2px 9px; border-radius: 99px;

# &#x20; font-size: 0.64rem; font-weight: 700; letter-spacing: .06em;

# &#x20; text-transform: uppercase; flex-shrink: 0; margin-left: 6px;

# }

# .pb-high   { background: #fef2f2; color: #b91c1c; border: 1px solid #fecaca; }

# .pb-med    { background: var(--amber-l); color: var(--amber); border: 1px solid var(--amber-m); }

# .pb-low    { background: var(--green-l); color: var(--green); border: 1px solid var(--green-m); }

# 

# /\* ─── PRINT STYLES ───────────────────────────────────────── \*/

# @media print {

# &#x20; .nav, .mob-menu, #prog, .ham, .nav-cta, footer, .calc-form, #resultActions,

# &#x20; .hero-tags, .hero-cards, .hero-kicker, .result-tabs, #btt { display: none !important; }

# &#x20; main { padding-top: 0; }

# &#x20; body { font-size: 12px; }

# &#x20; .result-panel { display: block !important; box-shadow: none; }

# &#x20; .tab-content { display: block !important; }

# &#x20; section { padding: 24px 0; }

# &#x20; .fu { opacity: 1 !important; transform: none !important; }

# &#x20; a\[href]:after { content: none; }

# }

# 

# /\* ─── BACK TO TOP ────────────────────────────────────────── \*/

# \#btt {

# &#x20; position: fixed; bottom: 24px; right: 24px; z-index: 900;

# &#x20; width: 40px; height: 40px; border-radius: 50%;

# &#x20; background: var(--ink); color: var(--white); border: none;

# &#x20; font-size: 1rem; cursor: pointer; opacity: 0; pointer-events: none;

# &#x20; transition: opacity 0.3s; display: flex; align-items: center; justify-content: center;

# &#x20; box-shadow: 0 4px 16px rgba(0,0,0,0.2);

# }

# \#btt.show { opacity: 1; pointer-events: auto; }

# \#btt:hover { background: var(--blue); }

# @media(max-width:820px) {

# &#x20; .nav-links, .nav-cta { display: none; }

# &#x20; .ham { display: flex; }

# }

# @media(max-width:640px) {

# &#x20; .footer-grid { grid-template-columns: 1fr 1fr !important; }

# }

# @media(max-width:400px) {

# &#x20; .footer-grid { grid-template-columns: 1fr !important; }

# }

# @media(max-width:480px) {

# &#x20; .form-grid { grid-template-columns: 1fr 1fr; }

# &#x20; .hero-cards { grid-template-columns: 1fr 1fr; }

# &#x20; .g4 { grid-template-columns: 1fr 1fr; }

# &#x20; .result-header { grid-template-columns: repeat(2, 1fr) !important; }

# }

# @media(max-width:360px) {

# &#x20; .form-grid { grid-template-columns: 1fr; }

# &#x20; .hero-cards { grid-template-columns: 1fr; }

# }

# 

# /\* Fix pill variants for summary table \*/

# .pill-blue  { background: var(--blue-l);  color: var(--blue);  border: 1px solid var(--blue-m); }

# .pill-amber { background: var(--amber-l); color: var(--amber); border: 1px solid var(--amber-m); }

# .pill-green { background: var(--green-l); color: var(--green); border: 1px solid var(--green-m); }

# .pill-rose  { background: var(--rose-l);  color: var(--rose);  border: 1px solid var(--rose-m); }

# .pill-gray  { background: var(--stone);   color: var(--muted); border: 1px solid var(--border); }

# 

# /\* Exergaming cards \*/

# .exercise-stat {

# &#x20; background: var(--white); border: 1px solid var(--border);

# &#x20; border-radius: var(--r2); padding: 14px 16px;

# &#x20; text-align: center;

# }

# .exercise-stat .es-num {

# &#x20; font-family: 'Libre Baskerville', serif;

# &#x20; font-size: 1.5rem; font-weight: 700; line-height: 1;

# &#x20; margin-bottom: 4px;

# }

# .exercise-stat .es-label { font-size: 0.72rem; color: var(--muted); line-height: 1.4; }

# 

# /\* Banner callout \*/

# .banner-callout {

# &#x20; background: linear-gradient(135deg, var(--ink) 0%, #1e2a4a 100%);

# &#x20; border-radius: var(--r3); padding: 24px 28px; margin: 32px 0;

# &#x20; display: flex; gap: 16px; align-items: flex-start;

# }

# .banner-callout .bc-icon { font-size: 1.6rem; flex-shrink: 0; }

# .banner-callout .bc-title { font-family: 'Libre Baskerville', serif; font-size: 1rem; color: var(--white); margin-bottom: 6px; }

# .banner-callout .bc-text { font-size: 0.84rem; color: rgba(255,255,255,0.55); line-height: 1.65; }

# .banner-callout .bc-stats { display: flex; gap: 20px; margin-top: 12px; flex-wrap: wrap; }

# .banner-callout .bc-stat-n { font-family: 'Libre Baskerville', serif; font-size: 1.3rem; color: var(--white); line-height: 1; }

# .banner-callout .bc-stat-l { font-size: 0.7rem; color: rgba(255,255,255,0.4); text-transform: uppercase; letter-spacing: .06em; margin-top: 2px; }

# </style>

# </head>

# <body>

# 

# <div id="prog"></div>

# <button id="btt" aria-label="Back to top" onclick="window.scrollTo({top:0,behavior:'smooth'})">↑</button>

# 

# <!-- ▸ NAV -->

# <nav class="nav">

# &#x20; <div class="nav-wrap">

# &#x20;   <a href="#home" class="nav-logo">Bio<span>Optima</span></a>

# &#x20;   <ul class="nav-links">

# &#x20;     <li><a href="#cognitive">Cognitive</a></li>

# &#x20;     <li><a href="#behavioral">Behavioral</a></li>

# &#x20;     <li><a href="#pharmacological">Pharmacological</a></li>

# &#x20;     <li><a href="#mindfulness">Mindfulness</a></li>

# &#x20;     <li><a href="#edc">EDC \&amp; Toxins</a></li>

# &#x20;     <li><a href="#hormonal">Hormonal</a></li>

# &#x20;     <li><a href="#fasting">Fasting</a></li>

# &#x20;     <li><a href="#detox">Detox</a></li>

# &#x20;     <li><a href="#sleep">Sleep</a></li>

# &#x20;     <li><a href="#summary">Summary</a></li>

# &#x20;     <li><a href="#calculator">Routine</a></li>

# &#x20;   </ul>

# &#x20;   <a href="#calculator" class="nav-cta">Build My Routine ↓</a>

# &#x20;   <button class="ham" id="ham" aria-label="Menu" aria-expanded="false">

# &#x20;     <span></span><span></span><span></span>

# &#x20;   </button>

# &#x20; </div>

# </nav>

# <div class="mob-menu" id="mobMenu">

# &#x20; <a href="#cognitive">Cognitive Enhancement</a>

# &#x20; <a href="#behavioral">Behavioral Interventions</a>

# &#x20; <a href="#pharmacological">Pharmacological</a>

# &#x20; <a href="#mindfulness">Mindfulness \&amp; Hypnosis</a>

# &#x20; <a href="#edc">EDC \&amp; Endocrine Disruption</a>

# &#x20; <a href="#hormonal">Hormonal Optimisation</a>

# &#x20; <a href="#fasting">Fasting \&amp; Metabolism</a>

# &#x20; <a href="#detox">Detox \&amp; Nrf2</a>

# &#x20; <a href="#sleep">Sleep Optimisation</a>

# &#x20; <a href="#summary">Evidence Summary</a>

# &#x20; <a href="#calculator">🗓 Build My Routine</a>

# </div>

# 

# <main>

# 

# <!-- ▸ HERO -->

# <section class="hero" id="home">

# &#x20; <div class="wrap hero-inner">

# &#x20;   <div class="hero-kicker"><span class="hero-dot"></span> Peer-reviewed · Non-industry funded · RCT evidence</div>

# &#x20;   <h1 class="fu">Optimise Brain,<br>Hormones \&amp; Body</h1>

# &#x20;   <div class="hero-sub fu d1">Evidence-based interventions, not supplements marketing</div>

# &#x20;   <p class="hero-desc fu d2">

# &#x20;     A rigorous synthesis of randomised controlled trials, systematic reviews, and meta-analyses covering cognitive enhancement, hormonal health, endocrine disruption, and detoxification — with a personalised routine calculator.

# &#x20;   </p>

# &#x20;   <div class="hero-tags fu d2">

# &#x20;     <span class="hero-tag">🧠 Cognitive Focus</span>

# &#x20;     <span class="hero-tag">⚡ Testosterone</span>

# &#x20;     <span class="hero-tag">🌸 Female Hormonal Health</span>

# &#x20;     <span class="hero-tag">☣️ EDC / Toxins</span>

# &#x20;     <span class="hero-tag">🌿 Nrf2 \&amp; Detox</span>

# &#x20;     <span class="hero-tag">📋 CBT \&amp; Mindfulness</span>

# &#x20;     <span class="hero-tag">🕐 Intermittent Fasting</span>

# &#x20;     <span class="hero-tag">😴 Sleep Optimisation</span>

# &#x20;   </div>

# &#x20;   <div class="hero-cards fu d3">

# &#x20;     <div class="hero-card">

# &#x20;       <div class="hero-card-em">🧠</div>

# &#x20;       <h3>Cognitive Enhancement</h3>

# &#x20;       <p>CBT, MBSR, rehabilitation — ranked by evidence strength</p>

# &#x20;     </div>

# &#x20;     <div class="hero-card">

# &#x20;       <div class="hero-card-em">💊</div>

# &#x20;       <h3>Pharmacological</h3>

# &#x20;       <p>Methylphenidate, modafinil, guanfacine — what trials show</p>

# &#x20;     </div>

# &#x20;     <div class="hero-card">

# &#x20;       <div class="hero-card-em">⚡</div>

# &#x20;       <h3>Hormonal Optimisation</h3>

# &#x20;       <p>TRF, Mediterranean diet, EDC reduction — male \&amp; female</p>

# &#x20;     </div>

# &#x20;     <div class="hero-card">

# &#x20;       <div class="hero-card-em">☣️</div>

# &#x20;       <h3>EDC \&amp; Toxin Defence</h3>

# &#x20;       <p>BPA, phthalates, microplastics — what the data actually shows</p>

# &#x20;     </div>

# &#x20;     <div class="hero-card">

# &#x20;       <div class="hero-card-em">🌿</div>

# &#x20;       <h3>Endogenous Detox</h3>

# &#x20;       <p>Nrf2, autophagy, sulforaphane — activated from within</p>

# &#x20;     </div>

# &#x20;     <div class="hero-card">

# &#x20;       <div class="hero-card-em">😴</div>

# &#x20;       <h3>Sleep Architecture</h3>

# &#x20;       <p>CBT-I, environment targets, female lifespan sleep shifts</p>

# &#x20;     </div>

# &#x20;   </div>

# &#x20; </div>

# </section>

# 

# <!-- ▸ COGNITIVE — OVERVIEW -->

# <section id="cognitive" class="alt">

# &#x20; <div class="wrap">

# &#x20;   <div class="eyebrow blue fu">Cognitive Enhancement</div>

# &#x20;   <h2 class="fu">Brain Fog, Focus \&amp; Concentration</h2>

# &#x20;   <p class="lead fu" style="margin-bottom:40px;">

# &#x20;     "Brain fog" — poor focus, diminished concentration, and impaired processing speed — affects <span class="stat-pill sp-blue">32%</span> of post-COVID patients and is prevalent in depression, ADHD, and chronic fatigue. The research identifies a clear evidence hierarchy across interventions.

# &#x20;   </p>

# &#x20;   <div class="split">

# &#x20;     <div class="fu">

# &#x20;       <div class="steps">

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-blue">1</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>Cognitive Training / Rehabilitation</h4>

# &#x20;             <p>Strongest evidence base across all populations. Sustained improvements in attention, working memory, and cognitive flexibility — including post-COVID and post-cancer brain fog. <a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11794363/" class="cref" target="\_blank" rel="noopener noreferrer">1</a></p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-blue">2</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>Mindfulness-Based Interventions (MBIs)</h4>

# &#x20;             <p>Meta-analysis of 85+ trials: MBSR improves long-term mental fatigue, cortisol, sustained attention, and executive function. Premier first-line recommendation for brain fog. <a href="https://link.springer.com/article/10.1007/s44202-024-00162-1" class="cref" target="\_blank" rel="noopener noreferrer">2</a></p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-blue">3</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>CBT \&amp; Behavioural Activation</h4>

# &#x20;             <p>Medium-to-large effect sizes for ADHD-related brain fog, fatigue, and depression-adjacent cognitive decline. Benefits sustained at 6, 12, and 24 weeks. <a href="https://bpspsychub.onlinelibrary.wiley.com/doi/10.1111/papt.12455" class="cref" target="\_blank" rel="noopener noreferrer">3</a></p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-blue">4</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>Pharmacological Augmentation</h4>

# &#x20;             <p>Stimulants, modafinil, and guanfacine show moderate-to-large effects where cognitive profiles match drug mechanisms. Require medical supervision. <a href="https://www.sciencedirect.com/science/article/pii/S0890856724003046" class="cref" target="\_blank" rel="noopener noreferrer">4</a></p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;       </div>

# &#x20;     </div>

# &#x20;     <div class="fu d1">

# &#x20;       <div class="callout c-blue">

# &#x20;         <span class="callout-i">🔬</span>

# &#x20;         <div><strong>Evidence ranking (non-industry funded):</strong> MBIs hold the largest independent evidence base, supported extensively by NCCIH public funding. Cognitive rehabilitation holds the strongest single-modality effect in meta-analyses spanning 209 trials.</div>

# &#x20;       </div>

# &#x20;       <div class="callout c-rose" style="margin-top:10px;">

# &#x20;         <span class="callout-i">🌸</span>

# &#x20;         <div><strong>Female note:</strong> Brain fog is particularly prevalent in peri- and post-menopausal women due to oestrogen withdrawal effects on PFC function. MBIs showed particular promise in menopausal cohorts vs fatigue education controls. <a href="https://journals.sagepub.com/doi/10.3233/JAD-150992" class="cref" target="\_blank" rel="noopener noreferrer">5</a></div>

# &#x20;       </div>

# &#x20;       <div class="card" style="margin-top:14px;">

# &#x20;         <h4 style="margin-bottom:10px;">Neurophysiological markers of efficacy</h4>

# &#x20;         <ul class="clist cl-blue">

# &#x20;           <li>↑ theta power during focused attention meditation</li>

# &#x20;           <li>Bilateral dlPFC activation in novice meditators after 4 weeks</li>

# &#x20;           <li>↑ grey matter density in hippocampus and PFC with MBSR</li>

# &#x20;           <li>Reduced default-mode network rumination (open monitoring)</li>

# &#x20;           <li>Lower cortisol concentrations associated with lower mental fatigue scores</li>

# &#x20;         </ul>

# &#x20;       </div>

# &#x20;     </div>

# &#x20;   </div>

# &#x20; </div>

# </section>

# 

# <!-- ▸ BEHAVIORAL -->

# <section id="behavioral">

# &#x20; <div class="wrap">

# &#x20;   <div class="eyebrow blue fu">Behavioural Interventions</div>

# &#x20;   <h2 class="fu">Therapy, Activation \&amp; Rehabilitation</h2>

# &#x20;   <p class="lead fu" style="margin-bottom:36px;">Sustainable strategies targeting psychological and environmental drivers of brain fog — with strong non-commercial evidence bases.</p>

# &#x20;   <div class="acc-wrap fu">

# 

# &#x20;     <div class="acc">

# &#x20;       <button class="acc-btn" onclick="toggleAcc(this)">

# &#x20;         <span class="acc-icon">🧩</span>

# &#x20;         <span class="acc-title">Cognitive Behavioural Therapy (CBT)</span>

# &#x20;         <svg class="acc-chev" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 9l6 6 6-6"/></svg>

# &#x20;       </button>

# &#x20;       <div class="acc-body">

# &#x20;         <p>RCT demonstrated CBT significantly reduced mental fatigue after <span class="stat-pill sp-blue">6 weeks</span> (p = 0.001). Benefits maintained at 6, 12, and 24 weeks across three independent studies. <a href="https://www.researchgate.net/publication/259719789" class="cref" target="\_blank" rel="noopener noreferrer">6</a></p>

# &#x20;         <p>Meta-analysis for ADHD adults: significant decreases in core symptoms, depression, and anxiety — medium-to-large effect sizes. CBT targets the catastrophic beliefs about cognitive ability that maintain avoidance and reinforce mental fatigue. <a href="https://bpspsychub.onlinelibrary.wiley.com/doi/10.1111/papt.12455" class="cref" target="\_blank" rel="noopener noreferrer">3</a></p>

# &#x20;         <div class="callout c-green"><span class="callout-i">✓</span><span>CBT combined with cognitive rehabilitation shows the most robust long-term profile. First-line for ADHD brain fog, post-illness fatigue, Long COVID cognitive symptoms, and depression-adjacent decline.</span></div>

# &#x20;       </div>

# &#x20;     </div>

# 

# &#x20;     <div class="acc">

# &#x20;       <button class="acc-btn" onclick="toggleAcc(this)">

# &#x20;         <span class="acc-icon">⚡</span>

# &#x20;         <span class="acc-title">Behavioural Activation (BA)</span>

# &#x20;         <svg class="acc-chev" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 9l6 6 6-6"/></svg>

# &#x20;       </button>

# &#x20;       <div class="acc-body">

# &#x20;         <p>BA significantly improved depressive symptoms and reward sensitivity (NIMH Science of Behavior Change program). Measurable increases in motivation within 1–2 weeks via activity scheduling. <a href="https://pubmed.ncbi.nlm.nih.gov/38128402/" class="cref" target="\_blank" rel="noopener noreferrer">7</a></p>

# &#x20;         <p>Mobile-app-delivered psychoeducation about BA principles provided protective benefits against depression onset over <span class="stat-pill sp-blue">3 months</span>. Meta-analysis SMDs: <span class="stat-pill sp-blue">0.45–0.78</span> across outcome measures. <a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC2882847/" class="cref" target="\_blank" rel="noopener noreferrer">8</a></p>

# &#x20;         <div class="callout c-blue"><span class="callout-i">🔬</span><span><strong>BA vs MBCT for anhedonia:</strong> A parallel-arm RCT found BATA (Behavioral Activation Treatment for Anhedonia) and MBCT were both effective and did not differ significantly on primary outcomes — both are valid first-line choices for motivational deficits. <a href="https://www.sciencedirect.com/science/article/pii/S0005796724001475" class="cref" target="\_blank" rel="noopener noreferrer">9</a></span></div>

# &#x20;       </div>

# &#x20;     </div>

# 

# &#x20;     <div class="acc">

# &#x20;       <button class="acc-btn" onclick="toggleAcc(this)">

# &#x20;         <span class="acc-icon">🎯</span>

# &#x20;         <span class="acc-title">Cognitive Training \&amp; Rehabilitation</span>

# &#x20;         <svg class="acc-chev" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 9l6 6 6-6"/></svg>

# &#x20;       </button>

# &#x20;       <div class="acc-body">

# &#x20;         <p>Cognitive rehabilitation for post-COVID brain fog: significant improvements in self-reported cognitive skills and functional performance in survivors. <a href="https://pubmed.ncbi.nlm.nih.gov/39993494/" class="cref" target="\_blank" rel="noopener noreferrer">10</a></p>

# &#x20;         <p>Computerised rehabilitation targeting attention and executive function in acquired brain injury: significant improvements in sustained attention, working memory, and cognitive flexibility. Strategy-based rehabilitation in childhood brain tumour survivors also shows promise. <a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC12537419/" class="cref" target="\_blank" rel="noopener noreferrer">11</a></p>

# &#x20;         <div class="callout c-amber"><span class="callout-i">⚠️</span><span>Generalisation of lab-based cognitive training gains to everyday functioning remains debated. Ecological validity is stronger in rehabilitation programmes than abstract brain training apps.</span></div>

# &#x20;       </div>

# &#x20;     </div>

# 

# &#x20;   </div>

# &#x20; </div>

# </section>

# 

# <!-- ▸ PHARMACOLOGICAL -->

# <section id="pharmacological" class="alt">

# &#x20; <div class="wrap">

# &#x20;   <div class="eyebrow blue fu">Pharmacological</div>

# &#x20;   <h2 class="fu">Evidence-Based Drug Interventions</h2>

# &#x20;   <p class="lead fu" style="margin-bottom:28px;">All findings from independently funded RCTs. Medical supervision and individualised dosing are mandatory.</p>

# &#x20;   <div class="callout c-red fu" style="margin-bottom:32px;">

# &#x20;     <span class="callout-i">⚠️</span>

# &#x20;     <span>All pharmacological interventions require consultation with a qualified physician. The evidence below is informational only. Self-prescribing is dangerous and in most jurisdictions illegal.</span>

# &#x20;   </div>

# &#x20;   <div class="g2 fu" style="margin-bottom:20px;">

# &#x20;     <div class="card blue">

# &#x20;       <div class="icon-wrap iw-blue">⚙️</div>

# &#x20;       <h4 style="margin-bottom:6px;">Psychostimulants — Focus \&amp; Drive</h4>

# &#x20;       <p style="font-size:0.84rem;">Methylphenidate increases willingness to perform effortful tasks (EEfRT), directly improving motivation. Amphetamines and modafinil reduce fatigue. Systematic review (non-industry funded) shows moderate effect sizes vs placebo. <a href="https://www.sciencedirect.com/science/article/pii/S0890856724003046" class="cref" target="\_blank" rel="noopener noreferrer">4</a></p>

# &#x20;     </div>

# &#x20;     <div class="card blue">

# &#x20;       <div class="icon-wrap iw-blue">🛡️</div>

# &#x20;       <h4 style="margin-bottom:6px;">Guanfacine XR — Non-Stimulant Option</h4>

# &#x20;       <p style="font-size:0.84rem;">Selective α2A-adrenergic agonist. Multiple NIH-funded RCTs confirmed efficacy for ADHD, working memory, and executive control. Being investigated for Long COVID brain fog. Safe alternative for stimulant-intolerant individuals. <a href="https://pubmed.ncbi.nlm.nih.gov/18166547/" class="cref" target="\_blank" rel="noopener noreferrer">12</a></p>

# &#x20;     </div>

# &#x20;   </div>

# &#x20;   <div class="acc-wrap fu">

# 

# &#x20;     <div class="acc">

# &#x20;       <button class="acc-btn" onclick="toggleAcc(this)">

# &#x20;         <span class="acc-icon">⚙️</span>

# &#x20;         <span class="acc-title">Methylphenidate — ADHD, Long COVID \&amp; Fatigue</span>

# &#x20;         <svg class="acc-chev" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 9l6 6 6-6"/></svg>

# &#x20;       </button>

# &#x20;       <div class="acc-body">

# &#x20;         <p>Objectively increases willingness to expend cognitive effort (EEfRT task) — direct causal evidence for catecholamine role in incentive motivation. Reduced reaction time, improved sustained attention in ADHD and Parkinson's disease RCTs. Studied for Long COVID cognitive symptoms. <a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC6628703/" class="cref" target="\_blank" rel="noopener noreferrer">13</a></p>

# &#x20;         <div class="callout c-amber"><span class="callout-i">⚠️</span><span>Monitor for cardiovascular effects, hypertension, and dependency risk. Not appropriate for unsupervised use.</span></div>

# &#x20;       </div>

# &#x20;     </div>

# 

# &#x20;     <div class="acc">

# &#x20;       <button class="acc-btn" onclick="toggleAcc(this)">

# &#x20;         <span class="acc-icon">🌙</span>

# &#x20;         <span class="acc-title">Modafinil — Fatigue \&amp; Wakefulness</span>

# &#x20;         <svg class="acc-chev" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 9l6 6 6-6"/></svg>

# &#x20;       </button>

# &#x20;       <div class="acc-body">

# &#x20;         <p>Phase III RCT: significantly improved cognitive performance and reduced fatigue maintained over <span class="stat-pill sp-blue">12 weeks</span>. Evidence also for depression- and cancer-related fatigue. <a href="https://www.sciencedirect.com/science/article/abs/pii/S0165178108001935" class="cref" target="\_blank" rel="noopener noreferrer">14</a></p>

# &#x20;       </div>

# &#x20;     </div>

# 

# &#x20;     <div class="acc">

# &#x20;       <button class="acc-btn" onclick="toggleAcc(this)">

# &#x20;         <span class="acc-icon">💙</span>

# &#x20;         <span class="acc-title">Bupropion — Fatigue, Lethargy \&amp; Low Drive</span>

# &#x20;         <svg class="acc-chev" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 9l6 6 6-6"/></svg>

# &#x20;       </button>

# &#x20;       <div class="acc-body">

# &#x20;         <p>Dopaminergic/noradrenergic mechanism. Most effective for hypersomnia, increased appetite, and fatigue profiles. Advantages over SSRIs for sleepiness and fatigue resolution. Studies in MS-related fatigue. Energising antidepressant — even outside diagnosed depression context. <a href="https://journals.sagepub.com/doi/10.1177/0269881113514878" class="cref" target="\_blank" rel="noopener noreferrer">15</a></p>

# &#x20;       </div>

# &#x20;     </div>

# 

# &#x20;   </div>

# &#x20; </div>

# </section>

# 

# <!-- ▸ MINDFULNESS -->

# <section id="mindfulness">

# &#x20; <div class="wrap">

# &#x20;   <div class="eyebrow blue fu">Mindfulness \&amp; Psychology</div>

# &#x20;   <h2 class="fu">MBSR, Meditation \&amp; Placebo Effects</h2>

# &#x20;   <p class="lead fu" style="margin-bottom:36px;">The highest-ranked non-pharmacological intervention for focus and brain fog — with a growing neurophysiological evidence base and strong non-commercial funding.</p>

# 

# &#x20;   <div class="split fu">

# &#x20;     <div>

# &#x20;       <h3 style="margin-bottom:14px;">Mindfulness-Based Stress Reduction</h3>

# &#x20;       <p style="margin-bottom:12px;font-size:0.88rem;">Meta-analysis of <span class="stat-pill sp-blue">85+ controlled trials</span> demonstrates MBSR improves long-term mental fatigue, concentration, sustained vigilance, inhibition of distraction, and flexible attention shifting. <a href="https://link.springer.com/article/10.1007/s44202-024-00162-1" class="cref" target="\_blank" rel="noopener noreferrer">2</a></p>

# &#x20;       <p style="margin-bottom:14px;font-size:0.88rem;">A lower level of mental fatigue was associated with lower cortisol concentrations in participants undergoing mindfulness training — a key biological confirmation of the mechanism. Even brief sessions produce immediate attentional improvements. <a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC3541487/" class="cref" target="\_blank" rel="noopener noreferrer">16</a></p>

# &#x20;       <div class="g2" style="gap:10px;margin-bottom:18px;">

# &#x20;         <div class="card" style="padding:14px;">

# &#x20;           <h4 style="font-size:0.83rem;margin-bottom:5px;">Focused Attention (FA)</h4>

# &#x20;           <p style="font-size:0.77rem;">Activates bilateral dlPFC. Increases working memory in novices after short training. Builds sustained vigilance. <a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC8413779/" class="cref" target="\_blank" rel="noopener noreferrer">17</a></p>

# &#x20;         </div>

# &#x20;         <div class="card" style="padding:14px;">

# &#x20;           <h4 style="font-size:0.83rem;margin-bottom:5px;">Open Monitoring (OM)</h4>

# &#x20;           <p style="font-size:0.77rem;">3-armed RCT: significant improvements in cognitive flexibility and attention regulation via distinct neurocognitive mechanism. <a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC9286350/" class="cref" target="\_blank" rel="noopener noreferrer">18</a></p>

# &#x20;         </div>

# &#x20;       </div>

# &#x20;       <h3 style="margin-bottom:12px;">Clinical Hypnosis</h3>

# &#x20;       <p style="font-size:0.88rem;">Meta-analysis: hypnosis reduces mental fatigue and improves cognitive clarity. A single personalised session enhanced stress regulation and cognitive performance under load. Can be used alongside mindfulness as complementary intervention. <a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC10759527/" class="cref" target="\_blank" rel="noopener noreferrer">19</a></p>

# &#x20;     </div>

# &#x20;     <div>

# &#x20;       <div class="callout c-blue" style="margin-bottom:14px;">

# &#x20;         <span class="callout-i">🧪</span>

# &#x20;         <div><strong>Placebo is pharmacologically real.</strong> In major depression trials, placebo accounts for approximately <span class="stat-pill sp-blue">68–75%</span> of the total antidepressant response (Kirsch meta-analysis of FDA trial data; independent 96-trial meta-analysis, d = 1.69 placebo vs 2.50 drug). Expectation activates PFC, hippocampus, and endogenous opioid pathways — these are measurable neurobiological events, not imagined responses. <a href="https://academic.oup.com/book/27010/chapter/196244634" class="cref" target="\_blank" rel="noopener noreferrer">20</a></div>

# &#x20;       </div>

# &#x20;       <div class="card" style="margin-bottom:12px;">

# &#x20;         <h4 style="margin-bottom:10px;">Placebo mechanisms in cognition</h4>

# &#x20;         <ul class="clist cl-blue">

# &#x20;           <li>Placebo pill intake improves actual memory and attention in blinded RCTs</li>

# &#x20;           <li>Open-label placebos also show positive effects — even when patients know they are inert</li>

# &#x20;           <li>Self-induced placebo enhanced by mental imagery and perceived control</li>

# &#x20;           <li>SF-36 vitality scores improved following MBSR — linked to placebo-mediated expectation</li>

# &#x20;         </ul>

# &#x20;       </div>

# &#x20;       <div class="callout c-amber">

# &#x20;         <span class="callout-i">⚠️</span>

# &#x20;         <div><strong>Nocebo warning:</strong> Verbal nocebo information measurably <em>increases</em> experienced cognitive fatigue. How you frame an intervention to yourself matters — negative framing is a real performance cost. <a href="https://www.sciencedirect.com/science/article/pii/S0005791621000215" class="cref" target="\_blank" rel="noopener noreferrer">21</a></div>

# &#x20;       </div>

# &#x20;       <div class="callout c-rose" style="margin-top:10px;">

# &#x20;         <span class="callout-i">🌸</span>

# &#x20;         <div><strong>Female note:</strong> MBIs significantly improve cognitive function in breast cancer survivors and older adults with subjective cognitive impairment. Particularly effective for menopausal brain fog when combined with fatigue education. <a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC6260900/" class="cref" target="\_blank" rel="noopener noreferrer">22</a></div>

# &#x20;       </div>

# &#x20;     </div>

# &#x20;   </div>

# &#x20; </div>

# </section>

# 

# <!-- ═══════════════════════════════

# &#x20;    EDC \& ENDOCRINE DISRUPTION (NEW)

# ═══════════════════════════════ -->

# <section id="edc" class="stone">

# &#x20; <div class="wrap">

# &#x20;   <div class="eyebrow rose fu">Endocrine Disruption</div>

# &#x20;   <h2 class="fu">EDCs, Microplastics \&amp; Hormonal Disruption</h2>

# &#x20;   <p class="lead fu" style="margin-bottom:36px;">

# &#x20;     Endocrine-disrupting chemicals (EDCs) are pervasive in modern environments. Research now shows clear causal links to reproductive disorders, PCOS, premature ovarian insufficiency, and male testicular damage — with alarming odds ratios from population-level studies.

# &#x20;   </p>

# 

# &#x20;   <!-- Key stats -->

# &#x20;   <div class="g4 fu" style="margin-bottom:32px;">

# &#x20;     <div class="card rose" style="text-align:center;padding:18px 14px;">

# &#x20;       <div style="font-family:'Libre Baskerville',serif;font-size:2rem;font-weight:700;color:var(--rose);">OR \~3.8</div>

# &#x20;       <div style="font-size:0.76rem;color:var(--muted);margin-top:4px;">Cadmium → PCOS risk<br><span style="font-size:0.68rem;">(systematic review; cadmium consistently elevated in PCOS across multiple studies)</span></div>

# &#x20;     </div>

# &#x20;     <div class="card rose" style="text-align:center;padding:18px 14px;">

# &#x20;       <div style="font-family:'Libre Baskerville',serif;font-size:2rem;font-weight:700;color:var(--rose);">OR 3.4</div>

# &#x20;       <div style="font-size:0.76rem;color:var(--muted);margin-top:4px;">Phthalates → POI risk<br><span style="font-size:0.68rem;">(premature ovarian insufficiency)</span></div>

# &#x20;     </div>

# &#x20;     <div class="card amber" style="text-align:center;padding:18px 14px;">

# &#x20;       <div style="font-family:'Libre Baskerville',serif;font-size:2rem;font-weight:700;color:var(--amber);">1%</div>

# &#x20;       <div style="font-size:0.76rem;color:var(--muted);margin-top:4px;">Women with POI by age 40<br><span style="font-size:0.68rem;">(rising with EDC exposure)</span></div>

# &#x20;     </div>

# &#x20;     <div class="card green" style="text-align:center;padding:18px 14px;">

# &#x20;       <div style="font-family:'Libre Baskerville',serif;font-size:2rem;font-weight:700;color:var(--green);">600+</div>

# &#x20;       <div style="font-size:0.76rem;color:var(--muted);margin-top:4px;">Genes regulated by Nrf2<br><span style="font-size:0.68rem;">(activated by sulforaphane)</span></div>

# &#x20;     </div>

# &#x20;   </div>

# 

# &#x20;   <div class="split fu">

# &#x20;     <div>

# &#x20;       <div class="sex-badge sb-female">♀ Female-specific mechanisms</div>

# &#x20;       <h3 style="margin-bottom:12px;">Reproductive \&amp; Ovarian Damage</h3>

# &#x20;       <p style="font-size:0.88rem;margin-bottom:14px;">EDCs interfere with the hypothalamic-pituitary-gonadal (HPG) axis through multiple pathways. BPA mimics oestrogen (oestrogen receptor α binding), directly suppressing StAR and CYP11A1 — enzymes essential for oestradiol synthesis. Phthalates increase pro-apoptotic Bax while reducing Bcl-2, driving follicular atresia.</p>

# &#x20;       <div class="steps">

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-rose">BPA</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>BPA/BPS/BPF — Oestrogen Mimicry</h4>

# &#x20;             <p>Binds ERα, suppresses StAR \&amp; CYP11A1. Impairs oocyte maturation and implantation. Even "BPA-free" plastics contain BPS/BPF with similar activity. PCOS, POI, implantation failure.</p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-rose">PCB</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>PCBs, DDT, PFASs — Persistent Accumulation</h4>

# &#x20;             <p>Accumulate in ovarian stromal tissue. Alter steroidogenesis gene expression via miRNA modification. Associated with diminished ovarian reserve and earlier menopause.</p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-rose">Cd</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>Cadmium — Strongest PCOS Signal</h4>

# &#x20;             <p>Highest vs lowest urinary quartile OR \~3.8 for PCOS in one systematic review; consistently elevated across 15 independent studies. Acts as a metalloestrogen. DNA damage, mitochondrial dysfunction, direct granulosa cell apoptosis. Primary sources: cigarette smoke, contaminated rice/food.</p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-rose">Air</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>PM2.5 / NO₂ — Ovarian Reserve</h4>

# &#x20;             <p>Large cohort (<span class="stat-pill sp-rose">2,200 women</span>): long-term PM2.5 exposure significantly reduced AMH and antral follicle count — established markers of ovarian reserve. Systemic oxidative stress disrupts folliculogenesis. Exposure during <em>critical stages of follicle development</em> is particularly damaging.</p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;       </div>

# &#x20;     </div>

# &#x20;     <div>

# &#x20;       <div class="sex-badge sb-male">♂ Male-specific mechanisms</div>

# &#x20;       <h3 style="margin-bottom:12px;">Testicular Toxicity</h3>

# &#x20;       <p style="font-size:0.88rem;margin-bottom:14px;">Microplastics have been detected in human testicular tissue at <span class="stat-pill sp-amber">11.60 ± 15.52 particles/g</span> and semen at <span class="stat-pill sp-amber">0.23 ± 0.45 particles/mL</span>. This drives testicular inflammation, blood-testis barrier disruption, and ferroptosis of germ cells.</p>

# &#x20;       <div class="steps">

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-amber">ROS</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>Oxidative Stress</h4>

# &#x20;             <p>MPs generate ROS → lipid peroxidation, DNA strand breaks, germ cell apoptosis — directly impairing testosterone synthesis in Leydig cells.</p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-amber">IL6</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>Inflammation</h4>

# &#x20;             <p>MP accumulation triggers IL-6, TNF-α in testicular tissue → disrupts Leydig and Sertoli cell function and spermatogenesis.</p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-amber">EDC</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>Endocrine Disruption</h4>

# &#x20;             <p>MPs act as vectors delivering phthalates/bisphenols directly into testicular tissue. Leachates interfere with androgen receptors and HPG signalling.</p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-amber">BTB</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>Blood-Testis Barrier</h4>

# &#x20;             <p>Tight junction proteins compromised → immune infiltration of the immune-privileged testicular environment → autoimmune-like germ cell damage.</p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;       </div>

# &#x20;       <div class="callout c-green" style="margin-top:14px;">

# &#x20;         <span class="callout-i">🧬</span>

# &#x20;         <div><strong>Transgenerational impact (alarming finding):</strong> EDC-induced epigenetic changes can be passed to offspring. In the Seveso Women's Health Study, daughters of women exposed to dioxin (TCDD) in 1976 also experienced delays in time to pregnancy — despite never being directly exposed. Prenatal DEHP exposure in mice accelerated reproductive aging in the F3 generation (great-grandchildren).</div>

# &#x20;       </div>

# &#x20;     </div>

# &#x20;   </div>

# 

# &#x20;   <!-- EDC Table -->

# &#x20;   <div class="tbl-wrap fu" style="margin-top:32px;">

# &#x20;     <table>

# &#x20;       <thead>

# &#x20;         <tr>

# &#x20;           <th>Chemical / Class</th>

# &#x20;           <th>Primary Sources</th>

# &#x20;           <th>Mechanism</th>

# &#x20;           <th>Key Outcome</th>

# &#x20;           <th>Applies To</th>

# &#x20;         </tr>

# &#x20;       </thead>

# &#x20;       <tbody>

# &#x20;         <tr>

# &#x20;           <td>BPA / BPS / BPF</td>

# &#x20;           <td>Food packaging, thermal paper, plastic bottles</td>

# &#x20;           <td>ERα agonism; ↓StAR \&amp; CYP11A1; oocyte maturation impairment</td>

# &#x20;           <td>PCOS, POI, implantation failure</td>

# &#x20;           <td><span class="pill pill-rose">♀</span></td>

# &#x20;         </tr>

# &#x20;         <tr>

# &#x20;           <td>Phthalates (DEHP, DBP)</td>

# &#x20;           <td>PVC plastics, cosmetics, personal care, fragrances</td>

# &#x20;           <td>↑Bax, ↓Bcl-2 in follicles; follicular atresia; oxidative stress</td>

# &#x20;           <td>POI (OR 3.4), infertility, PCOS</td>

# &#x20;           <td><span class="pill pill-rose">♀</span></td>

# &#x20;         </tr>

# &#x20;         <tr>

# &#x20;           <td>Cadmium (Cd)</td>

# &#x20;           <td>Cigarette smoke, contaminated food/water, industrial</td>

# &#x20;           <td>Metalloestrogen; DNA damage; mitochondrial dysfunction; granulosa cell apoptosis</td>

# &#x20;           <td>PCOS (OR 3.8), ovarian damage</td>

# &#x20;           <td><span class="pill pill-rose">♀</span> <span class="pill pill-blue">♂</span></td>

# &#x20;         </tr>

# &#x20;         <tr>

# &#x20;           <td>PCBs / DDT / PFASs</td>

# &#x20;           <td>Pesticides, non-stick cookware, industrial chemicals</td>

# &#x20;           <td>Accumulate in ovarian tissue; alter miRNA; disrupt steroidogenesis</td>

# &#x20;           <td>Diminished ovarian reserve, early menopause</td>

# &#x20;           <td><span class="pill pill-rose">♀</span></td>

# &#x20;         </tr>

# &#x20;         <tr>

# &#x20;           <td>PM2.5 / NO₂ (air pollution)</td>

# &#x20;           <td>Traffic, industrial emissions</td>

# &#x20;           <td>Systemic oxidative stress; ↓AMH; ↓antral follicle count</td>

# &#x20;           <td>Reduced ovarian reserve (2,200-woman cohort)</td>

# &#x20;           <td><span class="pill pill-rose">♀</span></td>

# &#x20;         </tr>

# &#x20;         <tr>

# &#x20;           <td>Microplastics</td>

# &#x20;           <td>Food packaging, drinking water, dust, seafood</td>

# &#x20;           <td>Testicular inflammation; BTB disruption; ferroptosis; ROS generation</td>

# &#x20;           <td>Sperm dysfunction, ↓testosterone, ↓fertility</td>

# &#x20;           <td><span class="pill pill-blue">♂</span></td>

# &#x20;         </tr>

# &#x20;         <tr>

# &#x20;           <td>Melatonin disruption (MTNR1B variant)</td>

# &#x20;           <td>Light at night; insufficient darkness</td>

# &#x20;           <td>Impaired circadian-gonadal axis; altered LH pulsatility</td>

# &#x20;           <td>↑PCOS risk; impaired folliculogenesis</td>

# &#x20;           <td><span class="pill pill-rose">♀</span></td>

# &#x20;         </tr>

# &#x20;       </tbody>

# &#x20;     </table>

# &#x20;   </div>

# 

# &#x20;   <!-- Practical reduction -->

# &#x20;   <div class="callout c-green fu" style="margin-top:24px;">

# &#x20;     <span class="callout-i">🛡️</span>

# &#x20;     <div><strong>Highest-leverage EDC reduction actions:</strong> (1) Switch food storage to glass or stainless steel. (2) Never heat food in plastic. (3) Filter drinking water (reverse osmosis or activated carbon). (4) Choose phthalate-free, fragrance-free personal care products. (5) Avoid thermal paper receipts. (6) Reduce canned food consumption (BPA-lined cans). (7) Choose organic produce for the "Dirty Dozen."</div>

# &#x20;   </div>

# &#x20;   <div class="callout c-amber fu" style="margin-top:10px;">

# &#x20;     <span class="callout-i">⚠️</span>

# &#x20;     <div><strong>"BPA-free" is not safe:</strong> While traditional EDC concentrations showed declining trends in population studies, concentrations of <strong>bisphenol S (BPS), bisphenol F (BPF), and DINCH metabolites</strong> are increasing — with comparable or greater reproductive toxicity to BPA. Replace plastics entirely, not just BPA-labelled ones.</div>

# &#x20;   </div>

# &#x20;   <div class="callout c-rose fu" style="margin-top:10px;">

# &#x20;     <span class="callout-i">🔬</span>

# &#x20;     <div><strong>Microplastics in follicular fluid (2024 data):</strong> Microplastics \&lt;10 µm were detected in follicular fluid of 14 out of 18 women undergoing IVF, raising direct concerns about their biochemical interactions with maturing oocytes. Reduction of ongoing exposure is the only currently actionable strategy.</div>

# &#x20;   </div>

# &#x20; </div>

# </section>

# 

# <!-- ▸ HORMONAL -->

# <section id="hormonal">

# &#x20; <div class="wrap">

# &#x20;   <div class="eyebrow amber fu">Hormonal Optimisation</div>

# &#x20;   <h2 class="fu">Testosterone \&amp; Oestrogen — <em class="serif">Endogenous Support</em></h2>

# 

# &#x20;   <div class="split fu">

# &#x20;     <div>

# &#x20;       <div class="sex-badge sb-male">♂ Male</div>

# &#x20;       <h3 style="margin-bottom:12px;">Testosterone Upregulation</h3>

# &#x20;       <p style="font-size:0.88rem;margin-bottom:14px;">Dietary and lifestyle interventions that support endogenous testosterone production — no exogenous hormones. Works through insulin sensitivity, inflammation reduction, and mitochondrial biogenesis in Leydig cells.</p>

# &#x20;       <div class="callout c-amber" style="margin-bottom:14px;">

# &#x20;         <span class="callout-i">ℹ️</span>

# &#x20;         <span>Evidence primarily from young adult male populations. All interventions work via endogenous mechanisms. <a href="https://www.sciencedirect.com/science/article/pii/S2666914524000663" class="cref" target="\_blank" rel="noopener noreferrer">23</a></span>

# &#x20;       </div>

# &#x20;       <div class="callout c-rose" style="margin-bottom:14px;">

# &#x20;         <span class="callout-i">⚠️</span>

# &#x20;         <div><strong>Rapid weight loss caution:</strong> Very-low-calorie diets and bariatric surgery improve testosterone and fertility — but rapid adipose catabolism mobilises stored lipophilic toxicants (EDCs, PFASs) from fat tissue. This transiently elevates circulating pollutant concentrations and may increase susceptibility to their endocrine-disrupting effects. Favour gradual fat loss (0.5–1% body weight/week) combined with Nrf2 activation (cruciferous vegetables) to buffer this effect.</div>

# &#x20;       </div>

# &#x20;       <ul class="clist cl-amber">

# &#x20;         <li>Mediterranean diet: high MUFA and omega-3s support Leydig cell steroidogenesis</li>

# &#x20;         <li>TRF 16:8/18:6: ↑GH pulses during fast, ↑AMPK/PGC-1α → mitochondrial biogenesis</li>

# &#x20;         <li>Resistance training: acutely raises testosterone — compound lifts most effective</li>

# &#x20;         <li>Adequate sleep 7–9h: testosterone peaks in early AM; poor sleep reduces it by up to 15%</li>

# &#x20;         <li>Low-fat diets negatively correlate with testosterone regardless of BMI — prioritise healthy fats</li>

# &#x20;         <li>Reduce microplastic exposure: MPs detected in testicular tissue at detectable levels</li>

# &#x20;       </ul>

# &#x20;     </div>

# &#x20;     <div>

# &#x20;       <div class="sex-badge sb-female">♀ Female</div>

# &#x20;       <h3 style="margin-bottom:12px;">PCOS, Ovarian Reserve \&amp; Fertility</h3>

# &#x20;       <p style="font-size:0.88rem;margin-bottom:14px;">Dietary interventions for PCOS primarily work through insulin sensitivity improvement, reduction of hyperandrogenism, and restoration of ovulatory function. Weight loss as little as 5–10% can restore ovulatory cycles.</p>

# &#x20;       <div class="callout c-amber" style="margin-bottom:12px;">

# &#x20;         <span class="callout-i">⚠️</span>

# &#x20;         <div><strong>Rapid weight loss: hidden EDC risk.</strong> Rapid fat mobilisation (bariatric surgery, VLCD) transiently elevates circulating lipophilic toxicants — including EDCs and PFASs stored in adipose tissue. This may temporarily increase susceptibility to ovarian effects. Gradual, sustained weight loss is preferred over crash dieting.</div>

# &#x20;       </div>

# &#x20;       <div class="g2" style="gap:10px;">

# &#x20;         <div class="card rose" style="padding:16px;">

# &#x20;           <h4 style="font-size:0.84rem;margin-bottom:6px;">Weight Loss — Most Potent PCOS Intervention</h4>

# &#x20;           <p style="font-size:0.78rem;">5–10% body weight reduction restores ovulatory function in overweight women with PCOS via improved insulin sensitivity, increased SHBG, and normalised LH pulsatility. Bariatric surgery and very-low-calorie diets both show dramatic fertility improvements — but rapid fat loss transiently mobilises stored lipophilic EDCs. Favour gradual loss with Nrf2 support. <a href="https://www.mdpi.com/2072-6643/17/4/674" class="cref" target="\_blank" rel="noopener noreferrer">27</a></p>

# &#x20;         </div>

# &#x20;           <p style="font-size:0.78rem;">Significantly reduces total testosterone, LH, and free androgen index. ↑FSH, ↑SHBG, ↑AMH in PCOS patients. Low-GI diets also show <strong>higher fertility rates</strong> vs control diets. Calorie-restricted DASH and ketogenic diets show similar benefits — though benefit may partly arise from the caloric deficit itself rather than macronutrient composition. <a href="https://www.mdpi.com/2072-6643/16/21/3659" class="cref" target="\_blank" rel="noopener noreferrer">24</a></p>

# &#x20;         </div>

# &#x20;         <div class="card rose" style="padding:16px;">

# &#x20;           <h4 style="font-size:0.84rem;margin-bottom:6px;">Fasting in Women</h4>

# &#x20;           <p style="font-size:0.78rem;">⚠️ Fasting protocols \&gt;16h have limited female-specific evidence and may impair HPA axis function. Hair follicle stem cell apoptosis confirmed in mouse models; 18% slower regrowth in one human trial. <strong>Start with 14:10</strong>. If experiencing cycle irregularities or hair loss, reduce or pause fasting. <a href="https://www.nature.com/articles/s41366-024-01680-7" class="cref" target="\_blank" rel="noopener noreferrer">25</a></p>

# &#x20;         </div>

# &#x20;         <div class="card rose" style="padding:16px;">

# &#x20;           <h4 style="font-size:0.84rem;margin-bottom:6px;">Melatonin (DOR)</h4>

# &#x20;           <p style="font-size:0.78rem;">3 mg RCT in diminished ovarian reserve: ↑oestradiol, ↑mature MII oocytes — but <strong>no significant improvement in clinical pregnancy rates</strong> (6.2% vs 2.9%, p=NS). Useful as ovarian antioxidant; not a primary fertility driver. <a href="https://www.sciencedirect.com/science/article/pii/S0005796724001475" class="cref" target="\_blank" rel="noopener noreferrer">26</a></p>

# &#x20;         </div>

# &#x20;         <div class="card rose" style="padding:16px;">

# &#x20;           <h4 style="font-size:0.84rem;margin-bottom:6px;">Omega-3 \&amp; Anti-inflammatory</h4>

# &#x20;           <p style="font-size:0.78rem;">EPA/DHA reduces ovarian inflammation, supports folliculogenesis, and may improve IVF outcomes. 2–3 servings fatty fish/week or supplementation is the practical target. <a href="https://www.mdpi.com/2072-6643/16/21/3659" class="cref" target="\_blank" rel="noopener noreferrer">24</a></p>

# &#x20;         </div>

# &#x20;       </div>

# &#x20;     </div>

# &#x20;   </div>

# &#x20; </div>

# </section>

# 

# <!-- ▸ FASTING -->

# <section id="fasting" class="alt">

# &#x20; <div class="wrap">

# &#x20;   <div class="eyebrow amber fu">Time-Restricted Feeding</div>

# &#x20;   <h2 class="fu">Intermittent Fasting \&amp; Metabolic Reprogramming</h2>

# &#x20;   <p class="lead fu" style="margin-bottom:36px;">TRF creates the metabolic conditions for optimal body composition, hormonal balance, and cellular renewal — without caloric restriction when calories are maintained within the eating window.</p>

# &#x20;   <div class="g3 fu" style="margin-bottom:28px;">

# &#x20;     <div class="card">

# &#x20;       <h4 style="margin-bottom:5px;">Body Composition</h4>

# &#x20;       <p style="font-size:0.83rem;">Systematic review of 15 studies: TRF significantly reduced body weight, BMI, and waist circumference. Average loss of <span class="stat-pill sp-amber">2.3 kg</span> over 12 weeks vs. controls. <a href="https://www.sciencedirect.com/science/article/pii/S2666914524000663" class="cref" target="\_blank" rel="noopener noreferrer">23</a></p>

# &#x20;     </div>

# &#x20;     <div class="card">

# &#x20;       <h4 style="margin-bottom:5px;">Insulin Sensitivity</h4>

# &#x20;       <p style="font-size:0.83rem;">HOMA-IR scores decreased by <span class="stat-pill sp-amber">15–20%</span> across multiple TRF studies. Improved insulin sensitivity directly supports testosterone production (males) and reduces hyperandrogenism (females with PCOS). <a href="https://www.nature.com/articles/s41366-024-01680-7" class="cref" target="\_blank" rel="noopener noreferrer">25</a></p>

# &#x20;     </div>

# &#x20;     <div class="card">

# &#x20;       <h4 style="margin-bottom:5px;">Cardiovascular Markers</h4>

# &#x20;       <p style="font-size:0.83rem;">Systolic BP ↓ <span class="stat-pill sp-amber">5–8 mmHg</span>, diastolic ↓ <span class="stat-pill sp-amber">3–5 mmHg</span>. Improved endothelial function correlates with better reproductive vascular supply. <a href="https://www.nature.com/articles/s41366-024-01680-7" class="cref" target="\_blank" rel="noopener noreferrer">25</a></p>

# &#x20;     </div>

# &#x20;   </div>

# &#x20;   <div class="acc-wrap fu">

# 

# &#x20;     <div class="acc">

# &#x20;       <button class="acc-btn" onclick="toggleAcc(this)">

# &#x20;         <span class="acc-icon">🔄</span>

# &#x20;         <span class="acc-title">Mechanisms — Autophagy, GH Pulses \&amp; Mitochondrial Biogenesis</span>

# &#x20;         <svg class="acc-chev" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 9l6 6 6-6"/></svg>

# &#x20;       </button>

# &#x20;       <div class="acc-body">

# &#x20;         <p>During fasting, reduced insulin activates AMPK and PGC-1α, stimulating mitochondrial biogenesis. New, efficient mitochondria improve Leydig cell energy production — the primary site of testosterone synthesis. AMPK also inhibits mTOR, triggering autophagy and cellular cleanup, including clearance of damaged organelles with neuroprotective effects.</p>

# &#x20;         <p>Growth hormone pulses increase substantially during fasting (especially overnight). GH promotes fat mobilisation, muscle protein synthesis, and directly supports testicular function. Frequent feeding blunts these pulsatile GH patterns. FGF21 signalling further activates hepatic autophagy and lipid degradation.</p>

# &#x20;         <div class="callout c-green"><span class="callout-i">✓</span><span>TRF enhances efficacy of resistance training in obese males. Protein intake of <span class="stat-pill sp-green">1.6–2.2 g/kg/day</span> maintains lean mass. <a href="https://www.sciencedirect.com/science/article/pii/S2666914524000663" class="cref" target="\_blank" rel="noopener noreferrer">23</a></span></div>

# &#x20;         <div class="callout c-amber"><span class="callout-i">🕐</span><span><strong>Early vs late TRE (new evidence):</strong> Early TRE (8:00 AM – 2:00 PM) was superior to delayed TRE (12:00 PM – 6:00 PM) for weight management when combined with resistance training. This aligns with circadian biology — the body processes carbohydrates more efficiently in the morning. Start flexible; optimise timing after adaptation.</span></div>

# &#x20;         <div class="callout c-blue"><span class="callout-i">⚙️</span><span><strong>SIRT1→testosterone link:</strong> Sirtuin 1-mediated autophagy directly regulates testosterone synthesis in Leydig cells. Fasting-induced SIRT1 activation is therefore not just metabolic — it directly feeds back into hormonal output via cellular quality control.</span></div>

# &#x20;         <div class="callout c-rose"><span class="callout-i">🌸</span><span><strong>Female caution:</strong> Aggressive fasting (\&gt;16h) triggers apoptosis in activated hair follicle stem cells (HFSCs) in dermal adipose tissue, pushing follicles into a prolonged telogen (resting) phase. One human study found <strong>18% slower hair regrowth</strong> on 18:6 fasting. If hair loss is a concern, reduce to 14:10 and consider early eating windows.</span></div>

# &#x20;       </div>

# &#x20;     </div>

# 

# &#x20;     <div class="acc">

# &#x20;       <button class="acc-btn" onclick="toggleAcc(this)">

# &#x20;         <span class="acc-icon">🫒</span>

# &#x20;         <span class="acc-title">Mediterranean Diet — Male \&amp; Female Mechanisms</span>

# &#x20;         <svg class="acc-chev" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 9l6 6 6-6"/></svg>

# &#x20;       </button>

# &#x20;       <div class="acc-body">

# &#x20;         <p><strong>Males:</strong> Olive oil (oleic acid + polyphenols) enhances testosterone production and sperm quality. Fatty fish EPA/DHA (<span class="stat-pill sp-amber">2–3 servings/week</span>) improves insulin sensitivity and reduces inflammation — the dual drivers of testosterone decline. Polyphenols from vegetables and legumes preserve HPG axis signalling. Observational data links a "prudent" Mediterranean-style pattern to better sperm quality and higher total sperm counts vs a Western dietary pattern. <a href="https://www.mdpi.com/2072-6643/16/21/3659" class="cref" target="\_blank" rel="noopener noreferrer">24</a></p>

# &#x20;         <p><strong>Females with PCOS:</strong> Meta-analyses of isocaloric RCTs show low-GI Mediterranean diets significantly reduce total testosterone, LH, and the free androgen index while increasing FSH and SHBG. Low-GI diets are also associated with higher fertility rates vs control diets. Calorie-restricted DASH and ketogenic diets show similar improvements — though the authors note that much of the benefit is likely tied to overall caloric reduction rather than macronutrient composition alone.</p>

# &#x20;         <div class="callout c-blue"><span class="callout-i">🔬</span><span><strong>Vitamin D \&amp; ovarian reserve:</strong> 4 out of 7 reviewed studies found significant associations between serum 25(OH)D concentration and ovarian reserve markers. Although heterogeneity prevents definitive conclusions, ensuring adequate Vitamin D is a low-risk, high-plausibility action given the mechanistic evidence.</span></div>

# &#x20;         <div class="callout c-amber"><span class="callout-i">⚠️</span><span>Low-fat diets are negatively correlated with testosterone in males regardless of BMI. Prioritise monounsaturated and polyunsaturated fats — avoid ultra-low-fat approaches.</span></div>

# &#x20;       </div>

# &#x20;     </div>

# 

# &#x20;   </div>

# &#x20; </div>

# </section>

# 

# <!-- ▸ DETOX -->

# <section id="detox">

# &#x20; <div class="wrap">

# &#x20;   <div class="eyebrow green fu">Detoxification Research</div>

# &#x20;   <h2 class="fu">Nrf2, Sulforaphane \&amp; Endogenous Detox</h2>

# &#x20;   <p class="lead fu" style="margin-bottom:36px;">Cruciferous vegetables activate a master transcription factor regulating 600+ detoxification genes — confirmed in human RCTs. Intermittent fasting concurrently clears cellular debris via autophagy.</p>

# 

# &#x20;   <div class="split fu">

# &#x20;     <div>

# &#x20;       <h3 style="margin-bottom:12px;">Nrf2 — The Master Detox Switch</h3>

# &#x20;       <p style="font-size:0.86rem;margin-bottom:12px;">Sulforaphane (SFN) reacts with <strong>Cysteine 151 on KEAP1</strong>, releasing Nrf2 for nuclear translocation. Nrf2 binds antioxidant response elements (AREs), inducing 600+ cytoprotective genes. C151 mutagenesis impaired NRF2 induction by <span class="stat-pill sp-green">75%</span> vs wild-type — confirming this as the critical sensor.</p>

# &#x20;       <div class="callout c-green" style="margin-bottom:14px;">

# &#x20;         <span class="callout-i">🔬</span>

# &#x20;         <div>Human RCT (n=<span class="stat-pill sp-green">291</span>): broccoli sprout beverage ↑ benzene excretion by <span class="stat-pill sp-green">61%</span>, acrolein by <span class="stat-pill sp-green">23%</span>. Broccoli sprouts contain 10–100× more glucoraphanin than mature broccoli.</div>

# &#x20;       </div>

# &#x20;       <div class="card" style="margin-bottom:12px;">

# &#x20;         <h4 style="margin-bottom:10px;">Enzymes induced by sulforaphane</h4>

# &#x20;         <div class="g2" style="gap:12px;">

# &#x20;           <div>

# &#x20;             <p style="font-size:0.72rem;font-weight:700;color:var(--green);margin-bottom:5px;text-transform:uppercase;letter-spacing:.05em;">Phase II Detox</p>

# &#x20;             <ul class="clist cl-green" style="font-size:0.79rem;">

# &#x20;               <li>UDP-glucuronosyltransferases (UGTs)</li>

# &#x20;               <li>Glutathione S-transferases (GSTs)</li>

# &#x20;               <li>Sulfotransferases (SULTs)</li>

# &#x20;               <li>N-acetyltransferases (NATs)</li>

# &#x20;             </ul>

# &#x20;           </div>

# &#x20;           <div>

# &#x20;             <p style="font-size:0.72rem;font-weight:700;color:var(--green);margin-bottom:5px;text-transform:uppercase;letter-spacing:.05em;">Antioxidant</p>

# &#x20;             <ul class="clist cl-green" style="font-size:0.79rem;">

# &#x20;               <li>Heme oxygenase 1 (HO-1)</li>

# &#x20;               <li>NQO1 (quinone reductase)</li>

# &#x20;               <li>Glutathione reductase (GSR)</li>

# &#x20;               <li>Thioredoxin reductase (TrxR)</li>

# &#x20;             </ul>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;       </div>

# &#x20;       <div class="callout c-rose">

# &#x20;         <span class="callout-i">🌸</span>

# &#x20;         <div><strong>Female protective benefit:</strong> Nrf2 activation via sulforaphane has been shown to protect ovarian tissue from BaP, DBP, phthalate, and chemotherapy-induced oxidative damage. Melatonin also provides antioxidant protection to maturing follicles.</div>

# &#x20;       </div>

# &#x20;     </div>

# &#x20;     <div>

# &#x20;       <h3 style="margin-bottom:12px;">Practical Sulforaphane Protocol</h3>

# &#x20;       <div class="steps">

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-green">01</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>Choose Sprouts Over Mature Broccoli</h4>

# &#x20;             <p>50–100g broccoli sprouts daily = 150–200g broccoli equivalent for sulforaphane. Sprouts contain 10–100× more glucoraphanin.</p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-green">02</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>Preserve Myrosinase Activity</h4>

# &#x20;             <p>Myrosinase converts glucoraphanin to sulforaphane — it is heat-sensitive. Eat sprouts raw. If cooking broccoli: lightly steam (3–4 min max) and allow to rest before eating. Add raw mustard seed powder to cooked broccoli to restore myrosinase.</p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-green">03</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>Synergistic Nrf2 Activators</h4>

# &#x20;             <p>Pair with turmeric/curcumin, EGCG (green tea), resveratrol (red grapes), allicin (garlic), and quercetin (onions). All activate the KEAP1-Nrf2-ARE pathway via different residue modifications.</p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-green">04</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>Reduce Baseline Toxic Load First</h4>

# &#x20;             <p>Nrf2 activation is most impactful when ongoing toxic burden is reduced. Remove plastics from food prep, filter water, choose organic for high-pesticide produce.</p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;       </div>

# &#x20;       <div class="callout c-green" style="margin-top:14px;">

# &#x20;         <span class="callout-i">⚙️</span>

# &#x20;         <div><strong>Autophagy cascade via TRF:</strong> Fasting reduces the AMP:ATP ratio, activating AMPK → mTOR inhibition → autophagy initiation. SIRT1 (NAD⁺-dependent deacetylase) collaborates with AMPK to sustain autophagic flux. FGF21 signals the liver to upregulate hepatic autophagy and lipid degradation. Long-term TRF has been shown to improve cognitive function in Alzheimer's models — the mechanism is autophagy-dependent clearance of damaged neuronal components.</div>

# &#x20;       </div>

# &#x20;       <div class="callout c-amber" style="margin-top:8px;">

# &#x20;         <span class="callout-i">⚡</span>

# &#x20;         <div><strong>SIRT1 → testosterone:</strong> Sirtuin 1-mediated autophagy directly regulates testosterone synthesis in Leydig cells of the testes. Fasting is therefore not merely metabolic — it feeds back into androgen production through cellular quality control pathways. This is a direct mechanistic link between TRF and hormonal health in males.</div>

# &#x20;       </div>

# &#x20;       <div class="callout c-blue" style="margin-top:8px;">

# &#x20;         <span class="callout-i">🧬</span>

# &#x20;         <div><strong>Nrf2–autophagy positive feedback:</strong> Nrf2 activation induces autophagy-related proteins. Autophagy selectively removes damaged KEAP1, further stabilising Nrf2. Diet (SFN) and fasting (AMPK/SIRT1) converge on the same cellular defence network from two different angles — making the combination synergistic, not additive.</div>

# &#x20;       </div>

# &#x20;       <div class="callout c-amber" style="margin-top:8px;">

# &#x20;         <span class="callout-i">🧪</span>

# &#x20;         <div><strong>Direct protection vs EDCs:</strong> Sulforaphane protects against BPA-induced glucose intolerance and di-n-butylphthalate-induced testicular toxicity in animal models — via the same Nrf2 pathway. These are the precise EDCs that co-transport on microplastics into testicular and ovarian tissue. While human RCT data on this specific mechanism is pending, the biological rationale is strong and the dietary cost is zero.</div>

# &#x20;       </div>

# &#x20;     </div>

# &#x20;   </div>

# &#x20; </div>

# </section>

# 

# &#x20; <!-- ▸ SLEEP (NEW SECTION) -->

# &#x20; <section id="sleep" class="stone">

# &#x20;   <div class="wrap">

# &#x20;     <div class="eyebrow green fu">Sleep Architecture</div>

# &#x20;   <h2 class="fu">Sleep Optimisation \&amp; CBT-I</h2>

# &#x20;   <p class="lead fu" style="margin-bottom:32px;">Sleep is the foundational intervention. Poor sleep reduces testosterone by up to 15%, impairs prefrontal cognitive function, and raises cortisol — undoing every other intervention in this guide.</p>

# 

# &#x20;   <!-- Sleep environment targets -->

# &#x20;   <div class="sleep-grid fu">

# &#x20;     <div class="sleep-env-card">

# &#x20;       <div class="sec-icon">🌙</div>

# &#x20;       <div class="sec-label">Light at Night</div>

# &#x20;       <div class="sec-val">\&lt; 10 lux</div>

# &#x20;       <div class="sec-note">Evening light \&gt;10 lux (recommended maximum per PLOS Biology expert consensus) disrupts melatonin and delays sleep. One longitudinal study found every 5-lux increase in sleep-period light was associated with \~7.8-min greater irregularity in sleep onset timing</div>

# &#x20;     </div>

# &#x20;     <div class="sleep-env-card">

# &#x20;       <div class="sec-icon">🌡️</div>

# &#x20;       <div class="sec-label">Bedroom Temp</div>

# &#x20;       <div class="sec-val">20–25°C</div>

# &#x20;       <div class="sec-note">Optimal range per longitudinal study (n=50 older adults, 11,000 nights). Each 1°C rise = 0.7% drop in efficiency (Shanghai field study). 5–10% drop when temperature exceeds 25°C</div>

# &#x20;     </div>

# &#x20;     <div class="sleep-env-card">

# &#x20;       <div class="sec-icon">🔇</div>

# &#x20;       <div class="sec-label">Noise</div>

# &#x20;       <div class="sec-val">\&lt; 40 dB</div>

# &#x20;       <div class="sec-note">WHO European target: ≤40 dB annual average outdoor nighttime. Each 1 dB rise in indoor nighttime noise is associated with \~0.19% lower sleep efficiency (HEIJO-KYO cohort, n=231)</div>

# &#x20;     </div>

# &#x20;     <div class="sleep-env-card">

# &#x20;       <div class="sec-icon">☀️</div>

# &#x20;       <div class="sec-label">Morning Light</div>

# &#x20;       <div class="sec-val">Blue-rich, AM</div>

# &#x20;       <div class="sec-note">Dynamic lighting (dawn/dusk simulation) advances sleep onset by 33 min and raises sleep efficiency to 92.6%</div>

# &#x20;     </div>

# &#x20;     <div class="sleep-env-card">

# &#x20;       <div class="sec-icon">📱</div>

# &#x20;       <div class="sec-label">Screen Cutoff</div>

# &#x20;       <div class="sec-val">60–90 min</div>

# &#x20;       <div class="sec-note">Before bed. Blue light blocks melatonin. Use warm (yellow-white) lighting after 21:00 or night filter</div>

# &#x20;     </div>

# &#x20;     <div class="sleep-env-card">

# &#x20;       <div class="sec-icon">⏰</div>

# &#x20;       <div class="sec-label">Consistency</div>

# &#x20;       <div class="sec-val">±30 min</div>

# &#x20;       <div class="sec-note">Wake time consistency is more important than sleep time. Anchors the circadian cortisol curve</div>

# &#x20;     </div>

# &#x20;     <div class="sleep-env-card">

# &#x20;       <div class="sec-icon">👥</div>

# &#x20;       <div class="sec-label">Social Isolation</div>

# &#x20;       <div class="sec-val">Mitigate</div>

# &#x20;       <div class="sec-note">Loneliness is independently associated with worse objective sleep quality and shorter sleep duration — a bidirectional relationship</div>

# &#x20;     </div>

# &#x20;     <div class="sleep-env-card">

# &#x20;       <div class="sec-icon">🏠</div>

# &#x20;       <div class="sec-label">Space per Person</div>

# &#x20;       <div class="sec-val">\&gt;1 room</div>

# &#x20;       <div class="sec-note">Household crowding (\&gt;1 person/room) reduces likelihood of achieving long sleep durations (≥8.5h) by a statistically significant margin</div>

# &#x20;     </div>

# &#x20;   </div>

# 

# &#x20;   <div class="split fu" style="margin-top:32px;">

# &#x20;     <div>

# &#x20;       <h3 style="margin-bottom:12px;">CBT-I — Gold Standard for Insomnia</h3>

# &#x20;       <p style="font-size:0.86rem;margin-bottom:12px;">CBT-I is the first-line, non-pharmacological treatment for chronic insomnia. In a pooled RCT analysis, CBT-I produced the <strong>largest insomnia severity reduction</strong> compared to escitalopram, venlafaxine, exercise, yoga, and oral 17-beta-estradiol. Effects are durable — maintained at 24-week follow-up with no ongoing treatment.</p>

# &#x20;       <div class="callout c-blue" style="margin-bottom:14px;">

# &#x20;         <span class="callout-i">📊</span>

# &#x20;         <div><strong>Durability advantage:</strong> Unlike sleep medications that require ongoing use, CBT-I skills are lifelong. One RCT demonstrated significant superiority over a control group sustained to the 24-week follow-up mark — with continued improvement after treatment ended.</div>

# &#x20;       </div>

# &#x20;       <div class="steps">

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-blue">SC</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>Stimulus Control</h4>

# &#x20;             <p>Use bed only for sleep and sex. Leave bed if awake \&gt;20 min. Rebuilds conditioned bed-sleep association.</p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-blue">SR</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>Sleep Restriction</h4>

# &#x20;             <p>Temporarily restrict time in bed to match actual sleep time, then gradually extend. Builds sleep pressure — most effective single CBT-I component.</p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-blue">RT</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>Relaxation Training</h4>

# &#x20;             <p>Progressive muscle relaxation, diaphragmatic breathing, or body scan meditation. Reduces physiological arousal — key bridge between mindfulness and sleep.</p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;         <div class="step">

# &#x20;           <div class="step-num sn-blue">CR</div>

# &#x20;           <div class="step-content">

# &#x20;             <h4>Cognitive Restructuring</h4>

# &#x20;             <p>Challenge catastrophic beliefs about sleep. "If I don't sleep I'll fail" → "Poor sleep is unpleasant but manageable." Reduces anticipatory anxiety that perpetuates insomnia.</p>

# &#x20;           </div>

# &#x20;         </div>

# &#x20;       </div>

# &#x20;     </div>

# &#x20;     <div>

# &#x20;       <div class="sex-badge sb-female">♀ Female Sleep Lifespan</div>

# &#x20;       <div class="callout c-rose" style="margin-bottom:14px;">

# &#x20;         <span class="callout-i">🌸</span>

# &#x20;         <div>Insomnia prevalence rises from \~30% pre-menopause to \~50% post-menopause. Vasomotor symptoms (hot flashes, night sweats) fragment sleep architecture. CBT-I outperforms HRT for menopausal insomnia in pooled RCTs — and is safe during pregnancy (30% of pregnant women rarely get a good night's sleep) where pharmacological options are severely limited.</div>

# &#x20;       </div>

# &#x20;       <div class="callout c-amber" style="margin-bottom:14px;">

# &#x20;         <span class="callout-i">🤱</span>

# &#x20;         <div><strong>Postpartum women:</strong> Nearly 30% of mothers experience clinically significant sleep disruption. CBT-I breaks the cycle of poor sleep and mood disturbances — with an open-pilot trial in pregnant women showing improved diary-assessed sleep onset, efficiency, and total sleep time.</div>

# &#x20;       </div>

# &#x20;       <div class="card" style="margin-bottom:12px;">

# &#x20;         <h4 style="margin-bottom:10px;">Melatonin: Role \&amp; Limits</h4>

# &#x20;         <ul class="clist cl-amber">

# &#x20;           <li>Melatonin acts as both circadian regulator and ovarian antioxidant in females</li>

# &#x20;           <li>Protects against BaP, phthalate \&amp; chemotherapy-induced ovarian damage</li>

# &#x20;           <li>MTNR1B gene variant (meta-analysis of thousands of patients) is associated with ↑PCOS risk — night light exposure amplifies this genetic risk</li>

# &#x20;           <li>3 mg RCT in DOR: ↑oestradiol, ↑mature MII oocytes but <em>no</em> significant pregnancy rate improvement (6.2% vs 2.9%, NS)</li>

# &#x20;           <li>Best used as antioxidant adjunct — not a standalone fertility treatment</li>

# &#x20;         </ul>

# &#x20;       </div>

# &#x20;       <div class="sex-badge sb-male" style="margin-top:14px;">♂ Male Sleep \&amp; Testosterone</div>

# &#x20;       <div class="callout c-amber">

# &#x20;         <span class="callout-i">⚡</span>

# &#x20;         <div>Testosterone peaks in early morning during REM sleep. One week of sleep restriction to 5h/night reduces testosterone levels by <strong>10–15%</strong> in young healthy males — equivalent to ageing 10–15 years. Sleep is the most underrated testosterone intervention.</div>

# &#x20;       </div>

# &#x20;       <div class="card" style="margin-top:12px;padding:14px;">

# &#x20;         <h4 style="font-size:0.84rem;margin-bottom:8px;">Exergaming for Sleep (Age 60+)</h4>

# &#x20;         <p style="font-size:0.79rem;margin-bottom:8px;">Systematic review of 11 RCTs: exergaming significantly improves sleep quality (SMD = −0.31). Age matters — participants <strong>60+ years</strong> show a large effect (SMD = −1.38) while 18–60 shows no significant effect. Duration matters too: programmes ≥8 weeks effective; shorter programmes are not.</p>

# &#x20;         <p style="font-size:0.79rem;">Practical note: no significant difference vs traditional exercise — the "game" adds motivation, not superior physiology.</p>

# &#x20;       </div>

# &#x20;     </div>

# &#x20;   </div>

# &#x20; </div>

# </section>

# 

# <!-- ▸ EVIDENCE SUMMARY -->

# <section id="summary" class="alt">

# &#x20; <div class="wrap">

# &#x20;   <div class="eyebrow fu">Evidence Summary</div>

# &#x20;   <h2 class="fu">What the Evidence Actually Shows</h2>

# &#x20;   <p class="lead fu" style="margin-bottom:32px;">Ranked by strength of independent evidence, practical applicability, and breadth of systemic benefit. Sex-specific applicability noted where evidence diverges.</p>

# &#x20;   <div class="tbl-wrap fu">

# &#x20;     <table>

# &#x20;       <thead>

# &#x20;         <tr>

# &#x20;           <th>Intervention</th>

# &#x20;           <th>Domain</th>

# &#x20;           <th>Evidence Tier</th>

# &#x20;           <th>Key Benefit</th>

# &#x20;           <th>Applies To</th>

# &#x20;           <th>Effort</th>

# &#x20;         </tr>

# &#x20;       </thead>

# &#x20;       <tbody>

# &#x20;         <tr><td>Cognitive Training / Rehabilitation</td><td><span class="pill pill-blue">Cognitive</span></td><td>★★★★★ Strongest</td><td>Attention, working memory, processing speed</td><td><span class="pill pill-gray">All</span></td><td>Moderate</td></tr>

# &#x20;         <tr><td>MBIs (MBSR / MBCT)</td><td><span class="pill pill-blue">Cognitive</span></td><td>★★★★★ Strongest</td><td>Focus, brain fog, mental fatigue, cortisol</td><td><span class="pill pill-gray">All</span></td><td>Low–Moderate</td></tr>

# &#x20;         <tr><td>CBT + Behavioural Activation</td><td><span class="pill pill-blue">Cognitive</span></td><td>★★★★★ Strong</td><td>Fatigue, motivation, ADHD, depression</td><td><span class="pill pill-gray">All</span></td><td>Moderate</td></tr>

# &#x20;         <tr><td>CBT-I (for insomnia)</td><td><span class="pill pill-blue">Sleep</span></td><td>★★★★★ Gold Standard</td><td>Insomnia severity, WASO, sleep efficiency — 24-wk durability; outperforms HRT \&amp; medication</td><td><span class="pill pill-gray">All</span></td><td>Moderate</td></tr>

# &#x20;         <tr><td>EDC Reduction (lifestyle)</td><td><span class="pill pill-rose">Hormonal</span></td><td>★★★★★ Essential</td><td>Reproductive protection, HPG axis integrity</td><td><span class="pill pill-rose">♀ priority</span></td><td>Low</td></tr>

# &#x20;         <tr><td>Time-Restricted Feeding (14:10–16:8)</td><td><span class="pill pill-amber">Metabolic</span></td><td>★★★★ Strong</td><td>Body composition, insulin, testosterone, autophagy</td><td><span class="pill pill-blue">♂ 16:8</span> <span class="pill pill-rose">♀ 14:10</span></td><td>Very Low</td></tr>

# &#x20;         <tr><td>Mediterranean Diet</td><td><span class="pill pill-amber">Hormonal</span></td><td>★★★★ Strong</td><td>♂ testosterone ↑ · ♀ PCOS, androgen ↓</td><td><span class="pill pill-gray">All</span></td><td>Low</td></tr>

# &#x20;         <tr><td>Sleep 7–9h + Environment</td><td><span class="pill pill-blue">Sleep</span></td><td>★★★★ Strong</td><td>Testosterone, cognition, cortisol, fatigue</td><td><span class="pill pill-gray">All</span></td><td>Very Low</td></tr>

# &#x20;         <tr><td>Cruciferous Vegetables (Sulforaphane)</td><td><span class="pill pill-green">Detox</span></td><td>★★★★ Strong (RCT)</td><td>Nrf2 activation, Phase II enzymes, ovarian protection</td><td><span class="pill pill-gray">All</span></td><td>Very Low</td></tr>

# &#x20;         <tr><td>Modafinil / Methylphenidate</td><td><span class="pill pill-blue">Pharmacological</span></td><td>★★★★ Strong (Rx)</td><td>Attention, wakefulness, motivation, fatigue</td><td><span class="pill pill-gray">All</span></td><td>Low (with Rx)</td></tr>

# &#x20;         <tr><td>Guanfacine XR</td><td><span class="pill pill-blue">Pharmacological</span></td><td>★★★★ Strong (Rx)</td><td>Working memory, ADHD, executive function</td><td><span class="pill pill-gray">All</span></td><td>Low (with Rx)</td></tr>

# &#x20;         <tr><td>Clinical Hypnosis</td><td><span class="pill pill-blue">Cognitive</span></td><td>★★★ Moderate</td><td>Motivation, fatigue, stress regulation</td><td><span class="pill pill-gray">All</span></td><td>Low (practitioner)</td></tr>

# &#x20;         <tr><td>Melatonin (DOR)</td><td><span class="pill pill-rose">Reproductive</span></td><td>★★★ Moderate (Rx)</td><td>↑mature oocytes; antioxidant protection</td><td><span class="pill pill-rose">♀ only</span></td><td>Low (with Rx)</td></tr>

# &#x20;         <tr><td>CBT-I (Insomnia)</td><td><span class="pill pill-blue">Sleep</span></td><td>★★★★★ Strongest</td><td>Insomnia severity; sleep efficiency; 24-wk durability</td><td><span class="pill pill-gray">All</span></td><td>Moderate</td></tr>

# &#x20;         <tr><td>Exergaming (Interactive Exercise)</td><td><span class="pill pill-green">Sleep/Movement</span></td><td>★★★ Moderate (60+)</td><td>Sleep quality (large SMD in 60+ cohort; no effect 18–60)</td><td><span class="pill pill-gray">60+ years</span></td><td>Very Low</td></tr>

# &#x20;         <tr><td>Placebo Optimisation</td><td><span class="pill pill-gray">Psychological</span></td><td>★★★ Moderate</td><td>Memory, attention, self-efficacy, framing effects</td><td><span class="pill pill-gray">All</span></td><td>Very Low</td></tr>

# &#x20;         <tr><td>Exergaming (60+ years)</td><td><span class="pill pill-blue">Sleep</span></td><td>★★★ Moderate</td><td>Sleep quality (SMD −1.38 in 60+); requires ≥8 weeks; no benefit in 18–60 age group</td><td><span class="pill pill-gray">60+ years</span></td><td>Low</td></tr>

# &#x20;       </tbody>

# &#x20;     </table>

# &#x20;   </div>

# 

# &#x20;   <!-- Action tiers -->

# &#x20;   <h3 class="fu" style="margin-top:40px;margin-bottom:20px;">Implementation Hierarchy — Where to Start</h3>

# &#x20;   <div class="g3 fu">

# &#x20;     <div class="card green" style="padding:20px;">

# &#x20;       <div style="display:flex;align-items:center;gap:10px;margin-bottom:12px;">

# &#x20;         <div class="icon-wrap iw-green" style="margin:0;">🏗️</div>

# &#x20;         <div>

# &#x20;           <div style="font-size:0.68rem;font-weight:700;letter-spacing:.08em;text-transform:uppercase;color:var(--green);">Tier 1 — Foundation</div>

# &#x20;           <div style="font-size:0.9rem;font-weight:700;color:var(--ink);font-family:'Libre Baskerville',serif;">Highest ROI, Lowest Effort</div>

# &#x20;         </div>

# &#x20;       </div>

# &#x20;       <ul class="clist cl-green" style="font-size:0.82rem;">

# &#x20;         <li>Sleep 7–9h + bedroom environment optimisation</li>

# &#x20;         <li>EDC reduction (switch food storage; filter water)</li>

# &#x20;         <li>Mediterranean diet framework (whole foods, olive oil, cruciferous)</li>

# &#x20;         <li>14:10–16:8 TRF (pick consistent eating window)</li>

# &#x20;         <li>Daily cruciferous vegetables + raw broccoli sprouts</li>

# &#x20;       </ul>

# &#x20;     </div>

# &#x20;     <div class="card blue" style="padding:20px;">

# &#x20;       <div style="display:flex;align-items:center;gap:10px;margin-bottom:12px;">

# &#x20;         <div class="icon-wrap iw-blue" style="margin:0;">🧠</div>

# &#x20;         <div>

# &#x20;           <div style="font-size:0.68rem;font-weight:700;letter-spacing:.08em;text-transform:uppercase;color:var(--blue);">Tier 2 — Behavioural</div>

# &#x20;           <div style="font-size:0.9rem;font-weight:700;color:var(--ink);font-family:'Libre Baskerville',serif;">Evidence-Based, Proven Durable</div>

# &#x20;         </div>

# &#x20;       </div>

# &#x20;       <ul class="clist cl-blue" style="font-size:0.82rem;">

# &#x20;         <li>MBSR / FA meditation — 15–20 min daily (NCCIH-funded evidence)</li>

# &#x20;         <li>CBT-I for any persistent insomnia (outperforms medication long-term)</li>

# &#x20;         <li>Behavioural Activation — weekly activity scheduling</li>

# &#x20;         <li>Resistance training 2–3×/week (synergises with TRF)</li>

# &#x20;         <li>Stress management — cortisol is the testosterone antagonist</li>

# &#x20;       </ul>

# &#x20;     </div>

# &#x20;     <div class="card amber" style="padding:20px;">

# &#x20;       <div style="display:flex;align-items:center;gap:10px;margin-bottom:12px;">

# &#x20;         <div class="icon-wrap iw-amber" style="margin:0;">🎯</div>

# &#x20;         <div>

# &#x20;           <div style="font-size:0.68rem;font-weight:700;letter-spacing:.08em;text-transform:uppercase;color:var(--amber);">Tier 3 — Targeted</div>

# &#x20;           <div style="font-size:0.9rem;font-weight:700;color:var(--ink);font-family:'Libre Baskerville',serif;">Adjunctive, Condition-Specific</div>

# &#x20;         </div>

# &#x20;       </div>

# &#x20;       <ul class="clist cl-amber" style="font-size:0.82rem;">

# &#x20;         <li>Melatonin (DOR / ovarian protection) — physician-guided</li>

# &#x20;         <li>Vitamin D3 supplementation if deficient (serum 50–80 nmol/L target)</li>

# &#x20;         <li>Cognitive rehabilitation for post-illness brain fog</li>

# &#x20;         <li>Pharmacological options (methylphenidate, guanfacine, bupropion) — Rx only</li>

# &#x20;         <li>HRT for menopausal vasomotor sleep disruption — gynaecologist assessment</li>

# &#x20;       </ul>

# &#x20;     </div>

# &#x20;   </div>

# &#x20; </div>

# </section>

# 

# <!-- ════════════════════════════════════════════════════════

# &#x20;    PERSONALISED ROUTINE CALCULATOR

# ════════════════════════════════════════════════════════ -->

# <section id="calculator" class="calc-section">

# &#x20; <div class="wrap">

# &#x20;   <div class="eyebrow fu">Personalised Tool</div>

# &#x20;   <h2 class="fu">Build Your Evidence-Based Routine</h2>

# &#x20;   <p class="lead fu" style="margin-bottom:32px;">Enter your details. The calculator tailors fasting windows, protein targets, sulforaphane dosing, meditation durations, EDC reduction priorities, and sex-specific hormonal guidance to your profile.</p>

# 

# &#x20;   <div class="calc-form fu">

# &#x20;     <div style="display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:12px;margin-bottom:20px;">

# &#x20;       <h3 style="font-size:0.95rem;">Your profile</h3>

# &#x20;       <div style="display:flex;align-items:center;gap:8px;flex-wrap:wrap;">

# &#x20;         <span style="font-size:0.76rem;color:var(--muted);font-weight:600;">Units:</span>

# &#x20;         <div class="unit-toggle">

# &#x20;           <button id="metricBtn" class="active" onclick="setUnit('metric')">Metric</button>

# &#x20;           <button id="imperialBtn" onclick="setUnit('imperial')">Imperial</button>

# &#x20;         </div>

# &#x20;       </div>

# &#x20;     </div>

# 

# &#x20;     <div class="form-grid">

# &#x20;       <div class="form-group">

# &#x20;         <label>Age</label>

# &#x20;         <input type="number" id="age" placeholder="28" min="16" max="80" inputmode="numeric">

# &#x20;         <span class="unit">years</span>

# &#x20;       </div>

# &#x20;       <div class="form-group">

# &#x20;         <label>Biological Sex</label>

# &#x20;         <div class="sex-toggle">

# &#x20;           <button id="btnMale" class="active-m" onclick="setSex('male')">♂ Male</button>

# &#x20;           <button id="btnFemale" onclick="setSex('female')">♀ Female</button>

# &#x20;         </div>

# &#x20;       </div>

# &#x20;       <div class="form-group">

# &#x20;         <label id="heightLabel">Height</label>

# &#x20;         <input type="number" id="height" placeholder="174" min="100" max="250" step="1" inputmode="decimal">

# &#x20;         <span class="unit" id="heightUnit">cm</span>

# &#x20;       </div>

# &#x20;       <div class="form-group">

# &#x20;         <label id="weightLabel">Weight</label>

# &#x20;         <input type="number" id="weight" placeholder="73" min="30" max="300" step="0.5" inputmode="decimal">

# &#x20;         <span class="unit" id="weightUnit">kg</span>

# &#x20;       </div>

# &#x20;       <div class="form-group">

# &#x20;         <label>Activity Level</label>

# &#x20;         <select id="activity">

# &#x20;           <option value="1.2">Sedentary (desk job, no exercise)</option>

# &#x20;           <option value="1.375">Lightly active (1–3×/week)</option>

# &#x20;           <option value="1.55" selected>Moderately active (3–5×/week)</option>

# &#x20;           <option value="1.725">Very active (6–7×/week)</option>

# &#x20;           <option value="1.9">Athlete / physical job</option>

# &#x20;         </select>

# &#x20;       </div>

# &#x20;       <div class="form-group">

# &#x20;         <label>Sleep (hrs/night)</label>

# &#x20;         <input type="number" id="sleep" placeholder="7" min="3" max="12" step="0.5" inputmode="decimal">

# &#x20;         <span class="unit">hrs</span>

# &#x20;       </div>

# &#x20;       <div class="form-group">

# &#x20;         <label>Stress Level</label>

# &#x20;         <select id="stress">

# &#x20;           <option value="low">Low</option>

# &#x20;           <option value="moderate" selected>Moderate</option>

# &#x20;           <option value="high">High / chronic</option>

# &#x20;         </select>

# &#x20;       </div>

# &#x20;       <div class="form-group" id="cycleGroup" style="display:none;">

# &#x20;         <label>Menstrual Status</label>

# &#x20;         <select id="cycleStatus">

# &#x20;           <option value="regular">Regular cycles</option>

# &#x20;           <option value="irregular">Irregular / PCOS concern</option>

# &#x20;           <option value="peri">Perimenopause</option>

# &#x20;           <option value="post">Post-menopause</option>

# &#x20;           <option value="pregnant">Pregnant / breastfeeding</option>

# &#x20;         </select>

# &#x20;       </div>

# &#x20;     </div>

# 

# &#x20;     <!-- Goals -->

# &#x20;     <div style="margin-bottom:18px;">

# &#x20;       <label style="display:block;font-size:0.73rem;font-weight:600;letter-spacing:.05em;text-transform:uppercase;color:var(--muted);margin-bottom:10px;">Primary Goals (select all that apply)</label>

# &#x20;       <div class="goal-grid" id="goalGrid">

# &#x20;         <label class="goal-chip checked" onclick="toggleGoal(this, event)">

# &#x20;           <input type="checkbox" value="cognitive" checked>

# &#x20;           <div class="goal-chip-box">✓</div>

# &#x20;           🧠 Cognitive focus

# &#x20;         </label>

# &#x20;         <label class="goal-chip" onclick="toggleGoal(this, event)">

# &#x20;           <input type="checkbox" value="hormonal">

# &#x20;           <div class="goal-chip-box">✓</div>

# &#x20;           ⚡ Hormonal health

# &#x20;         </label>

# &#x20;         <label class="goal-chip" onclick="toggleGoal(this, event)">

# &#x20;           <input type="checkbox" value="detox">

# &#x20;           <div class="goal-chip-box">✓</div>

# &#x20;           🌿 Detox / EDC reduction

# &#x20;         </label>

# &#x20;         <label class="goal-chip" onclick="toggleGoal(this, event)">

# &#x20;           <input type="checkbox" value="sleep">

# &#x20;           <div class="goal-chip-box">✓</div>

# &#x20;           😴 Better sleep

# &#x20;         </label>

# &#x20;         <label class="goal-chip" onclick="toggleGoal(this, event)">

# &#x20;           <input type="checkbox" value="weight">

# &#x20;           <div class="goal-chip-box">✓</div>

# &#x20;           ⚖️ Body composition

# &#x20;         </label>

# &#x20;         <label class="goal-chip" onclick="toggleGoal(this, event)">

# &#x20;           <input type="checkbox" value="fertility">

# &#x20;           <div class="goal-chip-box">✓</div>

# &#x20;           🌱 Fertility support

# &#x20;         </label>

# &#x20;       </div>

# &#x20;     </div>

# 

# &#x20;     <!-- Toxin exposure checker -->

# &#x20;     <div style="margin-bottom:18px;">

# &#x20;       <label style="display:block;font-size:0.73rem;font-weight:600;letter-spacing:.05em;text-transform:uppercase;color:var(--muted);margin-bottom:6px;">EDC / Toxin Exposure Check <span style="font-weight:400;text-transform:none;letter-spacing:0;">(check all that apply to your routine)</span></label>

# &#x20;       <div class="tox-grid" id="toxGrid">

# &#x20;         <label class="tox-item" onclick="toggleTox(this, event)">

# &#x20;           <input type="checkbox" value="2"><div class="tox-box">✓</div> Heat food in plastic containers

# &#x20;         </label>

# &#x20;         <label class="tox-item" onclick="toggleTox(this, event)">

# &#x20;           <input type="checkbox" value="2"><div class="tox-box">✓</div> Use plastic water bottles regularly

# &#x20;         </label>

# &#x20;         <label class="tox-item" onclick="toggleTox(this, event)">

# &#x20;           <input type="checkbox" value="2"><div class="tox-box">✓</div> Canned food most days

# &#x20;         </label>

# &#x20;         <label class="tox-item" onclick="toggleTox(this, event)">

# &#x20;           <input type="checkbox" value="3"><div class="tox-box">✓</div> Handle thermal/receipt paper often

# &#x20;         </label>

# &#x20;         <label class="tox-item" onclick="toggleTox(this, event)">

# &#x20;           <input type="checkbox" value="2"><div class="tox-box">✓</div> Non-organic produce regularly

# &#x20;         </label>

# &#x20;         <label class="tox-item" onclick="toggleTox(this, event)">

# &#x20;           <input type="checkbox" value="2"><div class="tox-box">✓</div> Synthetic fragrance products

# &#x20;         </label>

# &#x20;         <label class="tox-item" onclick="toggleTox(this, event)">

# &#x20;           <input type="checkbox" value="3"><div class="tox-box">✓</div> Tobacco smoke (active or passive)

# &#x20;         </label>

# &#x20;         <label class="tox-item" onclick="toggleTox(this, event)">

# &#x20;           <input type="checkbox" value="2"><div class="tox-box">✓</div> Unfiltered tap water

# &#x20;         </label>

# &#x20;         <label class="tox-item" onclick="toggleTox(this, event)">

# &#x20;           <input type="checkbox" value="3"><div class="tox-box">✓</div> Occupational chemical exposure

# &#x20;         </label>

# &#x20;         <label class="tox-item" onclick="toggleTox(this, event)">

# &#x20;           <input type="checkbox" value="2"><div class="tox-box">✓</div> Non-stick cookware (PFAS)

# &#x20;         </label>

# &#x20;         <label class="tox-item" onclick="toggleTox(this, event)">

# &#x20;           <input type="checkbox" value="1"><div class="tox-box">✓</div> High air pollution environment

# &#x20;         </label>

# &#x20;         <label class="tox-item" onclick="toggleTox(this, event)">

# &#x20;           <input type="checkbox" value="2"><div class="tox-box">✓</div> Conventional cleaning products

# &#x20;         </label>

# &#x20;       </div>

# &#x20;     </div>

# 

# &#x20;     <button class="calc-btn" id="calcBtn" onclick="calculate()">

# &#x20; <span id="btnText">Generate My Personalised Routine →</span>

# &#x20; <span id="btnLoading" style="display:none;">Generating...</span>

# </button>

# &#x20;   </div>

# 

# &#x20;   <!-- Result -->

# &#x20;   <div class="result-panel fu" id="resultPanel">

# &#x20;     <div class="result-header" id="resultStats"></div>

# 

# &#x20;     <!-- Tab navigation -->

# &#x20;     <div class="result-tabs" id="resultTabs" style="display:none;">

# &#x20;       <button class="rtab active" data-tab="routine" onclick="switchTab('routine',this)">📋 Daily Routine</button>

# &#x20;       <button class="rtab" data-tab="scores" onclick="switchTab('scores',this)">📊 Profile Scores</button>

# &#x20;       <button class="rtab" data-tab="notes" onclick="switchTab('notes',this)">💡 Smart Notes</button>

# &#x20;     </div>

# 

# &#x20;     <div class="result-body">

# &#x20;       <!-- Tab: Routine -->

# &#x20;       <div id="tab-routine" class="tab-content">

# &#x20;         <div id="resultRoutine"></div>

# &#x20;       </div>

# &#x20;       <!-- Tab: Scores -->

# &#x20;       <div id="tab-scores" class="tab-content" style="display:none;">

# &#x20;         <div id="resultScores"></div>

# &#x20;       </div>

# &#x20;       <!-- Tab: Notes -->

# &#x20;       <div id="tab-notes" class="tab-content" style="display:none;">

# &#x20;         <div id="resultNotes"></div>

# &#x20;       </div>

# 

# &#x20;       <div style="padding:16px 0 4px;display:flex;gap:8px;justify-content:flex-end;flex-wrap:wrap;" id="resultActions">

# &#x20;         <button onclick="copyRoutine()" id="copyBtn" style="padding:7px 14px;border-radius:var(--r);border:1.5px solid var(--border);background:var(--white);font-family:'Figtree',sans-serif;font-size:0.78rem;font-weight:600;color:var(--muted);cursor:pointer;transition:all 0.15s;">📋 Copy Routine</button>

# &#x20;         <button onclick="window.print()" style="padding:7px 14px;border-radius:var(--r);border:1.5px solid var(--border);background:var(--white);font-family:'Figtree',sans-serif;font-size:0.78rem;font-weight:600;color:var(--muted);cursor:pointer;transition:all 0.15s;" onmouseover="this.style.borderColor='var(--blue)';this.style.color='var(--blue)'" onmouseout="this.style.borderColor='var(--border)';this.style.color='var(--muted)'">🖨 Print</button>

# &#x20;       </div>

# &#x20;     </div>

# &#x20;   </div>

# 

# &#x20; </div>

# </section>

# 

# </main>

# 

# <!-- FOOTER -->

# <footer style="background:var(--ink);padding:clamp(40px,5vw,60px) 0 28px;">

# &#x20; <div class="wrap">

# &#x20;   <div style="display:grid;grid-template-columns:2fr repeat(3,1fr);gap:clamp(20px,4vw,44px);margin-bottom:36px;flex-wrap:wrap;" class="footer-grid">

# &#x20;     <div>

# &#x20;       <div style="font-family:'Libre Baskerville',serif;font-weight:700;font-size:1.05rem;color:var(--white);margin-bottom:10px;">BioOptima</div>

# &#x20;       <p style="font-size:0.8rem;color:rgba(255,255,255,0.3);line-height:1.7;max-width:260px;">Peer-reviewed, non-industry-funded research synthesis. Not medical advice — consult a qualified physician.</p>

# &#x20;     </div>

# &#x20;     <div>

# &#x20;       <p style="font-size:0.7rem;font-weight:700;letter-spacing:.08em;text-transform:uppercase;color:rgba(255,255,255,0.28);margin-bottom:10px;">Cognitive</p>

# &#x20;       <ul style="list-style:none;display:flex;flex-direction:column;gap:6px;">

# &#x20;         <li style="font-size:0.8rem;color:rgba(255,255,255,0.38);">CBT \&amp; BA</li>

# &#x20;         <li style="font-size:0.8rem;color:rgba(255,255,255,0.38);">MBSR / Mindfulness</li>

# &#x20;         <li style="font-size:0.8rem;color:rgba(255,255,255,0.38);">Cognitive Rehab</li>

# &#x20;         <li style="font-size:0.8rem;color:rgba(255,255,255,0.38);">Pharmacological</li>

# &#x20;       </ul>

# &#x20;     </div>

# &#x20;     <div>

# &#x20;       <p style="font-size:0.7rem;font-weight:700;letter-spacing:.08em;text-transform:uppercase;color:rgba(255,255,255,0.28);margin-bottom:10px;">Hormonal</p>

# &#x20;       <ul style="list-style:none;display:flex;flex-direction:column;gap:6px;">

# &#x20;         <li style="font-size:0.8rem;color:rgba(255,255,255,0.38);">EDC Reduction</li>

# &#x20;         <li style="font-size:0.8rem;color:rgba(255,255,255,0.38);">Fasting (TRF)</li>

# &#x20;         <li style="font-size:0.8rem;color:rgba(255,255,255,0.38);">Mediterranean Diet</li>

# &#x20;         <li style="font-size:0.8rem;color:rgba(255,255,255,0.38);">PCOS / Female Health</li>

# &#x20;       </ul>

# &#x20;     </div>

# &#x20;     <div>

# &#x20;       <p style="font-size:0.7rem;font-weight:700;letter-spacing:.08em;text-transform:uppercase;color:rgba(255,255,255,0.28);margin-bottom:10px;">Detox / Sleep</p>

# &#x20;       <ul style="list-style:none;display:flex;flex-direction:column;gap:6px;">

# &#x20;         <li style="font-size:0.8rem;color:rgba(255,255,255,0.38);">Nrf2 / KEAP1</li>

# &#x20;         <li style="font-size:0.8rem;color:rgba(255,255,255,0.38);">Sulforaphane</li>

# &#x20;         <li style="font-size:0.8rem;color:rgba(255,255,255,0.38);">Autophagy</li>

# &#x20;         <li style="font-size:0.8rem;color:rgba(255,255,255,0.38);">CBT-I Protocol</li>

# &#x20;       </ul>

# &#x20;     </div>

# &#x20;   </div>

# &#x20;   <div style="padding-top:20px;border-top:1px solid rgba(255,255,255,0.08);display:flex;justify-content:space-between;flex-wrap:wrap;gap:8px;">

# &#x20;     <p style="font-size:0.74rem;color:rgba(255,255,255,0.22);">Educational resource. All content from peer-reviewed literature. Not medical advice.</p>

# &#x20;     <p style="font-size:0.74rem;color:rgba(255,255,255,0.22);">BioOptima Research Synthesis</p>

# &#x20;   </div>

# &#x20; </div>

# </footer>

# 

# <script>

# /\* ── STATE ── \*/

# let useMetric = true;

# let selectedSex = 'male';

# 

# /\* ── UNIT TOGGLE ── \*/

# function setUnit(u) {

# &#x20; useMetric = u === 'metric';

# &#x20; document.getElementById('metricBtn').classList.toggle('active', useMetric);

# &#x20; document.getElementById('imperialBtn').classList.toggle('active', !useMetric);

# &#x20; document.getElementById('heightUnit').textContent = useMetric ? 'cm' : 'ft (e.g. 5.9)';

# &#x20; document.getElementById('weightUnit').textContent = useMetric ? 'kg' : 'lbs';

# &#x20; document.getElementById('height').placeholder = useMetric ? '174' : '5.9';

# &#x20; document.getElementById('weight').placeholder = useMetric ? '73' : '161';

# }

# 

# /\* ── SEX TOGGLE ── \*/

# function setSex(s) {

# &#x20; selectedSex = s;

# &#x20; document.getElementById('btnMale').className = s === 'male' ? 'active-m' : '';

# &#x20; document.getElementById('btnFemale').className = s === 'female' ? 'active-f' : '';

# &#x20; document.getElementById('cycleGroup').style.display = s === 'female' ? 'flex' : 'none';

# }

# 

# /\* ── GOAL CHIPS ── \*/

# function toggleGoal(el, event) {

# &#x20; event.preventDefault();

# &#x20; el.classList.toggle('checked');

# &#x20; const isChecked = el.classList.contains('checked');

# &#x20; el.querySelector('input').checked = isChecked;

# }

# 

# function getGoals() {

# &#x20; return Array.from(document.querySelectorAll('#goalGrid input:checked')).map(i => i.value);

# }

# 

# /\* ── TOX CHECKER ── \*/

# function toggleTox(el, event) {

# &#x20; event.preventDefault();

# &#x20; el.classList.toggle('checked');

# &#x20; const isChecked = el.classList.contains('checked');

# &#x20; el.querySelector('input').checked = isChecked;

# }

# 

# function getToxScore() {

# &#x20; let score = 0;

# &#x20; document.querySelectorAll('#toxGrid .tox-item.checked input').forEach(i => { score += parseInt(i.value); });

# &#x20; return score;

# }

# 

# /\* ── UNIT CONVERSION ── \*/

# function getKg() {

# &#x20; const w = parseFloat(document.getElementById('weight').value);

# &#x20; if (!w || w <= 0 || isNaN(w)) return null;

# &#x20; return useMetric ? w : w \* 0.453592;

# }

# function getCm() {

# &#x20; const h = parseFloat(document.getElementById('height').value);

# &#x20; if (!h || h <= 0 || isNaN(h)) return null;

# &#x20; if (useMetric) return h;

# &#x20; const ft = Math.floor(h); const inches = Math.round((h - ft) \* 10);

# &#x20; return ft \* 30.48 + inches \* 2.54;

# }

# 

# /\* ── ACCORDION ── \*/

# function toggleAcc(btn) {

# &#x20; const body = btn.nextElementSibling;

# &#x20; const isOpen = btn.classList.contains('open');

# &#x20; btn.closest('section').querySelectorAll('.acc-btn.open').forEach(b => {

# &#x20;   b.classList.remove('open'); b.nextElementSibling.classList.remove('open');

# &#x20; });

# &#x20; if (!isOpen) { btn.classList.add('open'); body.classList.add('open'); }

# }

# 

# /\* ── FADE IN ── \*/

# const obs = new IntersectionObserver(entries => {

# &#x20; entries.forEach(e => { if (e.isIntersecting) { e.target.classList.add('vis'); obs.unobserve(e.target); } });

# }, { threshold: 0.05, rootMargin: '0px 0px -40px 0px' });

# document.querySelectorAll('.fu').forEach(el => {

# &#x20; // Immediately show elements already in the viewport (hero section)

# &#x20; const rect = el.getBoundingClientRect();

# &#x20; if (rect.top < window.innerHeight \&\& rect.bottom > 0) {

# &#x20;   el.classList.add('vis');

# &#x20; } else {

# &#x20;   obs.observe(el);

# &#x20; }

# });

# 

# /\* ── PROGRESS BAR + BACK TO TOP ── \*/

# const bttBtn = document.getElementById('btt');

# window.addEventListener('scroll', () => {

# &#x20; const s = window.scrollY, d = document.documentElement.scrollHeight - window.innerHeight;

# &#x20; document.getElementById('prog').style.width = d > 0 ? (s/d\*100) + '%' : '0%';

# &#x20; bttBtn.classList.toggle('show', s > 600);

# }, { passive: true });

# 

# /\* ── HAMBURGER ── \*/

# document.getElementById('ham').addEventListener('click', function() {

# &#x20; const isOpen = this.classList.toggle('open');

# &#x20; document.getElementById('mobMenu').classList.toggle('open');

# &#x20; this.setAttribute('aria-expanded', isOpen);

# });

# document.getElementById('mobMenu').querySelectorAll('a').forEach(a => a.addEventListener('click', () => {

# &#x20; document.getElementById('ham').classList.remove('open');

# &#x20; document.getElementById('mobMenu').classList.remove('open');

# }));

# 

# /\* ── ACTIVE NAV ── \*/

# const navAs = document.querySelectorAll('.nav-links a');

# const secEls = document.querySelectorAll('section\[id]');

# const obs2 = new IntersectionObserver(entries => {

# &#x20; entries.forEach(e => {

# &#x20;   if (e.isIntersecting) {

# &#x20;     navAs.forEach(a => a.classList.remove('active'));

# &#x20;     const a = document.querySelector(`.nav-links a\[href="#${e.target.id}"]`);

# &#x20;     if (a) a.classList.add('active');

# &#x20;   }

# &#x20; });

# }, { threshold: 0.3 });

# secEls.forEach(s => obs2.observe(s));

# 

# /\* ════════════════════════════════════════════

# &#x20;  CALCULATOR LOGIC

# ════════════════════════════════════════════ \*/

# function calculate() {

# &#x20; // Show loading state

# &#x20; const btn = document.getElementById('calcBtn');

# &#x20; const btnText = document.getElementById('btnText');

# &#x20; const btnLoading = document.getElementById('btnLoading');

# &#x20; btn.disabled = true;

# &#x20; btnText.style.display = 'none';

# &#x20; btnLoading.style.display = 'inline';

# &#x20; 

# &#x20; const age = parseInt(document.getElementById('age').value) || 28;

# &#x20; const sex = selectedSex;

# &#x20; const weight = getKg();

# &#x20; const height = getCm();

# &#x20; const act = parseFloat(document.getElementById('activity').value);

# &#x20; const goals = getGoals();

# &#x20; const sleep = parseFloat(document.getElementById('sleep').value) || 7;

# &#x20; const stress = document.getElementById('stress').value;

# &#x20; const toxScore = getToxScore();

# &#x20; const cycleStatus = sex === 'female' ? (document.getElementById('cycleStatus').value || 'regular') : null;

# 

# &#x20; if (!weight || !height || isNaN(weight) || isNaN(height)) {

# &#x20;   let errEl = document.getElementById('calcError');

# &#x20;   if (!errEl) {

# &#x20;     errEl = document.createElement('div');

# &#x20;     errEl.id = 'calcError';

# &#x20;     errEl.style.cssText = 'margin-top:10px;padding:10px 14px;background:var(--red-l);border:1px solid #fecaca;border-radius:var(--r);font-size:0.83rem;color:var(--red);';

# &#x20;     btn.parentNode.insertBefore(errEl, btn.nextSibling);

# &#x20;   }

# &#x20;   errEl.textContent = '⚠️ Please enter valid height and weight values to generate your routine.';

# &#x20;   errEl.style.display = 'block';

# &#x20;   btn.disabled = false;

# &#x20;   btnText.style.display = 'inline';

# &#x20;   btnLoading.style.display = 'none';

# &#x20;   return;

# &#x20; }

# &#x20; // Clear any previous error

# &#x20; const errEl = document.getElementById('calcError');

# &#x20; if (errEl) errEl.style.display = 'none';

# 

# &#x20; /\* ── Derived metrics ── \*/

# &#x20; const bmi  = weight / Math.pow(height/100, 2);

# &#x20; const bmiC = bmi < 18.5 ? 'Underweight' : bmi < 25 ? 'Normal' : bmi < 30 ? 'Overweight' : 'Obese';

# 

# &#x20; // Mifflin-St Jeor BMR

# &#x20; const bmr = sex === 'male'

# &#x20;   ? 10\*weight + 6.25\*height - 5\*age + 5

# &#x20;   : 10\*weight + 6.25\*height - 5\*age - 161;

# &#x20; const tdee = Math.round(bmr \* act);

# 

# &#x20; // Protein targets

# &#x20; const protBase = sex === 'male' ? (goals.includes('hormonal') ? 1.9 : 1.7) : 1.6;

# &#x20; const protMin  = Math.round(weight \* protBase);

# &#x20; const protMax  = Math.round(weight \* (sex === 'male' ? 2.2 : 2.0));

# 

# &#x20; /\* ── Fasting window logic ── \*/

# &#x20; let fastWindow, eatStart, eatEnd;

# &#x20; if (sex === 'female') {

# &#x20;   // Women: more conservative

# &#x20;   if (cycleStatus === 'pregnant') {

# &#x20;     fastWindow = 'Not recommended'; eatStart = 'N/A'; eatEnd = 'N/A';

# &#x20;   } else if (bmi > 28 \&\& (goals.includes('hormonal') || goals.includes('weight'))) {

# &#x20;     fastWindow = '14:10'; eatStart = '10:00'; eatEnd = '20:00';

# &#x20;   } else {

# &#x20;     fastWindow = '14:10'; eatStart = '10:00'; eatEnd = '20:00';

# &#x20;   }

# &#x20; } else {

# &#x20;   // Males

# &#x20;   if (bmi > 30 \&\& goals.includes('hormonal')) {

# &#x20;     fastWindow = '18:6'; eatStart = '12:00'; eatEnd = '18:00';

# &#x20;   } else if (bmi < 18.5 || act >= 1.725) {

# &#x20;     fastWindow = '14:10'; eatStart = '10:00'; eatEnd = '20:00';

# &#x20;   } else {

# &#x20;     fastWindow = '16:8'; eatStart = '12:00'; eatEnd = '20:00';

# &#x20;   }

# &#x20; }

# 

# &#x20; // Sulforaphane

# &#x20; const sulph\_g = bmi > 27 ? 80 : 60;

# 

# &#x20; // Meditation

# &#x20; const medMin = stress === 'high' ? 25 : stress === 'moderate' ? 15 : 10;

# 

# &#x20; // Calorie target

# &#x20; let calTarget;

# &#x20; if (goals.includes('weight') \&\& bmi > 24) calTarget = Math.round(tdee \* 0.88);

# &#x20; else if (goals.includes('hormonal') \&\& sex === 'male') calTarget = Math.round(tdee \* 0.98);

# &#x20; else calTarget = tdee;

# 

# &#x20; // Toxin risk tier

# &#x20; const toxRisk = toxScore <= 3 ? 'Low' : toxScore <= 8 ? 'Moderate' : 'High';

# &#x20; const toxColour = toxScore <= 3 ? 'var(--green)' : toxScore <= 8 ? 'var(--amber)' : 'var(--red)';

# 

# &#x20; // Caffeine

# &#x20; const caffLimit = stress === 'high' ? '1 cup before 12:00' : age > 40 ? 'up to 2 cups, none after 14:00' : 'up to 2–3 cups, none after 14:00';

# 

# &#x20; // Sleep note

# &#x20; const sleepNote = sleep < 6

# &#x20;   ? '⚠️ Critical: sleep below 6h reduces testosterone 10–15% and severely impairs prefrontal cognition. This is your #1 priority above all other interventions.'

# &#x20;   : sleep < 7

# &#x20;   ? '⚠️ Below optimal. Aim for 7–9h. Even one extra hour improves testosterone, cortisol recovery, and cognitive consolidation significantly.'

# &#x20;   : sleep >= 9 \&\& sex === 'male'

# &#x20;   ? 'Good. Maintain consistent wake time (±30 min). Testosterone peaks in early AM REM sleep.'

# &#x20;   : 'Good. Maintain consistent sleep/wake times. Especially important for circadian hormonal patterning.';

# 

# &#x20; /\* ── STAT HEADER ── \*/

# &#x20; document.getElementById('resultStats').innerHTML = `

# &#x20;   <div class="result-stat">

# &#x20;     <div class="label">BMI</div>

# &#x20;     <div class="value">${bmi.toFixed(1)}</div>

# &#x20;     <div class="sub">${bmiC}</div>

# &#x20;   </div>

# &#x20;   <div class="result-stat">

# &#x20;     <div class="label">Daily Calories</div>

# &#x20;     <div class="value">${calTarget.toLocaleString()}</div>

# &#x20;     <div class="sub">kcal/day (TDEE ${tdee.toLocaleString()})</div>

# &#x20;   </div>

# &#x20;   <div class="result-stat">

# &#x20;     <div class="label">Protein Target</div>

# &#x20;     <div class="value">${protMin}–${protMax}g</div>

# &#x20;     <div class="sub">${(protMin/weight).toFixed(1)}–${(protMax/weight).toFixed(1)} g/kg</div>

# &#x20;   </div>

# &#x20;   <div class="result-stat">

# &#x20;     <div class="label">Fasting Window</div>

# &#x20;     <div class="value">${fastWindow}</div>

# &#x20;     <div class="sub">${eatStart !== 'N/A' ? `Eat ${eatStart}–${eatEnd}` : 'Not recommended now'}</div>

# &#x20;   </div>

# &#x20;   <div class="result-stat">

# &#x20;     <div class="label">Broccoli Sprouts</div>

# &#x20;     <div class="value">${sulph\_g}g</div>

# &#x20;     <div class="sub">daily (Nrf2 / detox)</div>

# &#x20;   </div>

# &#x20;   <div class="result-stat">

# &#x20;     <div class="label">EDC Risk Level</div>

# &#x20;     <div class="value" style="color:${toxColour}">${toxRisk}</div>

# &#x20;     <div class="sub">Score: ${toxScore}/26 checked</div>

# &#x20;   </div>

# &#x20;   <div class="result-stat">

# &#x20;     <div class="label">Meditation</div>

# &#x20;     <div class="value">${medMin} min</div>

# &#x20;     <div class="sub">daily minimum</div>

# &#x20;   </div>`;

# 

# &#x20; /\* ── ROUTINE BODY ── \*/

# &#x20; let html = '';

# 

# &#x20; // ─── PRIORITY ALERT ───

# &#x20; if (sleep < 7 || stress === 'high' || toxScore > 8) {

# &#x20;   html += `<div class="callout c-red" style="margin-bottom:20px;"><span class="callout-i">⚠️</span><div><strong>Priority flags in your profile:</strong><ul style="margin-top:6px;margin-left:14px;font-size:0.83rem;">`;

# &#x20;   if (sleep < 7) html += `<li>Sleep below optimal — prioritise this above all supplements or diet tweaks.</li>`;

# &#x20;   if (stress === 'high') html += `<li>Chronic high stress: cortisol is your #1 testosterone and cognitive suppressor. MBSR is your highest-ROI intervention.</li>`;

# &#x20;   if (toxScore > 8) html += `<li>High EDC exposure score: EDC reduction should be immediate priority, especially for reproductive health.</li>`;

# &#x20;   html += `</ul></div></div>`;

# &#x20; }

# 

# &#x20; // ─── EDC REDUCTION PLAN ───

# &#x20; if (goals.includes('detox') || toxScore >= 4) {

# &#x20;   html += `<div class="routine-block">

# &#x20;     <div class="rb-head"><span class="rb-badge" style="background:var(--rose-l);color:var(--rose);">🛡️ EDC Reduction — Priority Actions</span>

# &#x20;       <span style="font-size:0.75rem;color:var(--muted);">EDC Risk: <strong style="color:${toxColour}">${toxRisk}</strong> (score ${toxScore}/26)</span>

# &#x20;     </div>

# &#x20;     <div class="rb-items">`;

# &#x20;   html += rbItem('fem', 'Replace food storage', 'Glass / stainless', 'Highest single-impact action. Never heat food in plastic — temperature accelerates BPA/phthalate leaching. Use glass Tupperware or stainless steel containers.');

# &#x20;   html += rbItem('fem', 'Filter drinking water', 'Reverse osmosis or carbon filter', 'Removes microplastics, heavy metals (cadmium, lead), chlorine by-products and pharmaceutical residues. Refill in glass or stainless.');

# &#x20;   html += rbItem('fem', 'Switch personal care', 'Phthalate-free, fragrance-free', 'Check labels for "parfum/fragrance" — often contains phthalates. Use EWG Skin Deep database. Priority for females — phthalate exposure linked to POI (OR 3.4).');

# &#x20;   html += rbItem('det', 'Avoid thermal paper', 'Wash hands after receipts', 'Thermal paper is a major BPA source — absorbed transdermally. Opt for digital receipts. Particularly important for females of reproductive age.');

# &#x20;   if (sex === 'female') html += rbItem('fem', 'Choose organic Dirty Dozen', 'Priority 12 produce', 'Strawberries, spinach, kale, peaches, pears, nectarines, apples, grapes, capsicum, celery, cherries, tomatoes. Pesticide residues act as EDCs on the HPG axis.');

# &#x20;   html += `</div></div>`;

# &#x20; }

# 

# &#x20; // ─── MORNING ───

# &#x20; html += `<div class="routine-block">

# &#x20;   <div class="rb-head"><span class="rb-badge rb-morning">☀️ Morning</span><span style="font-size:0.75rem;color:var(--muted);">On waking → until ${eatStart}</span></div>

# &#x20;   <div class="rb-items">`;

# &#x20; html += rbItem('cog', 'Wake at consistent time', '±30 min every day', 'Anchors the cortisol awakening response. Most critical circadian signal — even on weekends. Sets daily testosterone and cortisol patterns.');

# &#x20; html += rbItem('det', 'Morning water — glass/stainless', '500 ml, room temperature', 'Rehydrate after overnight fast. Avoid plastic bottles. Filtered water preferred. No flavour additives.');

# &#x20; if (goals.includes('cognitive') || stress !== 'low') {

# &#x20;   html += rbItem('cog', 'Focused Attention Meditation', `${medMin} min`, `Activates bilateral dlPFC, increases theta power. Use breath-focus. Even ${medMin} min shows measurable attentional improvement after 4 weeks (NCCIH-funded evidence). App: Insight Timer (free) or Waking Up.`);

# &#x20; }

# &#x20; if (sex === 'male' \&\& fastWindow !== '14:10') {

# &#x20;   html += rbItem('hor', `Continue fast until ${eatStart}`, fastWindow + ' protocol', 'Maintains elevated GH pulses and AMPK activation for testosterone support. Black coffee/green tea permitted — zero calories only. Disrupting the fast halts GH pulsatility.');

# &#x20; }

# &#x20; if (sex === 'female') {

# &#x20;   html += rbItem('fem', `${fastWindow} fasting note`, 'End fast at ' + eatStart, cycleStatus === 'pregnant' ? '⚠️ Fasting not recommended during pregnancy/breastfeeding. Eat normally. Focus on dietary quality instead.' : 'Female-conservative 14:10 window. If hair loss is a concern, consider reducing to 12:12 or pausing fasting. Listen to body signals — some women do better eating within 2h of waking on training days.');

# &#x20; }

# &#x20; html += `</div></div>`;

# 

# &#x20; // ─── FIRST MEAL ───

# &#x20; html += `<div class="routine-block">

# &#x20;   <div class="rb-head"><span class="rb-badge rb-midday">🍽️ First Meal (${eatStart})</span></div>

# &#x20;   <div class="rb-items">`;

# &#x20; html += rbItem('hor', 'High-quality protein', `${Math.round(protMin \* 0.35)}–${Math.round(protMax \* 0.35)}g`, sex === 'female' ? 'Eggs, fish, legumes, Greek yoghurt. Leucine-rich sources for muscle protein synthesis. Essential for follicular health and hormonal precursor supply.' : 'Eggs, fish, or legumes. Leucine-rich sources support muscle protein synthesis. Rate-limiting for testosterone precursor availability.');

# &#x20; html += rbItem('det', 'Broccoli sprouts or broccoli', `${sulph\_g}g sprouts or 200g broccoli`, 'Lightly steam broccoli (3–4 min). Sprouts are 10–100× more potent — eat raw in smoothies or salads. Best on semi-empty stomach. Nrf2 activation peaks \~3h after intake.');

# &#x20; html += rbItem('hor', 'Extra-virgin olive oil', '1–2 tbsp', sex === 'female' ? 'Anti-inflammatory polyphenols support follicular health. Add to salad or vegetables. Mediterranean dietary pattern reduces PCOS androgen markers.' : 'Rich in oleic acid and polyphenols — supports testosterone synthesis and improves sperm quality. Add to salad or vegetables.');

# &#x20; if (sex === 'male' \&\& (goals.includes('hormonal') || goals.includes('weight'))) {

# &#x20;   html += rbItem('hor', 'Zinc-rich food', '30–40g pumpkin seeds or oysters', 'Zinc is rate-limiting cofactor for testosterone synthesis. Aim 11 mg/day. Pumpkin seeds and oysters are the most practical sources. Deficiency is widespread and directly suppresses LH and testosterone.');

# &#x20; }

# &#x20; if (sex === 'female' \&\& (goals.includes('fertility') || goals.includes('hormonal'))) {

# &#x20;   html += rbItem('fem', 'Folate-rich food', 'Leafy greens, legumes', 'Folate supports ovarian health and reduces neural tube defect risk if pregnancy is a goal. Spinach, lentils, asparagus — prioritise food sources over synthetic folic acid where possible.');

# &#x20; }

# &#x20; html += `</div></div>`;

# 

# &#x20; // ─── AFTERNOON ───

# &#x20; html += `<div class="routine-block">

# &#x20;   <div class="rb-head"><span class="rb-badge rb-midday">🌤️ Afternoon</span></div>

# &#x20;   <div class="rb-items">`;

# &#x20; if (goals.includes('cognitive')) {

# &#x20;   html += rbItem('cog', 'Structured cognitive work block', '90 min, then break', 'Work in 90-min ultradian cycles — matches natural alertness rhythms. Use Pomodoro if needed. Structured cognitive engagement IS your cognitive training without additional tools.');

# &#x20; }

# &#x20; html += rbItem('hor', 'Resistance training', '4–5 compound exercises, 3–4 sets', sex === 'female' ? 'Compound lifts (squat, hip hinge, push, pull). Resistance training improves insulin sensitivity (key for PCOS) and raises resting metabolic rate. Evidence is strong for female hormonal health.' : 'Compound lifts (squat, deadlift, press). Resistance training acutely raises testosterone and GH. Fasted or fed — both effective for hormonal response.');

# &#x20; if (goals.includes('cognitive') || stress !== 'low') {

# &#x20;   const omMin = Math.max(10, Math.round(medMin \* 0.6));

# &#x20;   html += rbItem('cog', 'Open Monitoring Meditation', `${omMin} min`, 'Post-workout or mid-afternoon. Observe thoughts without engaging — distinct mechanism from FA. Targets default-mode network regulation and reduces rumination. BA vs MBCT for anhedonia: both equally effective (2024 RCT).');

# &#x20; }

# &#x20; html += rbItem('hor', 'Fatty fish', '100–150g', sex === 'female' ? 'Salmon, mackerel, or sardines 2–3×/week. EPA/DHA reduces ovarian inflammation and supports folliculogenesis. Vitamin D from fish supports hormone synthesis. Low mercury options: sardines, mackerel, salmon.' : 'Salmon, mackerel, or sardines. EPA/DHA 2–3×/week reduces inflammation and supports Leydig cell function. Rich in vitamin D — often deficient in Indian populations.');

# &#x20; html += `</div></div>`;

# 

# &#x20; // ─── EVENING ───

# &#x20; html += `<div class="routine-block">

# &#x20;   <div class="rb-head"><span class="rb-badge rb-evening">🌙 Evening (last meal by ${eatEnd})</span></div>

# &#x20;   <div class="rb-items">`;

# &#x20; html += rbItem('hor', 'Remaining protein', `${Math.round(protMin \* 0.35)}–${Math.round(protMax \* 0.35)}g`, sex === 'female' ? 'Complete daily protein target. Slow-digesting sources (cottage cheese, lentils) for overnight repair and follicular support.' : 'Complete daily protein target. Slow-digesting sources (cottage cheese, legumes) for overnight muscle protein synthesis during GH pulses.');

# &#x20; html += rbItem('det', 'Diverse plant foods', '5+ plant varieties with dinner', 'Diverse plants bind microplastics and oestrogen metabolites in gut, facilitating excretion. Aim 30+ different plant foods/week (gut microbiome evidence). Fibre supports oestrogen clearance — critical for both sexes.');

# &#x20; html += rbItem('hor', 'Close eating window by', eatEnd, 'Strict adherence is the most important TRF variable. Late eating impairs insulin sensitivity and disrupts circadian hormonal patterns — particularly GH pulses and cortisol recovery overnight.');

# &#x20; if (sex === 'female' \&\& (cycleStatus === 'peri' || cycleStatus === 'post')) {

# &#x20;   html += rbItem('fem', 'CBT-I Sleep Protocol', 'Wind-down routine from 21:00', 'Menopausal insomnia affects 50% of post-menopausal women. CBT-I outperforms HRT for sleep in pooled RCTs. Stimulus control + relaxation training + cognitive restructuring. Apps: Sleepio (NHS-validated).');

# &#x20; }

# &#x20; html += rbItem('cog', 'No screens 60–90 min before bed', 'Blue light filter from 21:00', 'Blue light suppresses melatonin, delays sleep onset, and impairs overnight testosterone/GH pulses. Use warm lighting after 21:00. Critical for females with MTNR1B variant risk and PCOS.');

# &#x20; html += rbItem('cog', 'Sleep target', '7–9 hours', sleepNote);

# &#x20; html += `</div></div>`;

# 

# &#x20; // ─── FEMALE-SPECIFIC CYCLE SECTION ───

# &#x20; if (sex === 'female') {

# &#x20;   let cycleAdvice = '';

# &#x20;   if (cycleStatus === 'irregular') {

# &#x20;     cycleAdvice = 'PCOS / irregular cycles: prioritise EDC reduction, low-GI Mediterranean diet, and insulin sensitisation (resistance training + reduced refined carbs). Even 5–10% weight reduction restores ovulatory function in PCOS. Consider inositol supplementation (physician-guided).';

# &#x20;   } else if (cycleStatus === 'peri') {

# &#x20;     cycleAdvice = 'Perimenopause: hormone fluctuations disrupt sleep and cognition. CBT-I is first-line for sleep. MBSR shows particular promise for menopausal brain fog. Support adrenal resilience via stress management and adequate dietary fat.';

# &#x20;   } else if (cycleStatus === 'post') {

# &#x20;     cycleAdvice = 'Post-menopause: oestrogen withdrawal impairs PFC function and sleep. MBIs showed cognitive benefit specifically in post-menopausal cohorts. Resistance training preserves bone density and metabolic function. Discuss HRT suitability with a gynaecologist.';

# &#x20;   } else if (cycleStatus === 'pregnant') {

# &#x20;     cycleAdvice = 'Pregnancy/breastfeeding: avoid fasting, maximise dietary diversity and folate, avoid all EDC exposure where possible. Sulforaphane is generally considered safe — consult your midwife. Sleep optimisation and gentle movement are the primary focus.';

# &#x20;   } else {

# &#x20;     cycleAdvice = 'Regular cycles: EDC reduction remains important — BPA and phthalates accumulate and can affect future fertility even without current symptoms. Mediterranean diet and resistance training support hormonal balance and long-term ovarian reserve.';

# &#x20;   }

# &#x20;   html += `<div class="routine-block">

# &#x20;     <div class="rb-head"><span class="rb-badge rb-female">🌸 Female-Specific Guidance</span></div>

# &#x20;     <div class="rb-items">`;

# &#x20;   html += rbItem('fem', 'Cycle-specific notes', cycleStatus, cycleAdvice);

# &#x20;   html += rbItem('fem', 'Omega-3 priority', '2g EPA+DHA/day', 'Reduces ovarian inflammation and supports folliculogenesis. 2–3 servings oily fish/week OR high-quality supplement (algae-based for DHA is cleanest source). Anti-inflammatory effect directly relevant to PCOS and POI risk reduction.');

# &#x20;   html += rbItem('fem', 'Iron-rich foods (menstruating)', 'With vitamin C source', 'Menstrual blood loss creates iron deficit in many women. Iron supports energy, cognition, and thyroid function — all commonly attributed to "brain fog" in females. Red meat 1–2×/week, or lentils + lemon juice.');

# &#x20;   html += `</div></div>`;

# &#x20; }

# 

# &#x20; // ─── WEEKLY ───

# &#x20; html += `<div class="routine-block">

# &#x20;   <div class="rb-head"><span class="rb-badge rb-weekly">📅 Weekly</span></div>

# &#x20;   <div class="rb-items">`;

# &#x20; if (goals.includes('cognitive')) {

# &#x20;   html += rbItem('cog', 'Behavioural Activation planning', 'Sunday, 15 min', 'Schedule one genuinely rewarding activity per day for the week. NIMH-funded research: planned positive events increase reward sensitivity within 1–2 weeks. This breaks the lethargy-withdrawal-inactivity cycle.');

# &#x20; }

# &#x20; html += rbItem('psych', 'Social connection', '≥2 meaningful interactions', 'Isolation chronically elevates cortisol — directly antagonistic to testosterone and prefrontal cognitive function. Prioritise face-to-face contact where possible.');

# &#x20; html += rbItem('det', 'Audit EDC exposure', 'Ongoing reduction', 'Replace one plastic item per week with glass/stainless. Check EWG database for personal care products. Highest leverage: food storage → water → cookware.');

# &#x20; if (sex === 'male' \&\& (goals.includes('hormonal') || goals.includes('weight'))) {

# &#x20;   html += rbItem('hor', 'Sun exposure', '15–20 min, 3×/week', 'Vitamin D is a testosterone precursor. Deficiency is prevalent in South Asian populations. Arms/legs exposure — avoid sunscreen during this window. Supplement with 2000–4000 IU D3 in winter months.');

# &#x20; }

# &#x20; if (sex === 'female' \&\& goals.includes('hormonal')) {

# &#x20;   html += rbItem('fem', 'Vitamin D \& K2', '2000–4000 IU D3 + MK-7', 'Vitamin D deficiency is associated with PCOS and impaired folliculogenesis. K2 directs calcium to bones vs arteries. Physician testing recommended to determine individual needs — serum 25(OH)D target 50–80 nmol/L.');

# &#x20; }

# &#x20; html += `</div></div>`;

# 

# &#x20; // ─── SCORE BARS (tab 2) ───

# &#x20; const sleepScore = Math.min(100, sleep >= 8 ? 100 : sleep >= 7 ? 80 : sleep >= 6 ? 50 : 20);

# &#x20; const stressScore = stress === 'low' ? 95 : stress === 'moderate' ? 60 : 25;

# &#x20; const toxBar = Math.max(5, 100 - (toxScore / 26) \* 100);

# &#x20; const bmiScore = bmi >= 18.5 \&\& bmi <= 24.9 ? 95 : bmi < 18.5 ? 55 : bmi < 30 ? 60 : 30;

# &#x20; const actScore = act >= 1.725 ? 95 : act >= 1.55 ? 78 : act >= 1.375 ? 55 : 30;

# 

# &#x20; let scoresHtml = `

# &#x20;   <h3 style="margin-bottom:16px;">Your health profile scores</h3>

# &#x20;   <p style="font-size:0.83rem;color:var(--muted);margin-bottom:18px;">Scores reflect population-level benchmarks for each input. Higher = better baseline; lower = higher priority for intervention.</p>

# &#x20;   <div style="padding:18px;background:var(--off);border-radius:var(--r2);border:1px solid var(--border);margin-bottom:20px;">`;

# &#x20; scoresHtml += scoreBar('Sleep Quality', sleepScore, 'var(--blue)');

# &#x20; scoresHtml += scoreBar('Stress Resilience', stressScore, 'var(--green)');

# &#x20; scoresHtml += scoreBar('EDC / Toxin Protection', toxBar, 'var(--rose)');

# &#x20; scoresHtml += scoreBar('Body Composition', bmiScore, 'var(--amber)');

# &#x20; scoresHtml += scoreBar('Physical Activity', actScore, 'var(--blue)');

# &#x20; scoresHtml += `</div>`;

# 

# &#x20; // Score interpretation

# &#x20; const lowestScore = Math.min(sleepScore, stressScore, toxBar, bmiScore, actScore);

# &#x20; const lowestLabel = \[

# &#x20;   \['Sleep Quality', sleepScore], \['Stress Resilience', stressScore],

# &#x20;   \['EDC / Toxin Protection', toxBar], \['Body Composition', bmiScore], \['Physical Activity', actScore]

# &#x20; ].sort((a,b) => a\[1]-b\[1])\[0]\[0];

# 

# &#x20; scoresHtml += `<div class="callout c-blue">

# &#x20;   <span class="callout-i">🎯</span>

# &#x20;   <div><strong>Highest priority area:</strong> ${lowestLabel} (score: ${Math.round(lowestScore)}%). This is where targeted effort will yield the greatest systemic benefit. See the Smart Notes tab for specific guidance.</div>

# &#x20; </div>`;

# 

# &#x20; // ─── NOTES (tab 3) ───

# &#x20; let notesHtml = `<h3 style="margin-bottom:16px;">Personalised smart notes</h3><div class="notes-grid">`;

# &#x20; notesHtml += `<div class="note-card"><div class="note-title">☕ Caffeine</div>

# &#x20;   <p>Permitted during fast (black only). Limit: ${caffLimit}. Adenosine antagonism acutely improves focus. Avoid after 14:00 — caffeine half-life of 5–6h impairs sleep even when you feel unaffected.</p></div>`;

# &#x20; notesHtml += `<div class="note-card"><div class="note-title">💧 Hydration</div>

# &#x20;   <p>Target ${Math.round(weight \* 35)} ml/day (${(weight \* 35 / 1000).toFixed(1)} L). Use glass or stainless containers. Filtered preferred. Increase by 500 ml per hour of exercise.</p></div>`;

# &#x20; notesHtml += `<div class="note-card"><div class="note-title">🧠 Cognition</div>

# &#x20;   <p>${goals.includes('cognitive') ? 'Your primary goal. Start: 15 min FA meditation daily for 4 weeks. If brain fog persists: 8-week MBSR programme. Still persists: discuss pharmacological options (guanfacine, methylphenidate) with a physician.' : 'Consider 15 min/day FA meditation. NCCIH evidence base is strongest of all non-pharmacological cognitive interventions — effects compound significantly after 8 weeks.'}</p></div>`;

# &#x20; notesHtml += `<div class="note-card"><div class="note-title">🌿 Sulforaphane</div>

# &#x20;   <p>Best absorbed fasted. Avoid cooking above 70°C — destroys myrosinase. Add raw mustard seed powder to cooked broccoli to restore enzymatic conversion. Never freeze sprouts. 50g raw sprouts ≈ 200g mature broccoli in sulforaphane content.</p></div>`;

# &#x20; notesHtml += `<div class="note-card"><div class="note-title">🌡️ Sleep environment</div>

# &#x20;   <p>Bedroom: 20–25°C, \&lt;10 lux at night, \&lt;40 dB. Warm (yellow) lighting after 20:00. Wake at a consistent time — more important than consistent bedtime for circadian anchoring. CBT-I (Sleepio, NHS-validated) if insomnia persists \&gt;4 weeks.</p></div>`;

# &#x20; notesHtml += `<div class="note-card"><div class="note-title">🛡️ EDC audit</div>

# &#x20;   <p>Priority order: (1) switch food storage to glass/stainless, (2) filter drinking water, (3) swap synthetic fragrances, (4) choose organic for high-pesticide produce. Replace one item per week. Check personal care products at EWG Skin Deep.</p></div>`;

# &#x20; if (bmi > 27) notesHtml += `<div class="note-card"><div class="note-title">⚡ BMI ${bmi.toFixed(1)} note</div><p>Visceral fat drives ${sex === 'male' ? 'testosterone-to-oestrogen aromatisation, suppressing free testosterone. Fat loss will have an outsized hormonal benefit.' : 'insulin resistance and hyperandrogenism in PCOS. Even 5–10% weight reduction restores ovulatory function.'}  The TRF window + Mediterranean diet will synergise strongly here.</p></div>`;

# &#x20; if (bmi < 19) notesHtml += `<div class="note-card"><div class="note-title">⚠️ Low body weight</div><p>Insufficient dietary fat suppresses ${sex === 'male' ? 'testosterone' : 'oestrogen and ovulatory function'}. Ensure ≥25–30% of calories from fat (predominantly unsaturated). Do not restrict calories.</p></div>`;

# &#x20; if (sex === 'female' \&\& cycleStatus !== 'pregnant') notesHtml += `<div class="note-card"><div class="note-title">🌸 Female fasting note</div><p>Keep fasting window ≤16h. Evidence for longer fasts in women is limited. If cycle irregularities, hair loss, or fatigue worsen — reduce to 12:12 or stop. Avoid fasting in the luteal phase (days 15–28) if stress is elevated.</p></div>`;

# &#x20; if (stress === 'high') notesHtml += `<div class="note-card"><div class="note-title">🧘 Stress — top priority</div><p>Chronic cortisol is your #1 testosterone, cognitive, and sleep suppressor. MBSR for ${medMin} min/day has the strongest ROI of any single intervention — prioritise this above all other additions.</p></div>`;

# &#x20; if (age >= 60) notesHtml += `<div class="note-card"><div class="note-title">🎮 Exergaming note</div><p>For age 60+, interactive exergaming shows a large effect on sleep quality (SMD = −1.38) when maintained ≥8 weeks — comparable to traditional exercise but with higher adherence for many. Consider Wii Fit, Ring Fit Adventure, or dance games.</p></div>`;

# &#x20; notesHtml += `</div>

# &#x20; <div class="result-disclaimer">

# &#x20;   ⚠️ <strong>Medical disclaimer:</strong> This routine is generated from population-level research adjusted for your biometric and lifestyle inputs. It is not personalised medical advice. Consult a qualified physician before starting any new dietary, fasting, or supplementation protocol — especially if you have existing health conditions, PCOS, fertility concerns, or are pregnant/breastfeeding. Pharmacological interventions require a valid prescription and individual risk assessment.

# &#x20; </div>`;

# 

# &#x20; // ─── INJECT INTO TABS ───

# &#x20; document.getElementById('resultRoutine').innerHTML = html;

# &#x20; document.getElementById('resultScores').innerHTML = scoresHtml;

# &#x20; document.getElementById('resultNotes').innerHTML = notesHtml;

# 

# &#x20; // Show tabs

# &#x20; document.getElementById('resultTabs').style.display = 'flex';

# &#x20; switchTab('routine', document.querySelector('.rtab\[data-tab="routine"]'));

# 

# &#x20; document.getElementById('resultPanel').classList.add('visible');

# &#x20; setTimeout(() => document.getElementById('resultPanel').scrollIntoView({ behavior: 'smooth', block: 'start' }), 80);

# 

# &#x20; // Reset button state

# &#x20; btn.disabled = false;

# &#x20; btnText.style.display = 'inline';

# &#x20; btnLoading.style.display = 'none';

# }

# 

# /\* ── TAB SWITCHING ── \*/

# function switchTab(tabName, btn) {

# &#x20; document.querySelectorAll('.tab-content').forEach(t => t.style.display = 'none');

# &#x20; document.querySelectorAll('.rtab').forEach(b => b.classList.remove('active'));

# &#x20; document.getElementById('tab-' + tabName).style.display = 'block';

# &#x20; if (btn) btn.classList.add('active');

# }

# 

# /\* ── COPY ROUTINE ── \*/

# function copyRoutine() {

# &#x20; const routineEl = document.getElementById('resultRoutine');

# &#x20; if (!routineEl) return;

# &#x20; const text = routineEl.innerText || routineEl.textContent;

# &#x20; navigator.clipboard.writeText(text).then(() => {

# &#x20;   const btn = document.getElementById('copyBtn');

# &#x20;   btn.textContent = '✓ Copied!';

# &#x20;   btn.style.color = 'var(--green)';

# &#x20;   btn.style.borderColor = 'var(--green)';

# &#x20;   setTimeout(() => {

# &#x20;     btn.textContent = '📋 Copy Routine';

# &#x20;     btn.style.color = '';

# &#x20;     btn.style.borderColor = '';

# &#x20;   }, 2000);

# &#x20; }).catch(() => {

# &#x20;   // Fallback for older browsers

# &#x20;   const range = document.createRange();

# &#x20;   range.selectNode(routineEl);

# &#x20;   window.getSelection().removeAllRanges();

# &#x20;   window.getSelection().addRange(range);

# &#x20;   document.execCommand('copy');

# &#x20;   window.getSelection().removeAllRanges();

# &#x20; });

# }

# 

# function rbItem(type, name, dose, note) {

# &#x20; return `<div class="rb-item ${type}">

# &#x20;   <div class="rb-name">${name}</div>

# &#x20;   <div class="rb-dose">${dose}</div>

# &#x20;   <div class="rb-note">${note}</div>

# &#x20; </div>`;

# }

# 

# function scoreBar(label, pct, colour) {

# &#x20; const rounded = Math.round(pct);

# &#x20; const desc = rounded >= 80 ? 'Good' : rounded >= 55 ? 'Fair' : 'Needs attention';

# &#x20; const descCol = rounded >= 80 ? 'var(--green)' : rounded >= 55 ? 'var(--amber)' : 'var(--red)';

# &#x20; return `<div class="score-bar-wrap" style="margin-bottom:12px;">

# &#x20;   <div class="score-bar-label">

# &#x20;     <span>${label}</span>

# &#x20;     <span style="display:flex;gap:8px;align-items:center;">

# &#x20;       <span style="font-size:0.68rem;font-weight:700;color:${descCol};">${desc}</span>

# &#x20;       <span style="color:var(--muted);font-size:0.7rem;">${rounded}%</span>

# &#x20;     </span>

# &#x20;   </div>

# &#x20;   <div class="score-bar"><div class="score-fill" style="width:${rounded}%;background:${colour};transition:width 1s ease;"></div></div>

# &#x20; </div>`;

# }

# </script>

# </body>

# </html>

