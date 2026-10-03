<!DOCTYPE html>
<html lang="en" data-theme="light">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover">
<meta name="theme-color" content="#eef6ff">
<title>Footstep Power Generation | Ω(1) Thinkers</title>
<style>
/* ============================================================
   MODULE 01 — Footstep base tokens
   ============================================================ */
:root{--mtc:#0b2a63;--mts:0 2px 16px rgba(255,255,255,.75);--tx:#06214d;--g:rgba(255,255,255,.38);--gb:rgba(255,255,255,.75);--sh:rgba(20,70,160,.35);--k1:rgba(255,255,255,.6);--k2:rgba(80,160,255,.4)}
:root[data-theme="dark"]{--mtc:#fff;--mts:0 0 22px rgba(120,190,255,.55);--tx:#eaf5ff;--g:rgba(110,170,255,.12);--gb:rgba(150,200,255,.35);--sh:rgba(0,0,0,.55);--k1:rgba(130,200,255,.4);--k2:rgba(20,90,220,.4)}
*{box-sizing:border-box}

/* ============================================================
   MODULE 02 — Lumenglass theme tokens
   ============================================================ */
:root{
  --bg-base:#eef6ff;
  --blob-a:rgba(122,176,255,.58);
  --blob-b:rgba(172,216,255,.62);
  --blob-c:rgba(228,242,255,.95);
  --glass-brd:rgba(255,255,255,.72);
  --glow:rgba(118,178,255,.9);
  --vig:rgba(78,132,205,.16);
  --toggle-bg:rgba(255,255,255,.46);
  --toggle-shadow:
      0 12px 34px rgba(31,84,155,.20),
      inset 0 1px 0 rgba(255,255,255,.85);
  --theme-fade:2s;
  --theme-ease:cubic-bezier(.4,0,.2,1);
}
html[data-theme="dark"]{
  --bg-base:#050b1a;
  --blob-a:rgba(46,102,220,.55);
  --blob-b:rgba(28,62,160,.6);
  --blob-c:rgba(96,148,245,.42);
  --glass-brd:rgba(152,196,255,.26);
  --glow:rgba(132,188,255,.95);
  --vig:rgba(1,4,16,.72);
  --toggle-bg:rgba(126,170,255,.14);
  --toggle-shadow:
      0 12px 34px rgba(0,6,25,.55),
      inset 0 1px 0 rgba(180,215,255,.25);
}

/* ============================================================
   MODULE 03 — Page shell (body now defers to .bg layer)
   ============================================================ */
html,body{height:100%}
body{
  margin:0;height:100vh;height:100dvh;overflow:hidden;
  -webkit-tap-highlight-color:transparent;-webkit-user-select:none;
  touch-action:none;overscroll-behavior:none;-webkit-text-size-adjust:100%;
  color:var(--tx);
  font-family:system-ui,-apple-system,"Segoe UI",Roboto,sans-serif;
  background:var(--bg-base);
  transition:background-color var(--theme-fade) var(--theme-ease),
             color var(--theme-fade) var(--theme-ease);
  user-select:none;
  /* GPU hint for the whole page background layer */
  transform:translateZ(0);
}

/* ============================================================
   MODULE 04 — Living background container (isolated layout)
   ============================================================ */
.bg{
  position:fixed;inset:0;z-index:-1;overflow:hidden;
  background:var(--bg-base);
  transition:background-color var(--theme-fade) var(--theme-ease);
  contain:strict;                 /* no layout/paint escapes */
  transform:translateZ(0);
}

/* ============================================================
   MODULE 05 — Blue blobs (day palette)
   ============================================================ */
.blob{
  position:absolute;border-radius:50%;filter:blur(64px);
  pointer-events:none;
  transition:background var(--theme-fade) var(--theme-ease);
  /* pre-promote to their own compositor layer */
  will-change:transform;
  backface-visibility:hidden;
  transform:translate3d(0,0,0);
}
.blob-a{
  width:78vmax;height:78vmax;top:-24vmax;left:-18vmax;
  background:radial-gradient(circle at 50% 50%,var(--blob-a),transparent 66%);
  animation:driftA 28s ease-in-out infinite alternate;
}
.blob-b{
  width:72vmax;height:72vmax;bottom:-26vmax;right:-20vmax;
  background:radial-gradient(circle at 50% 50%,var(--blob-b),transparent 66%);
  animation:driftB 37s ease-in-out infinite alternate;
}
.blob-c{
  width:58vmax;height:58vmax;top:14%;left:32%;
  background:radial-gradient(circle at 50% 50%,var(--blob-c),transparent 70%);
  animation:driftC 22s ease-in-out infinite alternate;
}
@keyframes driftA{
  0%{transform:translate3d(0,0,0) scale(1)}
  50%{transform:translate3d(16vw,9vh,0) scale(1.14)}
  100%{transform:translate3d(-7vw,21vh,0) scale(.94)}
}
@keyframes driftB{
  0%{transform:translate3d(0,0,0) scale(1.05)}
  50%{transform:translate3d(-19vw,-11vh,0) scale(.92)}
  100%{transform:translate3d(8vw,-22vh,0) scale(1.16)}
}
@keyframes driftC{
  0%{transform:translate3d(0,0,0) scale(.96) rotate(0deg)}
  50%{transform:translate3d(-14vw,15vh,0) scale(1.18) rotate(40deg)}
  100%{transform:translate3d(12vw,-9vh,0) scale(1.02) rotate(-30deg)}
}

/* ============================================================
   MODULE 06 — Night veil (slow crossfade)
   ============================================================ */
.veil{
  position:absolute;inset:0;
  background:radial-gradient(135% 105% at 50% 0%,
              rgba(9,18,44,.92),rgba(2,5,14,.975) 78%);
  opacity:0;
  transition:opacity var(--theme-fade) var(--theme-ease);
  pointer-events:none;
  will-change:opacity;
}
html[data-theme="dark"] .veil{opacity:1}

/* ============================================================
   MODULE 07 — Night-only glow blobs
   ============================================================ */
.night-only{
  opacity:0;
  transition:opacity var(--theme-fade) var(--theme-ease);
  mix-blend-mode:screen;
  will-change:opacity;
}
html[data-theme="dark"] .night-only{opacity:.95}
.blob-d{
  width:70vmax;height:70vmax;top:-16vmax;right:-14vmax;
  background:radial-gradient(circle at 50% 50%,rgba(58,120,240,.55),transparent 68%);
  animation:driftB 31s ease-in-out infinite alternate;
}
.blob-e{
  width:64vmax;height:64vmax;bottom:-20vmax;left:-16vmax;
  background:radial-gradient(circle at 50% 50%,rgba(24,66,185,.6),transparent 68%);
  animation:driftA 41s ease-in-out infinite alternate;
}

/* ============================================================
   MODULE 08 — Starfield (created once in JS)
   ============================================================ */
.stars{
  position:absolute;inset:0;opacity:0;
  transition:opacity var(--theme-fade) var(--theme-ease);
  pointer-events:none;
  will-change:opacity;
}
html[data-theme="dark"] .stars{opacity:1}
.star{
  position:absolute;border-radius:50%;background:#fff;
  box-shadow:0 0 6px rgba(190,220,255,.95),0 0 14px rgba(120,175,255,.55);
  animation:twinkle 3s ease-in-out infinite;
  will-change:opacity,transform;
}
@keyframes twinkle{
  0%,100%{opacity:.22;transform:scale(.75)}
  50%{opacity:1;transform:scale(1.2)}
}

/* ============================================================
   MODULE 09 — Film grain texture
   ============================================================ */
.grain{
  position:absolute;inset:-60%;
  background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='220' height='220'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.8' numOctaves='4' stitchTiles='stitch'/%3E%3CfeColorMatrix type='saturate' values='0'/%3E%3C/filter%3E%3Crect width='220' height='220' filter='url(%23n)'/%3E%3C/svg%3E");
  opacity:.22;mix-blend-mode:overlay;pointer-events:none;
  transition:opacity var(--theme-fade) var(--theme-ease),
             mix-blend-mode var(--theme-fade) var(--theme-ease);
}
html[data-theme="dark"] .grain{opacity:.30;mix-blend-mode:soft-light}

/* ============================================================
   MODULE 10 — Vignette
   ============================================================ */
.vignette{
  position:absolute;inset:0;
  background:radial-gradient(120% 92% at 50% 40%,transparent 44%,var(--vig) 100%);
  pointer-events:none;
  transition:background var(--theme-fade) var(--theme-ease);
}

/* ============================================================
   MODULE 11 — Toggle button shell
   ============================================================ */
.toggle{
  position:fixed;
  top:calc(14px + env(safe-area-inset-top,0px));
  right:calc(20px + env(safe-area-inset-right,0px));
  z-index:6;
  width:104px;height:52px;padding:0;
  border-radius:999px;
  border:1px solid var(--glass-brd);
  background:var(--toggle-bg);
  box-shadow:var(--toggle-shadow);
  backdrop-filter:blur(14px) saturate(165%);
  -webkit-backdrop-filter:blur(14px) saturate(165%);
  cursor:pointer;
  transition:background var(--theme-fade) var(--theme-ease),
             border-color var(--theme-fade) var(--theme-ease),
             box-shadow var(--theme-fade) var(--theme-ease),
             transform .35s var(--theme-ease);
  transform:translateZ(0);
  will-change:transform;
}
.toggle:hover{transform:translateY(-1px) translateZ(0)}
.toggle:active{transform:translateY(0) scale(.985) translateZ(0)}
.toggle:focus-visible{outline:2px solid var(--glow);outline-offset:4px}
.sky{position:absolute;inset:0;border-radius:inherit;overflow:hidden;z-index:1}

/* ============================================================
   MODULE 12 — Cloud (slow to-and-fro drift)
   ============================================================ */
.cloud{
  position:absolute;left:44px;top:26px;
  width:34px;height:11px;border-radius:999px;
  background:radial-gradient(ellipse at 40% 28%,
      #ffffff 0%,#f3f8ff 55%,#dbe8f8 100%);
  box-shadow:
    0 3px 10px rgba(110,165,255,.32),
    inset 0 -2px 3px rgba(190,215,255,.55),
    inset 0 2px 3px rgba(255,255,255,.95);
  transition:opacity 1.2s var(--theme-ease),
             scale 1.2s var(--theme-ease);
  animation:cloudFloat 10s ease-in-out infinite alternate;
  will-change:transform;
}
.cloud::before{
  content:"";position:absolute;width:16px;height:16px;border-radius:50%;
  left:3px;top:-8px;
  background:radial-gradient(circle at 35% 32%,
      #ffffff 0%,#f0f7ff 70%,#dbe8f8 100%);
  box-shadow:inset 0 -2px 3px rgba(190,215,255,.5);
}
.cloud::after{
  content:"";position:absolute;width:12px;height:12px;border-radius:50%;
  left:18px;top:-6px;
  background:radial-gradient(circle at 35% 32%,
      #ffffff 0%,#f0f7ff 70%,#dbe8f8 100%);
  box-shadow:inset 0 -2px 3px rgba(190,215,255,.5);
}
@keyframes cloudFloat{
  from{transform:translateX(-8px)}
  to{transform:translateX(8px)}
}
html[data-theme="dark"] .cloud{opacity:0;scale:.65}

/* ============================================================
   MODULE 13 — Mini stars inside the pill
   ============================================================ */
.mini-stars{
  position:absolute;inset:0;opacity:0;
  transition:opacity 1.1s var(--theme-ease) .25s;
  will-change:opacity;
}
html[data-theme="dark"] .mini-stars{opacity:1}
.mini-stars i{
  position:absolute;width:3px;height:3px;border-radius:50%;
  background:#fff;box-shadow:0 0 6px rgba(185,218,255,.95);
  animation:twinkle 2.4s ease-in-out infinite;
}
.mini-stars i:nth-child(1){left:18px;top:16px;animation-delay:0s}
.mini-stars i:nth-child(2){left:30px;top:29px;animation-delay:.7s}
.mini-stars i:nth-child(3){left:14px;top:33px;animation-delay:1.3s}
.mini-stars i:nth-child(4){left:34px;top:12px;animation-delay:1.9s}

/* ============================================================
   MODULE 14 — Orb slider + pulse feedback
   ============================================================ */
.orb{
  position:absolute;top:5px;left:6px;
  width:40px;height:40px;border-radius:50%;
  display:grid;place-items:center;z-index:2;
  transition:transform 1.4s cubic-bezier(.4,0,.2,1);
  will-change:transform;
}
html[data-theme="dark"] .orb{transform:translateX(52px)}
.toggle.pulse{animation:togglePulse 1.6s var(--theme-ease)}
@keyframes togglePulse{
  0%{box-shadow:var(--toggle-shadow),0 0 0 0 rgba(150,200,255,.55)}
  45%{box-shadow:var(--toggle-shadow),0 0 0 12px rgba(150,200,255,0)}
  100%{box-shadow:var(--toggle-shadow),0 0 0 0 rgba(150,200,255,0)}
}

/* ============================================================
   MODULE 15 — Realistic sun (glow moved to opacity layer for GPU)
   ============================================================ */
.sun{
  position:absolute;width:26px;height:26px;border-radius:50%;
  background:radial-gradient(circle at 38% 32%,
      #ffffff 0%,
      #fff7cf 14%,
      #ffe066 38%,
      #ffc23a 62%,
      #ffa321 82%,
      #ff8513 100%);
  box-shadow:
    inset -3px -3px 6px rgba(255,130,30,.55),
    inset  2px  2px 5px rgba(255,255,225,.95),
    0 0  10px rgba(255,215,120,.90),
    0 0  22px rgba(255,180, 70,.70),
    0 0  38px rgba(255,140, 40,.45),
    0 0  64px rgba(255,110, 40,.22);
  transition:opacity 1.1s var(--theme-ease),
             transform 1.4s cubic-bezier(.4,0,.2,1);
  will-change:opacity,transform;
}
/* pulsing glow is a separate opacity-only layer (cheap on GPU) */
.sun::after{
  content:"";position:absolute;inset:-30px;border-radius:50%;
  background:radial-gradient(circle,
      rgba(255,225,140,.55) 0%,
      rgba(255,180, 70,.28) 40%,
      rgba(255,120, 40,0)   72%);
  animation:sunPulse 3.8s ease-in-out infinite alternate;
  pointer-events:none;
  will-change:opacity,transform;
}
@keyframes sunPulse{
  from{opacity:.45;transform:scale(.9)}
  to  {opacity:1;  transform:scale(1.18)}
}
/* rotating rays — transform-only animation, GPU-accelerated */
.sun::before{
  content:"";position:absolute;inset:-7px;border-radius:50%;
  background:repeating-conic-gradient(
    from 0deg,
    rgba(255,222,135,.78) 0deg 4.5deg,
    transparent           4.5deg 20deg
  );
  -webkit-mask:radial-gradient(circle,
      transparent 46%,#000 56%,#000 72%,transparent 84%);
  mask:radial-gradient(circle,
      transparent 46%,#000 56%,#000 72%,transparent 84%);
  animation:sunRays 24s linear infinite;
  pointer-events:none;
  will-change:transform;
}
@keyframes sunRays{to{transform:rotate(360deg)}}
html[data-theme="dark"] .sun{opacity:0;transform:scale(.3) rotate(-120deg)}

/* ============================================================
   MODULE 16 — Moon
   ============================================================ */
.moon{
  position:absolute;width:26px;height:26px;border-radius:50%;
  box-shadow:inset -8px -6px 0 0 #e8f2ff;
  filter:drop-shadow(0 0 7px rgba(172,212,255,.9));
  opacity:0;transform:scale(.3) rotate(120deg);
  transition:opacity 1.1s var(--theme-ease) .15s,
             transform 1.4s cubic-bezier(.4,0,.2,1) .1s;
  will-change:opacity,transform;
}
html[data-theme="dark"] .moon{opacity:1;transform:scale(1) rotate(0deg)}

/* ============================================================
   MODULE 17 — Footstep shared components (glass, brand, heading)
   ============================================================ */
.glass{background:var(--g);border:1px solid var(--gb);backdrop-filter:blur(18px) saturate(150%);-webkit-backdrop-filter:blur(18px) saturate(150%);box-shadow:0 10px 34px var(--sh),inset 0 1px 0 rgba(255,255,255,.5),inset 1px 0 0 rgba(255,255,255,.45),inset -1px 0 0 rgba(255,255,255,.2)}
#brand{position:fixed;top:calc(18px + env(safe-area-inset-top,0px));left:calc(20px + env(safe-area-inset-left,0px));z-index:5;padding:10px 18px;border-radius:999px;font-weight:700;font-size:18px}
h1{position:fixed;z-index:4;top:24px;left:50%;transform:translateX(-50%);margin:0;font-size:clamp(15px,2vw,22px);font-weight:600;white-space:nowrap}
#mt{position:fixed;z-index:4;top:calc(56px + env(safe-area-inset-top,0px));left:50%;transform:translateX(-50%);width:94vw;text-align:center;pointer-events:none;font:800 clamp(24px,4.4vw,56px)/1.05 "Helvetica Neue","Segoe UI",Roboto,Arial,sans-serif;letter-spacing:.14em;text-transform:uppercase;color:var(--mtc);text-shadow:var(--mts);transition:color .8s,text-shadow .8s}
#mt .wd{display:inline-block;white-space:nowrap}
#mt .w{display:inline-block;overflow:hidden;vertical-align:bottom;padding:.12em .05em}
#mt .w i{display:inline-block;font-style:normal;animation:rise 1s cubic-bezier(.16,1,.3,1) backwards;animation-delay:calc(var(--i)*50ms)}
@keyframes rise{from{transform:translateY(105%)}}

/* ============================================================
   MODULE 18 — 3D stage & device primitives
   ============================================================ */
#stage{z-index:2;position:fixed;top:0;left:0;right:0;bottom:0;display:grid;place-items:center;-webkit-perspective:1700px;perspective:1700px;padding-right:min(340px,30vw);cursor:pointer;touch-action:none;contain:layout style}
#zone{grid-area:1/1;place-self:center;width:min(100%,940px);height:min(92%,660px);pointer-events:none}
#dev{position:relative;width:0;height:0;grid-area:1/1;place-self:center;will-change:transform}
#dev,#in,.unit,.part,.sp,.box,.wr,.foot{-webkit-transform-style:preserve-3d;transform-style:preserve-3d}
#in,.unit,.part,.sp,.box,.wr,.foot{position:absolute;left:0;top:0}
#in.sq{animation:sq .6s ease-out}
@keyframes sq{35%{transform:scale3d(1.02,.94,1.02)}70%{transform:scale3d(.995,1.01,.995)}}
.part{transform:translate3d(0,var(--a),0);transform-origin:0 var(--a) 0;transition:transform var(--split-time,1.5s) cubic-bezier(.22,1,.36,1),translate .35s ease,scale .55s cubic-bezier(.34,1.3,.64,1);transition-delay:calc(var(--k)*.08s),0s,0s}
.ex .part{transform:translate3d(var(--dx,0px),var(--e),0);transform-origin:var(--dx,0px) var(--e) 0}
.part.mg{scale:var(--mz,1.45)}
.sp{transform:translate3d(var(--x),0,var(--z));transition:transform var(--split-time,1.5s) cubic-bezier(.22,1,.36,1);transition-delay:calc(var(--k)*.08s)}
.ex .sp{transform:translate3d(calc(var(--x)*1.7),0,calc(var(--z)*1.7))}
.wr{transform-origin:0 0;transform:translate3d(var(--x),0,var(--z)) scaleY(var(--la));transition:transform var(--split-time,1.5s) cubic-bezier(.22,1,.36,1);transition-delay:calc((var(--k) + 1)*.08s)}
.ex .wr{transform:translate3d(var(--x),0,var(--z)) scaleY(var(--le))}
.f{position:absolute;left:0;top:0;-webkit-backface-visibility:hidden;backface-visibility:hidden;display:flex;align-items:center;justify-content:center;font:700 12px system-ui;color:#0b2a55;text-align:center;transition:opacity .4s,filter .3s}
.cap{border-radius:50%}
.f small{font-size:10px;color:#eaffe8;line-height:1.2}
.ex .part:hover .f{filter:brightness(1.25)}
.part.sel .f{filter:brightness(1.4);animation:selp .9s ease-out}
.has .part:not(.sel) .f{opacity:.3}
.foot{display:none}
.demo .foot{display:block;translate:0 -120px;animation:ft 2.4s cubic-bezier(.45,0,.3,1) infinite}
.demo .pr,.demo .pl{animation:pr 2.4s ease-in-out infinite}
.demo .pz{animation:pzs 2.4s ease-in-out infinite}
.demo .sp{animation:sc 2.4s ease-in-out infinite}
@keyframes ft{0%{translate:0 -120px;rotate:1 0 0 10deg}26%{translate:0 -14px;rotate:1 0 0 14deg}32%{translate:0 0;rotate:1 0 0 0deg}45%,55%{translate:0 12px;rotate:1 0 0 0deg}66%{translate:0 -10px;rotate:1 0 0 -12deg}100%{translate:0 -120px;rotate:1 0 0 8deg}}
@keyframes pr{0%,30%{translate:0 0}45%,55%{translate:0 12px}70%,100%{translate:0 0}}
@keyframes sc{0%,30%{scale:1 1}45%,55%{scale:1 .72}70%,100%{scale:1 1}}
@keyframes pzs{0%,30%{scale:1 1}45%,55%{scale:1 .5}70%,100%{scale:1 1}}
.s2 .pz .f,.s3 .b4 .f,.s4 .bc .f,.s5 .bat .f,.s6 .sol .f,.s7 .inv .f,.s3 .w1 .f,.s4 .w2 .f,.s5 .w3 .f,.s6 .swr .f,.s7 .w4 .f{animation:cg .5s ease-in-out infinite alternate}
@keyframes cg{to{filter:brightness(1.9) saturate(1.3)}}
.ww{opacity:0;top:-14px}
.s8 .ww{animation:wf 1.8s ease-out infinite}
.ww .f{background:transparent!important;border:2px solid #7fe3ff;box-shadow:0 0 10px #7fe3ff}
@keyframes wf{0%{transform:scale(.3);opacity:.9}100%{transform:scale(2.6);opacity:0}}
#in{animation:bob 7s ease-in-out infinite}
#in.sq{animation:bob 7s ease-in-out infinite,sq .9s cubic-bezier(.16,1,.3,1)}
@keyframes bob{50%{translate:0 -7px}}
.ex .part:hover{translate:0 -8px}

/* ============================================================
   MODULE 19 — Captions, hint, dock
   ============================================================ */
#cap{position:fixed;z-index:6;left:50%;bottom:172px;max-width:min(92vw,540px);padding:10px 18px;border-radius:18px;font-size:14px;font-weight:600;text-align:center;opacity:0;pointer-events:none;transform:translate(-50%,10px);transition:opacity .4s,transform .4s}
#cap.on{opacity:1;transform:translate(-50%,0)}
#dock{position:fixed;z-index:5;bottom:22px;left:0;right:0;padding-right:min(340px,30vw);display:flex;gap:14px;justify-content:center}
#hint{position:fixed;z-index:3;bottom:126px;left:0;right:0;padding-right:min(340px,30vw);text-align:center;font:italic 500 16px Georgia,"Palatino Linotype","Times New Roman",serif;letter-spacing:.4px;text-shadow:0 1px 10px rgba(0,30,90,.35);opacity:.95;pointer-events:none}
#dk{display:flex;flex-wrap:wrap;justify-content:center;gap:30px;padding:14px 26px;border-radius:30px;border:2px solid transparent;background:linear-gradient(160deg,var(--g),rgba(80,160,255,.2)) padding-box,linear-gradient(135deg,rgba(215,247,255,.95),rgba(70,160,255,.55) 50%,rgba(215,247,255,.9)) border-box;-webkit-backdrop-filter:blur(18px) saturate(150%);backdrop-filter:blur(18px) saturate(150%);box-shadow:0 12px 34px var(--sh),inset 0 1px 0 rgba(255,255,255,.5);animation:dk .9s .3s cubic-bezier(.22,1,.36,1) backwards}
@keyframes dk{from{opacity:0;transform:translateY(24px) scale(.95)}}

/* ============================================================
   MODULE 20 — Buttons & ripples
   ============================================================ */
.key{position:relative;font:500 15px system-ui;color:var(--tx);padding:11px 22px;border-radius:14px;border:1px solid rgba(200,238,255,.65);cursor:pointer;background:linear-gradient(160deg,var(--t1,rgba(150,215,255,.4)),var(--t2,rgba(50,120,235,.26)));-webkit-backdrop-filter:blur(12px);backdrop-filter:blur(12px);box-shadow:inset 0 1px 0 rgba(255,255,255,.4);transition:transform .28s cubic-bezier(.34,1.56,.64,1),filter .2s,box-shadow .25s}
.key::before{content:none}
.key:hover{filter:brightness(1.15)}
.key:active,.key.mag{transform:scale(1.08);filter:brightness(1.08)}
.key.glow{animation:glow .7s ease-out}
@keyframes glow{0%{box-shadow:0 0 14px 2px rgba(140,225,255,.7)}100%{box-shadow:inset 0 1px 0 rgba(255,255,255,.4)}}
.rip{position:fixed;width:36px;height:36px;margin:-18px;border-radius:50%;pointer-events:none;z-index:99;background:radial-gradient(circle,rgba(200,242,255,.6),rgba(120,200,255,.25) 45%,transparent 70%);animation:rip .95s cubic-bezier(.16,1,.3,1) forwards;will-change:transform,opacity}
.rip::after{content:"";position:absolute;top:0;left:0;right:0;bottom:0;border-radius:50%;border:1.5px solid rgba(255,255,255,.7);animation:rip2 .95s .06s cubic-bezier(.16,1,.3,1) both}
@keyframes rip{0%{transform:scale(.2);opacity:.9}100%{transform:scale(3.4);opacity:0}}
@keyframes rip2{0%{transform:scale(.6);opacity:.9}100%{transform:scale(1.7);opacity:0}}

/* ============================================================
   MODULE 21 — Info popup panel
   ============================================================ */
#pop{position:fixed;z-index:6;right:24px;top:50%;width:310px;padding:22px;border-radius:26px;opacity:0;pointer-events:none;transform-origin:right center;filter:blur(8px);transform:perspective(1000px) translateY(-50%) translateX(44px) rotateY(-14deg) scale(.96);transition:opacity .7s cubic-bezier(.16,1,.3,1),transform .85s cubic-bezier(.16,1,.3,1),filter .7s ease;overflow:hidden}
#pop.show{opacity:1;pointer-events:auto;filter:none;transform:perspective(1000px) translateY(-50%)}
#pop::before{content:"";position:absolute;top:0;left:-60%;width:40%;height:100%;background:linear-gradient(100deg,transparent,rgba(255,255,255,.5),transparent);transform:skewX(-20deg);opacity:0;pointer-events:none}
#pop.pp{animation:glowin 1.6s ease-out}
#pop.pp::before{animation:sweep 1.5s .3s ease-in-out}
#pop.pp>:not(.key){animation:up .75s cubic-bezier(.16,1,.3,1) backwards}
#pop.pp>:nth-child(2){animation-delay:.1s}#pop.pp>:nth-child(3){animation-delay:.18s}#pop.pp>:nth-child(4){animation-delay:.26s}#pop.pp>:nth-child(5){animation-delay:.34s}#pop.pp>:nth-child(6){animation-delay:.42s}
#pop::after{content:"";position:absolute;left:22px;right:22px;top:0;height:2px;background:linear-gradient(90deg,transparent,rgba(150,225,255,.95),transparent);transform:scaleX(0);transition:transform 1s .25s cubic-bezier(.16,1,.3,1)}
#pop.show::after{transform:scaleX(1)}
#pop.pp #ps span{animation:up .7s cubic-bezier(.16,1,.3,1) backwards;animation-delay:.5s}
#pop.pp #ps span:nth-child(2){animation-delay:.58s}
#pop.pp #ps span:nth-child(3){animation-delay:.66s}
@keyframes glowin{0%{box-shadow:0 10px 34px var(--sh),0 0 0 0 rgba(150,225,255,0)}40%{box-shadow:0 10px 34px var(--sh),0 0 42px 2px rgba(150,225,255,.45)}100%{box-shadow:0 10px 34px var(--sh),0 0 42px 2px rgba(150,225,255,0)}}
@keyframes sweep{0%{left:-60%;opacity:.5}100%{left:130%;opacity:.5}}
@keyframes up{from{opacity:0;transform:translateY(10px);filter:blur(4px)}}
#pop small{font-size:12px;opacity:.75;letter-spacing:.5px;text-transform:uppercase}
#pop h3{margin:4px 0 10px;font-size:20px;padding-right:34px}
#pop p{margin:0 0 12px;font-size:14px;line-height:1.55}
#ps span{display:inline-block;margin:0 6px 6px 0;padding:5px 11px;border-radius:99px;font-size:12px;border:1px solid var(--gb);background:rgba(255,255,255,.15)}
#pb{display:none;height:4px;border-radius:9px;background:rgba(255,255,255,.3);margin-top:8px;overflow:hidden}
.tour #pb{display:block}
#pb i{display:block;height:100%;background:linear-gradient(90deg,#7fe3ff,#4b8dff)}
@keyframes pb{from{width:0}to{width:100%}}
#x{position:absolute;top:12px;right:12px;padding:2px 11px;border-radius:12px;font-size:18px}

/* ============================================================
   MODULE 22 — Realistic view (canvas overlay + HUD)
   ============================================================ */
#rv{position:fixed;top:0;left:0;right:0;bottom:0;z-index:30;background:#0b1f4d;visibility:hidden;opacity:0;clip-path:circle(0% at 50% 100%);transition:clip-path 1s cubic-bezier(.16,1,.3,1),opacity .5s,visibility 0s 1s}
#rv.on{visibility:visible;opacity:1;clip-path:circle(150% at 50% 100%);transition:clip-path 1.1s cubic-bezier(.16,1,.3,1),opacity .4s,visibility 0s}
#cv{position:absolute;top:0;left:0;width:100%;height:100%}
#rt,#rs{position:absolute;left:50%;transform:translateX(-50%);color:#eaf5ff;background:rgba(10,25,60,.5)}
#rt{top:calc(18px + env(safe-area-inset-top,0px));padding:10px 20px;border-radius:999px;font-weight:600;white-space:nowrap;max-width:64vw;overflow:hidden;text-overflow:ellipsis}
#rb{position:absolute;top:calc(14px + env(safe-area-inset-top,0px));right:calc(20px + env(safe-area-inset-right,0px));color:#eaf5ff}
#rs{bottom:calc(24px + env(safe-area-inset-bottom,0px));display:flex;gap:26px;align-items:center;padding:12px 24px;border-radius:22px;font-size:15px;white-space:nowrap}
#rs b{font-size:20px;margin-left:6px;font-variant-numeric:tabular-nums}
#n3{display:inline-block;width:90px;height:8px;border-radius:9px;background:rgba(255,255,255,.25);margin-left:8px;overflow:hidden;vertical-align:middle}
#n3 u{display:block;height:100%;width:0;background:linear-gradient(90deg,#ffd76a,#fff3b0);text-decoration:none}

/* ============================================================
   MODULE 23 — Tooltip + preset + vignette overlay for popup
   ============================================================ */
#tip{position:fixed;left:0;top:0;z-index:50;padding:5px 12px;border-radius:99px;font-size:12px;font-weight:600;opacity:0;pointer-events:none;transition:opacity .2s;will-change:transform}
#tip.on{opacity:1}
body::after{content:"";position:fixed;top:0;left:0;right:0;bottom:0;z-index:2;pointer-events:none;background:radial-gradient(circle at 35% 50%,transparent 38%,rgba(0,25,70,.4));opacity:0;transition:opacity .6s;will-change:opacity}
body.pv::after{opacity:1}
@keyframes blurin{from{filter:blur(10px)}}
@keyframes selp{0%{filter:brightness(2.3)}100%{filter:brightness(1.4)}}
@supports not ((backdrop-filter:blur(1px)) or (-webkit-backdrop-filter:blur(1px))){.glass,.key{background:rgba(40,110,200,.6)}}

/* ============================================================
   MODULE 24 — Responsive & accessibility
   ============================================================ */
@media (pointer:coarse){.f{box-shadow:none}.glass,.key,#dk{-webkit-backdrop-filter:blur(8px);backdrop-filter:blur(8px)}.key{min-height:46px}}
@media (max-width:700px){
  h1{display:none}
  #stage{padding:110px 0 320px}
  #dock,#hint{padding-right:0}
  #dock{flex-wrap:wrap;gap:10px}
  .key{padding:10px 14px;font-size:14px}
  #dock .key{min-width:0}
  #dk{gap:14px;padding:8px 12px;max-width:96vw}
  #hint{bottom:156px}
  #rs{gap:14px;padding:10px 16px;font-size:13px;flex-wrap:wrap;justify-content:center;left:3vw;right:3vw;transform:none}
  #rt{max-width:56vw;font-size:13px}
  #pop{left:12px;right:12px;top:auto;bottom:176px;width:auto;transform:translateY(30px) scale(.95)}
  #pop.show{transform:none}
  #mt{top:calc(64px + env(safe-area-inset-top,0px))}
  #n3{width:60px}
}
@media (prefers-reduced-motion:reduce){
  .blob,.star,.cloud,.mini-stars i,.sun,.sun::before,.sun::after{animation:none!important}
  .orb,.sun,.moon,.toggle,body,.bg,.veil,.stars,.grain,.vignette,.blob{transition-duration:.25s!important}
  .toggle.pulse{animation:none!important}
}

/* ===== WebGL layer overrides ===== */
#gl{position:fixed;inset:0;width:100%;height:100%;z-index:1;display:block;touch-action:none;cursor:pointer}
.blob{animation:none!important;will-change:auto}            /* static background = more GPU time for 3D = higher FPS */
#cv{display:none}
#rv,#rv.on{background:transparent;clip-path:none;pointer-events:none}
#rb{pointer-events:auto}
.walk #dock,.walk #brand,.walk h1,.walk #mt,.walk #hint,.walk #cap,.walk #toggle{opacity:0;pointer-events:none;transition:opacity .4s}
#brand,h1,#mt,#dock,#toggle{transition:opacity .4s}

/* ============================================================
   NEUMORPHISM + TINTED GLASS  (soft raised / pressed panels with blue-tinted frosted glass)
   Edit the --nm-* variables to change the look.
   ============================================================ */
:root{--nm-tint:rgba(120,180,255,.30);--nm-bg:linear-gradient(145deg,rgba(238,248,255,.60),rgba(150,200,250,.30));--nm-bd:rgba(255,255,255,.65);
 --nm-out:9px 9px 22px rgba(52,104,190,.34),-9px -9px 22px rgba(255,255,255,.85),inset 1px 1px 1px rgba(255,255,255,.85),inset -1px -1px 2px rgba(70,120,205,.18);
 --nm-in:inset 6px 6px 14px rgba(52,104,190,.30),inset -6px -6px 14px rgba(255,255,255,.8);
 --nm-sm:5px 5px 12px rgba(52,104,190,.30),-5px -5px 12px rgba(255,255,255,.8),inset 1px 1px 1px rgba(255,255,255,.8)}
:root[data-theme="dark"]{--nm-tint:rgba(70,130,235,.28);--nm-bg:linear-gradient(145deg,rgba(72,112,188,.40),rgba(14,34,80,.58));--nm-bd:rgba(150,200,255,.22);
 --nm-out:9px 9px 22px rgba(0,5,25,.6),-7px -7px 18px rgba(110,170,255,.14),inset 1px 1px 1px rgba(170,215,255,.28),inset -1px -1px 2px rgba(0,0,0,.35);
 --nm-in:inset 6px 6px 14px rgba(0,5,25,.6),inset -5px -5px 12px rgba(110,170,255,.14);
 --nm-sm:5px 5px 12px rgba(0,5,25,.55),-4px -4px 10px rgba(110,170,255,.13),inset 1px 1px 1px rgba(170,215,255,.25)}
.glass,#brand,#cap,#pop,#rt,#rs,#tip,#dk{background:var(--nm-bg)!important;border:1px solid var(--nm-bd)!important;box-shadow:var(--nm-out)!important;backdrop-filter:blur(22px) saturate(150%);-webkit-backdrop-filter:blur(22px) saturate(150%)}
.key{background:linear-gradient(145deg,rgba(255,255,255,.42),var(--nm-tint))!important;border:1px solid var(--nm-bd)!important;box-shadow:var(--nm-sm)!important;transition:box-shadow .25s,transform .25s,filter .25s}
.key:hover{filter:brightness(1.08)}
.key:active,.key.mag{box-shadow:var(--nm-in)!important;transform:scale(.98);filter:none}
#ps span{background:transparent!important;border:0!important;box-shadow:var(--nm-in)}
#rt,#rs{color:var(--tx)}


/* ===== REALISTIC VIEW — CSS 3D scene (no WebGL). Edit colours here. ===== */
:root{--nd:0;--grass:#4f9a3f;--grass2:#428a35;--pave:#bdb8ae;--asph:#3a3d42;--sky1:#3f8fe8;--sky2:#9fd0ff;--sky3:#e8f4ff;--hz:226,240,255}
:root[data-theme="dark"]{--nd:.5;--grass:#21402a;--grass2:#1a3322;--pave:#55555d;--asph:#17191d;--sky1:#030818;--sky2:#101c42;--sky3:#1c2c58;--hz:10,18,48}
#cw{position:fixed;inset:0;z-index:29;overflow:hidden;perspective:2000px;perspective-origin:50% 34%;visibility:hidden;opacity:0;transition:opacity .6s,visibility 0s .6s;pointer-events:none}
#cw.on{visibility:visible;opacity:1;transition:opacity .6s}
#sky{position:absolute;inset:0;background:linear-gradient(var(--sky1),var(--sky2) 52%,var(--sky3))}
#sky::before{content:'';position:absolute;right:14%;top:6%;width:150px;height:150px;border-radius:50%;background:radial-gradient(circle,rgba(255,252,225,.95) 0 13%,rgba(255,240,180,.4) 30%,transparent 62%)}
:root[data-theme="dark"] #sky::before{width:90px;height:90px;background:radial-gradient(circle,#f4f1e0 0 8%,rgba(200,215,255,.3) 26%,transparent 60%)}
.cl{position:absolute;height:48px;width:230px;border-radius:50px;background:rgba(255,255,255,.88);filter:blur(7px);animation:drift 170s linear infinite}
.cl:nth-child(1){top:8%;animation-delay:-20s}.cl:nth-child(2){top:16%;width:300px;animation-delay:-90s}.cl:nth-child(3){top:5%;width:180px;animation-delay:-140s}
:root[data-theme="dark"] .cl{opacity:calc(.1 - var(--ri)*.05)}
@keyframes drift{from{transform:translateX(-320px)}to{transform:translateX(calc(100vw + 320px))}}
#world{position:absolute;left:50%;top:58%;width:0;height:0;transform-style:preserve-3d;will-change:transform}
#haze{position:absolute;inset:0;pointer-events:none;background:linear-gradient(rgba(var(--hz),.75),rgba(var(--hz),0) 36%)}
#world *{position:absolute;box-sizing:border-box}
#world,.bx,.ent{transform-style:preserve-3d}
.grass{background:radial-gradient(rgba(255,255,255,.07) 1px,transparent 2px) 0 0/9px 7px,repeating-linear-gradient(95deg,var(--grass) 0 14px,var(--grass2) 14px 28px)}
.path{background:linear-gradient(90deg,rgba(60,55,50,.45) 2px,transparent 2px) 0 0/120px 100%,linear-gradient(rgba(60,55,50,.35) 2px,transparent 2px) 0 0/100% 120px,radial-gradient(rgba(255,255,255,.1) 1px,transparent 2px) 0 0/7px 7px,var(--pave)}
.drain{background:linear-gradient(#0b1722,#2a6489 55%,#0b1722)}
.grate{background:repeating-linear-gradient(90deg,#8c969f 0 5px,transparent 5px 12px),linear-gradient(transparent 12%,#8c969f 12% 24%,transparent 24% 76%,#8c969f 76% 88%,transparent 88%)}
.road{background:radial-gradient(rgba(255,255,255,.08) 1px,transparent 2px) 0 0/6px 6px,radial-gradient(rgba(0,0,0,.3) 1px,transparent 2px) 3px 3px/9px 9px,var(--asph)}
.dash{background:repeating-linear-gradient(90deg,#f4f4f0 0 240px,transparent 240px 480px)}
.solid,.zeb{background:#f4f4f0}
.mh{border-radius:50%;background:radial-gradient(circle,#555 0 38%,#2d2d2d 40%);border:3px solid #7a7a7a}
.bsq{background:linear-gradient(145deg,#dfe5ec,#8f99a5);border-radius:3px;box-shadow:inset 0 0 0 2px #4a525c,0 2px 3px rgba(0,0,0,.35)}
.tq{transition:scale .22s cubic-bezier(.22,1,.36,1);will-change:scale}.tq.pr{scale:.965;transition-duration:.1s}
.tq::after{content:'';inset:0;border-radius:3px;background:radial-gradient(circle,rgba(70,255,150,.55),rgba(70,255,150,0) 70%);opacity:0;transition:opacity .35s ease-out;pointer-events:none;transform:translateZ(0)}.tq.pr::after{opacity:1;transition-duration:.08s}
.tri{inset:0}
.tri.a{clip-path:polygon(1% 1%,95% 1%,1% 95%);background:radial-gradient(circle at 9% 9%,#e8edf3 0 3px,#59626d 3.5px 5px,transparent 5.5px),radial-gradient(circle at 86% 9%,#e8edf3 0 3px,#59626d 3.5px 5px,transparent 5.5px),radial-gradient(circle at 9% 86%,#e8edf3 0 3px,#59626d 3.5px 5px,transparent 5.5px),radial-gradient(circle at 33% 33%,#35ff82 0 1.6px,transparent 2.6px),repeating-linear-gradient(90deg,rgba(255,255,255,.6) 0 1px,transparent 1px 12px),repeating-linear-gradient(0deg,rgba(255,255,255,.6) 0 1px,transparent 1px 12px),linear-gradient(135deg,#2f6fe0,#0a2f86)}
.tri.c{clip-path:polygon(99% 99%,99% 5%,5% 99%);background:radial-gradient(circle at 91% 91%,#e8edf3 0 3px,#59626d 3.5px 5px,transparent 5.5px),radial-gradient(circle at 91% 14%,#e8edf3 0 3px,#59626d 3.5px 5px,transparent 5.5px),radial-gradient(circle at 14% 91%,#e8edf3 0 3px,#59626d 3.5px 5px,transparent 5.5px),radial-gradient(circle at 67% 67%,#35ff82 0 1.6px,transparent 2.6px),repeating-linear-gradient(90deg,rgba(255,255,255,.6) 0 1px,transparent 1px 12px),repeating-linear-gradient(0deg,rgba(255,255,255,.6) 0 1px,transparent 1px 12px),linear-gradient(135deg,#1d5fd0,#0a2f86)}
.f{background:var(--c,#999);outline:1px solid transparent;backface-visibility:hidden}
.fl,.pf{outline:1px solid transparent}
#world .lb,#world .ps{backface-visibility:hidden}
#cw{-webkit-font-smoothing:antialiased}
.f.t{background:linear-gradient(rgba(255,255,255,.1),rgba(255,255,255,.1)),linear-gradient(rgba(5,10,35,var(--nd)),rgba(5,10,35,var(--nd))),var(--c)}
.f.s{background:linear-gradient(rgba(5,10,35,calc(var(--nd) + .05)),rgba(5,10,35,calc(var(--nd) + .05))),var(--c)}
.f.n{background:linear-gradient(rgba(5,10,35,calc(var(--nd) + .15)),rgba(5,10,35,calc(var(--nd) + .15))),var(--c)}
.f.w,.f.e{background:linear-gradient(rgba(5,10,35,calc(var(--nd) + .28)),rgba(5,10,35,calc(var(--nd) + .28))),var(--c)}
.wg{inset:5% 4% 12% 4%;display:grid;gap:10px 8px}
#world .wn{position:static;background:linear-gradient(160deg,#a9cdef,#4f7ba8);border-radius:2px;box-shadow:inset 0 0 0 2px #ece8e0,inset 0 8px 10px rgba(255,255,255,.25)}
:root[data-theme="dark"] #world .wn{background:linear-gradient(#0f1a2a,#1a2b40)}
:root[data-theme="dark"] #world .wn.l{background:#ffd88a;box-shadow:0 0 14px rgba(255,216,138,.85)}
.door{background:linear-gradient(#22343f,#101c24);border:3px solid #aeb6c0;border-radius:3px 3px 0 0}
#world .hedge .f{background:radial-gradient(circle at 30px 20px,#f9d71c 0 2px,transparent 3px) 0 0/90px 60px,radial-gradient(circle at 60px 36px,#ff6f91 0 2px,transparent 3px) 0 0/110px 60px,radial-gradient(circle at 12px 10px,#5aa84a 0 7px,transparent 8px) 0 0/28px 22px,radial-gradient(circle at 22px 18px,#2a6f31 0 8px,transparent 9px) 0 0/28px 22px,#357f38}
.tree .tr{left:46%;bottom:0;width:8%;height:44%;background:linear-gradient(90deg,#4e3520,#7a5532,#4e3520)}
.tree .cn{inset:0 0 26% 0;background:radial-gradient(circle at 50% 38%,#4aa24a 0 34%,transparent 35%),radial-gradient(circle at 28% 60%,#3d8f3f 0 27%,transparent 28%),radial-gradient(circle at 72% 60%,#3d8f3f 0 27%,transparent 28%),radial-gradient(circle at 50% 22%,#68bd5c 0 22%,transparent 23%);filter:drop-shadow(0 6px 5px rgba(0,0,0,.28))}
:root[data-theme="dark"] .tree{filter:brightness(.4)}
.tsh,.psh,.csh{background:radial-gradient(ellipse,rgba(0,0,0,.45),transparent 70%)}
.lampb .lp{left:calc(50% - 3px);bottom:0;width:6px;height:100%;background:linear-gradient(90deg,#222,#778,#222)}
.lampb .la{right:calc(50% - 3px);top:2px;width:70px;height:5px;background:#333}
.lampb .lh{right:calc(50% + 62px);top:2px;width:32px;height:9px;background:#fff6d0;border-radius:3px 3px 9px 9px;opacity:calc(.4 + var(--lv,0)*.6);box-shadow:0 0 calc(var(--lv,0)*26px) calc(var(--lv,0)*10px) rgba(255,224,150,.85)}
.pool{background:radial-gradient(ellipse,rgba(255,226,150,.6),transparent 68%);opacity:0}
.cab .s,.cab .n{background:linear-gradient(#233548,#0e1822)}.cab .w,.cab .e{background:#101a24}
.wh{border-radius:50%;background:radial-gradient(circle,#c9d0d8 0 22%,#4a4a4a 24% 40%,#101010 42%)}
.hl{background:#fff4c4;box-shadow:0 0 6px #fff}:root[data-theme="dark"] .hl{box-shadow:0 0 18px 6px rgba(255,240,180,.9)}
.tl{background:#d22;box-shadow:0 0 5px #f33}
.lb{transform-origin:50% 0}

/* ===== RAIN + NATURAL TOUCHES ===== */
#cw{--ri:0;--wl:0;--wt:0;--fl:0;--sd:1}
:root[data-theme="dark"] #cw{--sd:0}
#storm{position:absolute;inset:0;pointer-events:none;background:linear-gradient(rgba(58,70,86,.72),rgba(105,120,135,.3));opacity:var(--ri)}
#rainc{position:absolute;inset:0;width:100%;height:100%;pointer-events:none}
#sky::before{opacity:calc(1 - var(--ri)*.92)}
.cl{filter:blur(7px);will-change:transform;opacity:calc(1 - var(--ri)*.55)}
.ent{will-change:transform}
.wet{pointer-events:none;background:linear-gradient(115deg,rgba(255,255,255,0) 20%,rgba(200,225,255,.24) 40%,rgba(255,255,255,0) 60%) 0 0/640px 100%,rgba(16,32,48,.45);opacity:var(--wt)}
.dwater{background:linear-gradient(#173e5a,#3f86b5 50%,#173e5a);opacity:calc(.3 + var(--fl)*.7)}
.dflow{background:repeating-linear-gradient(90deg,rgba(210,235,255,.9) 0 22px,transparent 22px 70px);opacity:var(--fl);animation:dfl .7s linear infinite}
@keyframes dfl{to{background-position-x:70px}}
.rvl{background:repeating-linear-gradient(180deg,rgba(205,232,255,.9) 0 18px,transparent 18px 52px);background-size:100% 52px;opacity:calc(var(--wl)*1.15 + var(--ri)*.12);animation:rvl 1s linear infinite}
@keyframes rvl{to{background-position-y:52px}}
.pud{border-radius:50%;background:radial-gradient(ellipse at 40% 35%,rgba(238,247,255,.8),rgba(125,165,200,.72) 55%,rgba(70,105,140,.85));box-shadow:0 0 14px rgba(90,130,170,.55);opacity:clamp(0,calc((var(--wl) - var(--th,.3))*3),.92);scale:clamp(.2,calc(var(--wl) + .25),1)}
.rp{border:2px solid rgba(255,255,255,.8);border-radius:50%;opacity:0;animation:rpl 1.2s ease-out infinite}
@keyframes rpl{0%{transform:translateZ(3px) scale(.15);opacity:clamp(0,calc((var(--ri) - var(--rk,0))*3),.85)}100%{transform:translateZ(3px) scale(1.6);opacity:0}}
.bsh{pointer-events:none;background:linear-gradient(rgba(10,20,32,.36),rgba(10,20,32,.08));opacity:calc((1 - var(--ri))*var(--sd))}
.umb{left:14px;top:-12px;width:100px;height:36px;border-radius:50px 50px 4px 4px/36px 36px 4px 4px;box-shadow:inset 0 -7px 9px rgba(0,0,0,.28);opacity:clamp(0,calc((var(--ri) - .2)*4),1)}
.uh{left:63px;top:24px;width:2px;height:66px;background:#333;opacity:clamp(0,calc((var(--ri) - .2)*4),1)}
#cw.rn .hl{box-shadow:0 0 16px 5px rgba(255,240,180,.85)}
.tree .cn{transform-origin:50% 100%;animation:sway 5.5s ease-in-out infinite alternate}
@keyframes sway{from{transform:rotate(-1.1deg)}to{transform:rotate(calc(1.1deg + var(--ri)*1.8deg))}}
#rainb{position:absolute;top:calc(14px + env(safe-area-inset-top,0px));right:calc(150px + env(safe-area-inset-right,0px));pointer-events:auto}
#n5{display:inline-block;width:90px;height:8px;border-radius:9px;background:rgba(255,255,255,.3);margin-left:8px;overflow:hidden;vertical-align:middle}
#n5 u{display:block;height:100%;width:0;background:linear-gradient(90deg,#4aa3ff,#9ad4ff);text-decoration:none}

/* ===== REALISTIC+ : richer light, depth, materials (v9) ===== */
/* fix: green press-glow pseudo needs real positioning */
.tq::after{position:absolute}
/* sky + sun + layered clouds */
#sky{background:radial-gradient(ellipse 60% 40% at 82% 14%,rgba(255,244,205,.55),transparent 70%),linear-gradient(var(--sky1),var(--sky2) 48%,var(--sky3) 82%,#f4f1e6)}
:root[data-theme="dark"] #sky{background:radial-gradient(ellipse 50% 30% at 82% 12%,rgba(150,170,255,.18),transparent 70%),linear-gradient(var(--sky1),var(--sky2) 55%,var(--sky3))}
.cl{background:rgba(255,255,255,.9);box-shadow:80px -16px 0 -4px rgba(255,255,255,.88),-64px 10px 0 -8px rgba(255,255,255,.8),140px 12px 0 -12px rgba(255,255,255,.75),inset 0 -14px 16px rgba(150,175,210,.35)}
#haze{background:linear-gradient(rgba(var(--hz),.85),rgba(var(--hz),.35) 22%,rgba(var(--hz),0) 44%)}
/* grade: warm key light + soft vignette */
#cw::after{content:'';position:absolute;inset:0;pointer-events:none;background:radial-gradient(ellipse at 50% 55%,transparent 55%,rgba(8,16,36,.32)),linear-gradient(200deg,rgba(255,214,150,calc(.1*var(--sd))),transparent 55%)}
/* ground materials */
.grass{background:radial-gradient(ellipse at 30% 40%,rgba(255,255,255,.08),transparent 40%) 0 0/340px 260px,radial-gradient(ellipse at 70% 70%,rgba(0,40,0,.18),transparent 45%) 0 0/410px 300px,radial-gradient(rgba(255,255,255,.09) 1px,transparent 2px) 0 0/9px 7px,radial-gradient(rgba(0,0,0,.12) 1px,transparent 2px) 4px 3px/11px 9px,repeating-linear-gradient(95deg,var(--grass) 0 22px,var(--grass2) 22px 44px)}
.path{background:radial-gradient(ellipse at 20% 30%,rgba(255,255,255,.14),transparent 45%) 0 0/520px 300px,radial-gradient(ellipse at 75% 65%,rgba(60,50,40,.14),transparent 50%) 0 0/430px 280px,linear-gradient(90deg,rgba(60,55,50,.5) 2px,rgba(255,255,255,.22) 2px 3px,transparent 3px) 0 0/120px 100%,linear-gradient(rgba(60,55,50,.4) 2px,rgba(255,255,255,.2) 2px 3px,transparent 3px) 0 0/100% 120px,radial-gradient(rgba(255,255,255,.12) 1px,transparent 2px) 0 0/7px 7px,radial-gradient(rgba(0,0,0,.1) 1px,transparent 2px) 3px 4px/9px 9px,var(--pave)}
.road{background:linear-gradient(transparent 16%,rgba(0,0,0,.2) 19% 22%,transparent 25% 29%,rgba(0,0,0,.2) 32% 35%,transparent 38% 62%,rgba(0,0,0,.18) 66% 69%,transparent 72% 76%,rgba(0,0,0,.18) 79% 82%,transparent 85%),radial-gradient(ellipse at 40% 50%,rgba(255,255,255,.06),transparent 50%) 0 0/600px 400px,radial-gradient(rgba(255,255,255,.1) 1px,transparent 2px) 0 0/6px 6px,radial-gradient(rgba(0,0,0,.35) 1px,transparent 2px) 3px 3px/9px 9px,var(--asph)}
.dash,.solid,.zeb{opacity:.88}
.mh{box-shadow:inset 0 0 6px rgba(0,0,0,.7),0 1px 0 rgba(255,255,255,.2);background:repeating-radial-gradient(circle,#4a4a4a 0 3px,#2d2d2d 3px 6px)}
/* buildings: brick courses, ambient occlusion, glassy windows */
.f.s::before,.f.n::before{content:'';position:absolute;inset:0;pointer-events:none;background:linear-gradient(transparent 60%,rgba(0,0,0,.22)),linear-gradient(rgba(255,255,255,.18),transparent 12%),repeating-linear-gradient(rgba(0,0,0,.055) 0 1px,transparent 1px 10px)}
#world .wn{background:linear-gradient(135deg,rgba(255,255,255,.5) 0 18%,transparent 34%),linear-gradient(170deg,#b7d6f2,#4a78a6 60%,#33597f);box-shadow:inset 0 0 0 2px #efebe3,inset 0 -3px 0 2px #c9c3b8,inset 3px 6px 9px rgba(0,0,0,.28),0 3px 3px rgba(0,0,0,.25)}
:root[data-theme="dark"] #world .wn{background:linear-gradient(135deg,rgba(150,180,255,.18),transparent 40%),linear-gradient(#0f1a2a,#1a2b40)}
:root[data-theme="dark"] #world .wn.l{background:radial-gradient(circle at 50% 70%,#ffe9b8,#ffc860);box-shadow:inset 0 0 0 2px #3a3328,0 0 18px rgba(255,200,110,.85)}
.door{box-shadow:inset 0 0 12px rgba(0,0,0,.6),inset 0 12px 0 rgba(255,255,255,.08)}
/* paint gloss on cars / roofs */
.ent .f.t::before{content:'';position:absolute;inset:0;background:linear-gradient(120deg,rgba(255,255,255,.5),rgba(255,255,255,.06) 45%,rgba(0,0,0,.16))}
.ent .f.s::before,.ent .f.n::before{background:linear-gradient(rgba(255,255,255,.28),transparent 30%,rgba(0,0,0,.3))}
.cab .s,.cab .n{background:linear-gradient(135deg,rgba(255,255,255,.3),transparent 30%),linear-gradient(#34506b,#0e1822)}
.wh{box-shadow:0 0 0 2px #0a0a0a}
.csh,.psh,.tsh{opacity:calc(.3 + var(--sd)*.7)}
/* trees: leaf light + inner shadow */
.tree .cn::after{content:'';position:absolute;inset:6% 4% 0;border-radius:50%;background:radial-gradient(circle at 34% 24%,rgba(255,255,190,.32),transparent 42%),radial-gradient(circle at 62% 88%,rgba(0,35,0,.4),transparent 55%)}
.tree .tr{box-shadow:inset -3px 0 4px rgba(0,0,0,.4)}
/* people: rounded shading on every body part */
#world .ps div:not(.umb):not(.uh){box-shadow:inset -4px -3px 6px rgba(0,0,0,.24),inset 3px 2px 5px rgba(255,255,255,.14)}
/* tiles + solar glass */
.tri::after{content:'';position:absolute;inset:0;background:linear-gradient(135deg,rgba(255,255,255,.3),rgba(255,255,255,.04) 42%,rgba(0,0,0,.18))}
.tq{box-shadow:0 0 0 .5px rgba(0,0,0,.35)}
.bsq{box-shadow:inset 0 0 0 2px #4a525c,inset 0 1px 0 3px rgba(255,255,255,.35),0 3px 5px rgba(0,0,0,.45)}
/* street lamp + bench details */
.lampb .lp{box-shadow:inset -2px 0 2px rgba(0,0,0,.5)}
.lampb .lh{border:1px solid rgba(0,0,0,.35)}
</style>
</head>
<body>

<!-- ============================================================
     MODULE 25 — Living background markup
     ============================================================ -->
<div class="bg" aria-hidden="true">
  <div class="blob blob-a"></div>
  <div class="blob blob-b"></div>
  <div class="blob blob-c"></div>
  <div class="veil"></div>
  <div class="blob blob-d night-only"></div>
  <div class="blob blob-e night-only"></div>
  <div class="stars" id="stars"></div>
  <div class="grain"></div>
  <div class="vignette"></div>
</div>

<!-- ============================================================
     MODULE 26 — Footstep chrome + Lumenglass toggle
     ============================================================ -->
<div id="brand" class="glass">Ω(1) Thinkers</div>
<h1>Footstep Power Generation</h1>
<div id="mt" title="Click to replay"></div>

<button class="toggle" id="toggle" type="button"
        role="switch" aria-checked="false"
        aria-label="Switch to night theme">
  <span class="sky">
    <span class="mini-stars"><i></i><i></i><i></i><i></i></span>
    <span class="cloud"></span>
  </span>
  <span class="orb">
    <span class="sun"></span>
    <span class="moon"></span>
  </span>
</button>

<canvas id="gl"></canvas>
<div id="cw"><div id="sky"><div class="cl"></div><div class="cl"></div><div class="cl"></div></div><div id="world"></div><div id="storm"></div><canvas id="rainc"></canvas><div id="haze"></div></div>
<div id="cap" class="glass"></div>
<div id="hint"></div>
<div id="dock"><div id="dk">
  <button class="key" id="kAsm">Assemble</button>
  <button class="key" id="kVid">▶ Split Video</button>
  <button class="key" id="kDemo">▶ Demo Video</button>
  <button class="key" id="kReal">REALISTIC VIEW</button>
</div></div>
<div id="pop" class="glass"><button class="key" id="x">×</button><small id="pn"></small><h3 id="pt"></h3><p id="pd"></p><div id="ps"></div><div id="pb"><i></i></div></div>
<div id="rv"><canvas id="cv"></canvas><div id="rt" class="glass">Realistic view · footpath with piezo + solar tile blocks</div><button class="key" id="rb">✕ Back</button><button class="key" id="rainb">☔ Start rain</button><div id="rs" class="glass"><span>Steps <b id="n1">0</b></span><span>Energy <b id="n2">0</b> J</span><span>Lamps <i id="n3"><u></u></i></span><span>Solar <b id="n4">0</b> W</span></div></div>
<label id="hp" aria-hidden="true" style="position:fixed;left:-99px;top:0;opacity:0;pointer-events:none"><input type="checkbox" switch></label>
<div id="tip" class="glass"></div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
<script>
/* ============================================================
   ★ EASY EDIT — change these values, save, refresh.
   ============================================================ */
const SETTINGS={
  teamName   :'Ω(1) Thinkers',
  title      :'Footstep Power Generation',
  bigHeading :'PIEZO SOLAR TILES',
  buttons    :{assemble:'Assemble',split:'▶ Split Video',demo:'▶ Demo Video',stopDemo:'■ Stop Demo',real:'REALISTIC VIEW'},
  rainSound  :true,   // soft rain sound when rain starts
  splitZoom  :1.15,   // >1 = device is magnified a little when split
  selectedShrink:1.25,// >1 = device gets smaller when a part is selected / magnified
  partPop    :1.03,   // how much the selected part itself grows
  deviceSize :1,      // bigger = device fills more of the screen
  smoothness :120,    // ms. Higher = silkier / slower mouse-follow
  splitSpeed :1.4,    // higher = slower fly-apart
  maxPixelRatio:2,    // sharpness. 1 = fastest, 2 = crisp (auto-lowers if the screen can't keep up)
  shadows    :true,
  walkers    :10,      // people in Realistic View
  tileBlocks :8,
  tileSize   :.6,     // size of each footpath piezo tile in metres (smaller = smaller device)       // blocks of 4 tiles on the footpath
};

/* ===== 01 · Helpers ===== */
const $=s=>document.querySelector(s),sleep=ms=>new Promise(r=>setTimeout(r,ms));
const mt=$('#mt');
const buildMt=()=>{let n=0;mt.innerHTML=SETTINGS.bigHeading.split(' ').map(w=>`<span class="wd">${w.split('').map(c=>`<span class="w" style="--i:${n++}"><i>${c}</i></span>`).join('')}</span>`).join(' ')};
buildMt();
/* ============================================================
   MODULE 48 — Lumenglass toggle: starfield, theme switch, keyboard
   ============================================================ */
(function buildStars(){
  const host=$('#stars');
  if(!host)return;
  const reduced=matchMedia('(prefers-reduced-motion: reduce)').matches;
  const frag=document.createDocumentFragment();
  const COUNT=reduced?40:120;
  for(let i=0;i<COUNT;i++){
    const s=document.createElement('span');
    s.className='star';
    const size=Math.random()<0.86?1.6:2.6;
    s.style.width =size.toFixed(2)+'px';
    s.style.height=size.toFixed(2)+'px';
    s.style.left  =(Math.random()*100).toFixed(3)+'%';
    s.style.top   =(Math.random()*100).toFixed(3)+'%';
    s.style.animationDelay   =(Math.random()*4).toFixed(2)+'s';
    s.style.animationDuration=(2.2+Math.random()*3.6).toFixed(2)+'s';
    frag.appendChild(s);
  }
  host.appendChild(frag);
})();

const toggleEl=$('#toggle');
const prefersReduced=matchMedia('(prefers-reduced-motion: reduce)').matches;

function applyTheme(isDark, animate){
  document.documentElement.dataset.theme = isDark ? 'dark' : 'light';
  toggleEl.setAttribute('aria-checked', String(isDark));
  toggleEl.setAttribute('aria-label',
    isDark ? 'Switch to day theme' : 'Switch to night theme');
  const meta=document.querySelector('meta[name="theme-color"]');
  if(meta)meta.setAttribute('content', isDark ? '#050b1a' : '#eef6ff');
  if(animate && !prefersReduced){
    toggleEl.classList.remove('pulse');
    void toggleEl.offsetWidth;
    toggleEl.classList.add('pulse');
  }
  buildMt();
}

applyTheme(matchMedia('(prefers-color-scheme: dark)').matches, false);

toggleEl.addEventListener('click', ()=>{
  applyTheme(document.documentElement.dataset.theme !== 'dark', true);
});

addEventListener('keydown', e=>{
  if((e.key==='t' || e.key==='T') && !(e.target instanceof HTMLInputElement)){
    applyTheme(document.documentElement.dataset.theme !== 'dark', true);
  }
});



/* ===== 02 · Renderer, scenes, cameras ===== */
const LOW=matchMedia('(pointer:coarse)').matches;
const gl=$('#gl'),R=new THREE.WebGLRenderer({canvas:gl,antialias:true,alpha:true,powerPreference:'high-performance'});
R.outputEncoding=THREE.sRGBEncoding;R.toneMapping=THREE.LinearToneMapping;R.toneMappingExposure=.95;
R.shadowMap.enabled=SETTINGS.shadows;R.shadowMap.type=THREE.PCFSoftShadowMap;
let PR=Math.min(devicePixelRatio,SETTINGS.maxPixelRatio);R.setPixelRatio(PR);
const sc=new THREE.Scene(),W=new THREE.Scene(),cam=new THREE.PerspectiveCamera(36,1,.1,200),cam2=new THREE.PerspectiveCamera(46,1,.1,200);
const dev=new THREE.Group();sc.add(dev);

/* Studio reflections (makes metal and glass look real) */
function makeEnv(){const s=new THREE.Scene(),c=document.createElement('canvas');c.width=4;c.height=256;const g=c.getContext('2d'),gr=g.createLinearGradient(0,0,0,256);
  gr.addColorStop(0,'#9cc0ea');gr.addColorStop(.5,'#e6edf6');gr.addColorStop(1,'#2e3947');g.fillStyle=gr;g.fillRect(0,0,4,256);
  s.add(new THREE.Mesh(new THREE.SphereGeometry(50,32,16),new THREE.MeshBasicMaterial({map:new THREE.CanvasTexture(c),side:THREE.BackSide})));
  [[0,30,10,30,2,20],[-30,10,0,2,20,30],[30,10,-10,2,16,24]].forEach(([x,y,z,w,h,d])=>{const m=new THREE.Mesh(new THREE.BoxGeometry(w,h,d),new THREE.MeshBasicMaterial({color:new THREE.Color(3.5,3.5,3.5)}));m.position.set(x,y,z);s.add(m)});
  const p=new THREE.PMREMGenerator(R),t=p.fromScene(s,.03).texture;p.dispose();return t}
const envTex=makeEnv();sc.environment=envTex;W.environment=envTex;

/* ===== 03 · Procedural textures ===== */
function ctex(w,h,fn,rx=1,ry=1,srgb=true){const c=document.createElement('canvas');c.width=w;c.height=h;fn(c.getContext('2d'),w,h);const t=new THREE.CanvasTexture(c);t.wrapS=t.wrapT=THREE.RepeatWrapping;t.repeat.set(rx,ry);t.anisotropy=8;if(srgb)t.encoding=THREE.sRGBEncoding;return t}
const rnd=(a,b)=>a+Math.random()*(b-a);
const aluT=ctex(256,256,(g,w,h)=>{g.fillStyle='#aeb6c0';g.fillRect(0,0,w,h);for(let i=0;i<900;i++){g.fillStyle=Math.random()<.5?'rgba(255,255,255,.22)':'rgba(0,0,0,.2)';g.fillRect(0,rnd(0,h),w,rnd(.5,1.5))}},2,2);
const solT=ctex(512,512,(g,w,h)=>{const gr=g.createLinearGradient(0,0,w,h);gr.addColorStop(0,'#0a3ec0');gr.addColorStop(.5,'#1d6bf0');gr.addColorStop(1,'#06246e');g.fillStyle=gr;g.fillRect(0,0,w,h);
  const n=4,c=w/n;g.strokeStyle='#f5f9ff';g.lineWidth=4;for(let i=0;i<=n;i++){g.beginPath();g.moveTo(i*c,0);g.lineTo(i*c,h);g.moveTo(0,i*c);g.lineTo(w,i*c);g.stroke()}
  g.strokeStyle='rgba(240,246,255,.8)';g.lineWidth=1.5;for(let i=0;i<n;i++)for(let k=1;k<4;k++){g.beginPath();g.moveTo(i*c+k*c/4,0);g.lineTo(i*c+k*c/4,h);g.stroke()}});
const pcbT=ctex(256,256,(g,w,h)=>{g.fillStyle='#0d8a4e';g.fillRect(0,0,w,h);g.strokeStyle='rgba(245,205,80,.8)';g.lineWidth=2;for(let i=0;i<40;i++){g.beginPath();let x=rnd(0,w),y=rnd(0,h);g.moveTo(x,y);g.lineTo(x+rnd(-70,70),y);g.lineTo(x+rnd(-70,70),y+rnd(-70,70));g.stroke()}
  g.fillStyle='#f5cc4a';for(let i=0;i<90;i++){g.beginPath();g.arc(rnd(0,w),rnd(0,h),2.2,0,7);g.fill()}});
const lblT=txt=>ctex(128,64,(g,w,h)=>{g.fillStyle='#1d49b5';g.fillRect(0,0,w,h);g.fillStyle='#fff';g.font='700 38px system-ui';g.textAlign='center';g.textBaseline='middle';g.fillText(txt,w/2,h/2)});
const grassT=ctex(256,256,(g,w,h)=>{g.fillStyle='#5f9a4a';g.fillRect(0,0,w,h);for(let i=0;i<2500;i++){g.fillStyle=`hsl(${rnd(85,115)},${rnd(35,55)}%,${rnd(28,46)}%)`;g.fillRect(rnd(0,w),rnd(0,h),2,rnd(2,5))}},24,24);
const concT=ctex(256,256,(g,w,h)=>{g.fillStyle='#b9b4aa';g.fillRect(0,0,w,h);for(let i=0;i<2500;i++){g.fillStyle=`rgba(${Math.random()<.5?'255,255,255':'60,55,50'},.08)`;g.fillRect(rnd(0,w),rnd(0,h),2,2)}},2,8);

/* ===== 04 · Materials ===== */
const S_=(c,m,r,o)=>new THREE.MeshStandardMaterial(Object.assign({color:c,metalness:m,roughness:r},o));
const MT={   /* NATURAL COLOURS — edit any hex value */
  alu:S_(0xffffff,1,.3,{map:aluT,bumpMap:aluT,bumpScale:.6}),             // brushed silver aluminium
  dark:S_(0x1b2229,.8,.35),rubber:S_(0x0b0d10,0,.85),chip:S_(0x070809,.2,.5),   // gunmetal base, black rubber & chips
  pcb:S_(0xffffff,.1,.45,{map:pcbT}),pcbEdge:S_(0x0a6b3c,.1,.55),copper:S_(0xd2711f,1,.28),gold:S_(0xf0b928,1,.25),
  ceramic:S_(0xf3e6b0,0,.45,{emissive:0x000000}),blue:S_(0x1544b8,.1,.38),cell:S_(0x1b4fd8,.15,.35),green:S_(0x12a84e,0,.45),beige:S_(0xe0c890,0,.55),
  pot:S_(0x1769e6,0,.35),led:S_(0x222222,0,.4,{emissive:0x3aa0ff,emissiveIntensity:1.4}),
  wRed:S_(0xe01e1e,0,.45),wBlack:S_(0x0b0b0b,0,.5),
  solar:new THREE.MeshPhysicalMaterial({map:solT,metalness:.2,roughness:.18,clearcoat:1,clearcoatRoughness:.03}),
  bulb:new THREE.MeshStandardMaterial({color:0xfff3b0,emissive:0xffd54a,emissiveIntensity:0,roughness:.2}),
  skinF:S_(0xe6b896,0,.7)
};
Object.values(MT).forEach(m=>m.envMapIntensity=.8);   // less washed-out reflections

const mesh=(g,m,x=0,y=0,z=0,cast=true)=>{const o=new THREE.Mesh(g,m);o.position.set(x,y,z);o.castShadow=cast&&SETTINGS.shadows;o.receiveShadow=true;return o};
const CY=(r,h,m,x,y,z,s=28)=>mesh(new THREE.CylinderGeometry(r,r,h,s),m,x,y,z);
const BX=(w,h,d,m,x,y,z)=>mesh(new THREE.BoxGeometry(w,h,d),m,x,y,z);
const pcbDisc=r=>mesh(new THREE.CylinderGeometry(r,r,.03,48),[MT.pcbEdge,MT.pcb,MT.pcb]);
const CAP=(x,y,z,r=.07,h=.2)=>{const g=new THREE.Group();g.add(CY(r,h,MT.blue,0,0,0,20),CY(r*.96,.012,MT.alu,0,h/2+.004,0,20));g.position.set(x,y,z);return g};
function coil(r,H,turns,wr,m){const pts=[],n=turns*14;for(let i=0;i<=n;i++){const a=i/14*Math.PI*2;pts.push(new THREE.Vector3(r*Math.cos(a),(i/n-.5)*H,r*Math.sin(a)))}return mesh(new THREE.TubeGeometry(new THREE.CatmullRomCurve3(pts),n*2,wr,6,false),m)}
function hullPts(Rd,Rt,n=14){const p=[];[90,210,330].forEach(a=>{const cx=Rd*Math.cos(a*Math.PI/180),cy=Rd*Math.sin(a*Math.PI/180);for(let i=0;i<=n;i++){const t=(a-60+120*i/n)*Math.PI/180;p.push(new THREE.Vector2(cx+Rt*Math.cos(t),cy+Rt*Math.sin(t)))}});return p}
function slab(pts,h,mats,bev=0){const g=new THREE.ExtrudeGeometry(new THREE.Shape(pts),{depth:h,bevelEnabled:!!bev,bevelSize:bev,bevelThickness:bev,bevelSegments:3,curveSegments:1});g.rotateX(-Math.PI/2);return mesh(g,mats)}

/* ===== 05 · One corner unit — every layer is built here ===== */
const L={
 base(){const g=new THREE.Group();g.add(CY(1.12,.16,MT.dark,0,.08,0,48),CY(.98,.02,MT.rubber,0,.17,0,48));
  for(let i=0;i<8;i++){const a=i*Math.PI/4;g.add(CY(.045,.03,MT.alu,1.05*Math.cos(a),.19,1.05*Math.sin(a),6))}
  [[.6,.6],[-.6,.6],[.6,-.6],[-.6,-.6]].forEach(([x,z])=>g.add(CY(.06,.1,MT.alu,x,.23,z,12)));
  const c=CY(.08,.16,MT.rubber,1.17,.09,0,16);c.rotation.z=Math.PI/2;g.add(c);return g},
 esp(){const g=new THREE.Group();g.add(BX(.74,.025,1,MT.pcb,0,0,0),BX(.34,.05,.38,MT.alu,0,.04,.1),BX(.5,.012,.22,MT.gold,0,.02,-.38),BX(.12,.06,.1,MT.alu,0,.04,.52),BX(.04,.02,.04,MT.led,.2,.03,-.15));
  [-.33,.33].forEach(x=>g.add(BX(.025,.05,.9,MT.chip,x,.035,0)));return g},
 inv(){const g=new THREE.Group();g.add(pcbDisc(.84),BX(.3,.18,.22,MT.chip,-.38,.11,-.2));const c=coil(.16,.15,9,.012,MT.copper);c.position.set(-.38,.11,-.2);g.add(c);
  [[.3,-.3],[.5,-.05],[.15,-.55]].forEach(([x,z])=>g.add(CAP(x,.12,z,.075,.2)));
  g.add(BX(.4,.03,.2,MT.alu,0,.03,.5));for(let i=0;i<9;i++)g.add(BX(.02,.13,.2,MT.alu,-.18+i*.045,.1,.5));
  g.add(BX(.1,.07,.04,MT.chip,-.1,.05,.32),BX(.1,.07,.04,MT.chip,.1,.05,.32),BX(.16,.04,.2,MT.chip,.25,.035,.1),BX(.24,.1,.12,MT.green,0,.07,-.7));
  for(let i=0;i<4;i++){const r=CY(.022,.12,MT.beige,-.62,.04,.15+i*.1,10);r.rotation.z=Math.PI/2;g.add(r)}return g},
 bat(){const g=new THREE.Group();[[.3,.3],[-.3,.3],[.3,-.3],[-.3,-.3]].forEach(([x,z])=>g.add(CY(.18,.34,MT.cell,x,0,z),CY(.17,.012,MT.alu,x,.176,z,24),CY(.05,.03,MT.alu,x,.2,z,12)));
  g.add(BX(.72,.015,.07,MT.copper,0,.22,.3),BX(.72,.015,.07,MT.copper,0,.22,-.3));return g},
 boost(){const g=new THREE.Group();g.add(BX(.95,.03,.8,MT.pcb,0,0,0),CY(.15,.1,MT.dark,-.25,.065,-.1,20));const c=coil(.17,.09,10,.011,MT.copper);c.position.set(-.25,.065,-.1);g.add(c,
  CAP(.3,.1,-.2,.07,.17),CAP(.3,.1,.1,.07,.17),BX(.24,.04,.15,MT.chip,0,.035,.28),BX(.2,.1,.12,MT.pot,-.4,.065,.28),CY(.025,.01,MT.gold,-.4,.12,.28,12),BX(.3,.07,.1,MT.green,0,.05,-.37),BX(.3,.07,.1,MT.green,0,.05,.37));return g},
 rect(){const g=new THREE.Group();g.add(pcbDisc(.85));
  [[-.2,.25],[.2,.25],[-.2,.45],[.2,.45]].forEach(([x,z])=>{const d=CY(.04,.14,MT.chip,x,.05,z,12),b=CY(.042,.02,MT.alu,x+.045,.05,z,12);d.rotation.z=b.rotation.z=Math.PI/2;g.add(d,b)});
  g.add(CAP(.55,.11,-.1,.07,.2),CAP(-.55,.11,-.1,.07,.2),BX(.3,.07,.12,MT.green,0,.05,.7));
  const lab=MT.l4||(MT.l4=S_(0xffffff,.1,.4,{map:lblT('4V')}));
  g.add(mesh(new THREE.BoxGeometry(.84,.24,.3),[MT.cell,MT.cell,lab,MT.cell,MT.cell,MT.cell],0,.14,-.3),CY(.04,.04,MT.alu,-.25,.28,-.3,12),CY(.04,.04,MT.alu,.25,.28,-.3,12));return g},
 plate(){const g=new THREE.Group();g.add(CY(1.12,.08,MT.alu,0,0,0,56));for(let i=0;i<8;i++){const a=i*Math.PI/4;g.add(CY(.045,.03,MT.alu,1.02*Math.cos(a),.05,1.02*Math.sin(a),6))}
  [[.95,0],[-.95,0],[0,.95],[0,-.95]].forEach(([x,z])=>{const s=coil(.09,.2,5,.018,MT.alu);s.position.set(x,-.14,z);g.add(s)});return g},
 piezo(){const g=new THREE.Group();g.add(CY(1,.02,MT.rubber,0,0,0,48),BX(.24,.05,.14,MT.green,0,.035,0));
  for(let i=0;i<6;i++){const a=(30+60*i)*Math.PI/180,x=.62*Math.cos(a),z=.62*Math.sin(a),w=BX(.35,.01,.012,MT.copper,.275*Math.cos(a),.017,.275*Math.sin(a));w.rotation.y=-a;
   g.add(CY(.17,.03,MT.gold,x,.025,z,32),CY(.115,.035,MT.ceramic,x,.045,z,28),w)}return g}
};

/* ===== 05b · Extra detail on every layer (add / remove freely) ===== */
const glassM=new THREE.MeshPhysicalMaterial({color:0xddeeff,transparent:true,opacity:.35,roughness:.1}),
  labM=S_(0xffffff,.6,.4,{map:ctex(256,128,(g,w,h)=>{g.fillStyle='#d7dde5';g.fillRect(0,0,w,h);g.fillStyle='#0b2a55';g.font='700 34px system-ui';g.textAlign='center';g.fillText('Ω(1) THINKERS',w/2,52);g.font='600 22px system-ui';g.fillText('12V · 180W · IP65',w/2,92)})}),
  dotM=S_(0xffffff,0,.9,{map:ctex(256,256,(g,w,h)=>{g.fillStyle='#14181d';g.fillRect(0,0,w,h);g.fillStyle='#2e353e';for(let y=8;y<h;y+=16)for(let x=8;x<w;x+=16){g.beginPath();g.arc(x,y,3,0,7);g.fill()}},3,3)});
const ex_=(f,fn)=>{const o=L[f];L[f]=()=>{const g=o();fn(g);return g}};
const ring=(r,t,m,x,y,z)=>{const q=mesh(new THREE.TorusGeometry(r,t,8,48),m,x,y,z);q.rotation.x=Math.PI/2;return q};
ex_('base',g=>{g.add(CY(1.14,.03,MT.alu,0,.015,0,56));[[.8,.8],[-.8,.8],[.8,-.8],[-.8,-.8]].forEach(([x,z])=>g.add(CY(.1,.04,MT.rubber,x,-.02,z,16)));
  const lb=BX(.5,.012,.25,labM,-.5,.185,.6);lb.rotation.y=.4;g.add(lb);[.39,2.49,4.59].forEach(a=>g.add(CY(.07,.07,MT.chip,1.06*Math.cos(a),.2,1.06*Math.sin(a),16),CY(.075,.02,MT.gold,1.06*Math.cos(a),.235,1.06*Math.sin(a),16)));g.add(ring(.9,.012,MT.alu,0,.18,0))});
ex_('esp',g=>{for(let i=0;i<15;i++)[-.33,.33].forEach(x=>g.add(BX(.012,.07,.012,MT.gold,x,.06,-.42+i*.06)));
  g.add(BX(.08,.03,.06,MT.alu,0,.03,.47),BX(.06,.03,.06,MT.alu,-.2,.03,-.48),BX(.06,.03,.06,MT.alu,.2,.03,-.48),CY(.03,.012,MT.alu,.28,.03,.3,12),BX(.04,.025,.04,MT.led,-.28,.03,.3));
  for(let i=0;i<6;i++)g.add(BX(.2,.012,.012,MT.gold,i%2?.06:-.06,.027,-.46+i*.03))});
ex_('inv',g=>{g.add(BX(.2,.08,.1,MT.green,-.3,.06,.68),CY(.025,.02,MT.alu,-.36,.11,.68,10),CY(.025,.02,MT.alu,-.24,.11,.68,10),BX(.22,.07,.07,glassM,.3,.06,.62),BX(.03,.08,.08,MT.alu,.18,.06,.62),BX(.03,.08,.08,MT.alu,.42,.06,.62));
  const t=mesh(new THREE.TorusGeometry(.1,.035,10,24),MT.copper,.45,.09,-.5);t.rotation.x=Math.PI/2;g.add(t,CAP(-.1,.12,-.55,.06,.18),CAP(.05,.12,-.62,.06,.18))});
ex_('bat',g=>{[[.3,.3],[-.3,.3],[.3,-.3],[-.3,-.3]].forEach(([x,z])=>g.add(CY(.182,.06,S_(0xf5f5f5,0,.5),x,.04,z,28),CY(.12,.012,MT.alu,x,.18,z,20)));
  g.add(BX(.6,.02,.24,MT.pcb,0,.23,0),BX(.14,.04,.1,MT.chip,-.15,.26,0),BX(.1,.04,.1,MT.chip,.15,.26,0),BX(.03,.03,.3,MT.wRed,.34,.22,.14),BX(.03,.03,.3,MT.wBlack,-.34,.22,-.14))});
ex_('boost',g=>{for(let i=0;i<8;i++)g.add(BX(.02,.14,.16,MT.alu,.18+i*.04,.1,.28));g.add(BX(.26,.02,.18,MT.alu,.3,.03,.28));
  g.add(BX(.14,.15,.05,MT.chip,.28,.1,-.05),BX(.14,.02,.05,MT.alu,.28,.19,-.05));for(let i=0;i<6;i++)g.add(BX(.045,.02,.025,MT.beige,-.35+i*.07,.03,-.3));g.add(BX(.03,.025,.03,MT.led,.4,.03,.0))});
ex_('rect',g=>{g.add(BX(.05,.03,.05,MT.led,.1,.03,.55),CY(.03,.1,MT.chip,-.55,.07,.4,10),BX(.2,.07,.07,glassM,.5,.06,.4));[-.12,0,.12].forEach(x=>g.add(CY(.012,.1,MT.alu,x,.04,.7,8)))});
ex_('plate',g=>{[.35,.55,.8].forEach(r=>g.add(ring(r,.012,MT.alu,0,.045,0)));for(let i=0;i<6;i++){const a=(30+60*i)*Math.PI/180;g.add(CY(.08,.03,MT.gold,.62*Math.cos(a),.05,.62*Math.sin(a),20))}});
ex_('piezo',g=>{g.add(CY(.98,.004,dotM,0,.012,0,48));for(let i=0;i<6;i++){const a=(30+60*i)*Math.PI/180,x=.62*Math.cos(a),z=.62*Math.sin(a);g.add(ring(.085,.008,MT.alu,x,.064,z),CY(.012,.01,MT.alu,x,.066,z,8))}});

/* ===== 06 · Parts table — edit names, text and explode distance (ex) here ===== */
const UN=[[0,-1.9],[1.645,.95],[-1.645,.95]];
const PARTS=[
 {n:'Piezoelectric Sensors',k:'piezo',y:1.3,ex:1.4,d:'Six brass-and-ceramic piezo discs sit on a rubber mat directly under the thick triangular cover. When your weight squeezes them, the crystal gives out a burst of AC voltage (the piezoelectric effect).',s:['6 piezo discs','Rubber mat','Piezoelectric effect']},
 {n:'Aluminium Support Plate & Springs',k:'plate',y:1.18,ex:.95,d:'An anodised aluminium plate with 8 hex bolts carries the piezo discs. Four coil springs give a little when you step and push everything back up when you step off.',s:['Aluminium alloy','8 hex bolts','4 return springs']},
 {n:'Rectifier & 4 V Battery',k:'rect',y:1,ex:.5,d:'Four diodes form a bridge rectifier that turns the piezo pulses into one-way DC. The DC charges a 4 V battery that smooths the short bursts from each step.',s:['Bridge rectifier','4 V Li-ion battery','Smooths bursts']},
 {n:'Boost Converter 4 V → 12 V',k:'boost',y:.85,ex:.05,d:'A step-up converter: a coil, a switching chip and a diode raise the 4 V to a steady 12 V. A trimmer screw sets the exact output voltage.',s:['4 V in','12 V out','Coil + IC + diode']},
 {n:'12 V Battery',k:'bat',y:.55,ex:-.4,d:'Four cells in series make 12 V. The battery stores the boosted piezo power and is also charged directly by the solar cells on top. It feeds the inverter and the ESP32.',s:['4 cells · 12 V','Boost input','Solar wired direct']},
 {n:'12V DC → 220V AC Inverter',k:'inv',y:.36,ex:-.85,d:'A switching chip drives two MOSFETs and a step-up transformer, turning 12 V DC into 220 V AC (180 W) to light the LED bulb. The board also carries a heatsink, capacitors and resistors.',s:['12 V DC in','220 V AC out','180 W rated']},
 {n:'ESP32 Wi-Fi Module',k:'esp',y:.22,ex:-1.3,d:'A Wi-Fi + Bluetooth microcontroller powered by the 12 V battery. Its antenna makes a hotspot; connect your phone and this website opens with live readings.',s:['Wi-Fi hotspot','Bluetooth','Phone dashboard']},
 {n:'Aluminium Base Housing',k:'base',y:0,ex:-1.7,d:'A rugged metal base holding every layer on four standoffs and 8 bolts. It shields the electronics from water and dust and has a sealed cable gland.',s:['Aluminium body','Standoffs & bolts','Sealed gland']},
 {n:'Thick Triangular Cover',y:1.43,ex:2.1,d:'A thick, load-bearing triangular slab in brushed aluminium with a dark rubber gasket band. It carries the solar cells, and when you step on it the underside presses evenly on the piezo discs.',s:['Thick aluminium slab','Rubber gasket','Presses the sensors']},
 {n:'Unbreakable Solar Cells',y:1.7,ex:2.8,d:'A triangular panel of solar cells under a tough unbreakable clear layer, so it can be walked on. In daylight it sends DC straight to the 12 V battery through cables that pass down through the cover.',s:['Unbreakable top','Walk-on solar cells','Wired to 12 V']}
];
const ORDER=[9,8,0,1,2,3,4,5,6,7];
const A=(o,x,y,z)=>{const a=new THREE.Object3D();a.position.set(x,y,z);o.add(a);return a};
PARTS.forEach(p=>{p.g=new THREE.Group();p.g.position.y=p.y;p.cur=0;p.at=0;dev.add(p.g);
  if(p.k){p.units=UN.map(([x,z])=>{const l=L[p.k]();l.position.set(x,0,z);p.g.add(l);l.aO=[A(l,-.1,.05,-.05),A(l,.1,.05,.05)];l.aI=[A(l,-.1,-.01,-.05),A(l,.1,-.01,.05)];l.aS=A(l,.3,.22,.3);return l})}});
{ /* cover + gasket + rim bolts */
  const c=PARTS[8].g,Rd=1.9,Rt=1.18;
  c.add(slab(hullPts(Rd,Rt),.26,[MT.alu,MT.alu],.015));const gk=slab(hullPts(Rd,Rt+.008),.07,MT.rubber);gk.position.y=.1;c.add(gk);
  [90,210,330].forEach(a=>{const u=a*Math.PI/180;c.add(CY(.045,.02,MT.alu,(Rd+Rt-.06)*Math.cos(u),.285,-(Rd+Rt-.06)*Math.sin(u),6))});
  [150,270,30].forEach(a=>{const u=a*Math.PI/180;c.add(CY(.045,.02,MT.alu,(Rd/2+Rt-.06)*Math.cos(u),.285,-(Rd/2+Rt-.06)*Math.sin(u),6))});
  const s=PARTS[9].g,fr=slab(hullPts(Rd,Rt-.12),.06,[MT.dark,MT.dark],.008),pn=slab(hullPts(Rd,Rt-.17),.03,[MT.solar,MT.dark]);pn.position.y=.06;s.add(fr,pn);
  s.sA=UN.map(([x,z])=>A(s,x,0,z));
}
{const jb=PARTS[9].g;jb.add(BX(.5,.08,.32,MT.chip,0,.1,-2.72),CY(.05,.1,MT.rubber,0,.1,-2.92,12),BX(.1,.02,.1,MT.alu,.18,.15,-2.72));[-1,1].forEach(k=>jb.add(CY(.04,.04,MT.rubber,k*.28*1,.05,-2.6,10)))}
PARTS.forEach((p,i)=>p.g.traverse(o=>o.userData.pi=i));

/* ===== 07 · Wires (stretch between layers while parts move) ===== */
const wires=[],_a=new THREE.Vector3(),_b=new THREE.Vector3(),_d=new THREE.Vector3(),UPV=new THREE.Vector3(0,1,0);
function wire(a,b,m,r=.012){const o=new THREE.Mesh(new THREE.CylinderGeometry(r,r,1,6),m);sc.add(o);const w={a,b,o};wires.push(w);return w}
UN.forEach((_,u)=>{[[0,2],[2,3],[3,4],[4,5],[5,6]].forEach(([p,q])=>[0,1].forEach(j=>wire(PARTS[p].units[u].aO[j],PARTS[q].units[u].aI[j],j?MT.wBlack:MT.wRed)));
  wire(PARTS[9].g.sA[u],PARTS[4].units[u].aS,MT.wRed,.016)});
function updWires(){wires.forEach(w=>{if(!w.o.visible)return;w.a.getWorldPosition(_a);w.b.getWorldPosition(_b);_d.subVectors(_b,_a);const l=_d.length()||.001;w.o.position.copy(_a).addScaledVector(_d,.5);w.o.scale.set(1,l,1);w.o.quaternion.setFromUnitVectors(UPV,_d.normalize())})}

/* ===== 08 · Demo props: foot, LED bulb, energy pulses ===== */
const foot=new THREE.Group();foot.add(BX(.62,.14,1.3,MT.skinF,0,0,0),CY(.24,1.5,MT.skinF,0,.8,-.45,20));for(let i=0;i<5;i++)foot.add(CY(.075-i*.006,.12,MT.skinF,-.22+i*.11,0,.7,10));
foot.visible=false;dev.add(foot);
const bulbG=new THREE.Group();bulbG.add(CY(.06,1.6,MT.dark,0,.8,0,12),CY(.16,.3,MT.alu,0,1.75,0,20),mesh(new THREE.SphereGeometry(.34,28,20),MT.bulb,0,2.1,0));
const bulbL=new THREE.PointLight(0xffd54a,0,14);bulbL.position.set(0,2.1,0);bulbG.add(bulbL);bulbG.position.set(4.3,-.7,.4);bulbG.visible=false;dev.add(bulbG);
const bAnch=A(bulbG,0,1.75,0),bWire=wire(PARTS[5].units[0].aO[0],bAnch,MT.wRed,.014);bWire.o.visible=false;
const pulses=UN.map(()=>{const m=new THREE.Mesh(new THREE.SphereGeometry(.07,12,10),new THREE.MeshBasicMaterial({color:0x8fe8ff}));m.visible=false;sc.add(m);return m});
const bh=new THREE.Box3Helper(new THREE.Box3(),0x7fe3ff);bh.visible=false;sc.add(bh);

/* ===== 09 · Lights (device scene) ===== */
const key=new THREE.DirectionalLight(0xfff7ea,2.6);key.position.set(5,9,7);key.castShadow=SETTINGS.shadows;key.shadow.mapSize.set(LOW?1024:2048,LOW?1024:2048);
Object.assign(key.shadow.camera,{left:-6,right:6,top:7,bottom:-6,near:1,far:30});key.shadow.bias=-.0004;key.shadow.normalBias=.02;key.shadow.camera.updateProjectionMatrix();sc.add(key,new THREE.HemisphereLight(0xffffff,0x1b2430,.22));
const rim=new THREE.PointLight(0x6fb8ff,1.4,30);rim.position.set(-6,3,-5);sc.add(rim);
const floor=new THREE.Mesh(new THREE.PlaneGeometry(30,30),new THREE.ShadowMaterial({opacity:.4}));floor.rotation.x=-Math.PI/2;floor.position.y=-2.05;floor.receiveShadow=true;sc.add(floor);

/* ===== 10 · Realistic View — built with CSS 3D (plain DOM + transforms, no WebGL) ===== */
const cw=$('#cw'),wd=$('#world'),M=80;                 // 1 metre = 80 px  (change M to scale the whole street)
const P=m=>(m*M).toFixed(1)+'px';
const el=(cls,st,par=wd)=>{const e=document.createElement('div');if(cls)e.className=cls;if(st)Object.assign(e.style,st);par.appendChild(e);return e};
const flat=(x,y,w,d,cls,z=0,st)=>el('fl '+cls,Object.assign({left:P(x),top:P(y),width:P(w),height:P(d),transform:`translateZ(${z}px)`},st||{}));
function box(x,y,w,d,h,z,col,par=wd,cls=''){const b=el('bx '+cls,{left:P(x),top:P(y),width:P(w),height:P(d),transform:`translateZ(${P(z)})`},par),H=P(h);b.style.setProperty('--c',col);b.F={};
  const f=(k,st)=>b.F[k]=el('f '+k,st,b);
  f('t',{left:0,top:0,width:'100%',height:'100%',transform:`translateZ(${H})`});
  f('s',{left:0,top:'100%',width:'100%',height:H,transformOrigin:'0 0',transform:'rotateX(90deg)'});
  f('n',{left:0,top:0,width:'100%',height:H,transformOrigin:'0 0',transform:'rotateX(90deg)'});
  f('w',{left:0,top:0,width:H,height:'100%',transformOrigin:'0 0',transform:'rotateY(-90deg)'});
  f('e',{left:'100%',top:0,width:H,height:'100%',transformOrigin:'0 0',transform:'rotateY(-90deg)'});return b}
const bb=(x,y,w,h,cls,par=wd,st)=>el('pf '+cls,Object.assign({left:P(x-w/2),top:(y*M-h*M)+'px',width:P(w),height:P(h),transformOrigin:'50% 100%',transform:'rotateX(-90deg)'},st||{}),par);
const R_=(a,b)=>a+Math.random()*(b-a);
/* ---- ground: lawn | hedge | footpath | drain | kerb | road | far kerb ---- */
const X0=4,XL=54;                                         // street runs from x=4 m to x=58 m
flat(X0,6,XL,26,'grass',-2);                              // lawn
flat(X0,8,XL,4.4,'path');                                 // FOOTPATH  y 8 … 12.4
flat(X0,12.4,XL,.4,'drain');flat(X0,12.4,XL,.4,'grate',1); // DRAINAGE channel + grate
box(X0,7.8,XL,.2,.12,0,'#d2cdc2');box(X0,12.8,XL,.4,.15,0,'#d2cdc2');
flat(X0,13.2,XL,7,'road');flat(X0,16.62,XL,.16,'dash',1);flat(X0,13.4,XL,.12,'solid',1);flat(X0,19.9,XL,.12,'solid',1);   // ROAD + markings
box(X0,20.2,XL,.4,.15,0,'#d2cdc2');
for(let i=0;i<8;i++)flat(44+i*.9,13.3,.5,6.8,'zeb',1);   // zebra crossing
[16,44].forEach(x=>flat(x-.3,11.2,.6,.6,'mh',1));         // manholes
/* ---- buildings on the far side of the footpath ---- */
let bx=X0;const bld=[];
[[9,10,'#c9a98b'],[10,14,'#b4c0cc'],[8,8,'#e0d4c0'],[11,16,'#9db39f'],[9,11,'#d0ac98'],[7,13,'#c2b7d0']].forEach(([w,h,col])=>{
  const b=box(bx,0,w,6.5,h,0,col),cols=Math.round(w/2.4),rows=Math.round(h/3.2),g=el('wg',{gridTemplateColumns:`repeat(${cols},1fr)`,gridTemplateRows:`repeat(${rows},1fr)`},b.F.s);
  for(let i=0;i<cols*rows;i++)el('wn'+(Math.random()<.55?' l':''),null,g);
  el('door',{left:P(w/2-.7),bottom:0,width:P(1.4),height:P(2.3)},b.F.s);
  box(bx+w/2-1.2,6.5,2.4,1.1,.1,2.4,'#aeb6c0');box(bx-.15,-.15,w+.3,6.8,.3,h,'#3a434c');bld.push([bx,w,h]);bx+=w});
bld.forEach(([x,w,h])=>{const s=Math.min(h*.42,5.6),W2=w+s*.55,pc=v=>(v/W2*100).toFixed(1)+'%';flat(x-s*.55,6.5,W2,s,'bsh',3,{clipPath:`polygon(${pc(s*.55)} 0,100% 0,${pc(w)} 100%,0 100%)`})});   // soft sun shadows from buildings
box(X0,6.6,XL,.8,.8,0,'#357f38',wd,'hedge');              // hedge with flowers
/* ---- trees ---- */
function tree(x,y,s){const t=bb(x,y,4*s,5.4*s,'tree');el('tr',null,t);el('cn',null,t);flat(x-1.4*s,y-.2,3.4*s,1.2*s,'tsh',.5)}
[[8,7.5,.7],[52,7.5,.7],[14,23,1.3],[46,23,1.2],[6,24,1.1],[55,23.5,1.4]].forEach(a=>tree(...a));
/* ---- street furniture ---- */
[22,36].forEach(x=>{box(x,7.9,1.6,.45,.05,.45,'#8a5a2b');box(x,7.85,1.6,.05,.4,.5,'#8a5a2b');box(x+.1,7.95,.06,.35,.45,0,'#333');box(x+1.44,7.95,.06,.35,.45,0,'#333')});
[27,41].forEach(x=>box(x,7.9,.4,.4,.7,0,'#2e7d4f'));
for(let x=18;x<=42;x+=3)box(x,12.0,.12,.12,.6,0,'#f2c230');
const lamps=[];[21,27,33,39].forEach(x=>{const l=bb(x,13.0,1.6,4.4,'lampb');el('lp',null,l);el('la',null,l);const h=el('lh',null,l),pool=flat(x-2.2,8.4,4.4,4,'pool',4);lamps.push([h,pool])});
/* ---- cars ---- */
const cars=[];
function car(col,lane,dir,x,v){const r=el('ent',{top:P(lane),left:0});el('csh',{left:P(-.1),top:P(.2),width:P(5.2),height:P(1.9),transform:'translateZ(.5px) skewX(-18deg)'},r);
  const lo=box(0,0,4.2,1.8,.55,.3,col,r),cab=box(.9,.1,2.2,1.6,.5,.85,col,r,'cab');
  [[.8,1.8],[3.4,1.8],[.8,0],[3.4,0]].forEach(([cx,cy])=>bb(cx,cy,.68,.68,'wh',r));
  [.12,.62].forEach(t=>{el(dir>0?'hl':'tl',{left:'18%',top:P(t),width:'64%',height:P(.22)},lo.F.e);el(dir>0?'tl':'hl',{left:'18%',top:P(t),width:'64%',height:P(.22)},lo.F.w)});
  cars.push({r,x,v,dir})}
[['#c62828',14,1,26,5],['#f5f5f5',14,1,50,6],['#2e7d32',14,1,8,5.5],['#1565c0',17.6,-1,40,6.5],['#f9a825',17.6,-1,14,5.5]].forEach(a=>car(...a));
/* ---- footpath tiles: 2 triangles = 1 square · 4 squares = 1 big square ---- */
const TS=SETTINGS.tileSize,BS=TS*2,tiles=[];
for(let b=0;b<SETTINGS.tileBlocks;b++){const x0=18+b*BS*2.5,y0=10.2-TS;
  el('bsq',{left:P(x0-.05),top:P(y0-.05),width:P(BS+.1),height:P(BS+.1),transform:'translateZ(1px)'});
  for(let i=0;i<2;i++)for(let j=0;j<2;j++){const tq=el('tq',{left:P(x0+i*TS),top:P(y0+j*TS),width:P(TS),height:P(TS),transform:'translateZ(2px)'});el('tri a',null,tq);el('tri c',null,tq);tiles.push({cx:x0+TS/2+i*TS,cy:y0+TS/2+j*TS,tq,was:0})}}
/* ---- people (side-view figures with swinging arms, legs and knees) ---- */
const UMB=['#d83a3a','#2f6fe0','#f2a33a','#7a4fd6','#1f9e6e'],SKc=['#f1c9a5','#d9a273','#a8693c','#6f4426'],HRc=['#2a1b12','#111','#6b4423','#b5651d','#d8c38a','#555'],TPc=['#e04f4f','#2f9e6e','#f2a33a','#4a6fd6','#e86aa5','#eeeeee','#2b2b3a','#8a5cd6'],PNc=['#2a3a5c','#1f2937','#4a4036','#6b7280','#2f4f4f'];
function limb(par,x,y,w,l1,l2,c1,c2,rad){const u=el('lb',{left:x-w/2+'px',top:y+'px',width:w+'px',height:l1+'px',background:c1,borderRadius:rad||'5px'},par),lo=el('lb',{left:0,top:l1-2+'px',width:'100%',height:l2+'px',background:c2,borderRadius:rad||'5px'},u);return{u,lo}}
function person(i){const lane=[10.0,10.4,9.8,8.8,11.5,10.2,9.9,9.0,11.2,10.6][i%10],dir=i%3==2?-1:1,sk=SKc[i%4],tp=TPc[i%8],pn=PNc[(i*2)%5],hr=HRc[i%6],root=el('ent',{top:P(lane),left:0});
  el('psh',{left:P(-.45),top:P(-.06),width:P(1.5),height:P(.32),transform:'translateZ(.5px) skewX(-38deg)'},root);
  const pf=bb(0,0,.9,1.8,'ps',root),S=(st,par)=>el('',st,par||pf);
  const lf=limb(pf,38,92,11,36,34,pn,pn),af=limb(pf,38,38,8,32,30,tp,sk,'4px');[lf,af].forEach(l=>{l.u.style.boxShadow='inset 0 0 0 99px rgba(0,0,0,.28)'});
  el('',{left:'-3px',top:'28px',width:'21px',height:'8px',background:i%2?'#f5f5f5':'#16161b',borderRadius:'3px 9px 3px 3px'},lf.lo);
  if(i%3===1)S({left:'12px',top:'38px',width:'15px',height:'32px',background:'#2f3d55',borderRadius:'5px'});
  S({left:'33px',top:'25px',width:'7px',height:'10px',background:sk});
  S({left:'22px',top:'32px',width:'29px',height:'50px',background:tp,borderRadius:'9px 9px 4px 4px'});
  S({left:'23px',top:'78px',width:'27px',height:'18px',background:pn,borderRadius:'3px'});
  S({left:'25px',top:'2px',width:'23px',height:'27px',background:sk,borderRadius:'50%'});
  S({left:'23px',top:'0',width:'26px',height:'15px',background:hr,borderRadius:'13px 13px 4px 4px'});
  S({left:'44px',top:'13px',width:'3px',height:'3px',background:'#222',borderRadius:'50%'});
  if(i%2)S({left:'17px',top:'9px',width:'8px',height:'22px',background:hr,borderRadius:'5px'});
  const ln=limb(pf,34,92,12,36,34,pn,pn),an=limb(pf,34,38,9,32,30,tp,sk,'4px');
  el('',{left:'-3px',top:'28px',width:'21px',height:'8px',background:i%2?'#fff':'#16161b',borderRadius:'3px 9px 3px 3px'},ln.lo);
  if(i%3===2)S({left:'42px',top:'66px',width:'17px',height:'15px',background:'#6b4a2b',borderRadius:'3px'});
  el('umb',{background:`repeating-linear-gradient(90deg,${UMB[i%5]} 0 14px,#fff 14px 28px)`},pf);el('uh',null,pf);
  ppl.push({root,pf,lf,af,ln,an,x:12+i*4.1,v:.85+(i%5)*.12,d:Math.random()*20,ph0:Math.random()*6,dir,lane})}
const ppl=[];for(let i=0;i<SETTINGS.walkers;i++)person(i);
/* ============================================================
   RAIN SYSTEM — wet ground, ripples, puddles, rivulets, drain flow, umbrellas
   Press "Start rain": rain builds slowly, water collects and, if it can't drain fast enough, floods;
   when the rain stops, the drain empties the water.   Tune the numbers in frameWalk (inflow / outflow).
   ============================================================ */
for(let x=X0;x<X0+XL;x+=9){flat(x,8,9.05,4.4,'wet',.6);flat(x,13.2,9.05,7,'wet',.6)}   /* strips: very wide elements get clipped by the browser */
flat(X0,12.4,XL,.4,'dwater',.6);flat(X0,12.4,XL,.4,'dflow',.8);
for(let i=0;i<18;i++)flat(R_(16,46),8,.07,4.4,'rvl',2.6,{animationDelay:-R_(0,1)+'s'});                       // rivulets running to the drain
[[19,8.5,2.2,1.1,.22],[27,8.8,2.6,1.2,.28],[34,8.4,2,1,.34],[41,8.9,2.4,1.1,.4],[23,11.3,3,.9,.78],[38,11.5,3.2,.9,.84],
 [20,13.4,3.4,.9,.2],[31,13.5,4,1,.3],[45,13.4,3.2,.9,.36],[28,17.6,3.8,1.6,.6],[40,15,3.4,1.5,.66]].forEach(([x,y,w,d,th])=>flat(x,y,w,d,'pud',2.8,{'--th':th}));
for(let i=0;i<80;i++)flat(R_(16,46),R_(8.4,19.6),.5,.5,'rp',3,{'--rk':R_(0,.9),animationDelay:-R_(0,1.2)+'s'});          // raindrop ripples
const rc=$('#rainc'),rx=rc.getContext('2d'),drops=[...Array(520)].map(()=>({x:Math.random(),y:Math.random(),z:Math.random()}));
function fitRain(){const d=Math.min(devicePixelRatio||1,2);rc.width=innerWidth*d;rc.height=innerHeight*d;rx.setTransform(d,0,0,d,0,0)}
let rainOn=false,rI=0,wl=0,wt=0,audio=null,lastVars={};
function rainAudio(){if(audio||!SETTINGS.rainSound)return;try{const A=new (window.AudioContext||window.webkitAudioContext)(),b=A.createBuffer(1,A.sampleRate*2,A.sampleRate),d=b.getChannelData(0);for(let i=0;i<d.length;i++)d[i]=Math.random()*2-1;
  const s=A.createBufferSource();s.buffer=b;s.loop=true;const hp=A.createBiquadFilter(),lp=A.createBiquadFilter(),g=A.createGain();hp.type='highpass';hp.frequency.value=500;lp.type='lowpass';lp.frequency.value=5000;g.gain.value=0;s.connect(hp);hp.connect(lp);lp.connect(g);g.connect(A.destination);s.start();audio={A,g}}catch(e){}}
function rainReset(){rainOn=false;rI=wl=wt=0;if(audio)audio.g.gain.value=0;$('#rainb').textContent='☔ Start rain';rx.clearRect(0,0,rc.width,rc.height)}
$('#rainb').onclick=()=>{rainOn=!rainOn;if(rainOn){rainAudio();audio&&audio.A.resume&&audio.A.resume()}$('#rainb').textContent=rainOn?'☀ Stop rain':'☔ Start rain'};
$('#rs').insertAdjacentHTML('beforeend','<span>Water <i id="n5"><u></u></i></span><span>Drain <b id="n6">Dry</b></span>');
/* ---- camera / day-night ---- */
let K=1,rzC=-4,walkDark=false;
function fitWorld(){K=Math.min(1.5,Math.max(.4,innerWidth/(28*M)))}
new MutationObserver(()=>{walkDark=document.documentElement.dataset.theme==='dark'}).observe(document.documentElement,{attributes:true,attributeFilter:['data-theme']});
walkDark=document.documentElement.dataset.theme==='dark';


/* ===== 11 · State + UI ===== */
let mode='dev',ex=false,cur=-1,tok=0,demoOn=false,hl=-1,yaw=.5,pitch=0,yawT=.5,pitchT=0,camD=14,camY=.9,steps=0,en=0,store=0,wp=0;
const pop=$('#pop'),tip=$('#tip'),hint=$('#hint'),cap=$('#cap'),kD=$('#kDemo');
const setEx=v=>{ex=v;const n=performance.now();PARTS.forEach((p,i)=>p.at=n+(v?9-i:i)*60)};
function render(){document.body.classList.toggle('pv',cur>=0);
  if(cur>=0){const p=PARTS[cur];$('#pn').textContent=`Part ${ORDER.indexOf(cur)+1} of ${ORDER.length}`;$('#pt').textContent=p.n;$('#pd').textContent=p.d;$('#ps').innerHTML=p.s.map(x=>`<span>${x}</span>`).join('');pop.classList.remove('pp');void pop.offsetWidth;pop.classList.add('pp','show')}else pop.classList.remove('show');
  kD.textContent=demoOn?SETTINGS.buttons.stopDemo:SETTINGS.buttons.demo;
  hint.textContent=(LOW?'Drag to rotate · ':'')+(ex?'Click or tap a part to see what it does':'Click or tap the device to split it')}
const say=t=>{cap.textContent=t||'';cap.classList.toggle('on',!!t)};
function stopDemo(){demoOn=false;foot.visible=bulbG.visible=bWire.o.visible=false;pulses.forEach(p=>p.visible=false);bulbL.intensity=0;MT.bulb.emissiveIntensity=0;MT.ceramic.emissive.setHex(0);hl=-1;say('');kD.textContent=SETTINGS.buttons.demo}
async function tour(){const k=++tok;stopDemo();mode='dev';setEx(true);cur=-1;render();await sleep(1700);pop.classList.add('tour');
  for(const i of ORDER){if(k!==tok)return;cur=i;render();const b=$('#pb i');b.style.animation='none';void b.offsetWidth;b.style.animation='pb 3.4s linear forwards';await sleep(3400)}
  if(k===tok){pop.classList.remove('tour');cur=-1;render()}}
const posOf=(x,u)=>x==='bulb'?bAnch.getWorldPosition(new THREE.Vector3()):x===9?PARTS[9].g.sA[u].getWorldPosition(new THREE.Vector3()):PARTS[x].units[u].getWorldPosition(new THREE.Vector3());
async function demo(){if(demoOn){tok++;stopDemo();render();return}
  const k=++tok;stopDemo();mode='dev';setEx(false);cur=-1;demoOn=true;foot.visible=bulbG.visible=bWire.o.visible=true;render();await sleep(900);
  const st=[[9,4,'Sunlight hits the unbreakable solar cells — they send DC straight to the 12 V battery.'],[0,2,'A footstep presses the cover onto the piezo discs, which give out a burst of AC voltage.'],[2,3,'The bridge rectifier turns the pulses into DC and charges the 4 V battery.'],[3,4,'The boost converter raises 4 V to 12 V.'],[4,5,'The 12 V battery stores the energy (solar charges it directly too).'],[5,'bulb','The inverter changes 12 V DC into 220 V AC and sends it to the LED bulb.']];
  for(const [a,b,t] of st){if(k!==tok)return;say(t);hl=a===9?9:a;const t0=performance.now();pulses.forEach((p,u)=>{p.visible=true;p.userData={a:posOf(a,u),b:posOf(b,u),t0}});await sleep(2500)}
  if(k!==tok)return;pulses.forEach(p=>p.visible=false);hl=-1;say('The LED bulb lights up — electricity from footsteps and sunlight!');MT.bulb.userData.on=1;await sleep(4500);if(k===tok){MT.bulb.userData.on=0;stopDemo();render()}}
const openWalk=()=>{tok++;stopDemo();mode='walk';setEx(false);cur=-1;render();document.body.classList.add('walk');$('#rv').classList.add('on');$('#cw').classList.add('on')};
const closeWalk=()=>{mode='dev';rainReset();document.body.classList.remove('walk');$('#rv').classList.remove('on');$('#cw').classList.remove('on')};
$('#kAsm').onclick=()=>{tok++;stopDemo();pop.classList.remove('tour');setEx(false);cur=-1;render()};
$('#kVid').onclick=tour;kD.onclick=demo;$('#kReal').onclick=openWalk;$('#rb').onclick=closeWalk;$('#x').onclick=()=>{tok++;pop.classList.remove('tour');cur=-1;render()};

/* ===== 12 · Pointer input ===== */
const ray=new THREE.Raycaster(),ndc=new THREE.Vector2();let down=null,drag=0,lx=0,ly=0,hov=null;
const pick=e=>{ndc.set(e.clientX/innerWidth*2-1,-(e.clientY/innerHeight)*2+1);ray.setFromCamera(ndc,cam);const h=ray.intersectObjects(dev.children,true).find(x=>x.object.userData.pi!=null);return h?h.object.userData.pi:-1};
gl.addEventListener('pointerdown',e=>{down={x:e.clientX,y:e.clientY,t:performance.now()};if(e.pointerType==='touch'){drag=1;lx=e.clientX;ly=e.clientY}});
addEventListener('pointerup',e=>{drag=0;if(!down||mode!=='dev')return;const m=Math.hypot(e.clientX-down.x,e.clientY-down.y);down=null;if(m>8||e.target!==gl)return;
  tok++;stopDemo();pop.classList.remove('tour');const i=pick(e);if(!ex){if(i>=0)setEx(true);cur=-1}else cur=i;render()});
addEventListener('pointermove',e=>{if(e.pointerType==='touch'){if(drag){yawT+=(e.clientX-lx)*.008;pitchT=Math.max(-.5,Math.min(.3,pitchT+(e.clientY-ly)*.004));lx=e.clientX;ly=e.clientY}return}
  yawT=(e.clientX/innerWidth-.5)*1.6+.4;pitchT=(e.clientY/innerHeight-.5)*.3;mx=e.clientX/innerWidth;hov=e;tip.style.transform=`translate(${e.clientX+14}px,${e.clientY+14}px)`});
let mx=.5;

/* ===== 13 · Frame loops ===== */
const ez=x=>x*x*(3-2*x);
const ss=(a,b,x)=>{x=Math.min(1,Math.max(0,(x-a)/(b-a)));return x*x*(3-2*x)};
function size(){fitWorld();fitRain();const w=innerWidth,h=innerHeight;R.setSize(w,h,false);cam.aspect=cam2.aspect=w/h;if(w>700)cam.setViewOffset(w,h,170,0,w,h);else cam.clearViewOffset();cam.updateProjectionMatrix();cam2.updateProjectionMatrix()}
addEventListener('resize',size);size();
function frameDev(dt,now){const kk=1-Math.exp(-dt*1000/SETTINGS.smoothness);
  yaw+=(yawT-yaw)*kk;pitch+=(pitchT-pitch)*kk;dev.rotation.y=yaw+(demoOn?Math.sin(now/2800)*.12:0);dev.rotation.x=pitch;dev.position.y=Math.sin(now/1300)*.05;
  let press=0;if(demoOn){const ph=(now/1000%2.6)/2.6,u=ss(.05,.3,ph)-ss(.62,.9,ph);foot.position.set(0,3.5-1.62*u,.3);foot.rotation.x=-.12*(1-u);press=ss(.85,1,u)}
  MT.ceramic.emissive.setHex(demoOn?0x38bdf8:0);MT.ceramic.emissiveIntensity=press*1.1;
  const on=MT.bulb.userData.on?1:0;MT.bulb.emissiveIntensity+=(on*2.2-MT.bulb.emissiveIntensity)*kk;bulbL.intensity=MT.bulb.emissiveIntensity*3;
  const ks=1-Math.exp(-dt/(SETTINGS.splitSpeed*.11));
  PARTS.forEach((p,i)=>{if(now>=p.at)p.cur+=((ex?1:0)-p.cur)*ks;p.g.position.y=p.y+p.cur*p.ex-(i>7?.05*press:0);const ts=cur===i?SETTINGS.partPop:1;p.g.scale.setScalar(p.g.scale.x+(ts-p.g.scale.x)*kk)});
  pulses.forEach(p=>{const d=p.userData;if(p.visible&&d.a){const t=Math.min(1,(now-d.t0)/2300);p.position.lerpVectors(d.a,d.b,ss(0,1,t))}});
  const f=Math.tan(cam.fov*Math.PI/360)*2,H=ex?7.2:3.8,asp=innerWidth/innerHeight,fw=innerWidth>700?(innerWidth-340)/innerWidth:1,fh=(innerHeight-300)/innerHeight;
  const D=Math.max(H/(f*Math.max(.35,fh)),7.6/(f*asp*fw))/SETTINGS.deviceSize*(demoOn?1.18:1)/(ex&&cur<0?SETTINGS.splitZoom:1)*(cur>=0?SETTINGS.selectedShrink:1);camD+=(D-camD)*kk;camY+=((ex?1.5:.95)-camY)*kk;
  cam.position.set(0,camD*.3+camY,camD*.95);cam.lookAt(0,camY,0);
  dev.updateMatrixWorld(true);updWires();
  const s=cur>=0?cur:hl;if(s>=0){bh.visible=true;bh.box.setFromObject(PARTS[s].g)}else bh.visible=false;
  if(hov&&ex&&!drag){const i=pick(hov);if(i>=0){tip.textContent=PARTS[i].n;tip.classList.add('on')}else tip.classList.remove('on');hov=null}else if(!ex)tip.classList.remove('on');
  R.toneMappingExposure=.95;R.render(sc,cam)}
const tc={};const setT=(k,v)=>{if(tc[k]!==v){tc[k]=v;$(k).textContent=v}},setW=(k,v)=>{if(tc[k]!==v){tc[k]=v;$(k).firstChild.style.width=v}};
function frameWalk(dt,now){let n=0;
  /* ---- rain physics: rain builds slowly · water level rises · the drain empties it ---- */
  rI+=((rainOn?1:0)-rI)*Math.min(1,dt*.22);if(!rainOn&&rI<.003)rI=0;
  const inflow=rI*.09,outflow=.05*Math.min(1,wl*2);wl=Math.min(1,Math.max(0,wl+(inflow-outflow)*dt));if(wl<.001&&inflow===0)wl=0;
  const damp=rI>.05||wl>.04;wt+=((damp?1:0)-wt)*Math.min(1,dt*(damp?.5:.05)),fl=wl>0?Math.min(1,wl*2):0;
  const V={'--ri':rI,'--wl':wl,'--wt':wt,'--fl':fl,'--nd':(walkDark?.5:0)+.2*rI};
  for(const k in V){const v=Math.round(V[k]*100)/100;if(lastVars[k]!==v){lastVars[k]=v;cw.style.setProperty(k,v)}}
  cw.classList.toggle('rn',rI>.3);if(audio)audio.g.gain.value=.16*rI;
  const um=rI>.3;
  ppl.forEach(p=>{const sp=p.v*(1+.25*rI);p.d+=dt*sp;p.x+=dt*sp*p.dir;if(p.x>52)p.x=8;if(p.x<8)p.x=52;
    const ph=p.d*2.3,sw=Math.sin(ph),c=Math.cos(ph),bob=c*c*3,dy=Math.sin(p.d*.35+p.ph0)*.12;p.cy=p.lane+dy;
    p.ln.u.style.transform=`rotate(${-sw*32}deg)`;p.ln.lo.style.transform=`rotate(${ez(Math.max(0,-c))*52}deg)`;
    p.lf.u.style.transform=`rotate(${sw*32}deg)`;p.lf.lo.style.transform=`rotate(${ez(Math.max(0,c))*52}deg)`;
    p.an.u.style.transform=um?'rotate(-20deg)':`rotate(${sw*26}deg)`;p.an.lo.style.transform=um?'rotate(-30deg)':'rotate(-18deg)';
    p.af.u.style.transform=`rotate(${-sw*26}deg)`;p.af.lo.style.transform='rotate(-18deg)';
    p.pf.style.transform=`rotateX(-90deg) translateY(${-bob}px) rotate(${(um?3:1.5)+sw*.8}deg) scaleX(${p.dir})`;p.root.style.transform=`translate3d(${(p.x*M).toFixed(2)}px,${(dy*M).toFixed(2)}px,0)`});
  cars.forEach(c=>{c.x+=dt*c.v*(1-.25*rI)*c.dir;if(c.x>58)c.x=2;if(c.x<2)c.x=58;c.r.style.transform=`translate3d(${(c.x*M).toFixed(2)}px,0,0)`});
  tiles.forEach(t=>{let pr=0;ppl.forEach(p=>{if(Math.abs(p.x-t.cx)<TS/2+.15&&Math.abs(p.cy-t.cy)<TS/2+.25)pr=1});if(pr!==t.was){t.was=pr;t.tq.classList.toggle('pr',!!pr);if(pr)steps++}n+=pr});
  const pw=n*2.4;en+=pw*dt;store=Math.min(1,Math.max(0,store+(pw*.08-.05)*dt));wp+=(store-wp)*(1-Math.exp(-dt*3));
  const lv=Math.max(wp,rI*.7);lamps.forEach(([h,pool])=>{h.style.setProperty('--lv',lv.toFixed(2));pool.style.opacity=(lv*(walkDark?1:.2)).toFixed(2)});
  setT('#n1',steps);setT('#n2',en.toFixed(1));setW('#n3',(wp*100).toFixed(0)+'%');setT('#n4',walkDark?'0.0':(7.4*(1-.7*rI)+Math.sin(now/900)*.3).toFixed(1));
  setW('#n5',(wl*100).toFixed(0)+'%');setT('#n6',wl>.85?'OVERFLOW':rainOn?(wl>.03?'Filling':'Dry'):(wl>.02?'Draining':'Dry'));
  /* ---- falling rain streaks ---- */
  if(rI>.004){const W_=innerWidth,H_=innerHeight,cnt=Math.ceil(drops.length*rI);rx.clearRect(0,0,W_,H_);rx.lineCap='round';
    for(let i=0;i<cnt;i++){const d=drops[i],len=10+d.z*34,spd=700+d.z*1000;d.y+=dt*spd/H_;d.x-=dt*spd*.16/W_;if(d.y>1){d.y=-.05;d.x=Math.random()*1.2}if(d.x<-.1)d.x=1.1;
      rx.strokeStyle=`rgba(215,232,255,${(.18+d.z*.45)*Math.min(1,rI*1.4)})`;rx.lineWidth=.6+d.z*1.3;rx.beginPath();const x=d.x*W_,y=d.y*H_;rx.moveTo(x,y);rx.lineTo(x-len*.16,y+len);rx.stroke()}}else if(lastVars.rain){rx.clearRect(0,0,innerWidth,innerHeight)}
  lastVars.rain=rI>.004;
  rzC+=(((mx-.5)*14-4+Math.sin(now/7000)*1.4)-rzC)*(1-Math.exp(-dt*2.2));
  wd.style.transform=`scale(${K}) rotateX(${(60+Math.sin(now/9000)*.8).toFixed(2)}deg) rotateZ(${rzC.toFixed(2)}deg) translate3d(${-30*M}px,${-10.9*M}px,0)`}

let last=performance.now(),acc=0,nf=0,sdt=.016;
function loop(now){requestAnimationFrame(loop);const dt=Math.min((now-last)/1000,.05);last=now;acc+=dt;nf++;
  if(acc>1.5){if(nf/acc<48&&PR>1){PR=Math.max(1,PR-.25);R.setPixelRatio(PR);size()}acc=0;nf=0}
  if(mode==='walk'){sdt+=(dt-sdt)*.15;frameWalk(sdt,now)}else frameDev(dt,now)}
document.title=SETTINGS.title+' | '+SETTINGS.teamName;$('#brand').textContent=SETTINGS.teamName;$('h1').textContent=SETTINGS.title;
$('#kAsm').textContent=SETTINGS.buttons.assemble;$('#kVid').textContent=SETTINGS.buttons.split;$('#kReal').textContent=SETTINGS.buttons.real;
render();setEx(true);requestAnimationFrame(t=>{last=t;loop(t)});setTimeout(()=>{if(!tok){setEx(false);render()}},1100);

</script>
</body>
</html>
