
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TVL Website - Team Profiles</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #FFDAB9;
            text-align: center;
        }
        .container {
            width: 80%;
            margin: auto;
        }
        .profile {
            background: white;
            margin: 15px;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0,0,0,0.1);
            border: 2px solid black;
            text-align: center;
            display: none;
        }
        .profile img {
            width: 100%;
            border-radius: 10px;
        }
        h2, p {
            margin: 10px 0;
        }
        .nav {
            margin: 20px;
        }
        .nav button {
            padding: 10px;
            margin: 5px;
            border: none;
            background: #FFB6C1;
            cursor: pointer;
            font-size: 16px;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <h1>Welcome to TVL- Website</h1>
    <h2>Meet Our Team</h2>
    <div class="nav">
        <button onclick="showProfile(1)">1</button>
        <button onclick="showProfile(2)">2</button>
        <button onclick="showProfile(3)">3</button>
        <button onclick="showProfile(4)">4</button>
        <button onclick="showProfile(5)">5</button>
    </div>
    <div class="container">
        <div class="profile" id="profile1">
            <img src="daisy.jpg" alt="Daisy A De Asir">
            <h2>Daisy A De Asir</h2>
            <p>Age: 18</p>
            <p>Address: Cogon Lala proper</p>
            <p>Email: deasirdaisy76@gmail.com</p>
            <p><em>"The best way to predict your future is to create it."</em></p>
        </div>
        <div class="profile" id="profile2">
            <img src="crizel.jpg" alt="Crizel Sumalpong Dioquino">
            <h2>Crizel Sumalpong Dioquino</h2>
            <p>Age: 18</p>
            <p>Address: Barangay Rebe LDN</p>
            <p>Email: 09853143274</p>
            <p><em>"Whenever you feel like giving up, look back and see how far you've come."</em></p>
        </div>
        <div class="profile" id="profile3">
            <img src="exequel.jpg" alt="Exequel Bentulan Canoos">
            <h2>Exequel Bentulan Canoos</h2>
            <p>Age: 17</p>
            <p>Address: Abaga LDN</p>
            <p>Email: canoosexequel0@gmail.com</p>
            <p><em>"Consciously release the past and choose to live in the present."</em></p>
        </div>
        <div class="profile" id="profile4">
            <img src="ashlee.jpg" alt="Ashlee E. Obial">
            <h2>Ashlee E. Obial</h2>
            <p>Age: 17</p>
            <p>Address: Cabasagan LDN</p>
            <p>Email: ashleeobial19@gmail.com</p>
            <p><em>"LIVE, LAUGH, and LOVED."</em></p>
        </div>
        <div class="profile" id="profile5">
            <img src="mariane.jpg" alt="Mariane Asumbrado Tejada">
            <h2>Mariane Asumbrado Tejada</h2>
            <p>Age: 16</p>
            <p>Address: La Libertad Kapatagan LDN</p>
            <p>Email: asumbradomariane@gmail.com</p>
            <p><em>"Dreams will always stay dreams, unless you act upon them."</em></p>
        </div>
    </div>
    <script>
        function showProfile(num) {
            let profiles = document.querySelectorAll('.profile');
            profiles.forEach(profile => profile.style.display = 'none');
            document.getElementById('profile' + num).style.display = 'block';
        }
    </script>
</body>
</html>
