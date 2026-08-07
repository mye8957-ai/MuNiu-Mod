
:root{
  --bg:#101216;
  --bg-raise:#181b21;
  --panel:#1c1f26;
  --line:rgba(255,255,255,0.08);
  --line-strong:rgba(255,255,255,0.14);
  --text:#eef0f2;
  --text-dim:#9096a1;
  --text-faint:#5c6270;
  --signal:#45e0a0;
  --signal-dim:#2b8f68;
  --warn:#e8a33d;
  --mono:'JetBrains Mono', 'SFMono-Regular', Consolas, monospace;
  --sans:-apple-system, BlinkMacSystemFont, "PingFang SC", "Microsoft YaHei", "Segoe UI", sans-serif;
}

*{margin:0;padding:0;box-sizing:border-box;}

html{scroll-behavior:smooth;}

body{
  background:var(--bg);
  color:var(--text);
  font-family:var(--sans);
  overflow-x:hidden;
  position:relative;
}

body::before{
  content:'';
  position:fixed;
  inset:0;
  background-image:
    radial-gradient(circle at 15% 10%, rgba(69,224,160,0.08), transparent 40%),
    radial-gradient(circle at 85% 60%, rgba(69,224,160,0.05), transparent 45%);
  pointer-events:none;
  z-index:0;
}

body::after{
  content:'';
  position:fixed;
  inset:0;
  background-image:
    linear-gradient(rgba(255,255,255,0.015) 1px, transparent 1px),
    linear-gradient(90deg, rgba(255,255,255,0.015) 1px, transparent 1px);
  background-size:48px 48px;
  pointer-events:none;
  z-index:0;
  mask-image:radial-gradient(ellipse 80% 60% at 50% 0%, black, transparent 70%);
}

::selection{
  background:var(--signal);
  color:#0a0c0f;
}

.wrap{
  position:relative;
  z-index:1;
  max-width:920px;
  margin:0 auto;
  padding:0 28px;
}

/* ---------- nav ---------- */

nav{
  position:fixed;
  top:0;
  left:0;
  right:0;
  z-index:100;
  padding:18px 0;
  transition:padding 0.4s cubic-bezier(0.16,1,0.3,1), background 0.4s ease;
}

nav.scrolled{
  padding:12px 0;
  background:rgba(16,18,22,0.55);
  backdrop-filter:blur(18px) saturate(140%);
  -webkit-backdrop-filter:blur(18px) saturate(140%);
  border-bottom:1px solid var(--line);
}

.nav-inner{
  max-width:920px;
  margin:0 auto;
  padding:0 28px;
  display:flex;
  align-items:center;
  justify-content:space-between;
}

.brand{
  display:flex;
  align-items:center;
  gap:10px;
  font-family:var(--mono);
  font-weight:700;
  font-size:15px;
  letter-spacing:0.02em;
}

.brand-dot{
  width:8px;
  height:8px;
  border-radius:50%;
  background:var(--signal);
  box-shadow:0 0 0 0 rgba(69,224,160,0.5);
  animation:pulse-dot 2.4s ease-out infinite;
}

@keyframes pulse-dot{
  0%{box-shadow:0 0 0 0 rgba(69,224,160,0.45);}
  70%{box-shadow:0 0 0 8px rgba(69,224,160,0);}
  100%{box-shadow:0 0 0 0 rgba(69,224,160,0);}
}

.nav-links{
  display:flex;
  gap:28px;
  font-size:13.5px;
  color:var(--text-dim);
}

.nav-links a{
  color:inherit;
  text-decoration:none;
  position:relative;
  transition:color 0.25s ease;
}

.nav-links a:hover{color:var(--text);}

.nav-links a::after{
  content:'';
  position:absolute;
  left:0;
  bottom:-4px;
  width:0;
  height:1px;
  background:var(--signal);
  transition:width 0.3s cubic-bezier(0.16,1,0.3,1);
}

.nav-links a:hover::after{width:100%;}

/* ---------- hero ---------- */

.hero{
  padding:168px 0 120px;
  position:relative;
}

.eyebrow{
  display:inline-flex;
  align-items:center;
  gap:8px;
  font-family:var(--mono);
  font-size:12px;
  color:var(--signal);
  letter-spacing:0.08em;
  padding:5px 12px;
  border:1px solid rgba(69,224,160,0.25);
  border-radius:100px;
  background:rgba(69,224,160,0.06);
  opacity:0;
  animation:rise 0.7s cubic-bezier(0.16,1,0.3,1) 0.1s forwards;
}

h1{
  font-size:56px;
  line-height:1.12;
  font-weight:800;
  letter-spacing:-0.02em;
  margin:22px 0 20px;
  opacity:0;
  animation:rise 0.8s cubic-bezier(0.16,1,0.3,1) 0.22s forwards;
}

h1 span{
  color:var(--signal);
  font-family:var(--mono);
}

.hero-desc{
  font-size:16.5px;
  line-height:1.75;
  color:var(--text-dim);
  max-width:560px;
  margin-bottom:40px;
  opacity:0;
  animation:rise 0.8s cubic-bezier(0.16,1,0.3,1) 0.34s forwards;
}

.hero-actions{
  display:flex;
  gap:14px;
  flex-wrap:wrap;
  opacity:0;
  animation:rise 0.8s cubic-bezier(0.16,1,0.3,1) 0.46s forwards;
}

@keyframes rise{
  from{opacity:0; transform:translateY(16px);}
  to{opacity:1; transform:translateY(0);}
}

.btn{
  display:inline-flex;
  align-items:center;
  gap:9px;
  padding:14px 26px;
  border-radius:10px;
  font-size:14.5px;
  font-weight:600;
  text-decoration:none;
  cursor:pointer;
  border:1px solid transparent;
  transition:transform 0.35s cubic-bezier(0.16,1,0.3,1), box-shadow 0.35s ease, background 0.3s ease, border-color 0.3s ease;
  position:relative;
  overflow:hidden;
}

.btn-primary{
  background:var(--signal);
  color:#0a0f0c;
}

.btn-primary::before{
  content:'';
  position:absolute;
  inset:0;
  background:linear-gradient(120deg, transparent, rgba(255,255,255,0.35), transparent);
  transform:translateX(-120%) skewX(-15deg);
  transition:transform 0.7s ease;
}

.btn-primary:hover::before{transform:translateX(120%) skewX(-15deg);}

.btn-primary:hover{
  transform:translateY(-2px);
  box-shadow:0 12px 28px -8px rgba(69,224,160,0.45);
}

.btn-primary:active{transform:translateY(0px) scale(0.98);}

.btn-ghost{
  background:rgba(255,255,255,0.03);
  color:var(--text);
  border-color:var(--line-strong);
  backdrop-filter:blur(10px);
}

.btn-ghost:hover{
  background:rgba(255,255,255,0.07);
  border-color:rgba(255,255,255,0.24);
  transform:translateY(-2px);
}

.btn-ghost:active{transform:translateY(0px) scale(0.98);}

/* ---------- tutorial dropdown ---------- */

.tutorial-drop{
  position:relative;
}

.tutorial-trigger{
  font-family:var(--sans);
}

.tutorial-caret{
  width:14px !important;
  height:14px !important;
  margin-left:-2px;
  transition:transform 0.35s cubic-bezier(0.16,1,0.3,1);
}

.tutorial-drop.open .tutorial-caret{
  transform:rotate(180deg);
}

.tutorial-drop.open .tutorial-trigger{
  background:rgba(255,255,255,0.07);
  border-color:rgba(255,255,255,0.24);
}

.tutorial-menu{
  position:absolute;
  top:calc(100% + 10px);
  left:0;
  min-width:210px;
  background:rgba(24,27,33,0.92);
  border:1px solid var(--line-strong);
  border-radius:12px;
  backdrop-filter:blur(20px) saturate(150%);
  -webkit-backdrop-filter:blur(20px) saturate(150%);
  box-shadow:0 20px 40px -16px rgba(0,0,0,0.55), inset 0 1px 0 rgba(255,255,255,0.06);
  padding:6px;
  z-index:20;

  opacity:0;
  visibility:hidden;
  transform:translateY(-8px) scale(0.97);
  transform-origin:top left;
  transition:opacity 0.3s cubic-bezier(0.16,1,0.3,1), transform 0.3s cubic-bezier(0.16,1,0.3,1), visibility 0s linear 0.3s;
}

.tutorial-drop.open .tutorial-menu{
  opacity:1;
  visibility:visible;
  transform:translateY(0) scale(1);
  transition:opacity 0.3s cubic-bezier(0.16,1,0.3,1), transform 0.3s cubic-bezier(0.16,1,0.3,1), visibility 0s linear 0s;
}

.tutorial-menu a{
  display:flex;
  align-items:center;
  gap:10px;
  padding:11px 12px;
  border-radius:8px;
  color:var(--text);
  text-decoration:none;
  font-size:13.5px;
  transition:background 0.2s ease, padding-left 0.25s ease;
}

.tutorial-menu a:hover{
  background:rgba(69,224,160,0.09);
  padding-left:16px;
}

.tutorial-menu-tag{
  font-family:var(--mono);
  font-size:10.5px;
  font-weight:700;
  color:var(--signal);
  border:1px solid rgba(69,224,160,0.3);
  border-radius:5px;
  padding:2px 6px;
  flex-shrink:0;
}

.btn svg{width:16px;height:16px;flex-shrink:0;}

/* ---------- panel (signature element) ---------- */

.panel-stage{
  margin-top:64px;
  opacity:0;
  animation:rise 1s cubic-bezier(0.16,1,0.3,1) 0.58s forwards;
  perspective:1400px;
  transition:margin-top 0.35s cubic-bezier(0.16,1,0.3,1);
}

.glass-filter-defs{
  position:absolute;
  width:0;
  height:0;
  overflow:hidden;
}

.panel{
  background:rgba(24,27,33,0.6);
  border:1px solid var(--line-strong);
  border-radius:16px;
  backdrop-filter:blur(22px) saturate(140%);
  -webkit-backdrop-filter:blur(22px) saturate(140%);
  overflow:hidden;
  box-shadow:0 30px 60px -30px rgba(0,0,0,0.6), inset 0 1px 0 rgba(255,255,255,0.06);
  transform:perspective(900px) rotateX(2deg);
  transition:transform 0.5s cubic-bezier(0.16,1,0.3,1), box-shadow 0.5s ease;
  will-change:transform;
  touch-action:none;
}

.panel.tilting{
  transition:transform 0.15s ease-out;
}

.panel.pressing{
  transition:transform 0.18s cubic-bezier(0.34, 1.4, 0.4, 1), filter 0.18s ease;
  filter:blur(0.4px);
}

.panel.pressing.dragging{
  transition:transform 0.05s linear, filter 0.18s ease;
}

.panel.settling{
  transition:transform 0.65s cubic-bezier(0.34, 1.56, 0.42, 1), filter 0.4s ease;
  filter:blur(0px);
}

.panel-glass-warp{
  position:absolute;
  inset:0;
  z-index:0;
  pointer-events:none;
  opacity:0;
  backdrop-filter:url(#liquid-distortion) blur(1px);
  -webkit-backdrop-filter:url(#liquid-distortion) blur(1px);
  transition:opacity 0.5s ease;
}

.panel:hover .panel-glass-warp,
.panel.tilting .panel-glass-warp,
.panel.pressing .panel-glass-warp,
.panel.settling .panel-glass-warp{opacity:0.5;}

.panel-glass-shine{
  position:absolute;
  inset:0;
  z-index:1;
  pointer-events:none;
  border-radius:16px;
  background:radial-gradient(circle at var(--mx,50%) var(--my,20%), rgba(255,255,255,0.09), transparent 45%);
  opacity:0;
  transition:opacity 0.4s ease;
}

.panel:hover .panel-glass-shine,
.panel.tilting .panel-glass-shine,
.panel.pressing .panel-glass-shine,
.panel.settling .panel-glass-shine{opacity:1;}

.panel-bar{
  position:relative;
  z-index:2;
  display:flex;
  align-items:center;
  gap:8px;
  padding:13px 18px;
  border-bottom:1px solid var(--line);
  background:rgba(255,255,255,0.02);
}

.panel-dot{width:9px;height:9px;border-radius:50%;background:var(--text-faint);}
.panel-bar span{
  font-family:var(--mono);
  font-size:12px;
  color:var(--text-faint);
  margin-left:8px;
}

.panel-body{
  position:relative;
  z-index:2;
  padding:28px 24px;
  font-family:var(--mono);
  font-size:13px;
  line-height:2;
  color:var(--text-dim);
}

.panel-body .prompt{color:var(--signal);}
.panel-body .ok{color:var(--signal);}
.panel-body .path{color:var(--text-faint);}
.type-cursor{
  display:inline-block;
  width:7px;
  height:14px;
  background:var(--signal);
  margin-left:2px;
  animation:blink 1s step-end infinite;
  vertical-align:middle;
}

@keyframes blink{
  0%,50%{opacity:1;}
  51%,100%{opacity:0;}
}

/* ---------- sections shared ---------- */

section{
  padding:100px 0;
  position:relative;
}

.section-head{
  margin-bottom:52px;
}

.section-tag{
  font-family:var(--mono);
  font-size:12px;
  color:var(--signal);
  letter-spacing:0.1em;
  display:block;
  margin-bottom:12px;
}

.section-title{
  font-size:32px;
  font-weight:800;
  letter-spacing:-0.01em;
}

.reveal{
  opacity:0;
  transform:translateY(24px);
  transition:opacity 0.8s cubic-bezier(0.16,1,0.3,1), transform 0.8s cubic-bezier(0.16,1,0.3,1);
}

.reveal.in{
  opacity:1;
  transform:translateY(0);
}

/* ---------- about ---------- */

.about-grid{
  display:grid;
  grid-template-columns:1fr;
  gap:0;
}

.about-text{
  font-size:16.5px;
  line-height:1.9;
  color:var(--text-dim);
  max-width:680px;
}

.about-text strong{
  color:var(--text);
  font-weight:600;
}

.feature-row{
  display:grid;
  grid-template-columns:repeat(3, 1fr);
  gap:1px;
  margin-top:44px;
  background:var(--line);
  border:1px solid var(--line);
  border-radius:14px;
  overflow:hidden;
}

.feature-cell{
  background:var(--panel);
  padding:26px 22px;
  transition:background 0.3s ease;
}

.feature-cell:hover{background:var(--bg-raise);}

.feature-num{
  font-family:var(--mono);
  font-size:11px;
  color:var(--signal);
  margin-bottom:14px;
  display:block;
}

.feature-cell h3{
  font-size:15px;
  font-weight:600;
  margin-bottom:8px;
}

.feature-cell p{
  font-size:13px;
  color:var(--text-dim);
  line-height:1.7;
}

/* ---------- faq ---------- */

.faq-list{
  display:flex;
  flex-direction:column;
  gap:12px;
}

.faq-item{
  border:1px solid var(--line);
  border-radius:12px;
  background:rgba(255,255,255,0.015);
  overflow:hidden;
  transition:border-color 0.3s ease, background 0.3s ease;
}

.faq-item:hover{border-color:var(--line-strong);}

.faq-item.open{
  background:rgba(255,255,255,0.03);
  border-color:rgba(69,224,160,0.22);
}

.faq-q{
  display:flex;
  align-items:center;
  justify-content:space-between;
  gap:16px;
  padding:20px 22px;
  cursor:pointer;
  user-select:none;
}

.faq-q-left{
  display:flex;
  align-items:baseline;
  gap:14px;
}

.faq-mark{
  font-family:var(--mono);
  font-size:13px;
  font-weight:700;
  color:var(--warn);
  flex-shrink:0;
}

.faq-q-text{
  font-size:15.5px;
  font-weight:600;
}

.faq-toggle{
  width:20px;
  height:20px;
  flex-shrink:0;
  position:relative;
}

.faq-toggle::before,
.faq-toggle::after{
  content:'';
  position:absolute;
  background:var(--text-dim);
  transition:transform 0.4s cubic-bezier(0.16,1,0.3,1), background 0.3s ease;
}

.faq-toggle::before{
  width:12px;
  height:1.5px;
  top:9px;
  left:4px;
}

.faq-toggle::after{
  width:1.5px;
  height:12px;
  top:4px;
  left:9px;
}

.faq-item.open .faq-toggle::after{transform:rotate(90deg);}
.faq-item.open .faq-toggle::before{background:var(--signal);}
.faq-item.open .faq-toggle::after{background:var(--signal);}

.faq-a{
  max-height:0;
  overflow:hidden;
  transition:max-height 0.45s cubic-bezier(0.16,1,0.3,1);
}

.faq-a-inner{
  padding:0 22px 22px 22px;
  padding-left:48px;
  font-size:14.5px;
  line-height:1.8;
  color:var(--text-dim);
}

/* ---------- footer ---------- */

footer{
  margin-top:60px;
  border-top:1px solid var(--line);
  padding:28px 0;
}

.footer-inner{
  display:flex;
  align-items:center;
  justify-content:space-between;
  font-family:var(--mono);
  font-size:12px;
  color:var(--text-faint);
  flex-wrap:wrap;
  gap:10px;
}

/* ---------- responsive ---------- */

@media (max-width:720px){
  h1{font-size:38px;}
  .hero{padding:140px 0 80px;}
  .nav-links{display:none;}
  .feature-row{grid-template-columns:1fr;}
  .section-title{font-size:26px;}
  .footer-inner{flex-direction:column;text-align:center;}
  .tutorial-menu{left:auto;right:0;transform-origin:top right;}
}

@media (prefers-reduced-motion: reduce){
  *{animation-duration:0.01ms !important; animation-iteration-count:1 !important; transition-duration:0.01ms !important;}
}
