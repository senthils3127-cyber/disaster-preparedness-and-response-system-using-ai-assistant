!DOCTYPE html>

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Disaster Preparedness & Response System</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Segoe UI',sans-serif;
}

:root{
--primary:#0f172a;
--secondary:#1e293b;
--accent:#06b6d4;
--danger:#ef4444;
--success:#22c55e;
--light:#f8fafc;
}

body{
background:#f1f5f9;
color:#333;
}

.dark{
background:#0f172a;
color:white;
}

header{
background:linear-gradient(135deg,#0f172a,#1e293b);
color:white;
padding:20px;
text-align:center;
}

nav{
display:flex;
justify-content:center;
flex-wrap:wrap;
gap:10px;
margin-top:15px;
}

nav a{
color:white;
text-decoration:none;
padding:10px 15px;
border-radius:8px;
}

nav a:hover{
background:rgba(255,255,255,.15);
}

.hero{
padding:80px 20px;
text-align:center;
background:linear-gradient(rgba(0,0,0,.55),rgba(0,0,0,.55)),
url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1600&q=80');
background-size:cover;
background-position:center;
color:white;
}

.hero h1{
font-size:3rem;
margin-bottom:15px;
}

.btn{
background:var(--accent);
border:none;
color:white;
padding:12px 20px;
border-radius:8px;
cursor:pointer;
margin:5px;
}

.section{
padding:60px 8%;
}

.section-title{
text-align:center;
margin-bottom:30px;
}

.grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:20px;
}

.card{
background:white;
padding:25px;
border-radius:15px;
box-shadow:0 8px 25px rgba(0,0,0,.08);
transition:.3s;
}

.card:hover{
transform:translateY(-6px);
}

.dark .card{
background:#1e293b;
color:white;
}

.stat{
text-align:center;
}

.stat h2{
color:#06b6d4;
font-size:2.5rem;
}

.alert{
border-left:5px solid red;
}

.contact{
padding:10px;
background:#f8fafc;
margin:8px 0;
border-radius:8px;
}

.dark .contact{
background:#334155;
}

input,textarea{
width:100%;
padding:12px;
margin:8px 0;
border:1px solid #ccc;
border-radius:8px;
}

footer{
background:#0f172a;
color:white;
text-align:center;
padding:20px;
}

#clock{
margin-top:10px;
font-weight:bold;
color:#67e8f9;
}

#sos{
position:fixed;
bottom:20px;
right:20px;
width:80px;
height:80px;
border-radius:50%;
background:red;
color:white;
font-size:24px;
font-weight:bold;
border:none;
cursor:pointer;
box-shadow:0 0 25px rgba(255,0,0,.5);
}

.toggle{
position:fixed;
left:20px;
bottom:20px;
padding:12px 15px;
border:none;
border-radius:50px;
cursor:pointer;
background:#0f172a;
color:white;
}

#aiResponse{
margin-top:15px;
padding:15px;
background:#e0f2fe;
border-radius:10px;
}

.dark #aiResponse{
background:#334155;
}

@media(max-width:768px){
.hero h1{
font-size:2rem;
}
}
</style>

</head>

<body>

<header>
<h1>🌍 Disaster Preparedness & Response System</h1>
<p>Stay Informed • Stay Safe • Save Lives</p>
<div id="clock"></div>

<nav>
<a href="#dashboard">Dashboard</a>
<a href="#alerts">Alerts</a>
<a href="#resources">Resources</a>
<a href="#ai">AI Assistant</a>
<a href="#volunteer">Volunteer</a>
<a href="#contact">Contacts</a>
</nav>
</header>

<section class="hero">
<h1>Emergency Management Platform</h1>
<p>Real-time alerts, preparedness resources and AI-powered emergency assistance.</p>
<button class="btn" onclick="document.getElementById('alerts').scrollIntoView()">View Alerts</button>
</section>

<section class="section" id="dashboard">

<h2 class="section-title">📊 Dashboard</h2>

<div class="grid">

<div class="card stat">
<h2>12</h2>
<p>Active Alerts</p>
</div>

<div class="card stat">
<h2>145</h2>
<p>Rescue Teams</p>
</div>

<div class="card stat">
<h2>35</h2>
<p>Safe Shelters</p>
</div>

<div class="card stat">
<h2>99%</h2>
<p>System Uptime</p>
</div>

</div>

</section>

<section class="section" id="alerts">

<h2 class="section-title">🚨 Disaster Alerts</h2>

<div class="card alert">
<div id="alertBox">
No active alerts.
</div>

<br>

<button class="btn" onclick="generateAlert()">
Generate Alert
</button>
</div>

</section>

<section class="section" id="resources">

<h2 class="section-title">📚 Resources</h2>

<div class="grid">

<div class="card">
<h3>🎒 Emergency Kit</h3>
<p>Water, Food, Flashlight, Batteries, Medicines.</p>
</div>

<div class="card">
<h3>🏠 Evacuation Plan</h3>
<p>Create family meeting points and safe routes.</p>
</div>

<div class="card">
<h3>🩺 First Aid</h3>
<p>Learn CPR, wound care and emergency response.</p>
</div>

</div>

</section>

<section class="section" id="ai">

<h2 class="section-title">🤖 AI Emergency Assistant</h2>

<div class="card">

<textarea id="question" rows="4"
placeholder="Ask about floods, earthquakes, first aid, safety plans..."></textarea>

<button class="btn" onclick="askAI()">
Ask AI
</button>

<div id="aiResponse">
AI responses will appear here.
</div>

</div>

</section>
<section id="volunteer" class="section">
<div class="card">
<h2>Volunteer Registration</h2>
<input id="volName" placeholder="Full Name">
<input id="volEmail" placeholder="Email">
<input id="volSkills" placeholder="Skills (medical, rescue, fire, tech)">
<input id = "contact number for emergency help"placeholder = "mobile number">
<button class="btn btn-primary" onclick="registerVolunteer()">Register</button>
<div id="registrationResult"></div>
</div>
</section>
</section><section class="section" id="volunteer">

<h2 class="s

<section class="section" id="contact">

<h2 class="section-title">📞 Emergency Contacts</h2>

<div class="card">

<div class="contact">🚔 Police : 100</div>

<div class="contact">🚑 Ambulance : 108</div>

<div class="contact">🔥 Fire Service : 101</div>

<div class="contact">🆘 Emergency : 112</div>

</div>

</section>

<button id="sos" onclick="sos()">
SOS
</button>

<button class="toggle" onclick="toggleTheme()">
🌙
</button>

<footer>
<p>© 2026 Disaster Preparedness & Response System</p>
<p><strong>Owner :</strong> Senthil.S</p>
</footer>

<script>

function updateClock(){
let now=new Date();

document.getElementById("clock").innerHTML=
now.toLocaleDateString()+" | "+
now.toLocaleTimeString();
}

setInterval(updateClock,1000);
updateClock();

function generateAlert(){

const alerts=[
"⚠️ Flood Warning: Heavy rainfall expected.",
"⚠️ Cyclone Alert: Strong winds approaching.",
"⚠️ Heatwave Advisory: Stay hydrated.",
"⚠️ Earthquake Preparedness Notice."
];

const random=
alerts[Math.floor(Math.random()*alerts.length)];

document.getElementById("alertBox").innerHTML=random;
}

function askAI(){       

let q=
document.getElementById("question").value.toLowerCase();

let answer="Please follow official emergency instructions.";

if(q.includes("flood"))
answer="Move to higher ground, avoid flooded roads and keep emergency supplies ready.";

else if(q.includes("earthquake"))
answer="Drop, Cover and Hold On. Stay away from windows and heavy objects.";

else if(q.includes("cyclone"))
answer="Stay indoors, secure loose objects and monitor official alerts.";

else if(q.includes("first aid"))
answer="Ensure safety first, call emergency services if required and provide basic first aid.";

document.getElementById("aiResponse").innerHTML=
"<strong>AI Assistant:</strong><br>"+answer;
}

function sos(){
alert("SOS ACTIVATED!\n\nContact emergency services immediately.");
}

function toggleTheme(){
document.body.classList.toggle("dark");
}
function registerVolunteer(){
let n=volName.value.trim(),e=volEmail.value.trim(),s=volSkills.value.trim().toLowerCase();
if(!n||!e||!s) return alert("Fill all fields");
if(!/^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(e)) return alert("Invalid email");
let team="General Support Team",badge="🌟 Community Helper";
if(s.includes("medical")){team="Medical Response Team";badge="🏥 Medical Hero";}
else if(s.includes("rescue")){team="Rescue Operations Team";badge="🚑 Rescue Specialist";}
else if(s.includes("fire")){team="Fire Safety Team";badge="🔥 Fire Guardian";}
else if(s.includes("tech")){team="Technical Support Team";badge="💻 Tech Volunteer";}
let volunteer={n,e,s,team,badge};
let list=JSON.parse(localStorage.getItem("volunteers")||"[]");
list.push(volunteer);
localStorage.setItem("volunteers",JSON.stringify(list));
registrationResult.innerHTML=`<div class='card'><h3>✅ Registration Successful</h3><p>${team}</p><p>${badge}</p></div>`;
toast("Volunteer Registered");
showVolunteers();
}

function showVolunteers(){
let list=JSON.parse(localStorage.getItem("volunteers")||"[]");
if(list.length===0) return;
let html="<h3>Registered Volunteers</h3>";
list.forEach(v=>{html+=`<p>${v.n} - ${v.team} ${v.badge}</p>`});
registrationResult.innerHTML+=html;
}
showVolunteers();
</script>

</body>
</html> 
