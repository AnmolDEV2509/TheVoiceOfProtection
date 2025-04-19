<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>The Voice of Protection</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', sans-serif; }
    body {
      background: linear-gradient(to right, #f8f9fa, #e0f7fa);
      color: #333;
    }
    header {
      height: 300px;
      background: url('your-image.jpg') no-repeat center center/cover;
      color: white;
      display: flex; justify-content: center; align-items: center;
      box-shadow: 0 2px 6px rgba(0, 0, 0, 0.2);
    }
    .hero {
      text-align: center;
      background-color: rgba(0, 0, 0, 0.5);
      padding: 30px;
      border-radius: 12px;
    }
    header h1 {
      font-size: 28px;
      margin-bottom: 5px;
      background: linear-gradient(45deg, #ff6f61, #ffca28);
      -webkit-background-clip: text;
      color: transparent;
    }
    nav {
      background-color: #0a9396;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      padding: 10px;
      gap: 10px;
    }
    nav a {
      color: white;
      text-decoration: none;
      padding: 8px 18px;
      border-radius: 20px;
      background-color: rgba(255, 255, 255, 0.1);
      transition: all 0.3s ease;
    }
    nav a:hover {
      background-color: #94d2bd;
      color: #000;
      transform: scale(1.05);
    }
    section {
      padding: 24px 16px;
      max-width: 900px;
      margin: 25px auto;
      display: none;
      background-color: white;
      border-radius: 18px;
      box-shadow: 0 4px 14px rgba(0, 0, 0, 0.08);
      animation: fadeIn 0.4s ease-in-out;
    }
    section.active {
      display: block;
    }
    h2 {
      font-size: 22px;
      text-align: center;
      margin-bottom: 15px;
      color: #005f73;
    }
    p {
      font-size: 16px;
      line-height: 1.6;
      text-align: justify;
      color: #444;
    }
    footer {
      background-color: #005f73;
      color: white;
      text-align: center;
      padding: 16px 10px;
      margin-top: 40px;
      font-size: 13px;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(10px); }
      to { opacity: 1; transform: translateY(0); }
    }
    .chat-buttons {
      display: flex;
      flex-direction: column;
      gap: 10px;
      justify-content: center;
      align-items: center;
      margin: 10px 0;
      visibility: visible;
    }
    .chat-buttons button {
      background-color: #e63946;
      color: white;
      border: none;
      border-radius: 20px;
      padding: 12px 30px;
      font-size: 14px;
      cursor: pointer;
      width: 100%;
    }
    .chat-buttons button:hover {
      background-color: #d12e2e;
    }
    .chat-input {
      display: flex;
      gap: 6px;
    }
    .chat-input input {
      flex: 1;
      padding: 6px;
      border: 1px solid #ccc;
    }
    .chat-input button {
      background-color: #0a9396;
      color: white;
      border: none;
      padding: 6px 12px;
      cursor: pointer;
    }
    .chat-tabs {
      display: flex;
      justify-content: center;
      margin-bottom: 10px;
    }
    .chat-tabs button {
      background: #ddd;
      padding: 6px 14px;
      border: none;
      border-radius: 6px;
      margin: 0 4px;
      cursor: pointer;
    }
    .chat-tabs button.active {
      background: #0a9396;
      color: white;
    }
    #chat-box-ai, #chat-box-community {
      height: 250px;
      overflow-y: auto;
      border: 1px solid #ccc;
      padding: 10px;
      margin-bottom: 10px;
      background: #f1f1f1;
      display: none;
    }
    #chat-box-ai.active, #chat-box-community.active {
      display: block;
    }
    /* Map section styles */
    .map-section {
      margin: 20px 0;
      text-align: center;
    }
    .map-box {
      background: white;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      display: inline-block;
      width: 90%;
      max-width: 600px;
    }
    iframe {
      width: 100%;
      height: 300px;
      border: none;
      border-radius: 8px;
      margin-top: 20px;
      display: block; /* Ensure the map iframe is visible */
    }
  </style>
</head>
<body>
  <header>
    <div class="hero">
      <h1>The Voice of Protection</h1>
      <p>Empowering safety and awareness</p>
    </div>
  </header>

  <nav>
    <a href="#" onclick="showSection('home')">Home</a>
    <a href="#" onclick="showSection('about')">About</a>
    <a href="#" onclick="showSection('contact')">Contact</a>
    <a href="#" onclick="showSection('chat')"><i class="fas fa-comments"></i> Chat</a>
    <a href="#" onclick="showSection('map')">View Map</a> <!-- Map button here -->
  </nav>

  <section id="home" class="active">
    <h2>Welcome</h2>
    <p>
      "The Voice of Protection" is more than just a website — it's a movement. This platform is designed to spread awareness about women's safety and empower people with tools, knowledge, and a supportive community.
    </p>
    <p>
      We believe that awareness is the first step toward change. Through educational content, emergency resources, and real-time support systems, we aim to build a society that respects, protects, and uplifts every woman.
    </p>
    <p>
      Whether it's reporting harassment, seeking help in emergencies, or simply having someone to talk to — our platform is here, 24/7. Because no one should ever feel alone or unsafe.
    </p>
  </section>

  <section id="about">
    <h2>About Us</h2>
    <p>
      We are a community of young changemakers committed to educating people on respecting women, stopping harassment, and supporting those in need. This project was built with the mission to make safety accessible and conversations around protection normal and necessary.
    </p>
  </section>

  <section id="contact">
    <h2>Contact</h2>
    <p>Email: support@voiceofprotection.org</p>
    <p>Instagram: @voiceofprotection</p>
  </section>

  <section id="chat">
    <h2>Live Chat</h2>
    <div class="chat-tabs">
      <button onclick="switchChat('ai')" id="tab-ai" class="active">AI Chat</button>
      <button onclick="switchChat('community')" id="tab-community">Community Chat</button>
    </div>

    <div id="chat-box-ai" class="active">
      <div class="chat-buttons">
        <button onclick="quickMsg('Call Police 🚨')">Call Police</button>
        <button onclick="quickMsg('I need help now')">Need Help</button>
        <button onclick="quickMsg('I’m in danger')">I’m in Danger</button>
        <button onclick="quickMsg('Track Me')">Track Me</button>
      </div>
      <div id="chat-box"></div>
      <div class="chat-input">
        <input type="text" id="chatInput" placeholder="Type a message..." />
        <button onclick="sendMsg()">Send</button>
      </div>
    </div>

    <div id="chat-box-community">
      <p style="text-align:center; color:#555;">Community chat coming soon!</p>
    </div>
  </section>

  <section id="map">
    <h2>Your Current Location</h2>
    <div class="map-section">
      <button onclick="getLocation()">Get My Location</button>
      <div class="map-box" id="map-box">
        <iframe id="location-map" style="display: none;"></iframe>
      </div>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 The Voice of Protection. All Rights Reserved.</p>
  </footer>

  <script>
    let currentSection = 'home';

    function showSection(section) {
      document.getElementById(currentSection).classList.remove('active');
      document.getElementById(section).classList.add('active');
      currentSection = section;
    }

    function switchChat(chatType) {
      document.getElementById('tab-ai').classList.remove('active');
      document.getElementById('tab-community').classList.remove('active');
      document.getElementById('chat-box-ai').classList.remove('active');
      document.getElementById('chat-box-community').classList.remove('active');

      if (chatType === 'ai') {
        document.getElementById('tab-ai').classList.add('active');
        document.getElementById('chat-box-ai').classList.add('active');
      } else {
        document.getElementById('tab-community').classList.add('active');
        document.getElementById('chat-box-community').classList.add('active');
      }
    }

    function quickMsg(message) {
      document.getElementById('chatInput').value = message;
    }

    function sendMsg() {
      const msg = document.getElementById('chatInput').value;
      if (msg.trim() === '') return;
      document.getElementById('chat-box').innerHTML += `<p><strong>You:</strong> ${msg}</p>`;
      document.getElementById('chatInput').value = '';
    }

    function getLocation() {
      if (navigator.geolocation) {
        navigator.geolocation.getCurrentPosition(showMap);
      } else {
        alert('Geolocation is not supported by this browser.');
      }
    }

    function showMap(position) {
      const lat = position.coords.latitude;
      const lon = position.coords.longitude;
      const url = `https://www.google.com/maps?q=${lat},${lon}&hl=es;z=14&output=embed`;
      document.getElementById('location-map').src = url;
      document.getElementById('location-map').style.display = 'block';
    }
  </script>
</body>
</html>
