
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Team Profiles</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #FFDAB9;
            text-align: center;
        }
        .container {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }
        .profile img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            cursor: pointer;
            transition: transform 0.3s;
        }
        .profile img:hover {
            transform: scale(1.1);
        }
        .info {
            display: none;
            background: white;
            margin-top: 20px;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0,0,0,0.1);
            width: 300px;
            margin-left: auto;
            margin-right: auto;
        }
    </style>
    <script>
        function showInfo(id) {
            document.querySelectorAll('.info').forEach(info => info.style.display = 'none');
            document.getElementById(id).style.display = 'block';
        }
    </script>
</head>
<body>
    <h1>Welcome to TVL - Website</h1>
    <div class="container">
        <div class="profile" onclick="showInfo('info1')">
            <img src="mariane.jpg" alt="Mariane Asumbrado Tejada">
        </div>
        <div class="profile" onclick="showInfo('info2')">
            <img src="daisy.jpg" alt="Daisy A De Asir">
        </div>
        <div class="profile" onclick="showInfo('info3')">
            <img src="crizel.jpg" alt="Crizel Sumalpong Dioquino">
        </div>
        <div class="profile" onclick="showInfo('info4')">
            <img src="exequel.jpg" alt="Exequel Bentulan Canoos">
        </div>
        <div class="profile" onclick="showInfo('info5')">
            <img src="ashlee.jpg" alt="Ashlee E. Obial">
        </div>
    </div>
    
    <div id="info1" class="info">
        <h2>Mariane Asumbrado Tejada</h2>
        <p>Age: 16 years old</p>
        <p>Address: La Libertad Kapatagan LDN</p>
        <p>Email: asumbradomariane@gmail.com</p>
        <p><em>"Dreams will always stay dreams, unless you act upon them."</em></p>
    </div>
    <div id="info2" class="info">
        <h2>Daisy A De Asir</h2>
        <p>Age: 18 years old</p>
        <p>Address: Cogon Lala proper</p>
        <p>Email: deasirdaisy76@gmail.com</p>
        <p><em>"The best way to predict your future is to create it."</em></p>
    </div>
    <div id="info3" class="info">
        <h2>Crizel Sumalpong Dioquino</h2>
        <p>Age: 18 years old</p>
        <p>Address: Barangay Rebe LDN</p>
        <p>Email: 09853143274</p>
        <p><em>"Whenever you feel like giving up, look back and see how far you've come."</em></p>
    </div>
    <div id="info4" class="info">
        <h2>Exequel Bentulan Canoos</h2>
        <p>Age: 17 years old</p>
        <p>Address: Abaga LDN</p>
        <p>Email: canoosexequel0@gmail.com</p>
        <p><em>"Consciously release the past and choose to live in the present."</em></p>
    </div>
    <div id="info5" class="info">
        <h2>Ashlee E. Obial</h2>
        <p>Age: 17 years old</p>
        <p>Address: Cabasagan LDN</p>
        <p>Email: ashleeobial19@gmail.com</p>
        <p><em>"LIVE, LAUGH, and LOVED."</em></p>
    </div>
</body>
</html>
