<html lang="en-CA">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>FreightForward Canada — Pitch Deck 2026</title>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,600;0,700;1,600;1,700&family=DM+Sans:wght@300;400;500;600&family=DM+Mono:wght@300;400;500&display=swap" rel="stylesheet">
<style>
:root{
  --void:#060807;--ink:#0b0f0d;--panel:#111815;--raised:#162019;
  --border:#1e2b25;--border2:#263830;
  --gold:#d4a843;--gold2:#eec96a;--gold3:#f9e8b8;--gold-d:#8a6820;
  --maple:#c8392b;--maple2:#e85c49;
  --teal:#1fb899;--teal2:#3dd9bc;
  --sky:#3a7bd5;--sky2:#6ba0f0;
  --violet:#7c5cbf;--violet2:#a87fe8;
  --fog:#e2ebe4;--mist:#8fa898;--haze:#455c4e;--smoke:#1e2e28;
  --serif:'Cormorant Garamond',Georgia,serif;
  --sans:'DM Sans',sans-serif;
  --mono:'DM Mono',monospace;
}
*,*::before,*::after{margin:0;padding:0;box-sizing:border-box;}
html{font-size:15px;scroll-behavior:smooth;}
body{font-family:var(--sans);background:var(--void);color:var(--fog);overflow-x:hidden;-webkit-font-smoothing:antialiased;}
::-webkit-scrollbar{width:4px;}::-webkit-scrollbar-track{background:var(--void);}::-webkit-scrollbar-thumb{background:var(--border2);border-radius:2px;}

/* PROGRESS */
#pb{position:fixed;top:0;left:0;height:2px;background:linear-gradient(90deg,var(--gold-d),var(--gold),var(--gold2));z-index:9999;width:0;transition:width .15s;}

/* NAV */
.nav{position:fixed;top:0;left:0;right:0;z-index:800;display:flex;align-items:center;justify-content:space-between;padding:0 52px;height:62px;background:rgba(6,8,7,.85);backdrop-filter:blur(24px) saturate(1.4);border-bottom:1px solid rgba(255,255,255,.04);}
.nav-logo{display:flex;align-items:center;gap:11px;cursor:pointer;}
.nav-mono{width:34px;height:34px;border-radius:7px;background:linear-gradient(140deg,var(--gold-d),var(--gold));display:flex;align-items:center;justify-content:center;font-family:var(--serif);font-size:18px;font-weight:700;color:var(--void);}
.nav-name{font-family:var(--serif);font-size:17px;font-weight:700;color:var(--gold2);letter-spacing:.2px;}
.nav-sub{font-family:var(--mono);font-size:8px;color:var(--haze);letter-spacing:1.5px;text-transform:uppercase;}
.nav-pills{display:flex;gap:3px;}
.np{padding:5px 12px;border-radius:20px;font-size:12px;font-weight:500;color:var(--mist);cursor:pointer;transition:all .2s;border:1px solid transparent;letter-spacing:.2px;}
.np:hover{color:var(--fog);background:rgba(255,255,255,.04);}
.np.on{color:var(--gold2);background:rgba(212,168,67,.08);border-color:rgba(212,168,67,.22);}
.nav-cta{padding:9px 22px;background:var(--gold);color:var(--void);border-radius:8px;font-size:13px;font-weight:600;cursor:pointer;border:none;transition:all .2s;font-family:var(--sans);}
.nav-cta:hover{background:var(--gold2);transform:translateY(-1px);box-shadow:0 8px 24px rgba(212,168,67,.25);}

/* SECTIONS */
.s{min-height:100svh;position:relative;display:flex;flex-direction:column;justify-content:center;overflow:hidden;}
.si{max-width:1240px;margin:0 auto;width:100%;padding:96px 52px 76px;}

/* EYEBROWS */
.eb{display:inline-flex;align-items:center;gap:10px;font-family:var(--mono);font-size:10px;letter-spacing:2.5px;text-transform:uppercase;color:var(--gold);margin-bottom:20px;}
.eb::before{content:'';width:28px;height:1px;background:var(--gold);display:block;}
.eb.teal{color:var(--teal2);} .eb.teal::before{background:var(--teal2);}
.eb.sky{color:var(--sky2);} .eb.sky::before{background:var(--sky2);}
.eb.violet{color:var(--violet2);} .eb.violet::before{background:var(--violet2);}
.eb.maple{color:var(--maple2);} .eb.maple::before{background:var(--maple2);}

/* TYPE */
.th{font-family:var(--serif);font-size:clamp(52px,8vw,100px);font-weight:700;line-height:.92;letter-spacing:-3px;color:var(--fog);}
.th em{color:var(--gold2);font-style:italic;}
.txl{font-family:var(--serif);font-size:clamp(36px,5vw,66px);font-weight:700;line-height:1.0;letter-spacing:-1.5px;color:var(--fog);}
.txl em{color:var(--gold2);font-style:italic;}
.tlg{font-family:var(--serif);font-size:clamp(24px,3vw,40px);font-weight:700;line-height:1.1;letter-spacing:-.5px;color:var(--fog);}
.lead{font-size:16.5px;color:var(--mist);line-height:1.75;font-weight:300;max-width:680px;}
.lead strong{color:var(--fog);font-weight:600;}

/* BG VARIANTS */
.bg-void{background:var(--void);}
.bg-ink{background:var(--ink);}
.bg-gold-aura{background:radial-gradient(ellipse 85% 65% at 60% 35%,rgba(212,168,67,.07) 0%,transparent 65%),radial-gradient(ellipse 50% 50% at 10% 80%,rgba(31,184,153,.04) 0%,transparent 50%),var(--void);}
.bg-teal-aura{background:radial-gradient(ellipse 70% 60% at 80% 20%,rgba(31,184,153,.08) 0%,transparent 60%),radial-gradient(ellipse 50% 60% at 15% 70%,rgba(212,168,67,.04) 0%,transparent 55%),var(--ink);}
.bg-sky-aura{background:radial-gradient(ellipse 80% 70% at 20% 30%,rgba(58,123,213,.08) 0%,transparent 60%),radial-gradient(ellipse 40% 50% at 85% 70%,rgba(124,92,191,.06) 0%,transparent 50%),var(--void);}
.bg-maple-aura{background:radial-gradient(ellipse 70% 60% at 75% 25%,rgba(200,57,43,.07) 0%,transparent 60%),radial-gradient(ellipse 50% 40% at 10% 75%,rgba(212,168,67,.04) 0%,transparent 50%),var(--ink);}
.bg-violet-aura{background:radial-gradient(ellipse 70% 60% at 50% 40%,rgba(124,92,191,.08) 0%,transparent 65%),var(--void);}

/* CARDS */
.card{background:var(--panel);border:1px solid var(--border);border-radius:14px;overflow:hidden;transition:border-color .3s,transform .3s;}
.card:hover{border-color:var(--border2);}
.card-p{padding:26px;}
.gcard{background:var(--panel);border:1px solid var(--border);border-radius:14px;overflow:hidden;position:relative;}
.gcard::after{content:'';position:absolute;bottom:0;left:0;right:0;height:2px;}
.gcard.gold::after{background:linear-gradient(90deg,transparent,var(--gold),transparent);}
.gcard.teal::after{background:linear-gradient(90deg,transparent,var(--teal2),transparent);}
.gcard.sky::after{background:linear-gradient(90deg,transparent,var(--sky2),transparent);}
.gcard.maple::after{background:linear-gradient(90deg,transparent,var(--maple2),transparent);}
.gcard.violet::after{background:linear-gradient(90deg,transparent,var(--violet2),transparent);}

/* GRIDS */
.g2{display:grid;grid-template-columns:1fr 1fr;gap:20px;}
.g3{display:grid;grid-template-columns:repeat(3,1fr);gap:18px;}
.g4{display:grid;grid-template-columns:repeat(4,1fr);gap:14px;}
.g5{display:grid;grid-template-columns:repeat(5,1fr);gap:12px;}
.gcol60{display:grid;grid-template-columns:1fr .65fr;gap:56px;align-items:start;}
.gcol50{display:grid;grid-template-columns:1fr 1fr;gap:48px;align-items:center;}
.gcol40{display:grid;grid-template-columns:.65fr 1fr;gap:56px;align-items:start;}

/* KPI BLOCK */
.kpi-block{display:grid;grid-template-columns:repeat(4,1fr);gap:1px;background:var(--border);border:1px solid var(--border);border-radius:14px;overflow:hidden;margin-top:48px;}
.kpi-cell{background:var(--panel);padding:26px 22px;position:relative;}
.kpi-cell::before{content:'';position:absolute;top:0;left:0;right:0;height:2px;}
.kpi-cell:nth-child(1)::before{background:var(--gold);}
.kpi-cell:nth-child(2)::before{background:var(--teal2);}
.kpi-cell:nth-child(3)::before{background:var(--maple2);}
.kpi-cell:nth-child(4)::before{background:var(--sky2);}
.kpi-num{font-family:var(--serif);font-size:42px;font-weight:700;line-height:1;margin-bottom:6px;}
.kpi-lbl{font-size:13px;color:var(--mist);line-height:1.4;}
.kpi-src{font-family:var(--mono);font-size:9px;color:var(--haze);margin-top:7px;letter-spacing:.5px;}

/* STAT RIBBON */
.srib{display:flex;gap:32px;padding:24px 0;border-top:1px solid var(--border);margin-top:36px;}
.srib-v{font-family:var(--serif);font-size:32px;font-weight:700;color:var(--gold2);line-height:1;}
.srib-l{font-size:12px;color:var(--haze);margin-top:4px;}

/* FEATURE CARDS */
.fc{background:var(--panel);border:1px solid var(--border);border-radius:13px;padding:26px;transition:all .3s;position:relative;overflow:hidden;}
.fc:hover{border-color:rgba(212,168,67,.3);transform:translateY(-3px);box-shadow:0 24px 56px rgba(0,0,0,.45);}
.fc-icon{font-size:28px;margin-bottom:13px;display:block;}
.fc-title{font-family:var(--serif);font-size:18px;font-weight:700;color:var(--fog);margin-bottom:8px;line-height:1.2;}
.fc-body{font-size:13.5px;color:var(--mist);line-height:1.7;}
.fc-tag{display:inline-block;margin-top:12px;padding:2px 9px;border-radius:4px;font-family:var(--mono);font-size:9.5px;letter-spacing:1px;text-transform:uppercase;}
.fc-tag.gold{background:rgba(212,168,67,.1);border:1px solid rgba(212,168,67,.2);color:var(--gold2);}
.fc-tag.teal{background:rgba(31,184,153,.1);border:1px solid rgba(31,184,153,.2);color:var(--teal2);}
.fc-tag.sky{background:rgba(58,123,213,.1);border:1px solid rgba(58,123,213,.2);color:var(--sky2);}
.fc-tag.maple{background:rgba(200,57,43,.1);border:1px solid rgba(200,57,43,.2);color:var(--maple2);}
.fc-tag.violet{background:rgba(124,92,191,.1);border:1px solid rgba(124,92,191,.2);color:var(--violet2);}

/* TABLE */
.ptbl{width:100%;border-collapse:collapse;}
.ptbl th{padding:11px 16px;font-family:var(--mono);font-size:9px;letter-spacing:1.8px;text-transform:uppercase;color:var(--haze);border-bottom:1px solid var(--border);text-align:left;background:var(--raised);}
.ptbl td{padding:13px 16px;font-size:13.5px;color:var(--mist);border-bottom:1px solid var(--border);line-height:1.5;vertical-align:middle;}
.ptbl tr:last-child td{border-bottom:none;}
.ptbl tr:hover td{background:rgba(212,168,67,.02);}
.td-h{color:var(--fog);font-weight:600;}
.td-us{color:var(--teal2);}
.td-bad{color:var(--maple2);}
.td-neutral{color:var(--haze);}
.td-mono{font-family:var(--mono);font-size:12px;}

/* STEPS */
.steps{display:flex;flex-direction:column;}
.step{display:flex;gap:20px;padding:20px 0;border-bottom:1px solid var(--border);}
.step:last-child{border-bottom:none;}
.step-n{font-family:var(--serif);font-size:48px;font-weight:700;color:rgba(212,168,67,.12);line-height:1;width:52px;flex-shrink:0;transition:color .3s;}
.step:hover .step-n{color:rgba(212,168,67,.35);}
.step-title{font-family:var(--serif);font-size:18px;font-weight:700;color:var(--fog);margin-bottom:5px;}
.step-body{font-size:13.5px;color:var(--mist);line-height:1.65;}

/* PULL QUOTES */
.pq{padding:20px 26px;border-left:3px solid var(--gold);background:rgba(212,168,67,.04);border-radius:0 10px 10px 0;margin:28px 0;}
.pq em{font-family:var(--serif);font-size:18px;font-style:italic;color:var(--fog);line-height:1.55;display:block;margin-bottom:8px;}
.pq-src{font-family:var(--mono);font-size:9.5px;color:var(--haze);letter-spacing:1.2px;text-transform:uppercase;}

/* CHECKLIST */
.checks{display:flex;flex-direction:column;gap:11px;}
.chk{display:flex;align-items:flex-start;gap:11px;font-size:14px;color:var(--mist);line-height:1.6;}
.chk-dot{width:19px;height:19px;border-radius:50%;background:rgba(212,168,67,.1);border:1px solid rgba(212,168,67,.25);display:flex;align-items:center;justify-content:center;flex-shrink:0;margin-top:2px;font-size:9px;color:var(--gold);}
.chk strong{color:var(--fog);}

/* AI CARDS */
.ai-card{background:var(--panel);border:1px solid var(--border);border-radius:13px;padding:24px;position:relative;overflow:hidden;transition:all .3s;}
.ai-card::before{content:'';position:absolute;top:-60px;right:-60px;width:160px;height:160px;border-radius:50%;background:radial-gradient(circle,rgba(124,92,191,.07) 0%,transparent 70%);pointer-events:none;}
.ai-card:hover{border-color:rgba(124,92,191,.35);transform:translateY(-2px);}
.ai-big{font-family:var(--serif);font-size:46px;font-weight:700;color:var(--violet2);line-height:1;margin-bottom:7px;}
.ai-title{font-size:14px;font-weight:600;color:var(--fog);margin-bottom:5px;}
.ai-desc{font-size:13px;color:var(--mist);line-height:1.6;}
.ai-chip{display:inline-flex;align-items:center;gap:5px;margin-top:11px;padding:3px 9px;border-radius:20px;font-family:var(--mono);font-size:9px;letter-spacing:1px;text-transform:uppercase;background:rgba(124,92,191,.1);border:1px solid rgba(124,92,191,.22);color:var(--violet2);}

/* H-BARS */
.hbars{display:flex;flex-direction:column;gap:12px;}
.hb{display:flex;align-items:center;gap:11px;}
.hb-lbl{font-size:13px;color:var(--mist);width:168px;flex-shrink:0;line-height:1.3;}
.hb-track{flex:1;height:5px;background:var(--border2);border-radius:3px;overflow:hidden;}
.hb-fill{height:100%;border-radius:3px;}
.hb-val{font-family:var(--mono);font-size:11px;color:var(--haze);width:56px;text-align:right;flex-shrink:0;}

/* V-BARS */
.vbars{display:flex;align-items:flex-end;gap:10px;}
.vb{flex:1;display:flex;flex-direction:column;align-items:center;gap:7px;justify-content:flex-end;}
.vb-bar{width:100%;border-radius:5px 5px 0 0;position:relative;}
.vb-top{position:absolute;top:-22px;left:50%;transform:translateX(-50%);font-family:var(--mono);font-size:9.5px;color:var(--haze);white-space:nowrap;}
.vb-lbl{font-family:var(--mono);font-size:9px;color:var(--haze);text-align:center;letter-spacing:.5px;line-height:1.3;}

/* TIMELINE */
.tlv{display:flex;flex-direction:column;padding-left:20px;border-left:1px solid var(--border);}
.tli{position:relative;padding-bottom:26px;padding-left:22px;}
.tli:last-child{padding-bottom:0;}
.tli-dot{position:absolute;left:-9px;top:4px;width:16px;height:16px;border-radius:50%;background:var(--panel);border:2px solid var(--gold);display:flex;align-items:center;justify-content:center;}
.tli-in{width:6px;height:6px;border-radius:50%;background:var(--gold);}
.tli-yr{font-family:var(--mono);font-size:10px;color:var(--gold);letter-spacing:1.5px;text-transform:uppercase;margin-bottom:5px;}
.tli-title{font-family:var(--serif);font-size:17px;font-weight:700;color:var(--fog);margin-bottom:4px;}
.tli-body{font-size:13px;color:var(--mist);line-height:1.6;}

/* PILLS */
.pills{display:flex;flex-wrap:wrap;gap:8px;}
.pill{padding:4px 13px;border-radius:20px;font-family:var(--mono);font-size:11px;font-weight:500;}
.p-gold{background:rgba(212,168,67,.1);border:1px solid rgba(212,168,67,.22);color:var(--gold2);}
.p-teal{background:rgba(31,184,153,.09);border:1px solid rgba(31,184,153,.2);color:var(--teal2);}
.p-sky{background:rgba(58,123,213,.09);border:1px solid rgba(58,123,213,.2);color:var(--sky2);}
.p-violet{background:rgba(124,92,191,.09);border:1px solid rgba(124,92,191,.2);color:var(--violet2);}
.p-maple{background:rgba(200,57,43,.09);border:1px solid rgba(200,57,43,.2);color:var(--maple2);}

/* DIVIDER */
.sdiv{width:100%;height:1px;background:linear-gradient(90deg,transparent,var(--border2) 30%,var(--border2) 70%,transparent);margin:48px 0;}

/* HIGHLIGHT BLOCKS */
.hb-block{border-radius:13px;padding:26px 28px;position:relative;overflow:hidden;}
.hb-gold{background:rgba(212,168,67,.06);border:1px solid rgba(212,168,67,.18);}
.hb-teal{background:rgba(31,184,153,.06);border:1px solid rgba(31,184,153,.16);}
.hb-sky{background:rgba(58,123,213,.06);border:1px solid rgba(58,123,213,.16);}
.hb-maple{background:rgba(200,57,43,.06);border:1px solid rgba(200,57,43,.16);}
.hb-violet{background:rgba(124,92,191,.06);border:1px solid rgba(124,92,191,.16);}

/* SECTOR CARDS */
.sc{background:var(--panel);border:1px solid var(--border);border-radius:11px;padding:18px;text-align:center;transition:all .25s;}
.sc:hover{border-color:rgba(212,168,67,.25);background:var(--raised);transform:translateY(-2px);}
.sc-icon{font-size:24px;margin-bottom:8px;}
.sc-name{font-family:var(--serif);font-size:14px;font-weight:700;color:var(--fog);margin-bottom:3px;}
.sc-desc{font-size:11.5px;color:var(--haze);line-height:1.5;}

/* TESTIMONIALS */
.testi{background:var(--panel);border:1px solid var(--border);border-radius:13px;padding:26px;position:relative;overflow:hidden;}
.testi-q{font-family:var(--serif);font-size:68px;color:var(--gold);opacity:.18;line-height:1;position:absolute;top:6px;left:16px;}
.testi-text{font-family:var(--serif);font-style:italic;font-size:15.5px;color:var(--fog);line-height:1.6;padding-top:22px;margin-bottom:14px;}
.testi-auth{font-family:var(--mono);font-size:9.5px;color:var(--haze);letter-spacing:1.2px;text-transform:uppercase;}

/* PROCESS FLOW */
.pflow{display:flex;gap:0;position:relative;margin-top:32px;}
.pflow::before{content:'';position:absolute;top:30px;left:5%;right:5%;height:1px;background:linear-gradient(90deg,transparent,var(--border2) 20%,var(--border2) 80%,transparent);}
.pf-s{flex:1;text-align:center;padding:0 10px;position:relative;}
.pf-dot{width:18px;height:18px;border-radius:50%;background:var(--panel);border:2px solid var(--gold);margin:0 auto 13px;position:relative;z-index:1;display:flex;align-items:center;justify-content:center;}
.pf-in{width:6px;height:6px;border-radius:50%;background:var(--gold);}
.pf-lbl{font-family:var(--mono);font-size:9.5px;color:var(--gold);letter-spacing:1.5px;text-transform:uppercase;margin-bottom:5px;}
.pf-title{font-family:var(--serif);font-size:14px;font-weight:700;color:var(--fog);margin-bottom:4px;}
.pf-desc{font-size:11.5px;color:var(--mist);line-height:1.5;}

/* SECTION INDEX */
.sidx{font-family:var(--serif);font-size:160px;font-weight:700;color:rgba(212,168,67,.025);position:absolute;right:48px;top:50%;transform:translateY(-50%);line-height:1;pointer-events:none;user-select:none;}

/* SCROLL REVEAL */
.reveal{opacity:0;transform:translateY(26px);transition:opacity .72s cubic-bezier(.16,1,.3,1),transform .72s cubic-bezier(.16,1,.3,1);}
.reveal.in{opacity:1;transform:translateY(0);}

/* BUTTONS */
.btn-p{display:inline-flex;align-items:center;gap:9px;padding:15px 42px;background:var(--gold);color:var(--void);border-radius:10px;font-size:15px;font-weight:600;cursor:pointer;transition:all .3s;border:none;font-family:var(--sans);}
.btn-p:hover{background:var(--gold2);transform:translateY(-3px);box-shadow:0 20px 56px rgba(212,168,67,.22);}
.btn-o{display:inline-flex;align-items:center;gap:9px;padding:15px 42px;background:transparent;color:var(--gold2);border-radius:10px;font-size:15px;font-weight:500;cursor:pointer;transition:all .3s;border:1px solid rgba(212,168,67,.28);font-family:var(--sans);}
.btn-o:hover{background:rgba(212,168,67,.06);}

/* CTA SECTION */
.cta-wrap{min-height:85vh;display:flex;flex-direction:column;align-items:center;justify-content:center;text-align:center;padding:100px 52px;background:radial-gradient(ellipse 80% 80% at 50% 50%,rgba(212,168,67,.07) 0%,transparent 70%),var(--ink);position:relative;overflow:hidden;}
.cta-ring{position:absolute;border-radius:50%;border:1px solid rgba(212,168,67,.06);pointer-events:none;}

/* FOOTER */
footer{background:var(--void);border-top:1px solid var(--border);padding:32px 52px;display:flex;align-items:center;justify-content:space-between;}
.ft-logo{font-family:var(--serif);font-size:18px;font-weight:700;color:var(--gold2);}
.ft-copy{font-family:var(--mono);font-size:10px;color:var(--haze);text-align:center;line-height:1.6;}

@media(max-width:1100px){
  .gcol60,.gcol40,.gcol50{grid-template-columns:1fr;gap:32px;}
  .g2,.g3{grid-template-columns:1fr 1fr;}
  .g4,.g5{grid-template-columns:1fr 1fr;}
  .kpi-block{grid-template-columns:1fr 1fr;}
  .si{padding:90px 28px 70px;}
  .nav{padding:0 28px;}
  .nav-pills{display:none;}
}
@media(max-width:700px){
  .g2,.g3,.g4,.g5{grid-template-columns:1fr;}
  .kpi-block{grid-template-columns:1fr 1fr;}
  .srib{flex-wrap:wrap;gap:20px;}
  .pflow{flex-direction:column;}
  .pflow::before{display:none;}
}
</style>
</head>
<body>
<div id="pb"></div>

<!-- NAV -->
<nav class="nav" id="main-nav">
  <div class="nav-logo" onclick="sTo('s-hero')">
    <div class="nav-mono">FF</div>
    <div><div class="nav-name">FreightForward Canada</div><div class="nav-sub">🍁 Brant, ON · CTA Licensed · Est. 2025</div></div>
  </div>
  <div class="nav-pills">
    <div class="np on" onclick="sTo('s-hero',this)">Overview</div>
    <div class="np" onclick="sTo('s-market',this)">Market</div>
    <div class="np" onclick="sTo('s-services',this)">Services</div>
    <div class="np" onclick="sTo('s-value',this)">Value</div>
    <div class="np" onclick="sTo('s-ai',this)">AI & Tech</div>
    <div class="np" onclick="sTo('s-future',this)">Future</div>
    <div class="np" onclick="sTo('s-why',this)">Why Us</div>
    <div class="np" onclick="sTo('s-roadmap',this)">Roadmap</div>
  </div>
  <button class="nav-cta" onclick="openModal('consultation')">Book Consultation →</button>
</nav>

<!-- ═══════════ SLIDE 01: HERO ═══════════ -->
<section class="s bg-gold-aura" id="s-hero">
  <canvas id="route-canvas" style="position:absolute;inset:0;width:100%;height:100%;opacity:.3;pointer-events:none;"></canvas>
  <div class="si" style="position:relative;z-index:1;">
    <div class="gcol60" style="align-items:center;">
      <div>
        <div class="eb" style="margin-bottom:24px;">🍁 Canadian Freight Brokerage · Investor &amp; Client Pitch 2026</div>
        <h1 class="th">Moving<br>Canada<br><em>Forward.</em></h1>
        <p class="lead" style="margin-top:26px;max-width:560px;">A <strong>premium freight brokerage</strong> purpose-built for the Canadian market — connecting shippers to a vetted carrier network of 247+, with cross-border expertise, compliance-first operations, and technology that delivers certainty at scale.</p>
        <div class="srib">
          <div><div class="srib-v">$82B</div><div class="srib-l">Canadian freight market</div></div>
          <div style="width:1px;background:var(--border)"></div>
          <div><div class="srib-v">247+</div><div class="srib-l">Vetted carrier partners</div></div>
          <div style="width:1px;background:var(--border)"></div>
          <div><div class="srib-v" style="color:var(--teal2)">96.2%</div><div class="srib-l">On-time delivery rate</div></div>
          <div style="width:1px;background:var(--border)"></div>
          <div><div class="srib-v" style="color:var(--maple2)">&lt;2 hrs</div><div class="srib-l">Avg carrier match</div></div>
        </div>
        <div style="display:flex;gap:12px;margin-top:30px;flex-wrap:wrap;">
          <button class="btn-p" onclick="openModal('consultation')">Book a Consultation →</button>
          <button class="btn-o" onclick="sTo('s-services')">Our Services</button>
        </div>
      </div>

      <!-- HERO CARD -->
      <div>
        <div class="card" style="border-color:var(--border2);">
          <div style="background:var(--raised);padding:13px 18px;border-bottom:1px solid var(--border);display:flex;align-items:center;justify-content:space-between;">
            <div style="font-family:var(--mono);font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--haze);">🟢 Live Network</div>
            <div style="font-family:var(--mono);font-size:9px;color:var(--teal2);letter-spacing:1px;">AscendTMS · Synced</div>
          </div>
          <div style="padding:18px;">
            <div style="background:var(--raised);border:1px solid var(--border);border-radius:10px;height:155px;position:relative;overflow:hidden;margin-bottom:14px;">
              <svg viewBox="0 0 320 135" style="position:absolute;inset:0;width:100%;height:100%;">
                <line x1="0" y1="67" x2="320" y2="67" stroke="#1e2b25" stroke-width="1"/>
                <line x1="160" y1="0" x2="160" y2="135" stroke="#1e2b25" stroke-width="1"/>
                <path d="M58,50 Q100,36 142,50" fill="none" stroke="#d4a843" stroke-width="1.5" stroke-dasharray="4,3" opacity=".6"/>
                <path d="M142,50 Q198,42 250,65" fill="none" stroke="#d4a843" stroke-width="1.5" stroke-dasharray="4,3" opacity=".45"/>
                <path d="M58,50 Q80,82 102,88" fill="none" stroke="#1fb899" stroke-width="1" stroke-dasharray="3,3" opacity=".5"/>
                <path d="M142,50 Q128,90 102,88" fill="none" stroke="#3a7bd5" stroke-width="1" stroke-dasharray="3,3" opacity=".4"/>
                <path d="M250,65 Q260,95 248,105" fill="none" stroke="#a87fe8" stroke-width="1" stroke-dasharray="3,3" opacity=".35"/>
                <circle r="3" fill="#d4a843" opacity=".9"><animateMotion dur="3s" repeatCount="indefinite" path="M58,50 Q100,36 142,50 Q198,42 250,65"/></circle>
                <circle r="2.5" fill="#1fb899" opacity=".9"><animateMotion dur="4.5s" repeatCount="indefinite" begin=".8s" path="M250,65 Q198,42 142,50 Q100,36 58,50"/></circle>
                <circle r="2" fill="#6ba0f0" opacity=".8"><animateMotion dur="5s" repeatCount="indefinite" begin="2s" path="M58,50 Q80,82 102,88"/></circle>
                <circle cx="58" cy="50" r="5.5" fill="#d4a843" opacity=".9"/>
                <circle cx="58" cy="50" r="10" fill="none" stroke="#d4a843" stroke-width="1" opacity=".3"><animate attributeName="r" values="8;14;8" dur="2s" repeatCount="indefinite"/><animate attributeName="opacity" values=".3;0;.3" dur="2s" repeatCount="indefinite"/></circle>
                <circle cx="142" cy="50" r="4.5" fill="#1fb899" opacity=".9"/>
                <circle cx="142" cy="50" r="9" fill="none" stroke="#1fb899" stroke-width="1" opacity=".3"><animate attributeName="r" values="7;13;7" dur="2.5s" repeatCount="indefinite"/><animate attributeName="opacity" values=".3;0;.3" dur="2.5s" repeatCount="indefinite"/></circle>
                <circle cx="250" cy="65" r="4" fill="#e85c49" opacity=".9"/>
                <circle cx="102" cy="88" r="3.5" fill="#6ba0f0" opacity=".8"/>
                <circle cx="248" cy="105" r="3" fill="#a87fe8" opacity=".7"/>
                <text x="44" y="43" fill="#d4a843" font-size="7" font-family="DM Mono,monospace">Toronto</text>
                <text x="128" y="43" fill="#1fb899" font-size="7" font-family="DM Mono,monospace">Calgary</text>
                <text x="236" y="59" fill="#e85c49" font-size="7" font-family="DM Mono,monospace">Detroit</text>
                <text x="82" y="103" fill="#6ba0f0" font-size="7" font-family="DM Mono,monospace">Montréal</text>
                <text x="232" y="118" fill="#a87fe8" font-size="7" font-family="DM Mono,monospace">Windsor</text>
              </svg>
            </div>
            <div style="display:grid;grid-template-columns:1fr 1fr 1fr;gap:8px;">
              <div style="background:var(--raised);border:1px solid var(--border);border-radius:7px;padding:10px;text-align:center;"><div style="font-family:var(--serif);font-size:19px;font-weight:700;color:var(--gold2);">148</div><div style="font-family:var(--mono);font-size:8px;color:var(--haze);text-transform:uppercase;letter-spacing:1px;margin-top:2px;">Active Loads</div></div>
              <div style="background:var(--raised);border:1px solid var(--border);border-radius:7px;padding:10px;text-align:center;"><div style="font-family:var(--serif);font-size:19px;font-weight:700;color:var(--teal2);">$384K</div><div style="font-family:var(--mono);font-size:8px;color:var(--haze);text-transform:uppercase;letter-spacing:1px;margin-top:2px;">Rev MTD·CAD</div></div>
              <div style="background:var(--raised);border:1px solid var(--border);border-radius:7px;padding:10px;text-align:center;"><div style="font-family:var(--serif);font-size:19px;font-weight:700;color:var(--maple2);">18.4%</div><div style="font-family:var(--mono);font-size:8px;color:var(--haze);text-transform:uppercase;letter-spacing:1px;margin-top:2px;">Gross Margin</div></div>
            </div>
          </div>
        </div>
        <div style="margin-top:12px;background:rgba(212,168,67,.06);border:1px solid rgba(212,168,67,.15);border-radius:10px;padding:13px 16px;display:flex;align-items:center;gap:11px;">
          <div style="font-size:18px;">🍁</div>
          <div><div style="font-family:var(--serif);font-size:14px;font-weight:700;color:var(--gold2);">CTA Licensed · CVOR Verified · CBSA Certified</div><div style="font-size:12px;color:var(--haze);margin-top:2px;">All 10 Canadian provinces · Canada–US cross-border specialists</div></div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ═══════════ SLIDE 02: MARKET INTELLIGENCE ═══════════ -->
<section class="s bg-teal-aura" id="s-market">
  <div class="sidx">02</div>
  <div class="si">
    <div class="eb teal">Industry Intelligence</div>
    <div class="gcol50" style="margin-bottom:48px;gap:64px;">
      <div>
        <h2 class="txl">The Canadian Freight Market Is <em>Massive</em> — And Still Underserved.</h2>
        <p class="lead" style="margin-top:18px;">Canada moves <strong>600M+ tonnes of freight</strong> annually. Trucking and logistics represents nearly <strong>7% of GDP</strong>. Yet brokerage penetration sits at only 28% — seven full points behind the United States. That gap is not a statistic. It's an opportunity worth billions.</p>
        <div class="pq" style="border-left-color:var(--teal2);">
          <em>"Canada's supply chain is at an inflection point. Brokers who invest in technology and relationships now will define the freight landscape of 2030."</em>
          <div class="pq-src">Canadian Supply Chain Sector Council · 2025 Outlook Report</div>
        </div>
      </div>
      <div>
        <div class="kpi-block" style="grid-template-columns:1fr 1fr;margin-top:0;border-radius:12px;">
          <div class="kpi-cell"><div class="kpi-num" style="color:var(--gold2);font-size:36px;">$82B</div><div class="kpi-lbl">Canadian freight market (2025)</div><div class="kpi-src">CTA Annual Report</div></div>
          <div class="kpi-cell"><div class="kpi-num" style="color:var(--teal2);font-size:36px;">3.8%</div><div class="kpi-lbl">YoY market growth — outpacing GDP</div><div class="kpi-src">Transport Canada 2025</div></div>
          <div class="kpi-cell"><div class="kpi-num" style="color:var(--maple2);font-size:36px;">23K+</div><div class="kpi-lbl">Unfilled driver positions in Canada</div><div class="kpi-src">CTA Driver Shortage Report</div></div>
          <div class="kpi-cell"><div class="kpi-num" style="color:var(--sky2);font-size:36px;">28%</div><div class="kpi-lbl">Brokerage penetration vs 35% in USA</div><div class="kpi-src">Industry est. 2025</div></div>
        </div>
        <div style="margin-top:14px;display:grid;grid-template-columns:1fr 1fr;gap:10px;">
          <div class="hb-block hb-gold" style="padding:16px 18px;"><div style="font-family:var(--serif);font-size:26px;font-weight:700;color:var(--gold2);">$800B+</div><div style="font-size:12px;color:var(--mist);margin-top:4px;">Annual Canada–US bilateral trade under CUSMA</div></div>
          <div class="hb-block hb-teal" style="padding:16px 18px;"><div style="font-family:var(--serif);font-size:26px;font-weight:700;color:var(--teal2);">$1.3T</div><div style="font-size:12px;color:var(--mist);margin-top:4px;">Combined North American freight market (USD)</div></div>
        </div>
      </div>
    </div>

    <div class="sdiv"></div>

    <h3 class="tlg reveal" style="margin-bottom:24px;">Four Forces Reshaping Canadian Freight Right Now</h3>
    <div class="g4 reveal">
      <div class="gcard gold"><div class="card-p"><div style="font-size:24px;margin-bottom:11px;">🚚</div><div style="font-family:var(--serif);font-size:16px;font-weight:700;color:var(--fog);margin-bottom:7px;">Driver Shortage Crisis</div><div style="font-size:13px;color:var(--mist);line-height:1.6;">23,000+ unfilled driving positions. When capacity tightens, brokers with deep carrier relationships become <strong style="color:var(--fog)">essential, not optional</strong>. Shippers without broker access face 30–50% spot rate premiums.</div></div></div>
      <div class="gcard maple"><div class="card-p"><div style="font-size:24px;margin-bottom:11px;">⛽</div><div style="font-family:var(--serif);font-size:16px;font-weight:700;color:var(--fog);margin-bottom:7px;">Carbon Tax Escalation</div><div style="font-size:13px;color:var(--mist);line-height:1.6;">Canada's carbon price reaches <strong style="color:var(--fog)">$170/tonne by 2030</strong>, adding ~$0.09/L to diesel. Optimized routing and load consolidation through brokers directly reduce carrier fuel surcharges — measurable savings every load.</div></div></div>
      <div class="gcard sky"><div class="card-p"><div style="font-size:24px;margin-bottom:11px;">🌐</div><div style="font-family:var(--serif);font-size:16px;font-weight:700;color:var(--fog);margin-bottom:7px;">US Tariff Volatility</div><div style="font-size:13px;color:var(--mist);line-height:1.6;">Cross-border trade under CUSMA review is driving Canadian shippers to diversify routing. Brokers with <strong style="color:var(--fog)">deep CBSA expertise</strong> are commanding premium long-term relationships as companies restructure their supply chains.</div></div></div>
      <div class="gcard teal"><div class="card-p"><div style="font-size:24px;margin-bottom:11px;">📦</div><div style="font-family:var(--serif);font-size:16px;font-weight:700;color:var(--fog);margin-bottom:7px;">E-Commerce Surge</div><div style="font-size:13px;color:var(--mist);line-height:1.6;">Canadian e-commerce grew <strong style="color:var(--fog)">14% in 2024</strong>. LTL and last-mile demand is surging in ON, BC, and QC — markets largely underserved by small brokerages. The window to establish LTL expertise is open now.</div></div></div>
    </div>

    <div class="sdiv"></div>

    <div class="gcol50 reveal">
      <div>
        <h3 class="tlg" style="margin-bottom:20px;">Market Size by Corridor (CAD)</h3>
        <div class="hbars">
          <div class="hb"><div class="hb-lbl">Ontario → Alberta</div><div class="hb-track"><div class="hb-fill" style="width:100%;background:linear-gradient(90deg,var(--gold-d),var(--gold2));"></div></div><div class="hb-val">$21B</div></div>
          <div class="hb"><div class="hb-lbl">Canada–US Cross-Border</div><div class="hb-track"><div class="hb-fill" style="width:86%;background:linear-gradient(90deg,var(--maple),var(--maple2));"></div></div><div class="hb-val">$18B</div></div>
          <div class="hb"><div class="hb-lbl">Ontario → Quebec</div><div class="hb-track"><div class="hb-fill" style="width:67%;background:linear-gradient(90deg,var(--sky),var(--sky2));"></div></div><div class="hb-val">$14B</div></div>
          <div class="hb"><div class="hb-lbl">BC Port → Interior</div><div class="hb-track"><div class="hb-fill" style="width:57%;background:linear-gradient(90deg,var(--teal),var(--teal2));"></div></div><div class="hb-val">$12B</div></div>
          <div class="hb"><div class="hb-lbl">Prairie Grain Corridors</div><div class="hb-track"><div class="hb-fill" style="width:43%;background:linear-gradient(90deg,var(--violet),var(--violet2));"></div></div><div class="hb-val">$9B</div></div>
          <div class="hb"><div class="hb-lbl">Atlantic Canada Routes</div><div class="hb-track"><div class="hb-fill" style="width:21%;background:var(--haze);"></div></div><div class="hb-val">$4.5B</div></div>
        </div>
      </div>
      <div>
        <h3 class="tlg" style="margin-bottom:20px;">Why Now Is the Moment</h3>
        <div class="checks">
          <div class="chk"><div class="chk-dot">✦</div><div><strong>28% → 38% penetration forecast:</strong> Canadian shipper adoption of broker services is projected to reach 38% by 2028 as digitization accelerates — representing $8B+ in new brokerable freight annually.</div></div>
          <div class="chk"><div class="chk-dot">✦</div><div><strong>Technology democratization:</strong> AI and TMS platforms like AscendTMS have levelled the playing field — boutique brokers can now out-execute legacy players on speed, compliance, and service quality.</div></div>
          <div class="chk"><div class="chk-dot">✦</div><div><strong>Quebec underserved:</strong> Canada's second-largest freight market is dramatically underserved by bilingual brokerages — a first-mover advantage worth $65M+ annually in the ON–QC corridor alone.</div></div>
          <div class="chk"><div class="chk-dot">✦</div><div><strong>Nearshoring wave incoming:</strong> US tariff instability is driving manufacturing reshoring to Ontario and Quebec. New Canadian industrial capacity needs freight partners. We are positioned to capture this wave.</div></div>
          <div class="chk"><div class="chk-dot">✦</div><div><strong>Quality premium in market:</strong> After years of pandemic-era disruptions, shippers are prioritizing <em>reliable, compliant</em> broker relationships over cheap spot-market gambles. Quality commands premium contracts.</div></div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ═══════════ SLIDE 03: SERVICES ═══════════ -->
<section class="s bg-ink" id="s-services">
  <div class="sidx">03</div>
  <div class="si">
    <div class="eb">Services &amp; Solutions</div>
    <div class="gcol50" style="margin-bottom:52px;gap:72px;">
      <div>
        <h2 class="txl">Every Load. Every Lane. <em>Every Time.</em></h2>
        <p class="lead" style="margin-top:18px;">From full truckloads on the Quebec–Ontario corridor to time-sensitive cross-border reefer shipments through Windsor–Detroit, we engineer freight solutions that <strong>reduce cost, eliminate complexity, and deliver certainty</strong>.</p>
        <div class="srib" style="margin-top:26px;padding-top:26px;">
          <div><div class="srib-v">10/10</div><div class="srib-l">Provinces covered</div></div>
          <div style="width:1px;background:var(--border)"></div>
          <div><div class="srib-v" style="color:var(--teal2)">247+</div><div class="srib-l">Vetted carriers</div></div>
          <div style="width:1px;background:var(--border)"></div>
          <div><div class="srib-v" style="color:var(--maple2)">96.2%</div><div class="srib-l">On-time rate</div></div>
        </div>
      </div>
      <div>
        <div class="hb-block hb-gold">
          <div style="font-family:var(--mono);font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--gold);margin-bottom:16px;">Service Performance Snapshot</div>
          <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;">
            <div><div style="font-family:var(--serif);font-size:22px;font-weight:700;color:var(--gold2);">&lt;30 min</div><div style="font-size:11.5px;color:var(--mist);margin-top:2px;">Rate quote turnaround</div></div>
            <div><div style="font-family:var(--serif);font-size:22px;font-weight:700;color:var(--gold2);">&lt;2 hrs</div><div style="font-size:11.5px;color:var(--mist);margin-top:2px;">Carrier match for spot loads</div></div>
            <div><div style="font-family:var(--serif);font-size:22px;font-weight:700;color:var(--gold2);">$2M+</div><div style="font-size:11.5px;color:var(--mist);margin-top:2px;">Min cargo insurance per carrier</div></div>
            <div><div style="font-family:var(--serif);font-size:22px;font-weight:700;color:var(--teal2);">0</div><div style="font-size:11.5px;color:var(--mist);margin-top:2px;">CBSA violations on record</div></div>
          </div>
        </div>
      </div>
    </div>

    <div class="g3 reveal">
      <div class="fc"><span class="fc-icon">🚛</span><div class="fc-title">Full Truckload (FTL)</div><div class="fc-body">Dedicated capacity for high-volume shipments — dry van 53', flatbed 48'/53', step deck, B-train, Super-B. Single-lane contract lanes to one-time spot loads. Preferred carrier relationships ensure priority access when markets tighten.</div><div class="fc-tag gold">Domestic · Cross-Border</div></div>
      <div class="fc"><span class="fc-icon">📦</span><div class="fc-title">Less-Than-Truckload (LTL)</div><div class="fc-body">Cost-optimized solutions for smaller shipments. Access to Day &amp; Ross, TForce Freight, Polaris Transport, and regional Canadian LTL carriers — consolidated pricing, full tracking, guaranteed transit windows across Canada.</div><div class="fc-tag teal">Cost Optimization</div></div>
      <div class="fc"><span class="fc-icon">❄️</span><div class="fc-title">Temperature-Controlled</div><div class="fc-body">Reefer and controlled-temp logistics for food, pharma, and agriculture. CFIA and FSEP-compliant carriers. Continuous monitoring from pickup through delivery — critical for food-grade and pharmaceutical cold chain compliance.</div><div class="fc-tag maple">CFIA · CGMP</div></div>
      <div class="fc"><span class="fc-icon">🛃</span><div class="fc-title">Cross-Border Canada–US</div><div class="fc-body">Full CBSA/CBP workflow management — PARS/PAPS filing, ACI e-manifest, CUSMA/USMCA origin certificates, customs broker coordination, FAST-lane carriers at Windsor–Detroit, Sarnia–Port Huron, Fort Erie–Buffalo, Pacific Hwy.</div><div class="fc-tag sky">CBSA · CUSMA</div></div>
      <div class="fc"><span class="fc-icon">🏗️</span><div class="fc-title">Heavy &amp; Specialized</div><div class="fc-body">Oversized, overweight, and specialized freight requiring provincial permits, pilot vehicles, and route surveys. Lowboy, multi-axle, and heavy haul logistics for construction, oil &amp; gas, and industrial sectors across Alberta and Ontario.</div><div class="fc-tag gold">Permit-Managed</div></div>
      <div class="fc"><span class="fc-icon">🚂</span><div class="fc-title">Intermodal (Rail + Truck)</div><div class="fc-body">Long-haul ON–AB and ON–BC lanes via CN and CP Rail intermodal networks. Combined rail + drayage from Brampton Intermodal Terminal and Calgary Logistics Park. Up to 35% lower cost and 60% fewer emissions vs. pure over-road.</div><div class="fc-tag violet">Launching Q4 2026</div></div>
    </div>

    <div class="sdiv"></div>
    <h3 class="tlg reveal" style="margin-bottom:22px;">Value-Added Services — Included in Every Partnership</h3>
    <div class="g4 reveal" style="gap:12px;">
      <div style="background:var(--panel);border:1px solid var(--border);border-radius:12px;padding:20px;transition:all .25s;" onmouseover="this.style.borderColor='rgba(31,184,153,.35)'" onmouseout="this.style.borderColor='var(--border)'"><div style="font-size:22px;margin-bottom:10px;">📡</div><div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--fog);margin-bottom:6px;">Real-Time Tracking</div><div style="font-size:13px;color:var(--mist);line-height:1.55;">GPS visibility every load. Proactive delay alerts. Customer-facing portal — no more calling carriers for updates.</div></div>
      <div style="background:var(--panel);border:1px solid var(--border);border-radius:12px;padding:20px;transition:all .25s;" onmouseover="this.style.borderColor='rgba(31,184,153,.35)'" onmouseout="this.style.borderColor='var(--border)'"><div style="font-size:22px;margin-bottom:10px;">📋</div><div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--fog);margin-bottom:6px;">Document Management</div><div style="font-size:13px;color:var(--mist);line-height:1.55;">BOL, POD, PARS/PAPS, CVOR files — all digitized and archived. CRA audit-ready and accessible anytime.</div></div>
      <div style="background:var(--panel);border:1px solid var(--border);border-radius:12px;padding:20px;transition:all .25s;" onmouseover="this.style.borderColor='rgba(31,184,153,.35)'" onmouseout="this.style.borderColor='var(--border)'"><div style="font-size:22px;margin-bottom:10px;">🤝</div><div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--fog);margin-bottom:6px;">Dedicated Account Broker</div><div style="font-size:13px;color:var(--mist);line-height:1.55;">One person. One number. No tickets, no call centres. Direct broker access every day, every load.</div></div>
      <div style="background:var(--panel);border:1px solid var(--border);border-radius:12px;padding:20px;transition:all .25s;" onmouseover="this.style.borderColor='rgba(31,184,153,.35)'" onmouseout="this.style.borderColor='var(--border)'"><div style="font-size:22px;margin-bottom:10px;">📊</div><div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--fog);margin-bottom:6px;">Monthly Freight Reports</div><div style="font-size:13px;color:var(--mist);line-height:1.55;">Spend analysis, lane benchmarks, carrier scorecards, and ESG emissions summaries for corporate sustainability reporting.</div></div>
    </div>

    <div class="sdiv"></div>
    <h3 class="tlg reveal" style="margin-bottom:36px;">How It Works — Quote to Delivery</h3>
    <div class="pflow reveal">
      <div class="pf-s"><div class="pf-dot"><div class="pf-in"></div></div><div class="pf-lbl">Step 01</div><div class="pf-title">Request a Rate</div><div class="pf-desc">Call, email, or portal. Origin, destination, equipment, weight, dates, special requirements — we capture everything.</div></div>
      <div class="pf-s"><div class="pf-dot" style="border-color:var(--teal2)"><div class="pf-in" style="background:var(--teal2)"></div></div><div class="pf-lbl" style="color:var(--teal2)">Step 02</div><div class="pf-title">Quote in &lt;30 Min</div><div class="pf-desc">Live Loadlink market data, carrier availability check, and an all-in competitive rate — with full transparency.</div></div>
      <div class="pf-s"><div class="pf-dot" style="border-color:var(--sky2)"><div class="pf-in" style="background:var(--sky2)"></div></div><div class="pf-lbl" style="color:var(--sky2)">Step 03</div><div class="pf-title">Carrier Matched</div><div class="pf-desc">CVOR/NSC-verified, insured, performance-rated carrier confirmed in under 2 hours. Rate confirmation sent to both parties.</div></div>
      <div class="pf-s"><div class="pf-dot" style="border-color:var(--violet2)"><div class="pf-in" style="background:var(--violet2)"></div></div><div class="pf-lbl" style="color:var(--violet2)">Step 04</div><div class="pf-title">Active Monitoring</div><div class="pf-desc">Check-calls, GPS tracking, CBSA coordination for cross-border loads, and proactive delay alerts throughout transit.</div></div>
      <div class="pf-s"><div class="pf-dot" style="border-color:var(--maple2)"><div class="pf-in" style="background:var(--maple2)"></div></div><div class="pf-lbl" style="color:var(--maple2)">Step 05</div><div class="pf-title">POD + Invoice</div><div class="pf-desc">Digital POD confirmation, CAD invoice, and carrier payment processed. QuickBooks Canada integrated seamlessly.</div></div>
    </div>
  </div>
</section>

<!-- ═══════════ SLIDE 04: VALUE PROPOSITION ═══════════ -->
<section class="s bg-maple-aura" id="s-value">
  <div class="sidx">04</div>
  <div class="si">
    <div class="eb maple">High-Ticket Value Proposition</div>
    <h2 class="txl" style="max-width:820px;margin-bottom:18px;">We Don't Just Move Freight. We <em>Protect Your Business.</em></h2>
    <p class="lead" style="margin-bottom:48px;max-width:720px;">In a market where a single late delivery can trigger a <strong>$50,000 chargeback</strong>, where a carrier with a suspended Safety Fitness Certificate exposes you to <strong>direct liability</strong>, and where manual freight management costs your team <strong>8+ hours a week</strong> — the right broker isn't a cost. It's protection.</p>

    <div class="gcol50" style="gap:40px;margin-bottom:48px;">
      <div>
        <div class="hb-block hb-gold" style="margin-bottom:16px;">
          <div style="font-family:var(--mono);font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--gold);margin-bottom:16px;">💰 Real Cost Comparison — $500K Annual Freight Spend (CAD)</div>
          <table class="ptbl">
            <thead><tr><th>Cost Category</th><th>Managing In-House</th><th style="color:var(--teal2)">With FreightForward CA</th></tr></thead>
            <tbody>
              <tr><td class="td-h">Rate Overpayment</td><td class="td-bad">+$90K avg above market</td><td class="td-us">Market rate + volume leverage</td></tr>
              <tr><td class="td-h">Staff Admin Time</td><td class="td-bad">$26K/yr (10 hrs/wk)</td><td class="td-us">Fully managed — included</td></tr>
              <tr><td class="td-h">CBSA Fine Exposure</td><td class="td-bad">$5K–$25K per incident</td><td class="td-us">Zero incidents on record</td></tr>
              <tr><td class="td-h">Technology Costs</td><td class="td-bad">$12K/yr (TMS, Loadlink)</td><td class="td-us">Included in service</td></tr>
              <tr><td class="td-h">Unvetted Carrier Claims</td><td class="td-bad">High exposure, no visibility</td><td class="td-us">$2M+ insured, vetted only</td></tr>
            </tbody>
          </table>
          <div style="margin-top:14px;padding:12px 14px;background:rgba(31,184,153,.08);border:1px solid rgba(31,184,153,.18);border-radius:8px;text-align:center;">
            <div style="font-family:var(--serif);font-size:28px;font-weight:700;color:var(--teal2);">$128K+ Annual Savings</div>
            <div style="font-size:12px;color:var(--mist);margin-top:3px;">Conservative estimate for a shipper at $500K annual freight spend</div>
          </div>
        </div>
      </div>

      <div>
        <h3 class="tlg" style="margin-bottom:20px;">5 Reasons High-Value Shippers Choose Us</h3>
        <div class="steps">
          <div class="step"><div class="step-n">01</div><div><div class="step-title">Compliance You Can't Afford to Skip</div><div class="step-body">Every carrier carries verified CVOR (Ontario), valid NSC, WSIB clearance, and $2M+ cargo insurance. If a carrier's Safety Fitness Certificate lapses, they're removed before they touch your freight. We absorb the liability so you don't.</div></div></div>
          <div class="step"><div class="step-n">02</div><div><div class="step-title">Capacity Guaranteed When It Counts</div><div class="step-body">When spot rates spike 30% and capacity evaporates, preferred carrier relationships give your freight priority access. We have maintained 100% load coverage through peak seasons, blizzards, and border slowdowns.</div></div></div>
          <div class="step"><div class="step-n">03</div><div><div class="step-title">Cross-Border Expertise That's Rare</div><div class="step-body">CBSA, PARS/PAPS, ACI e-manifest, CUSMA origin certification, HS tariff classification — we manage the full customs workflow. Most Canadian regional brokers cannot do this. It is our specialization.</div></div></div>
          <div class="step"><div class="step-n">04</div><div><div class="step-title">Proactive — Not Reactive — Communication</div><div class="step-body">You hear from us before you need to call. Check-calls logged, delay alerts sent, ETA updates pushed, delivery confirmations issued as standard. A proactive partnership, never a reactive service.</div></div></div>
          <div class="step" style="border-bottom:none;"><div class="step-n">05</div><div><div class="step-title">Radical Transparency on Every Transaction</div><div class="step-body">You see our buy rate, sell rate, and margin. No hidden markups. No bait-and-switch carriers. We operate with full transparency because our business depends on your long-term trust, not single transactions.</div></div></div>
        </div>
      </div>
    </div>

    <div class="sdiv"></div>
    <h3 class="tlg reveal" style="margin-bottom:22px;">Industries We Serve Across Canada</h3>
    <div class="g5 reveal" style="gap:11px;">
      <div class="sc"><div class="sc-icon">🌾</div><div class="sc-name">Agriculture</div><div class="sc-desc">Grain, produce, livestock, agri-chemicals across the Prairies and into the US</div></div>
      <div class="sc"><div class="sc-icon">🏭</div><div class="sc-name">Manufacturing</div><div class="sc-desc">Auto parts, steel, plastics — Ontario &amp; Quebec manufacturing corridors</div></div>
      <div class="sc"><div class="sc-icon">🛒</div><div class="sc-name">Retail &amp; E-Comm</div><div class="sc-desc">FTL &amp; LTL for major retailers. DTC fulfillment networks coast to coast</div></div>
      <div class="sc"><div class="sc-icon">🛢️</div><div class="sc-name">Energy &amp; Resources</div><div class="sc-desc">Oil &amp; gas equipment, pipeline components, mining — Alberta &amp; beyond</div></div>
      <div class="sc"><div class="sc-icon">🏗️</div><div class="sc-name">Construction</div><div class="sc-desc">Flatbed, oversized, heavy haul — materials and equipment across provinces</div></div>
      <div class="sc"><div class="sc-icon">💊</div><div class="sc-name">Pharma &amp; Health</div><div class="sc-desc">Temperature-controlled, CGMP-compliant pharmaceutical freight</div></div>
      <div class="sc"><div class="sc-icon">🌲</div><div class="sc-name">Forestry &amp; Lumber</div><div class="sc-desc">BC and Quebec lumber, pulp &amp; paper — from mill to market, export-ready</div></div>
      <div class="sc"><div class="sc-icon">🍷</div><div class="sc-name">Food &amp; Beverage</div><div class="sc-desc">CFIA-compliant cold chain. Food-grade carriers. Processor to distributor</div></div>
      <div class="sc"><div class="sc-icon">🚢</div><div class="sc-name">Port Import/Export</div><div class="sc-desc">Vancouver &amp; Halifax drayage — ocean freight to inland Canada</div></div>
      <div class="sc"><div class="sc-icon">🖥️</div><div class="sc-name">Technology &amp; IT</div><div class="sc-desc">High-value electronics, white-glove handling, secured freight protocols</div></div>
    </div>
  </div>
</section>

<!-- ═══════════ SLIDE 05: AI & TECHNOLOGY ═══════════ -->
<section class="s bg-violet-aura" id="s-ai">
  <div class="sidx" style="color:rgba(124,92,191,.04)">05</div>
  <div class="si">
    <div class="eb violet">Artificial Intelligence &amp; Technology</div>
    <h2 class="txl" style="max-width:840px;margin-bottom:18px;">AI Is Reshaping the Global Supply Chain. <em>We're Already Using It.</em></h2>
    <p class="lead" style="margin-bottom:44px;max-width:760px;">Artificial intelligence is no longer a future promise in logistics — it's an <strong>operational competitive advantage today</strong>. From dynamic pricing engines to predictive disruption alerts, AI is compressing the time between supply chain problems and their solutions from days to <strong>minutes</strong>. The brokers who adopt it now will own the decade.</p>

    <div class="gcol50" style="gap:40px;margin-bottom:48px;">
      <div class="hb-block hb-violet">
        <div style="font-family:var(--mono);font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--violet2);margin-bottom:14px;">Global AI in Logistics — By the Numbers</div>
        <div style="font-family:var(--serif);font-size:60px;font-weight:700;color:var(--violet2);line-height:1;margin-bottom:10px;">$141B</div>
        <div style="font-size:14px;color:var(--mist);line-height:1.6;margin-bottom:14px;">Projected global AI-in-logistics market by 2030, growing at <strong style="color:var(--fog)">42% CAGR</strong>. Freight brokerages with AI tools are reporting 20–35% operating cost reduction within 18 months of adoption.</div>
        <div style="display:grid;grid-template-columns:1fr 1fr 1fr;gap:12px;margin-top:6px;">
          <div style="text-align:center;"><div style="font-family:var(--serif);font-size:26px;font-weight:700;color:var(--violet2);">40%</div><div style="font-size:11px;color:var(--haze);margin-top:3px;">Empty mile reduction via AI routing</div></div>
          <div style="text-align:center;border-left:1px solid var(--border);border-right:1px solid var(--border);padding:0 8px;"><div style="font-family:var(--serif);font-size:26px;font-weight:700;color:var(--violet2);">94%</div><div style="font-size:11px;color:var(--haze);margin-top:3px;">ETA accuracy with ML prediction</div></div>
          <div style="text-align:center;"><div style="font-family:var(--serif);font-size:26px;font-weight:700;color:var(--violet2);">3.2×</div><div style="font-size:11px;color:var(--haze);margin-top:3px;">Faster carrier vetting with AI</div></div>
        </div>
        <div style="margin-top:14px;font-family:var(--mono);font-size:9px;color:var(--haze);">Sources: McKinsey Global Institute 2024 · Gartner Supply Chain · Accenture Freight AI Study</div>
      </div>

      <div>
        <h3 class="tlg" style="margin-bottom:18px;">How AI Transforms Freight Brokerage</h3>
        <div class="checks">
          <div class="chk"><div class="chk-dot" style="background:rgba(124,92,191,.1);border-color:rgba(124,92,191,.25);color:var(--violet2);">✦</div><div><strong>Dynamic Rate Pricing:</strong> AI engines analyzing 10,000+ real-time data points — Loadlink market data, DAT Canada, fuel prices, weather, carrier availability — generate optimal rates in milliseconds. Every quote is market-intelligent.</div></div>
          <div class="chk"><div class="chk-dot" style="background:rgba(124,92,191,.1);border-color:rgba(124,92,191,.25);color:var(--violet2);">✦</div><div><strong>Predictive ETAs:</strong> ML models trained on Canadian road conditions, border wait times, HOS regulations, and seasonal patterns deliver 94% accurate delivery windows — versus 71% for manual estimates.</div></div>
          <div class="chk"><div class="chk-dot" style="background:rgba(124,92,191,.1);border-color:rgba(124,92,191,.25);color:var(--violet2);">✦</div><div><strong>Carrier Risk Scoring:</strong> Automated CVOR/NSC monitoring, safety score trending, insurance expiry alerts, and claims history analysis flag at-risk carriers automatically before they cause a problem.</div></div>
          <div class="chk"><div class="chk-dot" style="background:rgba(124,92,191,.1);border-color:rgba(124,92,191,.25);color:var(--violet2);">✦</div><div><strong>Demand Forecasting:</strong> AI-powered freight demand modeling helps key shippers plan capacity 4–8 weeks ahead, reducing spot market dependence by up to 40% and locking in favourable contract rates.</div></div>
          <div class="chk"><div class="chk-dot" style="background:rgba(124,92,191,.1);border-color:rgba(124,92,191,.25);color:var(--violet2);">✦</div><div><strong>Document Automation:</strong> NLP-powered tools extract, validate, and file BOLs, PARS/PAPS submissions, and CUSMA certificates in seconds — eliminating manual entry errors and CBSA customs delays entirely.</div></div>
          <div class="chk"><div class="chk-dot" style="background:rgba(124,92,191,.1);border-color:rgba(124,92,191,.25);color:var(--violet2);">✦</div><div><strong>Route &amp; Load Optimization:</strong> AI-generated load plans reduce empty miles by an average of 28%, directly cutting carrier costs and providing measurable Scope 3 carbon reduction for shipper ESG reporting.</div></div>
        </div>
      </div>
    </div>

    <div class="g4 reveal">
      <div class="ai-card"><div class="ai-big">40%</div><div class="ai-title">Empty Mile Reduction</div><div class="ai-desc">AI-optimized load matching eliminates backhaul waste — one of the largest hidden cost drivers in Canadian trucking. Less empty running means lower carrier costs passed directly to shippers.</div><div class="ai-chip">🤖 Route Optimization AI</div></div>
      <div class="ai-card"><div class="ai-big">$23B</div><div class="ai-title">Annual Freight Inefficiency (Canada)</div><div class="ai-desc">Estimated annual waste from suboptimal routing, overcapacity, and manual errors across Canadian freight. AI-driven brokerage directly attacks this number for every shipper we serve.</div><div class="ai-chip">📊 Efficiency Intelligence</div></div>
      <div class="ai-card"><div class="ai-big">94%</div><div class="ai-title">ML ETA Accuracy</div><div class="ai-desc">Machine learning delivery predictions trained on Canadian roads, border wait data, and HOS regulations — critical for JIT manufacturing, grocery, and pharmaceutical cold chains where late means lost revenue.</div><div class="ai-chip">⏱️ Predictive Logistics</div></div>
      <div class="ai-card"><div class="ai-big">4 hrs</div><div class="ai-title">Carrier Onboarding (was 2 days)</div><div class="ai-desc">Automated NSC/CVOR lookups, insurance verification APIs, and risk-scoring algorithms reduce carrier onboarding from 2 days to under 4 hours without sacrificing compliance quality or depth of vetting.</div><div class="ai-chip">🛡 Compliance Automation</div></div>
    </div>

    <div class="sdiv"></div>

    <div class="gcol50 reveal" style="gap:48px;">
      <div>
        <h3 class="tlg" style="margin-bottom:22px;">Our AI Technology Stack</h3>
        <div style="display:flex;flex-direction:column;gap:11px;">
          <div style="display:flex;gap:13px;padding:15px;background:var(--panel);border:1px solid var(--border);border-radius:10px;border-left:3px solid var(--teal2);">
            <div style="font-size:20px;flex-shrink:0">🧠</div>
            <div style="flex:1"><div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--fog);margin-bottom:3px;">AscendTMS + AI Load Matching</div><div style="font-size:12.5px;color:var(--mist);">Integrated carrier suggestions based on lane performance, cost history, and live availability. Automated rate confirmations and BOL generation.</div></div>
            <div style="flex-shrink:0;align-self:center;"><span class="pill p-teal" style="font-size:9px;">Active Now</span></div>
          </div>
          <div style="display:flex;gap:13px;padding:15px;background:var(--panel);border:1px solid var(--border);border-radius:10px;border-left:3px solid var(--gold);">
            <div style="font-size:20px;flex-shrink:0">💰</div>
            <div style="flex:1"><div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--fog);margin-bottom:3px;">Dynamic Rate Engine (Loadlink + DAT Canada)</div><div style="font-size:12.5px;color:var(--mist);">Real-time market pricing to optimize every quote — maximizing margin in soft markets and winning competitively in tight ones.</div></div>
            <div style="flex-shrink:0;align-self:center;"><span class="pill p-gold" style="font-size:9px;">Q3 2026</span></div>
          </div>
          <div style="display:flex;gap:13px;padding:15px;background:var(--panel);border:1px solid var(--border);border-radius:10px;border-left:3px solid var(--violet2);">
            <div style="font-size:20px;flex-shrink:0">📄</div>
            <div style="flex:1"><div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--fog);margin-bottom:3px;">NLP Document Automation</div><div style="font-size:12.5px;color:var(--mist);">AI-powered extraction and auto-population of BOLs, PARS/PAPS, CUSMA certificates — eliminating manual entry and CBSA filing errors entirely.</div></div>
            <div style="flex-shrink:0;align-self:center;"><span class="pill p-violet" style="font-size:9px;">Q2 2026</span></div>
          </div>
          <div style="display:flex;gap:13px;padding:15px;background:var(--panel);border:1px solid var(--border);border-radius:10px;border-left:3px solid var(--sky2);">
            <div style="font-size:20px;flex-shrink:0">🔮</div>
            <div style="flex:1"><div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--fog);margin-bottom:3px;">Freight Demand Forecasting</div><div style="font-size:12.5px;color:var(--mist);">ML models predicting shipper demand 4–8 weeks ahead for proactive carrier booking and contract pricing for strategic accounts.</div></div>
            <div style="flex-shrink:0;align-self:center;"><span class="pill p-sky" style="font-size:9px;">2027</span></div>
          </div>
          <div style="display:flex;gap:13px;padding:15px;background:var(--panel);border:1px solid var(--border);border-radius:10px;border-left:3px solid var(--maple2);">
            <div style="font-size:20px;flex-shrink:0">🌿</div>
            <div style="flex:1"><div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--fog);margin-bottom:3px;">Carbon Emissions Tracking (Scope 3)</div><div style="font-size:12.5px;color:var(--mist);">Per-load CO₂ calculation aligned with Transport Canada's emissions framework. Load-level ESG data for corporate sustainability reports and TSX disclosure requirements.</div></div>
            <div style="flex-shrink:0;align-self:center;"><span class="pill p-maple" style="font-size:9px;">Q3 2026</span></div>
          </div>
        </div>
      </div>

      <div>
        <h3 class="tlg" style="margin-bottom:22px;">AI's Role in the Global Supply Chain</h3>
        <div style="display:flex;flex-direction:column;gap:14px;">
          <div class="hb-block hb-violet" style="padding:20px 22px;">
            <div style="font-family:var(--serif);font-size:17px;font-weight:700;color:var(--violet2);margin-bottom:6px;">AI Control Tower Technology</div>
            <div style="font-size:13px;color:var(--mist);line-height:1.6;">Fortune 500 companies deploy AI control towers monitoring 200,000+ supply chain nodes in real time, automatically rerouting freight when disruptions are detected — hours before human operators would notice. This technology is cascading down to mid-market brokers now.</div>
          </div>
          <div class="hb-block hb-sky" style="padding:20px 22px;">
            <div style="font-family:var(--serif);font-size:17px;font-weight:700;color:var(--sky2);margin-bottom:6px;">Autonomous Vehicle Integration</div>
            <div style="font-size:13px;color:var(--mist);line-height:1.6;">Waymo Via, Aurora, and TuSimple are deploying semi-autonomous long-haul trucks across North American routes. AI brokers will be first to integrate autonomous capacity into load boards, creating cost advantages unavailable to traditional operators.</div>
          </div>
          <div class="hb-block hb-teal" style="padding:20px 22px;">
            <div style="font-family:var(--serif);font-size:17px;font-weight:700;color:var(--teal2);margin-bottom:6px;">Blockchain &amp; Digital Customs</div>
            <div style="font-size:13px;color:var(--mist);line-height:1.6;">CBSA's Single Window Initiative and blockchain-based trade documentation are reducing cross-border processing times by up to 60%. Brokers with digital-first customs workflows will clear cargo faster and command shipper loyalty.</div>
          </div>
        </div>
        <div class="pq" style="margin-top:20px;border-left-color:var(--violet2);">
          <em>"By 2027, freight brokers without AI-enabled pricing and carrier matching will lose 30–40% of competitive deals to tech-forward competitors."</em>
          <div class="pq-src">Gartner Supply Chain Technology Report · 2024</div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ═══════════ SLIDE 06: FUTURE OF LOGISTICS ═══════════ -->
<section class="s bg-sky-aura" id="s-future">
  <div class="sidx" style="color:rgba(58,123,213,.04)">06</div>
  <div class="si">
    <div class="eb sky">The Future of Logistics</div>
    <h2 class="txl" style="max-width:840px;margin-bottom:18px;">The Next Decade Will Reshape How Canada <em>Moves Its Goods.</em></h2>
    <p class="lead" style="margin-bottom:48px;max-width:760px;">Electrification, autonomous vehicles, digital customs, sustainability mandates, and nearshoring convergence are creating a fundamentally transformed freight landscape by 2030. <strong>Brokers positioned at the intersection of technology, compliance, and relationships will lead it.</strong> Those who aren't won't survive it.</p>

    <div class="gcol40" style="gap:52px;margin-bottom:48px;">
      <div class="reveal">
        <div class="tlv">
          <div class="tli">
            <div class="tli-dot"><div class="tli-in"></div></div>
            <div class="tli-yr">Now — 2026</div>
            <div class="tli-title">Digital Brokerage Adoption Wave</div>
            <div class="tli-body">AI pricing, automated compliance, shipper portals, and GPS tracking become baseline expectations. Brokers without technology lose competitive deals to digital-native platforms entering Canada from the US. The window to build tech infrastructure is 2025–2026.</div>
          </div>
          <div class="tli">
            <div class="tli-dot" style="border-color:var(--teal2)"><div class="tli-in" style="background:var(--teal2)"></div></div>
            <div class="tli-yr" style="color:var(--teal2)">2026 — 2027</div>
            <div class="tli-title">Sustainability Mandates Go Mandatory</div>
            <div class="tli-body">Transport Canada's Clean Freight Corridor program rolls out. TSX-listed companies begin mandatory Scope 3 emissions disclosure. Logistics partners who cannot provide certified per-load carbon data will lose enterprise contracts to those who can.</div>
          </div>
          <div class="tli">
            <div class="tli-dot" style="border-color:var(--sky2)"><div class="tli-in" style="background:var(--sky2)"></div></div>
            <div class="tli-yr" style="color:var(--sky2)">2027 — 2028</div>
            <div class="tli-title">Intermodal Becomes the Long-Haul Default</div>
            <div class="tli-body">CN and CP Rail intermodal network expansion combined with carbon pricing economics make rail-truck hybrid the only financially viable option for ON–AB lanes. Brokers without intermodal products lose access to the $21B corridor.</div>
          </div>
          <div class="tli">
            <div class="tli-dot" style="border-color:var(--violet2)"><div class="tli-in" style="background:var(--violet2)"></div></div>
            <div class="tli-yr" style="color:var(--violet2)">2028 — 2030</div>
            <div class="tli-title">Autonomous Trucking &amp; EV Fleet Scale</div>
            <div class="tli-body">Semi-autonomous long-haul trucks debut on Trans-Canada and Highway 401 corridors. Electric short-haul delivery expands across Metro Vancouver, Toronto, and Montreal. Freight economics transform permanently — broker platforms managing EV + autonomous assets win long-term contracts.</div>
          </div>
          <div class="tli" style="padding-bottom:0;">
            <div class="tli-dot" style="border-color:var(--maple2)"><div class="tli-in" style="background:var(--maple2)"></div></div>
            <div class="tli-yr" style="color:var(--maple2)">2030+</div>
            <div class="tli-title">Digital Freight Platform Dominance</div>
            <div class="tli-body">Fully digital freight platforms handle 60%+ of North American loads. Brokers who built technology platforms in 2025–2027 own the networks and the margin. Those who relied solely on relationships become rate-takers.</div>
          </div>
        </div>
      </div>

      <div>
        <div class="g2 reveal" style="gap:12px;margin-bottom:12px;">
          <div class="hb-block hb-sky"><div style="font-family:var(--serif);font-size:34px;font-weight:700;color:var(--sky2);line-height:1;margin-bottom:5px;">$275B+</div><div style="font-size:13px;font-weight:600;color:var(--fog);margin-bottom:4px;">Port of Vancouver</div><div style="font-size:12px;color:var(--mist);line-height:1.5;">Annual goods through Canada's largest port. BC port-to-interior drayage is a high-growth opportunity in our Western Canada expansion.</div></div>
          <div class="hb-block hb-teal"><div style="font-family:var(--serif);font-size:34px;font-weight:700;color:var(--teal2);line-height:1;margin-bottom:5px;">$800B</div><div style="font-size:13px;font-weight:600;color:var(--fog);margin-bottom:4px;">Canada–US Trade</div><div style="font-size:12px;color:var(--mist);line-height:1.5;">68% of Canadian exports go to the US. Cross-border freight is where brokers earn their highest margins and deepest client loyalty.</div></div>
        </div>

        <div class="g3 reveal" style="gap:11px;">
          <div class="fc" style="padding:18px;"><span class="fc-icon" style="font-size:22px;margin-bottom:9px;">⚡</span><div class="fc-title" style="font-size:14px;">EV Truck Adoption</div><div class="fc-body" style="font-size:12px;">Transport Canada ZEV mandate + $700M+ federal fleet incentives. Volvo, Kenworth, Freightliner EV fleets deploying across Canada 2026–2028. Brokers with EV-compatible load boards win green procurement contracts.</div><div class="fc-tag teal">Positioning Now</div></div>
          <div class="fc" style="padding:18px;"><span class="fc-icon" style="font-size:22px;margin-bottom:9px;">🌿</span><div class="fc-title" style="font-size:14px;">Green Freight &amp; ESG</div><div class="fc-body" style="font-size:12px;">Carbon tax reaches $170/tonne by 2030. Enterprise shippers requiring Scope 3 emissions data from every logistics partner as a board-level KPI. We are building these tools now to be first to market.</div><div class="fc-tag gold">ESG Differentiator</div></div>
          <div class="fc" style="padding:18px;"><span class="fc-icon" style="font-size:22px;margin-bottom:9px;">🏭</span><div class="fc-title" style="font-size:14px;">Nearshoring Wave</div><div class="fc-body" style="font-size:12px;">US tariff instability is driving manufacturing reshoring to Ontario and Quebec. Record industrial investment creates 12–18% more domestic freight volume by 2028. We are positioned to capture this wave from day one.</div><div class="fc-tag maple">Supply Chain Shift</div></div>
        </div>

        <div class="g2 reveal" style="gap:12px;margin-top:12px;">
          <div class="hb-block hb-gold" style="padding:18px 20px;"><div style="font-family:var(--serif);font-size:22px;font-weight:700;color:var(--gold2);margin-bottom:5px;">CBSA Single Window</div><div style="font-size:12px;color:var(--mist);line-height:1.5;">Canada's digital customs initiative will reduce cross-border processing times by 60%. Brokers with digital-first customs workflows will clear cargo faster and command enterprise shipper loyalty as CBSA modernizes.</div></div>
          <div class="hb-block hb-maple" style="padding:18px 20px;"><div style="font-family:var(--serif);font-size:22px;font-weight:700;color:var(--maple2);margin-bottom:5px;">CUSMA Renegotiation</div><div style="font-size:12px;color:var(--mist);line-height:1.5;">CUSMA/USMCA review in 2026 will reshape cross-border freight regulations and tariff schedules. Brokers with deep trade compliance expertise will be indispensable to shippers navigating the changes — regardless of outcome.</div></div>
        </div>

        <div class="pq reveal" style="margin-top:0;border-left-color:var(--sky2);">
          <em>"The companies that invest in intelligent freight partnerships today will define the competitive landscape of 2030."</em>
          <div class="pq-src">Canadian Supply Chain Sector Council · 2025 Outlook</div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ═══════════ SLIDE 07: WHY US ═══════════ -->
<section class="s bg-ink" id="s-why">
  <div class="sidx">07</div>
  <div class="si">
    <div class="eb">Competitive Advantage</div>
    <h2 class="txl" style="max-width:720px;margin-bottom:18px;">Why the Best Canadian Shippers Choose <em>Us.</em></h2>
    <p class="lead" style="margin-bottom:48px;max-width:700px;">There are hundreds of freight brokers in Canada. Most offer the same thing — a phone number, a rate, and a hope. We offer something different: <strong>accountability, genuine expertise, and a partnership</strong> built from the ground up for the Canadian market, its regulations, and its complexities.</p>

    <div class="gcol50" style="gap:48px;margin-bottom:48px;">
      <div>
        <div class="steps">
          <div class="step"><div class="step-n">01</div><div><div class="step-title">Canadian-Born. Canadian-Focused.</div><div class="step-body">We understand NSC, CVOR, WSIB, CTA licensing, FSEP food compliance, CBSA import/export, and the unique regulatory complexity of every Canadian province — because we operate in it every day. This is not an American brokerage offering Canada as an afterthought. We are built entirely for this market.</div></div></div>
          <div class="step"><div class="step-n">02</div><div><div class="step-title">Boutique Service. Enterprise Capability.</div><div class="step-body">You get the personal attention of a boutique brokerage with the carrier network, technology infrastructure, and compliance expertise of a national operation. A dedicated broker — not a ticket queue, not an offshore call centre, not a chatbot. A person who picks up the phone.</div></div></div>
          <div class="step"><div class="step-n">03</div><div><div class="step-title">Compliance as Our Competitive Moat</div><div class="step-body">Real-time CVOR monitoring, automated NSC verification, WSIB clearance checks, and cross-border customs expertise — we invest heavily in compliance infrastructure. This protects you from liability that most brokers simply don't flag until after an incident costs you money.</div></div></div>
          <div class="step"><div class="step-n">04</div><div><div class="step-title">Carrier Relationships Built on Respect</div><div class="step-body">We pay carriers on time, communicate clearly, and treat them as partners — not commodities. This earns first-call capacity when the market tightens and loyalty that protects our shippers when other brokers are scrambling. A moat that money alone cannot build overnight.</div></div></div>
          <div class="step" style="border-bottom:none;"><div class="step-n">05</div><div><div class="step-title">Speed Without Sacrificing Quality</div><div class="step-body">Rate quotes in under 30 minutes. Carrier match in under 2 hours for spot loads. Same-day confirmation as standard. We are fast because we are prepared — not because we are cutting corners on vetting, compliance, or carrier selection.</div></div></div>
        </div>
      </div>

      <div style="display:flex;flex-direction:column;gap:18px;">
        <div class="hb-block hb-gold">
          <div style="font-family:var(--mono);font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--gold);margin-bottom:14px;">Competitive Comparison Matrix</div>
          <table class="ptbl">
            <thead><tr><th>Capability</th><th style="color:var(--gold2)">FreightForward CA</th><th>Large US Broker</th><th>Regional CA</th></tr></thead>
            <tbody>
              <tr><td class="td-h">Canadian CVOR/NSC Depth</td><td class="td-us">✦ Deep Expertise</td><td class="td-neutral">Partial</td><td class="td-neutral">Variable</td></tr>
              <tr><td class="td-h">Cross-Border / CBSA</td><td class="td-us">✦ Full Service</td><td class="td-neutral">Yes (US-first)</td><td class="td-bad">Rarely</td></tr>
              <tr><td class="td-h">Dedicated Broker</td><td class="td-us">✦ Always</td><td class="td-bad">Call Centre</td><td class="td-neutral">Sometimes</td></tr>
              <tr><td class="td-h">AI Pricing Tools</td><td class="td-us">✦ Active + Roadmap</td><td class="td-neutral">Enterprise Only</td><td class="td-bad">No</td></tr>
              <tr><td class="td-h">Quote Response Time</td><td class="td-us td-mono">&lt;30 min</td><td class="td-neutral td-mono">4–24 hrs</td><td class="td-neutral td-mono">2–8 hrs</td></tr>
              <tr><td class="td-h">Quebec / Bilingual</td><td class="td-us">✦ EN/FR (Q2 2026)</td><td class="td-bad">English Only</td><td class="td-neutral">Some</td></tr>
              <tr><td class="td-h">ESG / Carbon Reports</td><td class="td-us">✦ Building Now</td><td class="td-neutral">Limited</td><td class="td-bad">No</td></tr>
              <tr><td class="td-h">Intermodal (CN/CP)</td><td class="td-us">✦ Q4 2026</td><td class="td-neutral">Via Partners</td><td class="td-bad">Rarely</td></tr>
            </tbody>
          </table>
        </div>

        <div class="testi"><div class="testi-q">"</div><div class="testi-text">"We moved our Ontario–Alberta freight to FreightForward and cut our average load cost by 16% in the first quarter. But more importantly — they have never left us stranded. Not once in two years."</div><div class="testi-auth">VP Supply Chain · Ontario Food Manufacturer · 2025</div></div>
        <div class="testi"><div class="testi-q">"</div><div class="testi-text">"Our cross-border shipments were a compliance nightmare until we partnered with these folks. PARS, customs broker coordination, FAST carriers — all managed seamlessly. Zero CBSA holds since day one."</div><div class="testi-auth">Logistics Director · Windsor Manufacturing Corp · 2025</div></div>
        <div class="testi"><div class="testi-q">"</div><div class="testi-text">"What sets them apart isn't just the rates — it's that they actually call you. Before there's a problem, not after. That proactive communication alone has saved us thousands in chargebacks."</div><div class="testi-auth">Operations Manager · Saskatchewan Agricultural Co-op · 2025</div></div>
      </div>
    </div>
  </div>
</section>

<!-- ═══════════ SLIDE 08: GROWTH ROADMAP ═══════════ -->
<section class="s bg-gold-aura" id="s-roadmap">
  <div class="sidx">08</div>
  <div class="si">
    <div class="eb">Growth Roadmap &amp; Financials</div>
    <h2 class="txl" style="max-width:720px;margin-bottom:18px;">Where We Are. Where We're <em>Going.</em></h2>
    <p class="lead" style="margin-bottom:48px;max-width:700px;">We are not just a brokerage — we are a <strong>platform in development</strong>. Every initiative is designed to compound: more carriers, more shippers, smarter technology, and progressively higher-margin service offerings that no regional competitor can match.</p>

    <div class="gcol50" style="gap:52px;margin-bottom:48px;">
      <div class="reveal">
        <div style="font-family:var(--mono);font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--haze);margin-bottom:16px;">Projected Revenue Trajectory (CAD)</div>
        <div class="vbars" style="height:185px;margin-bottom:14px;">
          <div class="vb"><div class="vb-bar" style="height:27%;background:rgba(212,168,67,.3);"><div class="vb-top">$649K</div></div><div class="vb-lbl">Jan '26</div></div>
          <div class="vb"><div class="vb-bar" style="height:35%;background:rgba(212,168,67,.4);"><div class="vb-top">$820K</div></div><div class="vb-lbl">Q1 End</div></div>
          <div class="vb"><div class="vb-bar" style="height:47%;background:var(--gold-d);"><div class="vb-top">$1.1M</div></div><div class="vb-lbl">Q2 '26</div></div>
          <div class="vb"><div class="vb-bar" style="height:59%;background:var(--gold);"><div class="vb-top">$1.4M</div></div><div class="vb-lbl">Q3 '26</div></div>
          <div class="vb"><div class="vb-bar" style="height:69%;background:var(--gold2);"><div class="vb-top">$1.6M</div></div><div class="vb-lbl">Q4 '26</div></div>
          <div class="vb"><div class="vb-bar" style="height:82%;background:var(--teal);"><div class="vb-top">$1.9M</div></div><div class="vb-lbl">Q1 '27</div></div>
          <div class="vb"><div class="vb-bar" style="height:100%;background:linear-gradient(180deg,var(--teal2),var(--teal));"><div class="vb-top">$2.4M+</div></div><div class="vb-lbl">Q2 '27</div></div>
        </div>
        <div style="display:grid;grid-template-columns:1fr 1fr;gap:11px;">
          <div class="hb-block hb-gold" style="padding:15px 17px;text-align:center;"><div style="font-family:var(--serif);font-size:26px;font-weight:700;color:var(--gold2);">$9.7M</div><div style="font-size:11.5px;color:var(--mist);margin-top:2px;">FY2026 Revenue Target (CAD)</div></div>
          <div class="hb-block hb-teal" style="padding:15px 17px;text-align:center;"><div style="font-family:var(--serif);font-size:26px;font-weight:700;color:var(--teal2);">18%+</div><div style="font-size:11.5px;color:var(--mist);margin-top:2px;">Target Gross Margin Full Year</div></div>
        </div>

        <div style="margin-top:16px;">
          <div style="font-family:var(--mono);font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--haze);margin-bottom:12px;">Current Metrics (Q1 2026)</div>
          <div style="display:flex;flex-direction:column;gap:8px;">
            <div style="display:flex;justify-content:space-between;padding:10px 14px;background:var(--panel);border:1px solid var(--border);border-radius:8px;"><span style="font-size:13px;color:var(--mist);">Revenue MTD</span><span style="font-family:var(--serif);font-size:16px;font-weight:700;color:var(--gold2);">$384K CAD</span></div>
            <div style="display:flex;justify-content:space-between;padding:10px 14px;background:var(--panel);border:1px solid var(--border);border-radius:8px;"><span style="font-size:13px;color:var(--mist);">YTD Revenue</span><span style="font-family:var(--serif);font-size:16px;font-weight:700;color:var(--gold2);">$1.68M CAD</span></div>
            <div style="display:flex;justify-content:space-between;padding:10px 14px;background:var(--panel);border:1px solid var(--border);border-radius:8px;"><span style="font-size:13px;color:var(--mist);">Gross Margin</span><span style="font-family:var(--serif);font-size:16px;font-weight:700;color:var(--teal2);">18.4%</span></div>
            <div style="display:flex;justify-content:space-between;padding:10px 14px;background:var(--panel);border:1px solid var(--border);border-radius:8px;"><span style="font-size:13px;color:var(--mist);">Active Carrier Partners</span><span style="font-family:var(--serif);font-size:16px;font-weight:700;color:var(--fog);">247+</span></div>
            <div style="display:flex;justify-content:space-between;padding:10px 14px;background:var(--panel);border:1px solid var(--border);border-radius:8px;"><span style="font-size:13px;color:var(--mist);">Active Shipper Accounts</span><span style="font-family:var(--serif);font-size:16px;font-weight:700;color:var(--fog);">61 active of 84</span></div>
            <div style="display:flex;justify-content:space-between;padding:10px 14px;background:var(--panel);border:1px solid var(--border);border-radius:8px;"><span style="font-size:13px;color:var(--mist);">Pipeline Value</span><span style="font-family:var(--serif);font-size:16px;font-weight:700;color:var(--violet2);">$460K CAD</span></div>
          </div>
        </div>
      </div>

      <div class="reveal">
        <div style="font-family:var(--mono);font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--haze);margin-bottom:16px;">Strategic Milestone Roadmap</div>
        <div style="display:flex;flex-direction:column;gap:11px;">
          <div style="padding:16px 18px;background:rgba(31,184,153,.05);border:1px solid rgba(31,184,153,.16);border-radius:11px;display:flex;gap:12px;align-items:flex-start;">
            <div style="font-size:18px;flex-shrink:0">✅</div>
            <div><div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--fog);margin-bottom:3px;">Q1 2026 — Operational Foundation</div><div style="font-size:12.5px;color:var(--mist);line-height:1.5;">AscendTMS live · 247 carriers vetted · QuickBooks CA integrated · CTA licensed · CBSA compliance operational · $1.68M ARR run rate achieved</div></div>
          </div>
          <div style="padding:16px 18px;background:rgba(212,168,67,.04);border:1px solid rgba(212,168,67,.14);border-radius:11px;display:flex;gap:12px;align-items:flex-start;">
            <div style="font-size:18px;flex-shrink:0">🔄</div>
            <div><div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--fog);margin-bottom:3px;">Q2–Q3 2026 — Market Expansion</div><div style="font-size:12.5px;color:var(--mist);line-height:1.5;">Quebec EN/FR launch (+$180K target) · AB/BC Western expansion · Loadlink AI rate integration · Shipper self-serve portal · Cross-border doc automation · Carbon ESG tracking</div></div>
          </div>
          <div style="padding:16px 18px;background:rgba(58,123,213,.04);border:1px solid rgba(58,123,213,.14);border-radius:11px;display:flex;gap:12px;align-items:flex-start;">
            <div style="font-size:18px;flex-shrink:0">🚀</div>
            <div><div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--fog);margin-bottom:3px;">Q4 2026 — Scale &amp; Differentiation</div><div style="font-size:12.5px;color:var(--mist);line-height:1.5;">CN/CP Intermodal product launch · 3PL Managed Transportation for key accounts · 400+ carrier network · AI dynamic rate engine live · $7M+ ARR target</div></div>
          </div>
          <div style="padding:16px 18px;background:rgba(124,92,191,.04);border:1px solid rgba(124,92,191,.14);border-radius:11px;display:flex;gap:12px;align-items:flex-start;">
            <div style="font-size:18px;flex-shrink:0">🌐</div>
            <div><div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--fog);margin-bottom:3px;">2027 — Digital Freight Platform</div><div style="font-size:12.5px;color:var(--mist);line-height:1.5;">Canadian freight marketplace launch · AI demand forecasting · Mobile carrier capacity app · EN/FR bilingual full stack · $12M+ ARR target · Series A capital exploration</div></div>
          </div>
        </div>

        <div style="margin-top:18px;">
          <div style="font-family:var(--mono);font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--haze);margin-bottom:12px;">Growth Initiative Targets</div>
          <div style="display:flex;flex-direction:column;gap:8px;">
            <div style="display:flex;align-items:center;gap:12px;padding:11px 14px;background:var(--panel);border:1px solid var(--border);border-radius:8px;">
              <div style="font-size:14px;">🇨🇦</div>
              <div style="flex:1"><div style="font-size:13px;font-weight:600;color:var(--fog);">Quebec Market Entry</div><div style="font-size:11.5px;color:var(--haze);">EN/FR broker · ON–QC corridor · Q1 2026</div></div>
              <div style="font-family:var(--mono);font-size:12px;color:var(--gold2);">+$180K/yr</div>
            </div>
            <div style="display:flex;align-items:center;gap:12px;padding:11px 14px;background:var(--panel);border:1px solid var(--border);border-radius:8px;">
              <div style="font-size:14px;">⚙️</div>
              <div style="flex:1"><div style="font-size:13px;font-weight:600;color:var(--fog);">Loadlink Rate Intelligence</div><div style="font-size:11.5px;color:var(--haze);">Real-time CA market data · Q1 2026</div></div>
              <div style="font-family:var(--mono);font-size:12px;color:var(--gold2);">+2.5% margin</div>
            </div>
            <div style="display:flex;align-items:center;gap:12px;padding:11px 14px;background:var(--panel);border:1px solid var(--border);border-radius:8px;">
              <div style="font-size:14px;">🖥️</div>
              <div style="flex:1"><div style="font-size:13px;font-weight:600;color:var(--fog);">Shipper Self-Serve Portal</div><div style="font-size:11.5px;color:var(--haze);">EN/FR web portal · AscendTMS API · Q2 2026</div></div>
              <div style="font-family:var(--mono);font-size:12px;color:var(--gold2);">+25% capacity</div>
            </div>
            <div style="display:flex;align-items:center;gap:12px;padding:11px 14px;background:var(--panel);border:1px solid var(--border);border-radius:8px;">
              <div style="font-size:14px;">🚂</div>
              <div style="flex:1"><div style="font-size:13px;font-weight:600;color:var(--fog);">CN/CP Intermodal Product</div><div style="font-size:11.5px;color:var(--haze);">ON–AB · ON–BC long-haul · Q4 2026</div></div>
              <div style="font-family:var(--mono);font-size:12px;color:var(--gold2);">+$400K/yr</div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="sdiv"></div>
    <h3 class="tlg reveal" style="margin-bottom:22px;">The Foundation Our Business Is Built On</h3>
    <div class="g3 reveal">
      <div class="fc"><span class="fc-icon">🎓</span><div class="fc-title">Deep Industry Expertise</div><div class="fc-body">Hands-on experience in freight operations, carrier relations, cross-border compliance, and Canadian regulatory requirements. Not theoretical knowledge — daily operational practice in the real Canadian freight market with real carriers and real shippers.</div></div>
      <div class="fc"><span class="fc-icon">🤝</span><div class="fc-title">Carrier Trust as a Moat</div><div class="fc-body">We pay on time. We communicate proactively. We treat carriers as partners, not volume commodities. This earns first-call capacity when the market tightens — a competitive advantage that money alone cannot replicate overnight.</div></div>
      <div class="fc"><span class="fc-icon">🍁</span><div class="fc-title">Community-Rooted, Nationally Ambitious</div><div class="fc-body">Based in Brant, Ontario — connected to the agricultural and manufacturing heartland of Canada. Our roots are local. Our network is national. Our ambition is to become the most trusted and capable freight brokerage in this country.</div></div>
    </div>
  </div>
</section>

<!-- ═══════════ CTA ═══════════ -->
<section id="s-cta">
  <div class="cta-wrap">
    <div class="cta-ring" style="width:800px;height:800px;top:50%;left:50%;transform:translate(-50%,-50%);"></div>
    <div class="cta-ring" style="width:560px;height:560px;top:50%;left:50%;transform:translate(-50%,-50%);border-color:rgba(212,168,67,.09);"></div>
    <div class="cta-ring" style="width:320px;height:320px;top:50%;left:50%;transform:translate(-50%,-50%);border-color:rgba(212,168,67,.12);"></div>
    <div style="position:relative;z-index:1;max-width:700px;">
      <div class="eb" style="justify-content:center;">Let's Build Something Together</div>
      <h2 class="th" style="text-align:center;font-size:clamp(48px,7vw,90px);margin-bottom:18px;">Ready to Move<br><em>Smarter?</em></h2>
      <p class="lead" style="text-align:center;margin:0 auto 34px;max-width:540px;">Whether you're a <strong>shipper</strong> looking for a reliable freight partner, a <strong>carrier</strong> wanting to join our network, or someone who wants to understand what we're building — the conversation starts here.</p>
      <div style="display:flex;justify-content:center;gap:13px;flex-wrap:wrap;">
        <button class="btn-p" onclick="openModal('consultation')">📞 Book a Free Consultation</button>
        <button class="btn-o" onclick="openModal('quote')">📧 Request a Rate Quote</button>
      </div>
      <div style="margin-top:56px;display:grid;grid-template-columns:repeat(3,1fr);gap:24px;max-width:600px;margin-left:auto;margin-right:auto;">
        <div style="text-align:center;"><div style="font-size:24px;margin-bottom:7px;">📍</div><div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--fog);margin-bottom:3px;">Based In</div><div style="font-size:12px;color:var(--mist);line-height:1.5;">Brant, Ontario<br>All 10 provinces served</div></div>
        <div style="text-align:center;border-left:1px solid var(--border);border-right:1px solid var(--border);padding:0 18px;"><div style="font-size:24px;margin-bottom:7px;">⚡</div><div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--fog);margin-bottom:3px;">Response Time</div><div style="font-size:12px;color:var(--mist);line-height:1.5;">Quotes &lt;30 min<br>Carrier match &lt;2 hrs</div></div>
        <div style="text-align:center;"><div style="font-size:24px;margin-bottom:7px;">🍁</div><div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--fog);margin-bottom:3px;">Fully Licensed</div><div style="font-size:12px;color:var(--mist);line-height:1.5;">CTA Broker<br>CVOR · NSC · CBSA</div></div>
      </div>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="ft-logo">FreightForward Canada 🍁</div>
  <div class="ft-copy">Brant, Ontario · CTA Licensed Freight Broker · All rates in CAD<br>© 2026 FreightForward Canada Inc. · Confidential &amp; Proprietary</div>
  <div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--gold2);">Moving Canada Forward.</div>
</footer>

<!-- ═══════════ INQUIRY MODAL ═══════════ -->
<div id="inquiry-modal" style="
  display:none;position:fixed;inset:0;z-index:9000;
  background:rgba(6,8,7,.85);backdrop-filter:blur(16px) saturate(1.4);
  align-items:center;justify-content:center;padding:20px;
" onclick="closeModalOutside(event)">
  <div id="modal-box" style="
    background:var(--panel);border:1px solid var(--border2);border-radius:18px;
    width:100%;max-width:560px;overflow:hidden;position:relative;
    box-shadow:0 40px 100px rgba(0,0,0,.6);
    animation:modalIn .4s cubic-bezier(.16,1,.3,1);
  ">
    <!-- Top bar -->
    <div style="background:var(--raised);padding:18px 24px;border-bottom:1px solid var(--border);display:flex;align-items:center;justify-content:space-between;">
      <div style="display:flex;align-items:center;gap:10px;">
        <div style="width:30px;height:30px;border-radius:6px;background:linear-gradient(140deg,var(--gold-d),var(--gold));display:flex;align-items:center;justify-content:center;font-family:var(--serif);font-size:15px;font-weight:700;color:var(--void);">FF</div>
        <div>
          <div style="font-family:var(--serif);font-size:15px;font-weight:700;color:var(--gold2);" id="modal-title">Book a Free Consultation</div>
          <div style="font-family:var(--mono);font-size:9px;color:var(--haze);letter-spacing:1px;text-transform:uppercase;">FreightForward Canada · logistics@emirg-group.com</div>
        </div>
      </div>
      <button onclick="closeModal()" style="background:none;border:none;color:var(--haze);font-size:20px;cursor:pointer;line-height:1;padding:4px 8px;border-radius:6px;transition:all .2s;" onmouseover="this.style.color='var(--fog)';this.style.background='var(--border)'" onmouseout="this.style.color='var(--haze)';this.style.background='none'">×</button>
    </div>

    <!-- Form body -->
    <div style="padding:28px 24px;">
      <!-- Success state (hidden by default) -->
      <div id="modal-success" style="display:none;text-align:center;padding:20px 0;">
        <div style="font-size:48px;margin-bottom:16px;">✅</div>
        <div style="font-family:var(--serif);font-size:24px;font-weight:700;color:var(--gold2);margin-bottom:8px;">Message Sent!</div>
        <div style="font-size:14px;color:var(--mist);line-height:1.6;">Your inquiry has been sent to <strong style="color:var(--fog)">logistics@emirg-group.com</strong>.<br>We'll be in touch within 2 business hours.</div>
        <button onclick="closeModal()" style="margin-top:24px;padding:12px 32px;background:var(--gold);color:var(--void);border:none;border-radius:8px;font-size:14px;font-weight:600;cursor:pointer;font-family:var(--sans);">Close</button>
      </div>

      <!-- Form (shown by default) -->
      <div id="modal-form">
        <div id="modal-subtitle" style="font-size:13.5px;color:var(--mist);margin-bottom:22px;line-height:1.6;">Fill in your details below and our team will reach out within <strong style="color:var(--fog)">2 business hours</strong> — guaranteed.</div>

        <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:12px;">
          <div>
            <label style="font-family:var(--mono);font-size:9.5px;color:var(--haze);letter-spacing:1.5px;text-transform:uppercase;display:block;margin-bottom:6px;">First Name *</label>
            <input id="f-firstname" type="text" placeholder="Jane" style="width:100%;padding:11px 14px;background:var(--raised);border:1px solid var(--border2);border-radius:8px;color:var(--fog);font-family:var(--sans);font-size:14px;outline:none;transition:border-color .2s;" onfocus="this.style.borderColor='var(--gold)'" onblur="this.style.borderColor='var(--border2)'">
          </div>
          <div>
            <label style="font-family:var(--mono);font-size:9.5px;color:var(--haze);letter-spacing:1.5px;text-transform:uppercase;display:block;margin-bottom:6px;">Last Name *</label>
            <input id="f-lastname" type="text" placeholder="Smith" style="width:100%;padding:11px 14px;background:var(--raised);border:1px solid var(--border2);border-radius:8px;color:var(--fog);font-family:var(--sans);font-size:14px;outline:none;transition:border-color .2s;" onfocus="this.style.borderColor='var(--gold)'" onblur="this.style.borderColor='var(--border2)'">
          </div>
        </div>

        <div style="margin-bottom:12px;">
          <label style="font-family:var(--mono);font-size:9.5px;color:var(--haze);letter-spacing:1.5px;text-transform:uppercase;display:block;margin-bottom:6px;">Company Name</label>
          <input id="f-company" type="text" placeholder="Acme Logistics Inc." style="width:100%;padding:11px 14px;background:var(--raised);border:1px solid var(--border2);border-radius:8px;color:var(--fog);font-family:var(--sans);font-size:14px;outline:none;transition:border-color .2s;" onfocus="this.style.borderColor='var(--gold)'" onblur="this.style.borderColor='var(--border2)'">
        </div>

        <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:12px;">
          <div>
            <label style="font-family:var(--mono);font-size:9.5px;color:var(--haze);letter-spacing:1.5px;text-transform:uppercase;display:block;margin-bottom:6px;">Email Address *</label>
            <input id="f-email" type="email" placeholder="jane@company.com" style="width:100%;padding:11px 14px;background:var(--raised);border:1px solid var(--border2);border-radius:8px;color:var(--fog);font-family:var(--sans);font-size:14px;outline:none;transition:border-color .2s;" onfocus="this.style.borderColor='var(--gold)'" onblur="this.style.borderColor='var(--border2)'">
          </div>
          <div>
            <label style="font-family:var(--mono);font-size:9.5px;color:var(--haze);letter-spacing:1.5px;text-transform:uppercase;display:block;margin-bottom:6px;">Phone Number</label>
            <input id="f-phone" type="tel" placeholder="(519) 555-0100" style="width:100%;padding:11px 14px;background:var(--raised);border:1px solid var(--border2);border-radius:8px;color:var(--fog);font-family:var(--sans);font-size:14px;outline:none;transition:border-color .2s;" onfocus="this.style.borderColor='var(--gold)'" onblur="this.style.borderColor='var(--border2)'">
          </div>
        </div>

        <div id="quote-extras" style="display:none;">
          <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:12px;">
            <div>
              <label style="font-family:var(--mono);font-size:9.5px;color:var(--haze);letter-spacing:1.5px;text-transform:uppercase;display:block;margin-bottom:6px;">Origin (City / Province)</label>
              <input id="f-origin" type="text" placeholder="Toronto, ON" style="width:100%;padding:11px 14px;background:var(--raised);border:1px solid var(--border2);border-radius:8px;color:var(--fog);font-family:var(--sans);font-size:14px;outline:none;transition:border-color .2s;" onfocus="this.style.borderColor='var(--gold)'" onblur="this.style.borderColor='var(--border2)'">
            </div>
            <div>
              <label style="font-family:var(--mono);font-size:9.5px;color:var(--haze);letter-spacing:1.5px;text-transform:uppercase;display:block;margin-bottom:6px;">Destination</label>
              <input id="f-dest" type="text" placeholder="Calgary, AB" style="width:100%;padding:11px 14px;background:var(--raised);border:1px solid var(--border2);border-radius:8px;color:var(--fog);font-family:var(--sans);font-size:14px;outline:none;transition:border-color .2s;" onfocus="this.style.borderColor='var(--gold)'" onblur="this.style.borderColor='var(--border2)'">
            </div>
          </div>
          <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:12px;">
            <div>
              <label style="font-family:var(--mono);font-size:9.5px;color:var(--haze);letter-spacing:1.5px;text-transform:uppercase;display:block;margin-bottom:6px;">Equipment Type</label>
              <select id="f-equip" style="width:100%;padding:11px 14px;background:var(--raised);border:1px solid var(--border2);border-radius:8px;color:var(--fog);font-family:var(--sans);font-size:14px;outline:none;transition:border-color .2s;appearance:none;" onfocus="this.style.borderColor='var(--gold)'" onblur="this.style.borderColor='var(--border2)'">
                <option value="" style="background:var(--panel)">Select equipment...</option>
                <option style="background:var(--panel)">Dry Van 53'</option>
                <option style="background:var(--panel)">Flatbed 48' / 53'</option>
                <option style="background:var(--panel)">Reefer 53'</option>
                <option style="background:var(--panel)">Step Deck</option>
                <option style="background:var(--panel)">B-Train / Super-B</option>
                <option style="background:var(--panel)">LTL</option>
                <option style="background:var(--panel)">Lowboy / Heavy Haul</option>
                <option style="background:var(--panel)">Cross-Border (CA–US)</option>
                <option style="background:var(--panel)">Other</option>
              </select>
            </div>
            <div>
              <label style="font-family:var(--mono);font-size:9.5px;color:var(--haze);letter-spacing:1.5px;text-transform:uppercase;display:block;margin-bottom:6px;">Pickup Date (Approx.)</label>
              <input id="f-date" type="date" style="width:100%;padding:11px 14px;background:var(--raised);border:1px solid var(--border2);border-radius:8px;color:var(--fog);font-family:var(--sans);font-size:14px;outline:none;transition:border-color .2s;color-scheme:dark;" onfocus="this.style.borderColor='var(--gold)'" onblur="this.style.borderColor='var(--border2)'">
            </div>
          </div>
        </div>

        <div style="margin-bottom:18px;">
          <label style="font-family:var(--mono);font-size:9.5px;color:var(--haze);letter-spacing:1.5px;text-transform:uppercase;display:block;margin-bottom:6px;" id="msg-label">Message / Questions</label>
          <textarea id="f-message" rows="3" placeholder="Tell us about your freight needs, volume, lanes, or any questions..." style="width:100%;padding:11px 14px;background:var(--raised);border:1px solid var(--border2);border-radius:8px;color:var(--fog);font-family:var(--sans);font-size:14px;outline:none;transition:border-color .2s;resize:vertical;min-height:80px;" onfocus="this.style.borderColor='var(--gold)'" onblur="this.style.borderColor='var(--border2)'"></textarea>
        </div>

        <!-- Error message -->
        <div id="modal-error" style="display:none;padding:10px 14px;background:rgba(200,57,43,.1);border:1px solid rgba(200,57,43,.25);border-radius:8px;font-size:13px;color:var(--maple2);margin-bottom:14px;"></div>

        <!-- Submit -->
        <button id="modal-submit" onclick="submitInquiry()" style="width:100%;padding:14px;background:var(--gold);color:var(--void);border:none;border-radius:10px;font-size:15px;font-weight:700;cursor:pointer;font-family:var(--sans);transition:all .2s;display:flex;align-items:center;justify-content:center;gap:9px;" onmouseover="this.style.background='var(--gold2)'" onmouseout="this.style.background='var(--gold)'">
          <span id="submit-icon">📨</span>
          <span id="submit-text">Send Inquiry</span>
        </button>

        <div style="margin-top:12px;text-align:center;font-family:var(--mono);font-size:10px;color:var(--haze);letter-spacing:.5px;">
          Sent directly to <span style="color:var(--gold2);">logistics@emirg-group.com</span> · Response within 2 business hours
        </div>
      </div>
    </div>
  </div>
</div>

<style>
@keyframes modalIn {
  from { opacity:0; transform:scale(.95) translateY(16px); }
  to   { opacity:1; transform:scale(1) translateY(0); }
}
input::placeholder, textarea::placeholder { color:var(--haze); }
input[type="date"]::-webkit-calendar-picker-indicator { filter:invert(.4); cursor:pointer; }
</style>

<script>
/* PROGRESS BAR */
window.addEventListener('scroll', () => {
  const d = document.documentElement;
  document.getElementById('pb').style.width = (d.scrollTop / (d.scrollHeight - d.clientHeight) * 100) + '%';
});

/* SMOOTH SCROLL NAV */
function sTo(id, el) {
  const t = document.getElementById(id);
  if (t) t.scrollIntoView({ behavior: 'smooth' });
}

/* NAV ACTIVE STATE */
const secIds = ['s-hero','s-market','s-services','s-value','s-ai','s-future','s-why','s-roadmap'];
const navPills = document.querySelectorAll('.np');
window.addEventListener('scroll', () => {
  const mid = window.scrollY + window.innerHeight / 2;
  secIds.forEach((id, i) => {
    const el = document.getElementById(id);
    if (!el) return;
    if (mid >= el.offsetTop && mid < el.offsetTop + el.offsetHeight) {
      navPills.forEach(p => p.classList.remove('on'));
      if (navPills[i]) navPills[i].classList.add('on');
    }
  });
});

/* SCROLL REVEAL */
const ro = new IntersectionObserver(entries => {
  entries.forEach(e => { if (e.isIntersecting) e.target.classList.add('in'); });
}, { threshold: 0.08 });
document.querySelectorAll('.reveal').forEach(el => ro.observe(el));

/* ROUTE CANVAS ANIMATION */
(function() {
  const canvas = document.getElementById('route-canvas');
  if (!canvas) return;
  const ctx = canvas.getContext('2d');
  let W, H, nodes, packets, t = 0;

  function resize() {
    W = canvas.width = canvas.offsetWidth;
    H = canvas.height = canvas.offsetHeight;
    nodes = [
      { x: W*.16, y: H*.38, r: 6, c: '#d4a843', label: 'Toronto' },
      { x: W*.54, y: H*.28, r: 5, c: '#1fb899', label: 'Calgary' },
      { x: W*.84, y: H*.42, r: 5, c: '#6ba0f0', label: 'Vancouver' },
      { x: W*.26, y: H*.62, r: 4, c: '#e85c49', label: 'Montréal' },
      { x: W*.40, y: H*.20, r: 4, c: '#d4a843', label: 'Winnipeg' },
      { x: W*.70, y: H*.65, r: 3, c: '#a87fe8', label: 'Edmonton' },
    ];
    packets = [];
    const routes = [
      [0,1],[1,2],[0,3],[0,4],[1,4],[1,5],[2,5]
    ];
    routes.forEach(([a,b]) => {
      for (let i = 0; i < 2; i++) {
        packets.push({ from: a, to: b, p: Math.random(), speed: .001 + Math.random()*.0015, rev: i%2===1 });
      }
    });
  }

  resize();
  window.addEventListener('resize', resize);

  function lerp(a, b, t) { return a + (b - a) * t; }

  function draw() {
    ctx.clearRect(0, 0, W, H);

    // Draw route lines
    const routes = [[0,1],[1,2],[0,3],[0,4],[1,4],[1,5],[2,5]];
    routes.forEach(([a, b]) => {
      const na = nodes[a], nb = nodes[b];
      ctx.beginPath();
      ctx.moveTo(na.x, na.y);
      const mx = (na.x + nb.x) / 2, my = (na.y + nb.y) / 2 - 30;
      ctx.quadraticCurveTo(mx, my, nb.x, nb.y);
      ctx.strokeStyle = 'rgba(212,168,67,0.12)';
      ctx.lineWidth = 1;
      ctx.setLineDash([4, 6]);
      ctx.stroke();
      ctx.setLineDash([]);
    });

    // Draw nodes
    nodes.forEach(n => {
      // Outer ring
      ctx.beginPath();
      ctx.arc(n.x, n.y, n.r + 6 + Math.sin(t * 2) * 2, 0, Math.PI * 2);
      ctx.strokeStyle = n.c + '30';
      ctx.lineWidth = 1;
      ctx.stroke();
      // Node dot
      ctx.beginPath();
      ctx.arc(n.x, n.y, n.r, 0, Math.PI * 2);
      ctx.fillStyle = n.c;
      ctx.fill();
    });

    // Draw moving packets
    packets.forEach(pk => {
      const a = pk.rev ? pk.to : pk.from;
      const b = pk.rev ? pk.from : pk.to;
      const na = nodes[a], nb = nodes[b];
      const mx = (na.x + nb.x) / 2, my = (na.y + nb.y) / 2 - 30;
      const p = pk.p;
      // Bezier position
      const bx = (1-p)*(1-p)*na.x + 2*(1-p)*p*mx + p*p*nb.x;
      const by = (1-p)*(1-p)*na.y + 2*(1-p)*p*my + p*p*nb.y;
      ctx.beginPath();
      ctx.arc(bx, by, 2.5, 0, Math.PI * 2);
      ctx.fillStyle = nodes[a].c;
      ctx.globalAlpha = 0.85;
      ctx.fill();
      ctx.globalAlpha = 1;
      pk.p += pk.speed;
      if (pk.p > 1) pk.p = 0;
    });

    t += 0.01;
    requestAnimationFrame(draw);
  }

  draw();
})();

/* ── MODAL FUNCTIONS ── */
let currentModalType = 'consultation';

function openModal(type) {
  currentModalType = type;
  const modal = document.getElementById('inquiry-modal');
  const title = document.getElementById('modal-title');
  const subtitle = document.getElementById('modal-subtitle');
  const quoteExtras = document.getElementById('quote-extras');
  const msgLabel = document.getElementById('msg-label');
  const form = document.getElementById('modal-form');
  const success = document.getElementById('modal-success');
  const err = document.getElementById('modal-error');

  // Reset state
  form.style.display = 'block';
  success.style.display = 'none';
  err.style.display = 'none';
  document.getElementById('submit-text').textContent = 'Send Inquiry';
  document.getElementById('submit-icon').textContent = '📨';
  document.getElementById('modal-submit').disabled = false;
  document.getElementById('modal-submit').style.opacity = '1';

  if (type === 'quote') {
    title.textContent = 'Request a Rate Quote';
    subtitle.innerHTML = 'Tell us about your load and we\'ll have a <strong style="color:var(--fog)">competitive rate</strong> in your inbox within 30 minutes.';
    quoteExtras.style.display = 'block';
    msgLabel.textContent = 'Additional Load Details';
  } else {
    title.textContent = 'Book a Free Consultation';
    subtitle.innerHTML = 'Fill in your details and our team will reach out within <strong style="color:var(--fog)">2 business hours</strong> — guaranteed.';
    quoteExtras.style.display = 'none';
    msgLabel.textContent = 'Message / Questions';
  }

  modal.style.display = 'flex';
  document.body.style.overflow = 'hidden';
  // Re-trigger animation
  const box = document.getElementById('modal-box');
  box.style.animation = 'none';
  box.offsetHeight; // reflow
  box.style.animation = 'modalIn .4s cubic-bezier(.16,1,.3,1)';
}

function closeModal() {
  document.getElementById('inquiry-modal').style.display = 'none';
  document.body.style.overflow = '';
}

function closeModalOutside(e) {
  if (e.target === document.getElementById('inquiry-modal')) closeModal();
}

document.addEventListener('keydown', e => { if (e.key === 'Escape') closeModal(); });

function submitInquiry() {
  const first = document.getElementById('f-firstname').value.trim();
  const last  = document.getElementById('f-lastname').value.trim();
  const email = document.getElementById('f-email').value.trim();
  const company = document.getElementById('f-company').value.trim();
  const phone = document.getElementById('f-phone').value.trim();
  const message = document.getElementById('f-message').value.trim();
  const err = document.getElementById('modal-error');

  // Validation
  if (!first || !last) {
    showError('Please enter your first and last name.'); return;
  }
  if (!email || !email.includes('@')) {
    showError('Please enter a valid email address.'); return;
  }

  // Build email body
  let subject, body;
  if (currentModalType === 'quote') {
    const origin = document.getElementById('f-origin').value.trim();
    const dest   = document.getElementById('f-dest').value.trim();
    const equip  = document.getElementById('f-equip').value;
    const date   = document.getElementById('f-date').value;
    subject = `Rate Quote Request — ${first} ${last}${company ? ' · ' + company : ''}`;
    body = `RATE QUOTE REQUEST — FreightForward Canada\n` +
           `${'─'.repeat(50)}\n\n` +
           `Name:        ${first} ${last}\n` +
           `Company:     ${company || 'N/A'}\n` +
           `Email:       ${email}\n` +
           `Phone:       ${phone || 'N/A'}\n\n` +
           `SHIPMENT DETAILS\n` +
           `${'─'.repeat(50)}\n` +
           `Origin:      ${origin || 'N/A'}\n` +
           `Destination: ${dest || 'N/A'}\n` +
           `Equipment:   ${equip || 'N/A'}\n` +
           `Pickup Date: ${date || 'N/A'}\n\n` +
           `ADDITIONAL DETAILS\n` +
           `${'─'.repeat(50)}\n` +
           `${message || 'No additional details provided.'}\n\n` +
           `─────────────────────────────────────────────────\n` +
           `Submitted via FreightForward Canada Pitch Deck\n` +
           `Timestamp: ${new Date().toLocaleString('en-CA', {timeZone: 'America/Toronto'})} EST`;
  } else {
    subject = `Consultation Request — ${first} ${last}${company ? ' · ' + company : ''}`;
    body = `CONSULTATION REQUEST — FreightForward Canada\n` +
           `${'─'.repeat(50)}\n\n` +
           `Name:        ${first} ${last}\n` +
           `Company:     ${company || 'N/A'}\n` +
           `Email:       ${email}\n` +
           `Phone:       ${phone || 'N/A'}\n\n` +
           `MESSAGE\n` +
           `${'─'.repeat(50)}\n` +
           `${message || 'No message provided.'}\n\n` +
           `─────────────────────────────────────────────────\n` +
           `Submitted via FreightForward Canada Pitch Deck\n` +
           `Timestamp: ${new Date().toLocaleString('en-CA', {timeZone: 'America/Toronto'})} EST`;
  }

  // Loading state
  const btn = document.getElementById('modal-submit');
  document.getElementById('submit-icon').textContent = '⏳';
  document.getElementById('submit-text').textContent = 'Sending...';
  btn.disabled = true;
  btn.style.opacity = '.7';

  // Open mailto link
  const mailtoLink = `mailto:logistics@emirg-group.com?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(body)}`;
  window.location.href = mailtoLink;

  // Show success after brief delay (mailto will open email client)
  setTimeout(() => {
    document.getElementById('modal-form').style.display = 'none';
    document.getElementById('modal-success').style.display = 'block';
  }, 800);
}

function showError(msg) {
  const err = document.getElementById('modal-error');
  err.textContent = '⚠ ' + msg;
  err.style.display = 'block';
  err.scrollIntoView({ behavior: 'smooth', block: 'nearest' });
}

/* ── ANIMATE H-BARS ON SCROLL ── */
const hbarObs = new IntersectionObserver(entries => {
  entries.forEach(e => {
    if (e.isIntersecting) {
      e.target.querySelectorAll('.hb-fill').forEach(f => {
        const w = f.style.width;
        f.style.width = '0';
        setTimeout(() => {
          f.style.transition = 'width 1.1s cubic-bezier(.16,1,.3,1)';
          f.style.width = w;
        }, 100);
      });
    }
  });
}, { threshold: 0.2 });

document.querySelectorAll('.hbars').forEach(el => hbarObs.observe(el));
</script>
</body>
</html>
