<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Team Slideshow</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: #000;
            color: white;
            text-align: center;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
        }
        .slideshow {
            position: relative;
            width: 80%;
            height: 80vh;
        }
        .slide {
            position: absolute;
            width: 100%;
            height: 100%;
            opacity: 0;
            transition: opacity 1s;
        }
        .slide.active {
            opacity: 1;
        }
        img {
            width: 200px;
            border-radius: 10px;
        }
        audio {
            position: absolute;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
        }
    </style>
</head>
<body>
    <div class="slideshow">
        <div class="slide active">
            <img src="daisy.jpg" alt="Daisy A De Asir">
            <h2>Daisy A De Asir</h2>
            <p>Age: 18 | Address: Cogon Lala proper</p>
            <p>Email: deasirdaisy76@gmail.com</p>
            <p><em>"The best way to predict your future is to create it."</em></p>
        </div>
        <div class="slide">
            <img src="crizel.jpg" alt="Crizel Sumalpong Dioquino">
            <h2>Crizel Sumalpong Dioquino</h2>
            <p>Age: 18 | Address: Barangay Rebe LDN</p>
            <p>Email: 09853143274</p>
            <p><em>"Whenever you feel like giving up, look back and see how far you've come."</em></p>
        </div>
        <div class="slide">
            <img src="exequel.jpg" alt="Exequel Bentulan Canoos">
            <h2>Exequel Bentulan Canoos</h2>
            <p>Age: 17 | Address: Abaga LDN</p>
            <p>Email: canoosexequel0@gmail.com</p>
            <p><em>"Consciously release the past and choose to live in the present."</em></p>
        </div>
        <div class="slide">
            <img src="ashlee.jpg" alt="Ashlee E. Obial">
            <h2>Ashlee E. Obial</h2>
            <p>Age: 17 | Address: Cabasagan LDN</p>
            <p>Email: ashleeobial19@gmail.com</p>
            <p><em>"LIVE, LAUGH, and LOVED."</em></p>
        </div>
        <div class="slide">
            <img src="mariane.jpg" alt="Mariane Asumbrado Tejada">
            <h2>Mariane Asumbrado Tejada</h2>
            <p>Age: 16 | Address: La Libertad Kapatagan LDN</p>
            <p>Email: asumbradomariane@gmail.com</p>
            <p><em>"Dreams will always stay dreams, unless you act upon them."</em></p>
        </div>
    </div>
    
    <audio controls autoplay loop>
        <source src="9mm.mp3" type="audio/mpeg">
        Your browser does not support the audio element.
    </audio>
    
    <script>
        let slides = document.querySelectorAll('.slide');
        let index = 0;
        
        function showNextSlide() {
            slides[index].classList.remove('active');
            index = (index + 1) % slides.length;
            slides[index].classList.add('active');
        }
        
        setInterval(showNextSlide, 60000); // Change every 1 minute
    </script>
</body>
</html>
