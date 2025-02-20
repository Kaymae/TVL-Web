<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meet Our Team</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            color: white;
        }
        .video-bg {
            position: fixed;
            right: 0;
            bottom: 0;
            min-width: 100%;
            min-height: 100%;
            z-index: -1;
        }
        .container {
            position: relative;
            z-index: 1;
            padding: 50px 0;
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }
        .profile {
            background: rgba(0, 0, 0, 0.7);
            margin: 15px;
            padding: 20px;
            border-radius: 10px;
            width: 300px;
        }
        .profile img {
            width: 100%;
            border-radius: 10px;
        }
        h1 {
            margin-top: 50px;
        }
        #music-control {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background: rgba(0,0,0,0.5);
            padding: 10px;
            border-radius: 10px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <video class="video-bg" autoplay loop muted>
        <source src="background.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>
    
    <h1>Meet Our Team</h1>
    <div class="container">
        <div class="profile">
            <img src="daisy.jpg" alt="Daisy A De Asir">
            <h2>Daisy A De Asir</h2>
            <p>Age: 18</p>
            <p>Address: Cogon Lala proper</p>
            <p>Email: deasirdaisy76@gmail.com</p>
            <p><em>"The best way to predict your future is to create it."</em></p>
        </div>
        <div class="profile">
            <img src="crizel.jpg" alt="Crizel Sumalpong Dioquino">
            <h2>Crizel Sumalpong Dioquino</h2>
            <p>Age: 18</p>
            <p>Address: Barangay Rebe LDN</p>
            <p>Email: 09853143274</p>
            <p><em>"Whenever you feel like giving up, look back and see how far you've come."</em></p>
        </div>
        <div class="profile">
            <img src="exequel.jpg" alt="Exequel Bentulan Canoos">
            <h2>Exequel Bentulan Canoos</h2>
            <p>Age: 17</p>
            <p>Address: Abaga LDN</p>
            <p>Email: canoosexequel0@gmail.com</p>
            <p><em>"Consciously release the past and choose to live in the present."</em></p>
        </div>
        <div class="profile">
            <img src="ashlee.jpg" alt="Ashlee E. Obial">
            <h2>Ashlee E. Obial</h2>
            <p>Age: 17</p>
            <p>Address: Cabasagan LDN</p>
            <p>Email: ashleeobial19@gmail.com</p>
            <p><em>"LIVE, LAUGH, and LOVED."</em></p>
        </div>
        <div class="profile">
            <img src="mariane.jpg" alt="Mariane Asumbrado Tejada">
            <h2>Mariane Asumbrado Tejada</h2>
            <p>Age: 16</p>
            <p>Address: La Libertad Kapatagan LDN</p>
            <p>Email: asumbradomariane@gmail.com</p>
            <p><em>"Dreams will always stay dreams, unless you act upon them."</em></p>
        </div>
    </div>
    
    <audio id="background-music" loop>
        <source src="9mm.mp3" type="audio/mp3">
    </audio>
    <button id="music-control">Play Music</button>
    
    <script>
        const music = document.getElementById('background-music');
        const musicControl = document.getElementById('music-control');
        let isPlaying = false;

        musicControl.addEventListener('click', () => {
            if (isPlaying) {
                music.pause();
                musicControl.textContent = 'Play Music';
            } else {
                music.play();
                musicControl.textContent = 'Pause Music';
            }
            isPlaying = !isPlaying;
        });
    </script>
</body>
</html>
