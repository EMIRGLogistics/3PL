<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Network Toronto — A private social club for founders and operators</title>
<meta name="description" content="Network Toronto is a private social club for Toronto founders, operators and investors. Twelve-seat dinners, rooftop hours and quarterly deal nights. Membership by application and sponsor.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter+Tight:wght@500;600;700&family=Inter:wght@400;500;600&family=IBM+Plex+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
:root{
  --ink:#000000;
  --ink-1:#0b0d0f;
  --ink-2:#16191c;
  --bone:#f4f3ef;
  --muted:#a9b8bd;
  --glass:#5cc9bc;
  --glass-dim:#2c6d68;
  --brass:#d6ae68;
  --line:rgba(169,184,189,.2);
  --line-strong:rgba(169,184,189,.38);
  --display:"Inter Tight","Inter","Helvetica Neue",Helvetica,Arial,sans-serif;
  --body:"Inter","Helvetica Neue",Helvetica,Arial,sans-serif;
  --ui:"Inter","Helvetica Neue",Helvetica,Arial,sans-serif;
  --mono:"IBM Plex Mono",ui-monospace,SFMono-Regular,Menlo,monospace;
  --gut:clamp(20px,5vw,64px);
  --maxw:1180px;
}
*{box-sizing:border-box}
html{scroll-behavior:smooth;-webkit-text-size-adjust:100%}
body{
  margin:0;background:var(--ink);color:var(--bone);
  font-family:var(--body);font-size:17px;line-height:1.6;font-weight:400;
  text-rendering:optimizeLegibility;
  font-synthesis:none;
  overflow-x:hidden;
}
img{max-width:100%;display:block}
a{color:inherit}
:focus-visible{outline:2px solid var(--glass);outline-offset:3px;border-radius:2px}
::selection{background:var(--glass);color:var(--ink)}

/* ---------- primitives ---------- */
.wrap{max-width:var(--maxw);margin:0 auto;padding-left:var(--gut);padding-right:var(--gut)}
.eyebrow{
  font-family:var(--mono);font-size:11px;letter-spacing:.22em;text-transform:uppercase;
  color:var(--glass);margin:0 0 22px;display:flex;align-items:center;gap:12px;
}
.eyebrow::after{content:"";flex:1;height:1px;background:var(--line);max-width:180px}
.eyebrow.center{justify-content:center}
.eyebrow.center::after{display:none}
h1,h2,h3{font-family:var(--display);font-weight:600;margin:0;line-height:1.08;letter-spacing:-.028em}
h2{font-size:clamp(32px,4.6vw,54px)}
h3{font-size:22px;line-height:1.2}
p{margin:0 0 1em}
.lede{font-size:clamp(17px,1.7vw,20px);color:var(--muted);max-width:56ch;line-height:1.65}
.rule{height:1px;background:var(--line);border:0;margin:0}

.btn{
  display:inline-flex;align-items:center;gap:10px;
  font-family:var(--mono);font-size:12px;letter-spacing:.16em;text-transform:uppercase;
  padding:15px 26px;border-radius:2px;text-decoration:none;cursor:pointer;border:1px solid transparent;
  transition:background .25s ease,color .25s ease,border-color .25s ease,transform .25s ease;
}
.btn-solid{background:var(--brass);color:#1b1206;font-weight:500}
.btn-solid:hover{background:#dbb673;transform:translateY(-2px)}
.btn-ghost{border-color:var(--line-strong);color:var(--bone)}
.btn-ghost:hover{border-color:var(--glass);color:var(--glass)}

/* ---------- header ---------- */
.hdr{
  position:fixed;top:0;left:0;right:0;z-index:60;
  transition:background .35s ease,border-color .35s ease,backdrop-filter .35s ease;
  border-bottom:1px solid transparent;
  background:linear-gradient(to bottom,rgba(0,0,0,.75) 0%,rgba(0,0,0,0) 100%);
}
.hdr.stuck{background:rgba(0,0,0,.92);backdrop-filter:blur(14px);border-bottom-color:var(--line)}
.hdr-in{display:flex;align-items:center;justify-content:space-between;gap:24px;height:80px}
.mark{display:flex;align-items:center;gap:12px;text-decoration:none}
.mark-mono{
  width:30px;height:30px;border:1px solid var(--brass);color:var(--brass);
  display:grid;place-items:center;font-family:var(--ui);font-weight:600;font-size:14px;flex:none;
}
.mark-txt{font-family:var(--ui);font-size:15px;font-weight:600;letter-spacing:.02em;color:var(--bone)}
.nav{display:flex;align-items:center;gap:34px}
.nav a{
  font-family:var(--ui);font-size:15px;font-weight:500;letter-spacing:-.005em;
  text-decoration:none;color:#e2e9eb;transition:color .2s ease;
}
.nav a:hover{color:var(--glass)}
.hdr .btn{padding:11px 22px;font-family:var(--ui);font-size:14px;font-weight:600;letter-spacing:0;text-transform:none}
@media(max-width:900px){.nav{display:none}}

/* ---------- hero ---------- */
.hero{position:relative;min-height:100svh;display:flex;align-items:center;padding:120px 0 60px;overflow:hidden}
#web{position:absolute;inset:0;width:100%;height:100%;z-index:0}
.hero::after{
  content:"";position:absolute;inset:0;z-index:1;pointer-events:none;
  background:radial-gradient(120% 85% at 15% 40%,rgba(0,0,0,.3) 0%,rgba(0,0,0,.86) 60%,#000 100%);
}
.hero-in{position:relative;z-index:2;width:100%}
.hero h1{font-size:clamp(40px,7.4vw,88px);max-width:15ch;margin-bottom:26px}
.hero h1 em{font-style:normal;color:var(--brass)}
.hero .lede{max-width:50ch;margin-bottom:34px}
.hero-cta{display:flex;flex-wrap:wrap;gap:14px;align-items:center}
.hero-note{font-family:var(--mono);font-size:11px;letter-spacing:.14em;color:var(--muted);text-transform:uppercase}

/* ---------- sections ---------- */
.sect{padding:clamp(80px,11vw,140px) 0;position:relative}
.sect-alt{background:var(--ink-1)}
.sect-bone{background:var(--bone);color:#0c1b24}
.sect-bone .lede{color:#4a5f68}
.sect-bone .eyebrow{color:var(--glass-dim)}
.sect-bone .eyebrow::after{background:rgba(12,27,36,.18)}
.hd{display:flex;justify-content:space-between;align-items:flex-end;gap:40px;flex-wrap:wrap;margin-bottom:clamp(40px,6vw,68px)}
.hd h2{max-width:16ch}
.hd .lede{max-width:38ch;margin:0}

/* ledger */
.ledger{border-top:1px solid var(--line)}
.led-row{
  display:grid;grid-template-columns:92px 1fr 1fr 1.15fr;gap:clamp(12px,2.5vw,28px);align-items:center;
  padding:20px 4px;border-bottom:1px solid var(--line);transition:background .25s ease,padding-left .25s ease;
}
.led-row:hover{background:rgba(92,201,188,.06);padding-left:14px}
.led-row .when{font-family:var(--mono);font-size:11px;letter-spacing:.14em;text-transform:uppercase;color:var(--glass)}
.led-row .who{font-size:15.5px;color:var(--bone)}
.led-row .res{font-family:var(--display);font-weight:500;font-size:17px;letter-spacing:-.012em;color:var(--brass)}
@media(max-width:820px){
  .led-row{grid-template-columns:1fr;gap:6px;padding:20px 0}
  .led-row .res{margin-top:6px}
  .led-row:hover{padding-left:0}
}
.stats{display:grid;grid-template-columns:repeat(3,1fr);gap:2px;margin-top:56px;background:var(--line)}
.stat{background:var(--ink);padding:26px 22px}
.sect-alt .stat{background:var(--ink-1)}
.stat b{display:block;font-family:var(--display);font-size:clamp(30px,3.6vw,42px);font-weight:600;line-height:1;letter-spacing:-.035em;margin-bottom:10px}
.stat span{font-family:var(--mono);font-size:10.5px;letter-spacing:.16em;text-transform:uppercase;color:var(--muted)}
@media(max-width:700px){.stats{grid-template-columns:1fr 1fr}}

/* events */
.events{display:grid;grid-template-columns:repeat(auto-fit,minmax(300px,1fr));gap:2px;background:var(--line)}
.grid-2{grid-template-columns:repeat(2,1fr)}
@media(max-width:640px){.grid-2{grid-template-columns:1fr}}
.ev{
  background:var(--ink);padding:clamp(28px,3.4vw,40px);position:relative;
  transition:background .3s ease,transform .3s ease;display:flex;flex-direction:column;
}
.ev:hover{background:var(--ink-2);transform:translateY(-3px)}
.ev .cad{
  font-family:var(--mono);font-size:10.5px;letter-spacing:.2em;text-transform:uppercase;color:var(--glass);
  display:flex;justify-content:space-between;gap:12px;margin-bottom:26px;
}
.ev .cad span:last-child{color:var(--muted)}
.ev h3{margin-bottom:14px}
.ev p{color:var(--muted);font-size:15.5px;margin:0}
.ev .where{
  margin-top:24px;padding-top:16px;border-top:1px solid var(--line);
  font-family:var(--mono);font-size:11px;letter-spacing:.1em;color:var(--brass);
}
.ev-wide{grid-column:span 2}
@media(max-width:700px){.ev-wide{grid-column:span 1}}

/* steps */
.steps{display:grid;grid-template-columns:repeat(auto-fit,minmax(230px,1fr));gap:clamp(24px,3vw,40px)}
.step{border-top:1px solid rgba(12,27,36,.2);padding-top:22px}
.step .num{font-family:var(--mono);font-size:11px;letter-spacing:.2em;color:var(--glass-dim);display:block;margin-bottom:16px}
.step h3{font-size:20px;margin-bottom:10px}
.step p{font-size:15px;color:#4a5f68;margin:0}

/* membership */
.tiers{display:grid;grid-template-columns:repeat(auto-fit,minmax(270px,1fr));gap:clamp(18px,2.4vw,26px);margin-top:8px}
.tier{border:1px solid rgba(12,27,36,.16);padding:clamp(26px,3vw,34px);display:flex;flex-direction:column;background:rgba(255,255,255,.32)}
.tier.feature{background:#0c1b24;color:var(--bone);border-color:#0c1b24;position:relative}
.tier .name{font-family:var(--mono);font-size:11px;letter-spacing:.2em;text-transform:uppercase;color:var(--glass-dim);margin-bottom:20px}
.tier.feature .name{color:var(--brass)}
.tier .dues{font-family:var(--display);font-weight:600;font-size:40px;line-height:1;letter-spacing:-.035em;margin-bottom:6px}
.tier .per{font-family:var(--mono);font-size:11px;letter-spacing:.14em;text-transform:uppercase;color:#6d838c;margin-bottom:24px}
.tier.feature .per{color:var(--muted)}
.tier ul{list-style:none;margin:0 0 28px;padding:0;flex:1}
.tier li{padding:11px 0 11px 22px;border-top:1px solid rgba(12,27,36,.1);font-size:15px;position:relative}
.tier.feature li{border-top-color:rgba(169,184,189,.2)}
.tier li::before{content:"";position:absolute;left:0;top:19px;width:7px;height:7px;border:1px solid var(--glass-dim);transform:rotate(45deg)}
.tier.feature li::before{border-color:var(--brass)}
.tier .btn{justify-content:center}
.tier .cap{
  position:absolute;top:-1px;right:-1px;background:var(--brass);color:#1b1206;
  font-family:var(--mono);font-size:10px;letter-spacing:.16em;text-transform:uppercase;padding:6px 12px;
}

/* faq */
.faq{border-top:1px solid var(--line)}
.qa{border-bottom:1px solid var(--line)}
.qa summary{
  cursor:pointer;list-style:none;padding:24px 44px 24px 0;position:relative;
  font-family:var(--display);font-weight:500;font-size:clamp(18px,2vw,21px);letter-spacing:-.018em;transition:color .2s ease;
}
.qa summary::-webkit-details-marker{display:none}
.qa summary:hover{color:var(--glass)}
.qa summary::after{
  content:"+";position:absolute;right:6px;top:50%;transform:translateY(-50%);
  font-family:var(--mono);font-size:20px;color:var(--glass);transition:transform .25s ease;
}
.qa[open] summary::after{content:"–"}
.qa p{color:var(--muted);max-width:70ch;padding-right:44px;margin:0 0 24px;font-size:16px}

/* apply */
.apply-grid{display:grid;grid-template-columns:.85fr 1.15fr;gap:clamp(32px,5vw,72px);align-items:start}
@media(max-width:860px){.apply-grid{grid-template-columns:1fr}}
.form{display:grid;grid-template-columns:1fr 1fr;gap:18px}
.f-full{grid-column:1/-1}
label{display:block;font-family:var(--mono);font-size:10.5px;letter-spacing:.18em;text-transform:uppercase;color:var(--muted);margin-bottom:9px}
input,select,textarea{
  width:100%;background:transparent;border:1px solid var(--line);color:var(--bone);
  font-family:var(--body);font-size:16px;padding:13px 14px;border-radius:2px;transition:border-color .2s ease,background .2s ease;
}
textarea{resize:vertical;min-height:110px}
input:focus,select:focus,textarea:focus{border-color:var(--glass);background:rgba(92,201,188,.06);outline:none}
select{appearance:none;background-image:linear-gradient(45deg,transparent 50%,var(--glass) 50%),linear-gradient(135deg,var(--glass) 50%,transparent 50%);background-position:calc(100% - 20px) 22px,calc(100% - 14px) 22px;background-size:6px 6px;background-repeat:no-repeat}
select option{background:var(--ink-1);color:var(--bone)}
.err{border-color:#d4735f !important}
.form-note{font-family:var(--mono);font-size:11px;color:var(--muted);letter-spacing:.06em;line-height:1.6}
.sent{border:1px solid var(--glass);padding:38px;border-radius:3px;background:rgba(92,201,188,.07)}
.sent h3{color:var(--glass);margin-bottom:12px;font-size:26px}
.sent p{color:var(--muted);margin:0}
.contact-line{display:flex;flex-direction:column;gap:14px;margin-top:32px;padding-top:28px;border-top:1px solid var(--line)}
.contact-line a{font-family:var(--mono);font-size:12px;letter-spacing:.1em;color:var(--glass);text-decoration:none}
.contact-line a:hover{text-decoration:underline}

/* footer */
.ftr{background:var(--ink);border-top:1px solid var(--line);padding:70px 0 40px}
.ftr-in{display:grid;grid-template-columns:1.4fr 1fr 1fr;gap:40px}
@media(max-width:760px){.ftr-in{grid-template-columns:1fr 1fr}.ftr-brand{grid-column:1/-1}}
.ftr h4{font-family:var(--mono);font-size:10.5px;letter-spacing:.2em;text-transform:uppercase;color:var(--muted);margin:0 0 18px;font-weight:400}
.ftr ul{list-style:none;margin:0;padding:0;display:grid;gap:11px}
.ftr a{font-size:14.5px;text-decoration:none;color:var(--bone);opacity:.8;transition:opacity .2s ease,color .2s ease}
.ftr a:hover{opacity:1;color:var(--glass)}
.ftr-brand p{color:var(--muted);font-size:14.5px;max-width:34ch;margin:18px 0 0}
.ftr-btm{
  display:flex;justify-content:space-between;gap:20px;flex-wrap:wrap;margin-top:56px;padding-top:24px;border-top:1px solid var(--line);
  font-family:var(--mono);font-size:10.5px;letter-spacing:.14em;text-transform:uppercase;color:var(--muted);
}

/* reveal */
.rv{opacity:0;transform:translateY(22px);transition:opacity .8s cubic-bezier(.2,.7,.3,1),transform .8s cubic-bezier(.2,.7,.3,1)}
.rv.in{opacity:1;transform:none}
@media(prefers-reduced-motion:reduce){
  *{animation:none !important;transition:none !important;scroll-behavior:auto !important}
  .rv{opacity:1;transform:none}
}
</style>
</head>
<body>

<header class="hdr" id="hdr">
  <div class="wrap hdr-in">
    <a class="mark" href="#top" aria-label="Network Toronto, home">
      <span class="mark-mono" aria-hidden="true">N</span>
      <span class="mark-txt">Network Toronto</span>
    </a>
    <nav class="nav" aria-label="Main">
      <a href="#club">The club</a>
      <a href="#evenings">Evenings</a>
      <a href="#ledger">The ledger</a>
      <a href="#membership">Membership</a>
      <a href="#faq">Questions</a>
    </nav>
    <a class="btn btn-solid" href="#apply">Apply</a>
  </div>
</header>

<main id="top">

<!-- HERO -->
<section class="hero">
  <canvas id="web" aria-hidden="true"></canvas>
  <div class="wrap hero-in">
    <p class="eyebrow">Toronto, Ontario · By application · Est. 2023</p>
    <h1>Toronto is a small city, <em>once you know the right forty people.</em></h1>
    <p class="lede">A private social club for founders, operators and the people who fund them. Twelve seats at a long table, a rooftop in July, and a room where nobody is wearing a name tag.</p>
    <div class="hero-cta">
      <a class="btn btn-solid" href="#apply">Request membership</a>
      <a class="btn btn-ghost" href="#evenings">See the calendar</a>
      <span class="hero-note">10 seats open, starting Feb 2027</span>
    </div>

  </div>
</section>

<!-- THE CLUB -->
<section class="sect sect-alt" id="club">
  <div class="wrap">
    <div class="hd rv">
      <div>
        <p class="eyebrow">What this is</p>
        <h2>Not a networking event. A club that happens to be useful.</h2>
      </div>
      <p class="lede">Most rooms in this city sell you a ticket, hand you a lanyard and let you fend for yourself. We seat you. We know what you're building. We know who else is in the room.</p>
    </div>

    <div class="events grid-2 rv">
      <article class="ev">
        <div class="cad"><span>Principle 01</span><span>Seating</span></div>
        <h3>Every seat is assigned</h3>
        <p>Nobody sits beside a competitor, and nobody sits beside the person they came with. The seating chart is the product.</p>
      </article>
      <article class="ev">
        <div class="cad"><span>Principle 02</span><span>Scale</span></div>
        <h3>Small on purpose</h3>
        <p>Dinners cap at twelve, and the membership is capped too. When we grow, we grow the calendar — not the room.</p>
      </article>
      <article class="ev">
        <div class="cad"><span>Principle 03</span><span>Discretion</span></div>
        <h3>Nothing leaves the table</h3>
        <p>No photography at dinners, no press, no recording. Members talk about live deals here because they can.</p>
      </article>
      <article class="ev">
        <div class="cad"><span>Principle 04</span><span>Reciprocity</span></div>
        <h3>Give before you take</h3>
        <p>The committee tracks introductions made, not just attended. Members who only collect don't get renewed.</p>
      </article>
    </div>
  </div>
</section>

<!-- EVENINGS -->
<section class="sect" id="evenings">
  <div class="wrap">
    <div class="hd rv">
      <div>
        <p class="eyebrow">The calendar</p>
        <h2>Five formats, roughly thirty nights a year.</h2>
      </div>
      <p class="lede">Each format does one job. Members pick the ones that fit the season they're in.</p>
    </div>

    <div class="events rv">
      <article class="ev">
        <div class="cad"><span>Monthly</span><span>12 seats</span></div>
        <h3>The Round Table</h3>
        <p>One long table, one question, and a chef cooking a few feet away while you argue about it. Seats assigned by the committee the morning of.</p>
        <div class="where">Private room · Distillery District</div>
      </article>
      <article class="ev">
        <div class="cad"><span>May – September</span><span>60 guests</span></div>
        <h3>Harbour Hours</h3>
        <p>Sunset to close on a rooftop over the lake. The only evening where members bring guests freely — bring the person you've been meaning to introduce.</p>
        <div class="where">Rooftop terrace · Harbourfront</div>
      </article>
      <article class="ev">
        <div class="cad"><span>Six times a year</span><span>30 guests</span></div>
        <h3>The Cellar</h3>
        <p>One operator tells the whole story of one deal — the ugly middle included — off the record and unedited. Whisky, then questions until they run out.</p>
        <div class="where">Lower bar · Yorkville</div>
      </article>
      <article class="ev">
        <div class="cad"><span>Quarterly</span><span>Members + 1</span></div>
        <h3>The Exchange</h3>
        <p>Bring the thing you're stuck on, written on a card. Ninety minutes later you leave with three names and a reason each one will take your call.</p>
        <div class="where">Boardroom floor · Financial District</div>
      </article>
      <article class="ev ev-wide">
        <div class="cad"><span>Once a year</span><span>24 members</span></div>
        <h3>Off-Book</h3>
        <p>Two nights out of the city in Prince Edward County. No agenda, no programming, no phones at dinner. Members consistently rate it the reason they renew.</p>
        <div class="where">Country house · Prince Edward County · Applications open in March</div>
      </article>
    </div>
  </div>
</section>

<!-- LEDGER -->
<section class="sect sect-alt" id="ledger">
  <div class="wrap">
    <div class="hd rv">
      <div>
        <p class="eyebrow">The ledger</p>
        <h2>What actually came of it.</h2>
      </div>
      <p class="lede">A running record of introductions the club made, kept deliberately vague about who — and deliberately specific about what happened next.</p>
    </div>

    <div class="ledger rv">
      <div class="led-row">
        <span class="when">Jun 2026</span>
        <span class="who">Founder, logistics software</span>
        <span class="who">Partner, growth fund</span>
        <span class="res">A term sheet, eleven weeks later.</span>
      </div>
      <div class="led-row">
        <span class="when">May 2026</span>
        <span class="who">Restaurateur, three rooms on Ossington</span>
        <span class="who">Retail leasing lawyer</span>
        <span class="res">A fourth room, on Queen West.</span>
      </div>
      <div class="led-row">
        <span class="when">Apr 2026</span>
        <span class="who">Fractional CFO</span>
        <span class="who">Manufacturer scaling past $20M</span>
        <span class="res">A finance function, built in ninety days.</span>
      </div>
      <div class="led-row">
        <span class="when">Mar 2026</span>
        <span class="who">Design studio owner</span>
        <span class="who">CPG founder, national grocery launch</span>
        <span class="res">A rebrand, and a shelf.</span>
      </div>
      <div class="led-row">
        <span class="when">Feb 2026</span>
        <span class="who">Clinic group, four locations</span>
        <span class="who">Health tech founder</span>
        <span class="res">A pilot, then a purchase order.</span>
      </div>
      <div class="led-row">
        <span class="when">Jan 2026</span>
        <span class="who">Second-time founder, exited 2024</span>
        <span class="who">Two operators between things</span>
        <span class="res">A founding team, assembled over dinner.</span>
      </div>
    </div>

    <div class="stats rv">
      <div class="stat"><b>30</b><span>Nights a year</span></div>
      <div class="stat"><b>55</b><span>Introductions made</span></div>
      <div class="stat"><b>63%</b><span>Founders &amp; owners</span></div>
    </div>
  </div>
</section>

<!-- MEMBERSHIP + STEPS (inverted) -->
<section class="sect sect-bone" id="membership">
  <div class="wrap">
    <div class="hd rv">
      <div>
        <p class="eyebrow">Membership</p>
        <h2>Dues, and what they buy.</h2>
      </div>
      <p class="lede">Annual, billed once. Dues cover food, rooms and staff — the club takes no sponsorship money, because sponsors change who's in the room.</p>
    </div>

    <div class="tiers rv">
      <div class="tier">
        <div class="name">Associate</div>
        <div class="dues">$1,200</div>
        <div class="per">per year</div>
        <ul>
          <li>For businesses under three years old</li>
          <li>Harbour Hours and The Exchange</li>
          <li>Two Round Table seats a year</li>
          <li>Member directory access</li>
        </ul>
        <a class="btn btn-ghost" href="#apply" style="border-color:rgba(12,27,36,.25);color:#0c1b24">Apply as associate</a>
      </div>
      <div class="tier feature">
        <span class="cap">Most members</span>
        <div class="name">Full member</div>
        <div class="dues">$2,800</div>
        <div class="per">per year</div>
        <ul>
          <li>The entire calendar, every format</li>
          <li>Priority seating at Round Tables</li>
          <li>Two guest passes each quarter</li>
          <li>Direct introductions from the committee</li>
          <li>Eligible for Off-Book</li>
        </ul>
        <a class="btn btn-solid" href="#apply">Apply for membership</a>
      </div>
      <div class="tier">
        <span class="cap">40 seats</span>
        <div class="name">Founding Circle</div>
        <div class="dues">$7,500</div>
        <div class="per">per year</div>
        <ul>
          <li>Everything in full membership</li>
          <li>Host your own Round Table</li>
          <li>Concierge introductions, on request</li>
          <li>Reciprocal access to partner clubs</li>
          <li>A voice in who gets admitted</li>
        </ul>
        <a class="btn btn-ghost" href="#apply" style="border-color:rgba(12,27,36,.25);color:#0c1b24">Enquire about the circle</a>
      </div>
    </div>

    <div class="rv" style="margin-top:clamp(64px,8vw,100px)">
      <p class="eyebrow">Getting in</p>
      <h2 style="max-width:18ch;margin-bottom:clamp(36px,5vw,56px)">Four steps, about thirty days.</h2>
      <div class="steps">
        <div class="step">
          <span class="num">01 / Apply</span>
          <h3>Tell us what you're building</h3>
          <p>Ten minutes. What you run, what you're looking for, and who you could help.</p>
        </div>
        <div class="step">
          <span class="num">02 / Conversation</span>
          <h3>Coffee with the committee</h3>
          <p>Half an hour, in person where we can. It's a conversation, not an interview.</p>
        </div>
        <div class="step">
          <span class="num">03 / Sponsorship</span>
          <h3>A member vouches</h3>
          <p>If you don't know one yet, we'll seat you at an open evening so you can.</p>
        </div>
        <div class="step">
          <span class="num">04 / Decision</span>
          <h3>The committee votes</h3>
          <p>We meet the first Tuesday monthly. You'll hear either way within thirty days.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- FAQ -->
<section class="sect sect-alt" id="faq">
  <div class="wrap">
    <div class="hd rv">
      <div>
        <p class="eyebrow">Questions</p>
        <h2>Before you apply.</h2>
      </div>
    </div>
    <div class="faq rv">
      <details class="qa">
        <summary>Do I need to know a member already?</summary>
        <p>It helps, but no. About a third of members joined without a sponsor — we seat those applicants at an open evening first so they can meet a few people properly before the vote.</p>
      </details>
      <details class="qa">
        <summary>Is this a pitch event?</summary>
        <p>Pitching from a stage is banned. Pitching over dinner is what dinner is for. The difference matters: nobody performs here, but nobody pretends they aren't looking for something either.</p>
      </details>
      <details class="qa">
        <summary>What's the real time commitment?</summary>
        <p>Most members come to eight or nine evenings a year. Come to fewer than three and the club stops working for you — the value compounds with the number of people who recognise you.</p>
      </details>
      <details class="qa">
        <summary>Can I bring a guest?</summary>
        <p>Full members get two guest passes a quarter, plus open guest privileges at Harbour Hours. Guests can attend twice before they need to apply themselves.</p>
      </details>
      <details class="qa">
        <summary>I'm not in Toronto full time. Is it worth it?</summary>
        <p>Several members are based in Montreal, Calgary and New York and plan trips around the calendar. Tell us on your application and we'll flag the dates worth flying in for.</p>
      </details>
      <details class="qa">
        <summary>What if I'm not admitted?</summary>
        <p>You'll get a real answer about why, and an invitation to reapply when something changes. Roughly one in five applicants is admitted on a first application; a third of those declined and reapplied later got in.</p>
      </details>
      <details class="qa">
        <summary>Are dues refundable?</summary>
        <p>Dues are billed once a year and refundable pro rata within the first sixty days. After that we've already booked the rooms.</p>
      </details>
    </div>
  </div>
</section>

<!-- APPLY -->
<section class="sect" id="apply">
  <div class="wrap apply-grid">
    <div class="rv">
      <p class="eyebrow">Apply</p>
      <h2 style="margin-bottom:22px">Ten minutes, and then we'll talk.</h2>
      <p class="lede">The committee reviews applications the first Tuesday of every month. The more specific you are about what you're looking for, the better we can seat you.</p>
      <div class="contact-line">
        <a href="#evenings">Come to an open evening first</a>
        <a href="#faq">Read the questions members ask</a>
      </div>
    </div>

    <div class="rv">
      <div class="form" id="formWrap">
        <div>
          <label for="fn">First name</label>
          <input id="fn" name="fn" type="text" autocomplete="given-name" required>
        </div>
        <div>
          <label for="ln">Last name</label>
          <input id="ln" name="ln" type="text" autocomplete="family-name" required>
        </div>
        <div>
          <label for="em">Email</label>
          <input id="em" name="em" type="email" autocomplete="email" required>
        </div>
        <div>
          <label for="co">Company</label>
          <input id="co" name="co" type="text" autocomplete="organization">
        </div>
        <div>
          <label for="ro">Your role</label>
          <input id="ro" name="ro" type="text" placeholder="Founder, partner, operator…">
        </div>
        <div>
          <label for="ti">Membership</label>
          <select id="ti" name="ti">
            <option>Full member — $2,800</option>
            <option>Associate — $1,200</option>
            <option>Founding Circle — $7,500</option>
            <option>Not sure yet</option>
          </select>
        </div>
        <div class="f-full">
          <label for="lk">LinkedIn or website</label>
          <input id="lk" name="lk" type="text" placeholder="linkedin.com/in/…">
        </div>
        <div class="f-full">
          <label for="wh">What are you looking for this year?</label>
          <textarea id="wh" name="wh" placeholder="Capital, a co-founder, a first enterprise customer, an operator who has done this before…"></textarea>
        </div>
        <div class="f-full">
          <label for="sp">Sponsoring member, if you have one</label>
          <input id="sp" name="sp" type="text" placeholder="Leave blank and we'll seat you at an open evening">
        </div>
        <div class="f-full" style="display:flex;flex-wrap:wrap;gap:20px;align-items:center;margin-top:6px">
          <button class="btn btn-solid" id="submitBtn" type="button">Send application</button>
          <span class="form-note">Reviewed the first Tuesday of the month.<br>We reply either way within 30 days.</span>
        </div>
      </div>
      <div class="sent" id="sent" hidden>
        <h3>Application received</h3>
        <p>Thank you. The committee meets the first Tuesday of the month, and you'll hear from us either way within thirty days. If an open evening comes up before then, we'll send you a seat.</p>
      </div>
    </div>
  </div>
</section>

</main>

<footer class="ftr">
  <div class="wrap">
    <div class="ftr-in">
      <div class="ftr-brand">
        <a class="mark" href="#top">
          <span class="mark-mono" aria-hidden="true">N</span>
          <span class="mark-txt">Network Toronto</span>
        </a>
        <p>A private social club for founders, operators and investors. Toronto, Ontario.</p>
      </div>
      <div>
        <h4>The club</h4>
        <ul>
          <li><a href="#club">What this is</a></li>
          <li><a href="#evenings">Evenings</a></li>
          <li><a href="#ledger">The ledger</a></li>
          <li><a href="#membership">Membership</a></li>
        </ul>
      </div>
      <div>
        <h4>Elsewhere</h4>
        <ul>
          <li><a href="#evenings">Open evenings</a></li>
          <li><a href="#apply">Apply</a></li>
          <li><a href="#faq">Questions</a></li>
          <li><a href="#top">House rules</a></li>
        </ul>
      </div>
    </div>
    <div class="ftr-btm">
      <span>© 2026 Network Toronto</span>
      <span>Nothing said at the table leaves the table</span>
    </div>
  </div>
</footer>

<script>
(function(){
  var reduce = window.matchMedia('(prefers-reduced-motion: reduce)').matches;

  /* header state */
  var hdr = document.getElementById('hdr');
  function onScroll(){ hdr.classList.toggle('stuck', window.scrollY > 24); }
  onScroll(); window.addEventListener('scroll', onScroll, {passive:true});

  /* reveal on scroll */
  var els = document.querySelectorAll('.rv');
  if('IntersectionObserver' in window && !reduce){
    var io = new IntersectionObserver(function(entries){
      entries.forEach(function(e){ if(e.isIntersecting){ e.target.classList.add('in'); io.unobserve(e.target); } });
    },{threshold:.12, rootMargin:'0px 0px -60px'});
    els.forEach(function(el){ io.observe(el); });
  } else {
    els.forEach(function(el){ el.classList.add('in'); });
  }

  /* hero network canvas */
  var cv = document.getElementById('web');
  if(cv && cv.getContext){
    var ctx = cv.getContext('2d'), pts = [], raf, w, h, dpr;
    function build(){
      dpr = Math.min(window.devicePixelRatio || 1, 2);
      w = cv.offsetWidth; h = cv.offsetHeight;
      cv.width = w * dpr; cv.height = h * dpr;
      ctx.setTransform(dpr,0,0,dpr,0,0);
      var n = Math.min(52, Math.max(18, Math.round((w*h)/26000)));
      pts = [];
      for(var k=0;k<n;k++){
        pts.push({x:Math.random()*w, y:Math.random()*h, vx:(Math.random()-.5)*.22, vy:(Math.random()-.5)*.22, r:Math.random()*1.6+.8});
      }
    }
    function draw(){
      ctx.clearRect(0,0,w,h);
      for(var a=0;a<pts.length;a++){
        var p = pts[a];
        if(!reduce){ p.x += p.vx; p.y += p.vy; }
        if(p.x < -20) p.x = w+20; if(p.x > w+20) p.x = -20;
        if(p.y < -20) p.y = h+20; if(p.y > h+20) p.y = -20;
        for(var b=a+1;b<pts.length;b++){
          var q = pts[b], dx = p.x-q.x, dy = p.y-q.y, d = Math.sqrt(dx*dx+dy*dy);
          if(d < 165){
            ctx.strokeStyle = 'rgba(92,201,188,' + (0.2 * (1 - d/165)).toFixed(3) + ')';
            ctx.lineWidth = 1;
            ctx.beginPath(); ctx.moveTo(p.x,p.y); ctx.lineTo(q.x,q.y); ctx.stroke();
          }
        }
        ctx.fillStyle = 'rgba(214,174,104,.5)';
        ctx.beginPath(); ctx.arc(p.x,p.y,p.r,0,Math.PI*2); ctx.fill();
      }
      if(!reduce) raf = requestAnimationFrame(draw);
    }
    build(); draw();
    var t;
    window.addEventListener('resize', function(){
      clearTimeout(t);
      t = setTimeout(function(){ cancelAnimationFrame(raf); build(); draw(); }, 200);
    });
  }

  /* application form */
  var btn = document.getElementById('submitBtn'),
      formWrap = document.getElementById('formWrap'),
      sent = document.getElementById('sent');
  btn.addEventListener('click', function(){
    var required = ['fn','ln','em'], ok = true, first = null;
    required.forEach(function(id){
      var el = document.getElementById(id), good = el.value.trim() !== '';
      if(id === 'em') good = good && /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(el.value.trim());
      el.classList.toggle('err', !good);
      if(!good){ ok = false; if(!first) first = el; }
    });
    if(!ok){ first.focus(); return; }
    formWrap.hidden = true;
    sent.hidden = false;
    sent.scrollIntoView({block:'center', behavior: reduce ? 'auto' : 'smooth'});
  });
})();
</script>
</body>
</html>
