# Brilliant--Ai-Os
Add a README file
Add Brilliant AI OS dashboard core
const BrilliantMemory = {
 save(key,value){
   localStorage.setItem(key, JSON.stringify(value));
 },
index.html
 load(key){
   return JSON.parse(localStorage.getItem(key));
 }
}

<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Brilliant AI OS</title>

<style>
body {
    margin:0;
    height:100vh;
    background:
    radial-gradient(circle at center,#123b66,#050814 70%);
    color:white;
    font-family:Arial, sans-serif;
    display:flex;
    justify-content:center;
    align-items:center;
    overflow:hidden;
}

.core {
    text-align:center;
}

.logo {
    font-size:45px;
    font-weight:bold;
    letter-spacing:8px;
    color:#65d8ff;
    text-shadow:
    0 0 20px #00aaff,
    0 0 40px #0066ff;
}

.diamond {
    width:90px;
    height:90px;
    margin:40px auto;
    transform:rotate(45deg);
    background:#39c6ff;
    box-shadow:
    0 0 20px #00c8ff,
    0 0 60px #0088ff;
    animation:pulse 2s infinite;
}

@keyframes pulse {
    0%,100% {
        opacity:.8;
        transform:rotate(45deg) scale(1);
    }
    50% {
        opacity:1;
        transform:rotate(45deg) scale(1.15);
    }
}

.subtitle {
    color:#b9eaff;
    font-size:20px;
    margin-bottom:40px;
}

button {
    padding:15px 40px;
    border-radius:30px;
    border:1px solid #3bcfff;
    background:transparent;
    color:white;
    font-size:18px;
    cursor:pointer;
    box-shadow:0 0 20px #008cff;
}

button:hover {
    background:#008cff;
}
</style>

</head>

<body>

<div class="core">

<div class="logo">
BRILLIANT AI
</div>

<div class="diamond"></div>

<div class="subtitle">
Познать. Понять. Сохранить будущее.
</div>

<button onclick="enterOS()">
▶ Enter Universe
</button>

</div>


<script>

function enterOS(){

window.location.href="dashboard.html";

}

</script>

</body>
</html>
