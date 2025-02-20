
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
        .profile {
            background: white;
            margin: 15px;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0,0,0,0.1);
            width: 250px;
            text-align: center;
            cursor: pointer;
        }
        .profile img {
            width: 150px;
            height: 150px;
            border-radius: 10px;
            object-fit: cover;
        }
        .info {
            display: none;
        }
    </style>
    <script>
        function showInfo(id) {
            var elements = document.getElementsByClassName("info");
            for (var i = 0; i < elements.length; i++) {
                elements[i].style.display = "none";
            }
            document.getElementById(id).style.display = "block";
        }
    </script>
</head>
<body>
    <h1>Welcome to TVL - Website</h1>
    <div class="container">
        <div class="profile" onclick="showInfo('daisy-info')">
            <img src="daisy.jpg" alt="Daisy A De Asir">
        </div>
        <div class="profile" onclick="showInfo('crizel-info')">
            <img src="crizel.jpg" alt="Crizel Sumalpong Dioquino">
        </div>
        <div class="profile" onclick="showInfo('exequel-info')">
            <img src="exequel.jpg" alt="Exequel Bentulan Canoos">
        </div>
        <div class="profile" onclick="showInfo('ashlee-info')">
            <img src="ashlee.jpg" alt="Ashlee E. Obial">
        </div>
        <div class="profile" onclick="showInfo('mariane-info')">
            <img src="mariane.jpg" alt="Mariane Asumbrado Tejada">
        </div>
    </div>
    <div class="container">
        <div id="daisy-info" class="info">
            <h2>Daisy A De Asir</h2>
            <p>Age: 18</p>
            <p>Address: Cogon Lala proper</p>
            <p>Email: deasirdaisy76@gmail.com</p>
            <p><em>"The best way to predict your future is to create it."</em></p>
        </div>
        <div id="crizel-info" class="info">
            <h2>Crizel Sumalpong Dioquino</h2>
            <p>Age: 18</p>
            <p>Address: Barangay Rebe LDN</p>
            <p>Email: 09853143274</p>
            <p><em>"Whenever you feel like giving up, look back and see how far you've come."</em></p>
        </div>
        <div id="exequel-info" class="info">
            <h2>Exequel Bentulan Canoos</h2>
            <p>Age: 17</p>
            <p>Address: Abaga LDN</p>
            <p>Email: canoosexequel0@gmail.com</p>
            <p><em>"Consciously release the past and choose to live in the present."</em></p>
        </div>
        <div id="ashlee-info" class="info">
            <h2>Ashlee E. Obial</h2>
            <p>Age: 17</p>
            <p>Address: Cabasagan LDN</p>
            <p>Email: ashleeobial19@gmail.com</p>
            <p><em>"LIVE, LAUGH, and LOVED."</em></p>
        </div>
        <div id="mariane-info" class="info">
            <h2>Mariane Asumbrado Tejada</h2>
            <p>Age: 16</p>
            <p>Address: La Libertad Kapatagan LDN</p>
            <p>Email: asumbradomariane@gmail.com</p>
            <p><em>"Dreams will always stay dreams, unless you act upon them."</em></p>
        </div>
    </div>
</body>
</html>
