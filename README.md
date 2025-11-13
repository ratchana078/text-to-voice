# 🗣 Text to Voice Converter (HTML, CSS & JavaScript)

## 📘 Overview
This is a simple *Text-to-Speech (TTS)* web app built using *HTML, CSS, and JavaScript*.  
It uses the *Web Speech API* to convert written text into spoken voice — right inside your browser!  
No backend or extra setup required.

---

## 🚀 Features
- 🎤 Convert text into natural voice instantly  
- 🌍 Choose from multiple available voices  
- ⚙ Adjustable pitch and rate (optional to add)  
- 💾 Works completely offline  
- 🧩 Clean, responsive UI

---

## 🧩 Project Structure
HTML// 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Text to Voice</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <div class="container">
    <h1>🗣 Text to Voice</h1>
    <input type="text" id="text" placeholder="Enter the text" />
    <br />
    <button onclick="speak()">Speak</button>
  </div>
<script>
    function speak() {
      const input = document.getElementById("text").value;
      const utterance = new SpeechSynthesisUtterance(input);
      speechSynthesis.speak(utterance);
    }
  </script>


<header class="top-header">
  <div class="header-inner">
    <div class="logo">🗣</div>
    <div class="header-text">
      <h1>If you want.. I can create</h1>
      <p class="subtitle">Convert text to premium voice — clear smooth and professional
        
      </p>
    </div>
   
  </div>
  body {
  background:skyblue;
  font-family: "Poppins", sans-serif;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.container {
  background: white;
  padding: 40px;
  border-radius: 20px;
  text-align: center;
  box-shadow: 0 4px 15px black;
}

input {
  width: 250px;
  padding: 10px;
  border-radius: 10px;
  border: 1px solid white;
  margin-bottom: 10px;
}

button {
  background-color: skyblue;
  color: white;
  border: none;
  padding: 10px 20px;
  border-radius: 10px;
  cursor: pointer;
  transition: 0.3s;
}

button:hover {
  background-color:skyblue;
}

.top-header{
  width: 100%;
  padding: 18px 24px;
  box-sizing: border-box;
  position: fixed;
  top: 18px;
  left: 0;
  z-index: 50;
  display: flex;
  justify-content: center;
  pointer-events: none; 
}

.top-header .header-inner{
  width: min(1100px, 96%)
  background: linear-gradient;
  backdrop-filter: blur(6px);
  border-radius: 14px;
  padding: 12px 18px;
  display:flex;
  align-items:center;
  gap:14px;
  box-shadow: 0 8px 30px r:
  pointer-events: auto; 
}

/* logo */
.top-header .logo{
  font-size: 26px;
  width:48px;
  height:48px;
  display:flex;
  align-items:center;
  justify-content:center;
  background: rgba(255,255,255,0.06);
  border-radius:10px;
}

/* title */
.top-header h1{
  margin:0;
  font-size:20px;
  letter-spacing:1px;
  text-transform:uppercase;
  font-weight:700;
  color:#fff;
  text-shadow:0 1px 0 rgba(0,0,0,0.35);
}

/* subtitle */
.top-header .subtitle{
  margin:2px 0 0 0;
  font-size:12.5px;
  color:rgba(255,255,255,0.85);
  opacity:0.9;
}

/* CTA */
.header-cta{ margin-left:auto; }
.btn-primary{
  display:inline-block;
  padding:8px 14px;
  border-radius:10px;
  background: linear-gradient(135deg,#ff6b5f,#ff3b30);
  color:white;
  font-weight:600;
  text-decoration:none;
  box-shadow: 0 6px 18px rgba(255,59,48,0.18);
  transition: transform .15s ease, box-shadow .15s;
}
.btn-primary:hover{ transform: translateY(-3px); box-shadow: 0 10px 26px rgba(255,59,48,0.22); }

/* Responsive */
@media (max-width:720px){
  .top-header .header-inner{ flex-direction:column; align-items:flex-start; gap:10px; padding:10px; }
  .header-cta{ width:100%; display:flex; justify-content:stretch; }
  .btn-primary{ width:100%; text-align:center; }
}

</header>

🧪 How to Run
Download or copy all 3 files (index.html, style.css, script.js) into a folder.
Open index.html in any modern browser (Chrome, Edge, Firefox).
Type or paste text into the text box.
Click Speak to hear it aloud — click Stop to cancel.

https://ratchana078.github.io/text-to-voice/
