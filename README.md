<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Día de las Flores Amarillas 🌻</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Comic Sans MS', cursive, sans-serif;
            background: linear-gradient(135deg, #FFE4E1, #E6E6FA, #F0E68C);
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.5s ease;
        }

        .main-menu {
            text-align: center;
            padding: 40px;
            background: rgba(255, 255, 255, 0.8);
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            backdrop-filter: blur(10px);
        }

        .surprise-btn {
            background: linear-gradient(45deg, #FFD700, #FFA500);
            border: none;
            padding: 20px 40px;
            border-radius: 50px;
            font-size: 24px;
            font-weight: bold;
            color: white;
            cursor: pointer;
            box-shadow: 0 8px 20px rgba(255, 215, 0, 0.4);
            transition: all 0.3s ease;
            animation: bounce 2s infinite;
        }

        .surprise-btn:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 25px rgba(255, 215, 0, 0.6);
        }

        .surprise-menu {
            display: none;
            text-align: center;
            padding: 30px;
            background: linear-gradient(135deg, #FFE4B5, #F0E68C, #DDA0DD);
            min-height: 100vh;
            animation: fadeIn 1s ease;
        }

        .surprise-menu.active {
            display: block;
        }

        .greeting-text {
            font-size: 28px;
            color: #8B4513;
            margin: 30px 0;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
            line-height: 1.4;
        }

        .pets-gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin: 40px 0;
            max-width: 1200px;
            margin-left: auto;
            margin-right: auto;
        }

        .pet-card {
            background: rgba(255, 255, 255, 0.9);
            border: 4px solid #98D8C8;
            border-radius: 20px;
            padding: 20px;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
            animation: slideIn 0.8s ease;
        }

        .pet-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.2);
        }

        .pet-photo {
            width: 100%;
            height: 250px;
            object-fit: cover;
            border-radius: 15px;
            border: 3px solid #90EE90;
            margin-bottom: 15px;
        }

        .back-btn {
            background: linear-gradient(45deg, #FF69B4, #FFB6C1);
            border: none;
            padding: 15px 30px;
            border-radius: 25px;
            font-size: 18px;
            color: white;
            cursor: pointer;
            margin-top: 30px;
            transition: all 0.3s ease;
        }

        .back-btn:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 20px rgba(255, 105, 180, 0.4);
        }

        .flowers-decoration {
            font-size: 40px;
            margin: 20px;
            animation: float 3s ease-in-out infinite;
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: scale(0.9); }
            to { opacity: 1; transform: scale(1); }
        }

        @keyframes slideIn {
            from { opacity: 0; transform: translateY(50px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }

        .title {
            font-size: 32px;
            color: #FFD700;
            text-shadow: 3px 3px 6px rgba(0, 0, 0, 0.3);
            margin-bottom: 30px;
        }

        @media (max-width: 768px) {
            .pets-gallery {
                grid-template-columns: 1fr;
                gap: 20px;
            }
            
            .greeting-text {
                font-size: 22px;
                padding: 0 20px;
            }
            
            .surprise-btn {
                font-size: 20px;
                padding: 15px 30px;
            }
        }
    </style>
</head>
<body>
    <div id="mainMenu" class="main-menu">
        <div class="flowers-decoration">🌻🌼🌻</div>
        <h1 class="title">¡Un día muy especial! ✨</h1>
        <button class="surprise-btn" onclick="showSurprise()">
            Sorpresa 👀
        </button>
        <div class="flowers-decoration">🌻🌼🌻</div>
    </div>

    <div id="surpriseMenu" class="surprise-menu">
        <div class="flowers-decoration">🌻✨🌻✨🌻</div>
        
        <div class="greeting-text">
            <strong>HOLAAAA,</strong><br>
            Yo, Milo, Cloe, Foca guatona y Gatito de complejo<br>
            te deseamos un <strong>feliz día de las flores amarillas</strong><br>
            <strong>BROOOOOOOOOOO⭐</strong>
        </div>

        <div class="pets-gallery">
            <div class="pet-card" style="animation-delay: 0.2s;">
                <img src="https://i.imgur.com/iMLBTSZ.jpeg" alt="Milo" class="pet-photo">
            </div>
            
            <div class="pet-card" style="animation-delay: 0.4s;">
                <img src="https://i.imgur.com/VO3aky4.jpeg" alt="Cloe" class="pet-photo">
            </div>
            
            <div class="pet-card" style="animation-delay: 0.6s;">
                <img src="https://i.imgur.com/Jr4OgIU.jpeg" alt="Foca guatona" class="pet-photo">
            </div>
            
            <div class="pet-card" style="animation-delay: 0.8s;">
                <img src="https://i.imgur.com/oEynBzU.jpeg" alt="Gatito de complejo" class="pet-photo">
            </div>
        </div>

        <div class="flowers-decoration">🌻⭐🌻⭐🌻</div>
        
        <button class="back-btn" onclick="goBack()">
            ← Regresar
        </button>
    </div>

    <script>
        function showSurprise() {
            document.getElementById('mainMenu').style.display = 'none';
            document.getElementById('surpriseMenu').classList.add('active');
            
            // Cambiar el fondo del body
            document.body.style.background = 'linear-gradient(135deg, #FFE4B5, #F0E68C, #DDA0DD)';
        }

        function goBack() {
            document.getElementById('surpriseMenu').classList.remove('active');
            document.getElementById('mainMenu').style.display = 'flex';
            
            // Restaurar el fondo original
            document.body.style.background = 'linear-gradient(135deg, #FFE4E1, #E6E6FA, #F0E68C)';
        }

        // Agregar un poco de magia con partículas flotantes
        function createFloatingFlower() {
            const flower = document.createElement('div');
            flower.innerHTML = '🌻';
            flower.style.position = 'fixed';
            flower.style.left = Math.random() * 100 + '%';
            flower.style.animationDuration = Math.random() * 3 + 2 + 's';
            flower.style.opacity = '0.7';
            flower.style.fontSize = '20px';
            flower.style.pointerEvents = 'none';
            flower.style.zIndex = '-1';
            
            document.body.appendChild(flower);
            
            setTimeout(() => {
                flower.remove();
            }, 5000);
        }

        // Crear flores flotantes cada cierto tiempo
        setInterval(createFloatingFlower, 3000);
    </script>
</body>
</html>
