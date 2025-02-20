
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TVL - Website</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #FFDAB9;
            text-align: center;
        }
        .container {
            width: 50%;
            margin: auto;
            display: flex;
            flex-direction: column;
            align-items: center;
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
            padding: 20px;
            margin-top: 10px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0,0,0,0.1);
            width: 300px;
            text-align: center;
        }
    </style>
    <script>
        function showInfo(id) {
            var infos = document.querySelectorAll('.info');
            infos.forEach(info => info.style.display = 'none');
            document.getElementById(id).style.display = 'block';
        }
    </script>
</head>
<body>
    <h1>Welcome to TVL - Website</h1>
    <div class="container">
        <div class="profile">
            <img src="mariane.jpg" alt="Mariane" onclick="showInfo('mariane')">
        </div>
        <div class="profile">
            <img src="daisy.jpg" alt="Daisy" onclick="showInfo('daisy')">
        </div>
        <div class="profile">
            <img src="crizel.jpg" alt="Crizel" onclick="showInfo('crizel')">
        </div>
        <div class="profile">
            <img src="exequel.jpg" alt="Exequel" onclick="showInfo('exequel')">
        </div>
        <div class="profile">
            <img src="ashlee.jpg" alt="Ashlee" onclick="showInfo('ashlee')">
        </div>
    </div>
    
    <div id="mariane" class="info">
        <h2>Mariane Asumbrado Tejada</h2>
        <p>Age: 16</p>
        <p>Address: La Libertad Kapatagan LDN</p>
        <p>Email: asumbradomariane@gmail.com</p>
        <p><em>"Dreams will always stay dreams, unless you act upon them."</em></p>
    </div>
    
    <div id="daisy" class="info">
        <h2>Daisy A De Asir</h2>
        <p>Age: 18</p>
        <p>Address: Cogon Lala proper</p>
        <p>Email: deasirdaisy76@gmail.com</p>
        <p><em>"The best way to predict your future is to create it."</em></p>
    </div>
    
    <div id="crizel" class="info">
        <h2>Crizel Sumalpong Dioquino</h2>
        <p>Age: 18</p>
        <p>Address: Barangay Rebe LDN</p>
        <p>Email: 09853143274</p>
        <p><em>"Whenever you feel like giving up, look back and see how far you've come."</em></p>
    </div>
    
    <div id="exequel" class="info">
        <h2>Exequel Bentulan Canoos</h2>
        <p>Age: 17</p>
        <p>Address: Abaga LDN</p>
        <p>Email: canoosexequel0@gmail.com</p>
        <p><em>"Consciously release the past and choose to live in the present."</em></p>
    </div>
    
    <div id="ashlee" class="info">
        <h2>Ashlee E. Obial</h2>
        <p>Age: 17</p>
        <p>Address: Cabasagan LDN</p>
        <p>Email: ashleeobial19@gmail.com</p>
        <p><em>"LIVE, LAUGH, and LOVED."</em></p>
    </div>
</body>
</html>
