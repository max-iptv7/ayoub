<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About Ayoub Chaibi</title>
    <!-- FontAwesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* General Styles */
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #1a1a1a, #2c3e50);
            color: #fff;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            text-align: center;
        }

        .container {
            background: rgba(255, 255, 255, 0.1);
            padding: 40px;
            border-radius: 20px;
            backdrop-filter: blur(15px);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
            max-width: 600px;
            width: 90%;
            animation: fadeIn 1.5s ease-in-out;
        }

        h1 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            color: #ffdd57;
        }

        .profile-image {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 4px solid #ffdd57;
            margin-bottom: 20px;
            object-fit: cover;
            transition: transform 0.3s ease;
        }

        .profile-image:hover {
            transform: scale(1.1);
        }

        p {
            font-size: 1.1rem;
            line-height: 1.6;
            margin-bottom: 20px;
        }

        .highlight {
            color: #ffdd57;
            font-weight: bold;
        }

        .relationship-status {
            font-size: 1.2rem;
            margin-top: 20px;
            color: #ffdd57;
            cursor: pointer;
            text-decoration: underline;
            transition: color 0.3s ease;
        }

        .relationship-status:hover {
            color: #ffcc00;
        }

        .marouma-description {
            display: none;
            margin-top: 20px;
            font-size: 1rem;
            color: #fff;
            background: rgba(0, 0, 0, 0.3);
            padding: 15px;
            border-radius: 10px;
            animation: slideIn 0.5s ease;
        }

        .social-links {
            margin-top: 30px;
        }

        .social-links a {
            margin: 0 15px;
            text-decoration: none;
            color: #fff;
            font-size: 1.5rem;
            transition: color 0.3s ease, transform 0.3s ease;
        }

        .social-links a:hover {
            color: #ffdd57;
            transform: translateY(-5px);
        }

        .cta-button {
            margin-top: 30px;
            padding: 12px 24px;
            background: #ffdd57;
            color: #1a1a1a;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            font-size: 1rem;
            font-weight: bold;
            transition: background 0.3s ease, transform 0.3s ease;
            display: inline-block;
        }

        .cta-button:hover {
            background: #ffcc00;
            transform: translateY(-5px);
        }

        .marouma-button {
            margin-top: 20px;
            padding: 10px 20px;
            background: #ff6b6b;
            color: #fff;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            font-size: 1rem;
            font-weight: bold;
            transition: background 0.3s ease, transform 0.3s ease;
            display: inline-block;
        }

        .marouma-button:hover {
            background: #ff4757;
            transform: translateY(-5px);
        }

        /* Animations */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes slideIn {
            from { opacity: 0; transform: translateY(-10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }

        .pulse-animation {
            animation: pulse 2s infinite;
        }
    </style>
</head>
<body>
    <div class="container">
        <img src="https://media.discordapp.net/attachments/1335949141230096418/1336033334454779904/IMG_4495.jpg?ex=67dd0041&is=67dbaec1&hm=03445e4d37ac73f5b427abcb59cbbce9a2b2a1459c857ffd62435b2015928e52&" alt="Ayoub Chaibi" class="profile-image">
        <h1>Hi, I'm <span class="highlight">Ayoub Chaibi</span></h1>
        <p>
            I am a full-stack developer with a passion for technology and innovation. I specialize in building modern web applications using cutting-edge technologies like React, Node.js, and more. My goal is to create seamless user experiences and solve real-world problems through code.
        </p>
        <div class="relationship-status" onclick="showMaroumaDescription()">
            💍 Partnered with <span class="highlight">Marouma</span>
        </div>
        <div id="maroumaDescription" class="marouma-description">
            Marouma is the love of my life. She is my partner in everything, and together we make an unstoppable team. My love for her is 1000%! ❤️
        </div>
        <button class="marouma-button pulse-animation" onclick="showMaroumaDescription()">
            Click to know more about Marouma 💖
        </button>
        <div class="social-links">
            <a href="https://twitter.com/AyoubChaibi" target="_blank"><i class="fab fa-twitter"></i></a>
            <a href="https://github.com/AyoubChaibi" target="_blank"><i class="fab fa-github"></i></a>
            <a href="https://linkedin.com/in/AyoubChaibi" target="_blank"><i class="fab fa-linkedin"></i></a>
            <a href="https://instagram.com/ayoub.chaibi811" target="_blank"><i class="fab fa-instagram"></i></a>
        </div>
        <button class="cta-button" onclick="window.location.href='https://instagram.com/ayoub.chaibi811'">
            Contact Me <i class="fas fa-arrow-right"></i>
        </button>
    </div>

    <script>
        function showMaroumaDescription() {
            const description = document.getElementById("maroumaDescription");
            if (description.style.display === "none" || description.style.display === "") {
                description.style.display = "block";
            } else {
                description.style.display = "none";
            }
        }
    </script>
</body>
</html>
