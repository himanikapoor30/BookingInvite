<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">
    <title>Our 6th Anniversary! ❤️</title>
    <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@600;700&display=swap" rel="stylesheet">
    
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        
        body {
            font-family: 'Quicksand', sans-serif;
            background: linear-gradient(135deg, #ff9a9e 0%, #fecfef 99%, #fecfef 100%);
            color: #333;
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            height: 100dvh;
            text-align: center;
            position: relative;
        }

        .heart-bg {
            position: absolute;
            font-size: 22px;
            color: rgba(255, 100, 150, 0.4);
            animation: floatUp 4s linear infinite;
            z-index: 0;
        }
        @keyframes floatUp {
            0% { transform: translateY(100vh) scale(0.5); opacity: 1; }
            100% { transform: translateY(-10vh) scale(1.2); opacity: 0; }
        }

        .page {
            display: none;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            width: 100%;
            height: 100%;
            padding: 20px;
            opacity: 0;
            z-index: 10;
            transition: opacity 0.5s ease-in-out, transform 0.5s ease-in-out;
            transform: scale(0.9);
            position: absolute;
        }

        .active-page {
            display: flex;
            opacity: 1;
            transform: scale(1);
        }

        /* COMIC BUBBLE STYLING FOR PAGE 1 */
        .photo-story-container {
            position: relative;
            width: 85vw;
            max-width: 340px;
            height: 400px;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
            margin-bottom: 25px;
            background: #fff;
        }
        .photo-story-container img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        .comic-bubble {
            position: absolute;
            background: white;
            padding: 10px 15px;
            border-radius: 20px;
            font-size: 14px;
            font-weight: 700;
            color: #d6336c;
            box-shadow: 0 4px 10px rgba(0,0,0,0.15);
            max-width: 70%;
            animation: popIn 0.5s ease-out;
        }
        @keyframes popIn {
            0% { transform: scale(0); }
            80% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }
        .bubble-top { top: 15px; left: 15px; border-bottom-left-radius: 2px; }
        .bubble-bottom { bottom: 15px; right: 15px; border-top-right-radius: 2px; }

        /* FULL SCREEN COLLAGE FOR PAGE 2 */
        .fullscreen-collage {
            position: absolute;
            top: 0; left: 0; right: 0; bottom: 0;
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            grid-auto-rows: 25vh;
            z-index: -1;
        }
        .fullscreen-collage img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            opacity: 0.85;
        }
        .minimal-glass-banner {
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(10px);
            padding: 20px;
            border-radius: 20px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.15);
            width: 90%;
            max-width: 340px;
        }

        /* STANDARD CARDS */
        .card-container {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            padding: 25px 20px;
            border-radius: 25px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.15);
            width: 90%;
            max-width: 340px;
            margin-bottom: 20px;
        }
        .card-container img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 15px;
            margin-bottom: 15px;
        }

        h2 { font-size: 24px; font-weight: 700; margin-bottom: 10px; color: #d6336c; }
        p { font-size: 16px; line-height: 1.4; color: #444; font-weight: 600; }

        .btn {
            background: #ff477e;
            color: white;
            border: none;
            padding: 14px 30px;
            font-size: 16px;
            font-weight: 700;
            border-radius: 50px;
            cursor: pointer;
            box-shadow: 0 6px 15px rgba(255, 71, 126, 0.4);
            font-family: inherit;
            transition: all 0.2s;
            z-index: 20;
        }
        .btn:active { transform: scale(0.9); }

        .button-group {
            position: relative;
            width: 100%;
            height: 120px;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 10px;
        }
        #yesBtn { background: #ff477e; transition: all 0.3s ease; }
        #noBtn {
            background: #fff;
            color: #ff477e;
            border: 2px solid #ff477e;
            position: absolute;
            top: 60px;
            transition: all 0.2s ease;
        }
    </style>
</head>
<body>

    <!-- Background Music (Autoplays a soft romantic vibe) -->
    <audio id="bgMusic" loop>
        <source src="https://assets.mixkit.co/music/preview/mixkit-romantic-sec-483.mp3" type="audio/mpeg">
    </audio>

    <div id="heart-container"></div>

    <!-- PAGE 1: The Wedding Comic Scene -->
    <div id="page1" class="page active-page">
        <div class="photo-story-container">
            <!-- 📸 REPLACE WITH YOUR WEDDING GROUP PHOTO -->
            <img src="https://images.unsplash.com/photo-1519741497674-611481863552?auto=format&fit=crop&w=500&q=80" alt="Wedding Group">
            
            <div class="comic-bubble bubble-top">
                "Isse toh propose krungi..." 🤭
            </div>
            <div class="comic-bubble bubble-bottom">
                "Dekhte hain..." 👀
            </div>
        </div>
        <p style="color:white; text-shadow: 0 2px 5px rgba(0,0,0,0.3); margin-bottom: 20px;">October 2020. Never thought this boy would become my everything.</p>
        <button class="btn" onclick="startExperience(1, 2)">Let's go back ➔</button>
    </div>

    <!-- PAGE 2: Full Screen Smile Collage -->
    <div id="page2" class="page" style="padding: 0;">
        <div class="fullscreen-collage">
            <!-- 📸 REPLACE THESE WITH HIS SMILE SCREENSHOTS -->
            <img src="https://images.unsplash.com/photo-1506794778202-cad84cf45f1d?auto=format&fit=crop&w=300&q=80">
            <img src="https://images.unsplash.com/photo-1519085360753-af0119f7cbe7?auto=format&fit=crop&w=300&q=80">
            <img src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?auto=format&fit=crop&w=300&q=80">
            <img src="https://images.unsplash.com/photo-1530268729831-4b0b9e170218?auto=format&fit=crop&w=300&q=80">
            <img src="https://images.unsplash.com/photo-1506794778202-cad84cf45f1d?auto=format&fit=crop&w=300&q=80">
            <img src="https://images.unsplash.com/photo-1519085360753-af0119f7cbe7?auto=format&fit=crop&w=300&q=80">
            <img src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?auto=format&fit=crop&w=300&q=80">
            <img src="https://images.unsplash.com/photo-1530268729831-4b0b9e170218?auto=format&fit=crop&w=300&q=80">
            <img src="https://images.unsplash.com/photo-1506794778202-cad84cf45f1d?auto=format&fit=crop&w=300&q=80">
        </div>
        <div class="minimal-glass-banner">
            <h2>That Smile... 🫠</h2>
            <p style="margin-bottom: 15px; font-size: 15px;">Through every screenshot, I fell harder for this exact smile.</p>
            <button class="btn" onclick="nextPage(2, 3)">Next ➔</button>
        </div>
    </div>

    <!-- PAGE 3: Ambala Station Incident -->
    <div id="page3" class="page">
        <div class="card-container">
            <!-- 📸 REPLACE WITH AMBALA PHOTO -->
            <img src="https://images.unsplash.com/photo-1558980663-3685c1d673c4?auto=format&fit=crop&w=500&q=80" alt="Ambala Station">
            <h2>Ambala Station, 2024 🚂</h2>
            <p>You acted all strict, denying to meet me... until 5 minutes before my train. You melted and came running anyway! 🏃‍♂️💨</p>
        </div>
        <button class="btn" onclick="nextPage(3, 4)">Next ➔</button>
    </div>

    <!-- PAGE 4: 2025 Reunion & 2026 Promise -->
    <div id="page4" class="page">
        <div class="card-container">
            <!-- 📸 REPLACE WITH 2025/2026 PHOTO -->
            <img src="https://images.unsplash.com/photo-1518199266791-5375a83190b7?auto=format&fit=crop&w=500&q=80" alt="Reunion">
            <h2>Thick & Thin ❤️</h2>
            <p>2023 was rough, 2025 brought us back, and 2026 has its pressure. But I want you to know: I choose you, over and over again.</p>
        </div>
        <button class="btn" onclick="nextPage(4, 5)">I have a demand! ➔</button>
    </div>

    <!-- PAGE 5: The Date Ask & Paratha Bribe -->
    <div id="page5" class="page">
        <div class="card-container" style="text-align: center; padding: 20px;">
            <img src="https://media.tenor.com/J3yqXW1D6y8AAAAi/please-bubu.gif" alt="Please" style="width: 120px; height: 120px; object-fit: cover; border-radius: 50%; margin: 0 auto 10px auto;">
            <h2>Anniversary Date? 🥺</h2>
            <p style="font-size: 14px; margin-bottom: 15px;">Let's forget the house pressure and family stress for one day. My 21-year-old boy deserves a break.<br><b style="color:#d6336c;">(Bribing you with hot Aloo Parathas 😋🧈)</b></p>
            
            <div class="button-group">
                <button id="yesBtn" class="btn" onclick="nextPage(5, 6)">YES! Let's go! ❤️</button>
                <button id="noBtn" class="btn" onclick="runAway()">No 😒</button>
            </div>
        </div>
    </div>

    <!-- PAGE 6: Success! -->
    <div id="page6" class="page">
        <div class="card-container" style="text-align: center;">
            <img src="https://media.tenor.com/gK0Z-eNf3fMAAAAi/bubu-dudu-dance.gif" alt="Yay!" style="width: 140px; height: 140px; object-fit: cover; border-radius: 50%; margin: 0 auto 15px auto;">
            <h2>It's a Date! 🎉</h2>
            <p>I'll keep the parathas hot and the smiles ready. See you soon! ❤️</p>
        </div>
    </div>

    <script>
        // Start background music and music handling on first click
        function startExperience(currentId, nextId) {
            const music = document.getElementById('bgMusic');
            music.volume = 0.4;
            music.play().catch(e => console.log("Audio play blocked by browser:", e));
            nextPage(currentId, nextId);
        }

        const heartContainer = document.getElementById('heart-container');
        setInterval(() => {
            const heart = document.createElement('div');
            heart.classList.add('heart-bg');
            heart.innerHTML = ['❤️','✨','🥺','🥰'][Math.floor(Math.random() * 4)];
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.animationDuration = (Math.random() * 3 + 3) + 's';
            heartContainer.appendChild(heart);
            setTimeout(() => { heart.remove(); }, 6000);
        }, 400);

        function nextPage(currentId, nextId) {
            const currentPage = document.getElementById(`page${currentId}`);
            const nextPage = document.getElementById(`page${nextId}`);
            
            currentPage.style.transform = 'scale(0.9)';
            currentPage.style.opacity = '0';
            
            setTimeout(() => {
                currentPage.classList.remove('active-page');
                nextPage.classList.add('active-page');
                
                setTimeout(() => {
                    nextPage.style.opacity = '1';
                    nextPage.style.transform = 'scale(1)';
                }, 50);
            }, 500);
        }

        let noClickCount = 0;
        const cheekyMessages = [
            "Hey! Try again! 🥺",
            "Too slow! 🏃‍♂️💨",
            "You can't escape my parathas!",
            "Stop teasing me! 😭",
            "Just click YES already! 😡"
        ];

        function runAway() {
            const noBtn = document.getElementById('noBtn');
            const yesBtn = document.getElementById('yesBtn');
            
            const maxX = window.innerWidth - noBtn.offsetWidth - 20;
            const maxY = window.innerHeight - noBtn.offsetHeight - 20;
            
            const randomX = Math.max(20, Math.floor(Math.random() * maxX));
            const randomY = Math.max(20, Math.floor(Math.random() * maxY));
            
            noBtn.style.position = 'fixed';
            noBtn.style.left = randomX + 'px';
            noBtn.style.top = randomY + 'px';
            
            noBtn.innerText = cheekyMessages[noClickCount % cheekyMessages.length];
            noClickCount++;

            let currentScale = 1 + (noClickCount * 0.15);
            yesBtn.style.transform = `scale(${currentScale})`;
        }
    </script>
</body>
</html>
