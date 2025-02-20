<!DOCTYPE html>
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
            width: 80%;
            margin: auto;
            display: flex;
            flex-direction: row;
            justify-content: center;
            gap: 20px;
        }
        .profile {
            background: white;
            margin: 15px;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0,0,0,0.1);
            width: 300px;
            text-align: center;
            display: none;
        }
        .profile img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            cursor: pointer;
        }
        h2, p {
            margin: 10px 0;
        }
    </style>
    <script>
        function showProfile(id) {
            var profiles = document.querySelectorAll('.profile');
            profiles.forEach(profile => profile.style.display = 'none');
            document.getElementById(id).style.display = 'block';
        }
    </script>
</head>
<body>
    <h1>Welcome to TVL - Website</h1>
    <div class="container">
        <img src="daisy.jpg" alt="Daisy A De Asir" onclick="showProfile('daisy')">
        <img src="crizel.jpg" alt="Crizel Sumalpong Dioquino" onclick="showProfile('crizel')">
        <img src="exequel.jpg" alt="Exequel Bentulan Canoos" onclick="showProfile('exequel')">
        <img src="ashlee.jpg" alt="Ashlee E. Obial" onclick="showProfile('ashlee')">
        <img src="mariane.jpg" alt="Mariane Asumbrado Tejada" onclick="showProfile('mariane')">
    </div>
    <div id="daisy" class="profile">
        <h2>Daisy A De Asir</h2>
        <p>Age: 18</p>
        <p>Address: Cogon Lala proper</p>
        <p>Email: deasirdaisy76@gmail.com</p>
        <p><em>"The best way to predict your future is to create it."</em></p>
    </div>
    <div id="crizel" class="profile">
        <h2>Crizel Sumalpong Dioquino</h2>
        <p>Age: 18</p>
        <p>Address: Barangay Rebe LDN</p>
        <p>Email: 09853143274</p>
        <p><em>"Whenever you feel like giving up, look back and see how far you've come."</em></p>
    </div>
    <div id="exequel" class="profile">
        <h2>Exequel Bentulan Canoos</h2>
        <p>Age: 17</p>
        <p>Address: Abaga LDN</p>
        <p>Email: canoosexequel0@gmail.com</p>
        <p><em>"Consciously release the past and choose to live in the present."</em></p>
    </div>
    <div id="ashlee" class="profile">
        <h2>Ashlee E. Obial</h2>
        <p>Age: 17</p>
        <p>Address: Cabasagan LDN</p>
        <p>Email: ashleeobial19@gmail.com</p>
        <p><em>"LIVE, LAUGH, and LOVED."</em></p>
    </div>
    <div id="mariane" class="profile">
        <h2>Mariane Asumbrado Tejada</h2>
        <p>Age: 16</p>
        <p>Address: La Libertad Kapatagan LDN</p>
        <p>Email: asumbradomariane@gmail.com</p>
        <p><em>"Dreams will always stay dreams, unless you act upon them."</em></p>
    </div>
</body>
</html>
