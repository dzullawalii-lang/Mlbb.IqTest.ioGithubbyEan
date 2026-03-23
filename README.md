# Mlbb.IqTest.ioGithubbyEan
Eannnnnn
<!DOCTYPE html>
<html>
<head>
<title>Tes IQ MLBB</title>
<style>
body{
    font-family: Arial;
    background:#0f172a;
    color:white;
    text-align:center;
}
.container{
    width:80%;
    margin:auto;
    background:#1e293b;
    padding:20px;
    border-radius:10px;
}
button{
    padding:10px 20px;
    background:#facc15;
    border:none;
    border-radius:5px;
    cursor:pointer;
}
</style>
</head>

<body>

<div class="container">
<h1>Tes IQ MLBB</h1>
<p>Jawab 5 pertanyaan sulit untuk mengetahui IQ bermain MLBB kamu.</p>

<form id="quiz">

<p>1. Saat turtle spawn dan gold lane sedang ditekan musuh, apa keputusan terbaik?</p>
<input type="radio" name="q1" value="1"> Fokus farm sendiri<br>
<input type="radio" name="q1" value="2"> Bantu turtle bersama tim<br>
<input type="radio" name="q1" value="3"> Push turret sendirian<br>

<p>2. Sebagai roamer, kapan waktu terbaik membuka map?</p>
<input type="radio" name="q2" value="3"> Sebelum war untuk cek posisi musuh<br>
<input type="radio" name="q2" value="1"> Saat HP sekarat<br>
<input type="radio" name="q2" value="2"> Setelah war selesai<br>

<p>3. Tim kamu unggul 3 hero mati musuh. Apa yang paling prioritas?</p>
<input type="radio" name="q3" value="3"> Ambil Lord atau objektif<br>
<input type="radio" name="q3" value="1"> Recall spam<br>
<input type="radio" name="q3" value="2"> Kejar kill lagi<br>

<p>4. Jika core tim mati sebelum Lord fight?</p>
<input type="radio" name="q4" value="3"> Mundur dan clear lane<br>
<input type="radio" name="q4" value="1"> Tetap war 4v5<br>
<input type="radio" name="q4" value="2"> Solo ambil Lord<br>

<p>5. Apa tanda player punya macro bagus?</p>
<input type="radio" name="q5" value="3"> Fokus objektif dan map control<br>
<input type="radio" name="q5" value="1"> Banyak kill saja<br>
<input type="radio" name="q5" value="2"> Damage paling tinggi<br>

<br><br>
<button type="button" onclick="hasil()">Lihat Hasil</button>

</form>

<h2 id="result"></h2>

</div>

<script>
function hasil(){

let score = 0;

let q1 = document.querySelector('input[name="q1"]:checked');
let q2 = document.querySelector('input[name="q2"]:checked');
let q3 = document.querySelector('input[name="q3"]:checked');
let q4 = document.querySelector('input[name="q4"]:checked');
let q5 = document.querySelector('input[name="q5"]:checked');

if(q1) score += parseInt(q1.value);
if(q2) score += parseInt(q2.value);
if(q3) score += parseInt(q3.value);
if(q4) score += parseInt(q4.value);
if(q5) score += parseInt(q5.value);

let result = "";

if(score <= 7){
result = "IQ MLBB: 60 🗿 (Dark System Candidate)";
}
else if(score <= 11){
result = "IQ MLBB: 90 🙂 (Player Biasa)";
}
else{
result = "IQ MLBB: 120 🔥 (Roam Idaman)";
}

document.getElementById("result").innerText = result;

}
</script>

</body>
</html>
