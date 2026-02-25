<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>EMIRG Logistics | Canadian Freight Brokerage Solutions</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>
:root{
--black:#0d0d0d;
--gold:#C6A75E;
--gray:#9a9a9a;
--light-gray:#cfcfcf;
--divider:rgba(255,255,255,0.06);
--hover-scale:1.03;
}

*{margin:0; padding:0; box-sizing:border-box; font-family:'Inter',sans-serif; scroll-behavior:smooth;}
body{background:var(--black); color:white; line-height:1.6;}
.container{width:88%; max-width:1100px; margin:auto;}

/* HEADER */
header{position:fixed; top:0; width:100%; background:rgba(13,13,13,0.97); border-bottom:1px solid var(--divider); z-index:1000;}
.nav-wrapper{display:flex; justify-content:space-between; align-items:center; height:85px;}
.logo{font-weight:700; letter-spacing:1px; font-size:1.4rem; color:white;}
.logo span{color:var(--gold);}
nav ul{display:flex; gap:42px; list-style:none; align-items:center; height:100%;}
nav li{display:flex; align-items:center; height:100%;}
nav a{position:relative; text-decoration:none; color:var(--light-gray); font-weight:500; font-size:0.9rem; padding:8px 0; transition:all 0.3s ease;}
nav a::after{content:''; position:absolute; left:0; bottom:-6px; width:0; height:2px; background:var(--gold); transition:width 0.3s ease;}
nav a:hover{color:white; transform:translateY(-1px);}
nav a:hover::after{width:100%;}

/* HERO */
.hero{position:relative; padding-top:180px; padding-bottom:140px; border-bottom:1px solid var(--divider); overflow:hidden;}
#networkCanvas{position:absolute; top:0; left:0; width:100%; height:100%; z-index:0; opacity:0.15;}
.hero .container{position:relative; z-index:2;}
.hero h1{font-size:2.4rem; font-weight:600; margin-bottom:25px;}
.hero p{color:var(--gray); max-width:650px; margin-bottom:35px;}
.cta-btn{display:inline-block; padding:14px 36px; border:1px solid var(--gold); color:var(--gold); text-decoration:none; font-weight:600; font-size:0.85rem; letter-spacing:0.5px; transition:all 0.3s ease; background:none; cursor:pointer;}
.cta-btn:hover{background:var(--gold); color:black; transform:scale(var(--hover-scale));}

/* SECTIONS */
section{padding:120px 0; border-bottom:1px solid var(--divider);}
.section-title{font-size:1.8rem; font-weight:600; margin-bottom:60px;}
.grid{display:grid; grid-template-columns:repeat(auto-fit,minmax(260px,1fr)); gap:50px;}
.card{padding-top:10px; transition:all 0.5s ease; transform:translateY(20px) scale(0.98); opacity:0;}
.card.visible{transform:translateY(0) scale(1); opacity:1;}
.card h3{font-weight:600; margin-bottom:12px;}
.card p{color:var(--gray); margin-bottom:12px;}
.metric{color:var(--gold); font-weight:600; font-size:0.9rem;}

/* REVIEWS */
.review{background:#141414; padding:30px; border-radius:4px; transition:all 0.5s ease; transform:translateY(20px) scale(0.98); opacity:0;}
.review.visible{transform:translateY(0) scale(1); opacity:1;}
.review p{color:var(--gray); margin-bottom:15px; font-style:italic;}
.review strong{color:white; font-size:0.85rem;}
.review:hover{transform:scale(var(--hover-scale));}

/* FORM */
form{max-width:650px;}
form input, form textarea, form select{width:100%; padding:14px; margin-bottom:20px; background:#111; border:1px solid var(--divider); color:white; transition:all 0.3s ease;}
form input:hover, form input:focus, form textarea:hover, form textarea:focus, form select:hover, form select:focus{border-color:var(--gold); transform:scale(1.01);}

/* FADE */
.fade{opacity:0; transform:translateY(25px); transition:all 0.8s ease;}
.fade.visible{opacity:1; transform:translateY(0);}

/* MOBILE */
@media(max-width:768px){
.nav-wrapper{flex-direction:column; height:auto; padding:20px 0; gap:20px;}
nav ul{flex-wrap:wrap; justify-content:center; gap:20px;}
.hero h1{font-size:1.8rem;}
}
</style>
</head>
<body>

<header>
<div class="container nav-wrapper">
<div class="logo">EMIRG <span>Logistics</span></div>
<nav>
<ul>
<li><a href="#solutions">Solutions</a></li>
<li><a href="#market">Market Insights</a></li>
<li><a href="#ai">AI in Logistics</a></li>
<li><a href="#reviews">Testimonials</a></li>
<li><a href="#calculator">Estimator</a></li>
<li><a href="#booking">Book Load</a></li>
</ul>
</nav>
</div>
</header>

<section class="hero fade">
<canvas id="networkCanvas"></canvas>
<div class="container">
<h1>Efficient, AI-Enhanced Freight Brokerage Across Canada</h1>
<p>Optimizing supply chains from Vancouver to Halifax with predictive logistics and AI-driven operations.</p>
<a href="#booking" class="cta-btn">Book Your Load →</a>
</div>
</section>

<section id="solutions" class="fade">
<div class="container">
<h2 class="section-title">Our Solutions</h2>
<div class="grid">
<div class="card"><h3>Freight Brokerage</h3><p>Connecting carriers and shippers with precision and speed across Canada.</p><div class="metric">99% On-time Delivery Rate</div></div>
<div class="card"><h3>Route Optimization</h3><p>AI-driven routing reduces transit time and cost.</p><div class="metric">15–25% Reduced Transport Costs</div></div>
<div class="card"><h3>Inventory Visibility</h3><p>Real-time tracking of goods, warehouse, and transportation status.</p><div class="metric">Up to 20% Reduction in Stockouts</div></div>
<div class="card"><h3>Regulatory Compliance</h3><p>Expert handling of Canadian transport regulations and customs.</p><div class="metric">Full Compliance Across Provinces</div></div>
</div>
</div>
</section>

<section id="market" class="fade">
<div class="container">
<h2 class="section-title">Market Insights (Canada)</h2>
<p style="color:var(--gray);max-width:700px;">
The Canadian logistics market is growing rapidly with e-commerce and interprovincial trade expansion.
AI adoption in freight brokerage is increasing efficiency, reducing delays, and enabling predictive demand planning.
</p>
</div>
</section>

<section id="ai" class="fade">
<div class="container">
<h2 class="section-title">Relevance of AI in Supply Chain & Logistics</h2>
<div class="grid">
<div class="card"><h3>Predictive Routing</h3><p>AI predicts traffic patterns and weather impacts to avoid delays.</p></div>
<div class="card"><h3>Demand Forecasting</h3><p>Accurate forecasting ensures capacity matches seasonal demand.</p></div>
<div class="card"><h3>Autonomous Decision Support</h3><p>AI suggests optimal carrier selection and load allocation.</p></div>
</div>
</div>
</section>

<section id="reviews" class="fade">
<div class="container">
<h2 class="section-title">Client Testimonials</h2>
<div class="grid">
<div class="review"><p>"EMIRG Logistics consistently delivers our shipments on time across Canada."</p><strong>VP Supply Chain, Toronto</strong></div>
<div class="review"><p>"AI-enabled routing reduced our costs and improved predictability."</p><strong>Operations Manager, Vancouver</strong></div>
<div class="review"><p>"Excellent compliance and freight handling expertise."</p><strong>Logistics Director, Montreal</strong></div>
</div>
</div>
</section>

<section id="calculator" class="fade">
<div class="container">
<h2 class="section-title">Freight Cost & Transit Time Estimator</h2>
<div class="grid">
<div class="card">
<select id="calcOrigin" required>
<option value="">Select Origin (City/Province)</option>
<option value="Vancouver">Vancouver, BC</option>
<option value="Calgary">Calgary, AB</option>
<option value="Toronto">Toronto, ON</option>
<option value="Montreal">Montreal, QC</option>
<option value="Halifax">Halifax, NS</option>
</select>

<select id="calcDestination" required>
<option value="">Select Destination (City/Province)</option>
<option value="Vancouver">Vancouver, BC</option>
<option value="Calgary">Calgary, AB</option>
<option value="Toronto">Toronto, ON</option>
<option value="Montreal">Montreal, QC</option>
<option value="Halifax">Halifax, NS</option>
</select>

<select id="calcFreightType" required>
<option value="">Freight Type</option>
<option value="General">General</option>
<option value="Refrigerated">Refrigerated</option>
<option value="Hazardous">Hazardous</option>
</select>

<input type="number" id="calcWeight" placeholder="Weight (kg)" min="1" required>

<div style="margin-bottom:20px;color:var(--gold);" id="calcResult">Estimated cost & transit time will appear here</div>

<button class="cta-btn" onclick="transferToBooking()">Proceed to Booking →</button>
</div>
</div>
</div>
</section>

<section id="booking" class="fade">
<div class="container">
<h2 class="section-title">Book a Load / Inquiry Form</h2>
<form onsubmit="sendBookingEmail(); return false;">
<input type="text" id="shipperName" placeholder="Full Name" required>
<input type="text" id="companyName" placeholder="Company Name" required>
<input type="text" id="origin" placeholder="Origin (City/Province)" required>
<input type="text" id="destination" placeholder="Destination (City/Province)" required>
<select id="freightType" required>
<option value="">Select Freight Type</option>
<option value="General">General</option>
<option value="Refrigerated">Refrigerated</option>
<option value="Hazardous">Hazardous</option>
</select>
<textarea id="details" placeholder="Additional Load Details..." required></textarea>
<button class="cta-btn" type="submit">Submit Inquiry →</button>
</form>
</div>
</section>

<footer class="fade">
<div class="container" style="text-align:center;color:var(--gray);padding:40px 0;font-size:0.85rem;">
© 2026 EMIRG Logistics. All rights reserved.
</div>
</footer>

<script>
/* Scroll-trigger animations */
const faders=document.querySelectorAll('.fade');
const cards=document.querySelectorAll('.card');
const reviews=document.querySelectorAll('.review');
const observer=new IntersectionObserver(entries=>{
entries.forEach(entry=>{
if(entry.isIntersecting){
entry.target.classList.add('visible');
}
});
},{threshold:0.2});
faders.forEach(el=>observer.observe(el));
cards.forEach(el=>observer.observe(el));
reviews.forEach(el=>observer.observe(el));

/* Freight Estimator Logic */
function transferToBooking(){
let origin=document.getElementById("calcOrigin").value;
let destination=document.getElementById("calcDestination").value;
let freight=document.getElementById("calcFreightType").value;
let weight=parseFloat(document.getElementById("calcWeight").value);

if(!origin || !destination || !freight || !weight){
alert("Please fill out all fields to estimate freight.");
return;
}

const distanceFactor={
"Vancouver-Toronto":4500, "Vancouver-Montreal":5000, "Vancouver-Halifax":6000,
"Calgary-Toronto":3000, "Calgary-Montreal":3500, "Calgary-Halifax":4000,
"Toronto-Montreal":600, "Toronto-Halifax":1200,
"Montreal-Halifax":900
};

let key1=origin+"-"+destination;
let key2=destination+"-"+origin;
let dist=distanceFactor[key1] || distanceFactor[key2] || 1500;
let typeMultiplier=freight==="Refrigerated"?1.25:freight==="Hazardous"?1.5:1;
let cost=(dist*0.75 + weight*0.8)*typeMultiplier;
let days=Math.ceil(dist/1000);

document.getElementById("calcResult").innerHTML=`Estimated Cost: $${cost.toFixed(0)} CAD<br>Estimated Transit: ${days} days`;

window.freightEstimatorData=`Origin: ${origin}%0ADestination: ${destination}%0AFreight Type: ${freight}%0AWeight: ${weight}kg%0AEstimated Cost: $${cost.toFixed(0)} CAD%0ATransit Time: ${days} days%0A`;
document.getElementById("booking").scrollIntoView({behavior:"smooth"});
}

/* Integrate estimator data into booking form */
function sendBookingEmail(){
let name=document.getElementById("shipperName").value;
let company=document.getElementById("companyName").value;
let origin=document.getElementById("origin").value;
let destination=document.getElementById("destination").value;
let freight=document.getElementById("freightType").value;
let details=document.getElementById("details").value;

let estimator=window.freightEstimatorData || "";

let body=`Name: ${name}%0ACompany: ${company}%0AOrigin: ${origin}%0ADestination: ${destination}%0AFreight Type: ${freight}%0ADetails: ${details}%0A${estimator}`;

window.location.href=`mailto:logistics@emirg-group.com?subject=Load Inquiry - ${company}&body=${body}`;
}

/* Animated Network Background */
const canvas=document.getElementById("networkCanvas");
const ctx=canvas.getContext("2d");
let particles=[];
const particleCount=80;

function resizeCanvas(){canvas.width=canvas.offsetWidth; canvas.height=canvas.offsetHeight;}
resizeCanvas();
window.addEventListener("resize",resizeCanvas);

class Particle{constructor(){this.x=Math.random()*canvas.width; this.y=Math.random()*canvas.height; this.vx=(Math.random()-0.5)*0.4; this.vy=(Math.random()-0.5)*0.4; this.radius=2;}
update(){this.x+=this.vx; this.y+=this.vy; if(this.x<=0||this.x>=canvas.width)this.vx*=-1; if(this.y<=0||this.y>=canvas.height)this.vy*=-1;}
draw(){ctx.beginPath(); ctx.arc(this.x,this.y,this.radius,0,Math.PI*2); ctx.fillStyle="#C6A75E"; ctx.fill();}}
function init(){particles=[]; for(let i=0;i<particleCount;i++){particles.push(new Particle());}}
init();
function connect(){for(let a=0;a<particles.length;a++){for(let b=a;b<particles.length;b++){let dx=particles[a].x-particles[b].x; let dy=particles[a].y-particles[b].y; let distance=dx*dx+dy*dy; if(distance<12000){ctx.beginPath(); ctx.strokeStyle="rgba(198,167,94,0.08)"; ctx.lineWidth=1; ctx.moveTo(particles[a].x,particles[a].y); ctx.lineTo(particles[b].x,particles[b].y); ctx.stroke();}}}}
function animate(){ctx.clearRect(0,0,canvas.width,canvas.height); particles.forEach(p=>{p.update();p.draw();}); connect(); requestAnimationFrame(animate);}
animate();
</script>
</body>
</html>
