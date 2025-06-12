<html>
<head>
<title>Letzte Ehre erweisen</title>
<style>
body {
text-align: center;
font-family: Arial, sans-serif;
margin-top: 30px;
background-color: #f5f5f5;
}
h1 {
color: #333;
font-size: 18px;
margin-bottom: 20px;
padding: 0 10px;
}
#motorrad {
cursor: pointer;
width: 180px;
transition: transform 0.5s ease;
}
#counter {
font-size: 20px;
margin: 15px;
color: #555;
}
.hinweis {
font-size: 14px;
color: #777;
margin-top: 20px;
}
</style>
</head>
<body>
<h1>Damit wir ungefähr einschätzen können, wie viele keine letzte Ehre erweisen wollen, klicke bitte anonym auf dieses Motorrad:</h1>

<!-- Externes Motorrad-Bild (von deinem Link) -->
<img id="motorrad" src="https://szinezokvilaga.com/wp-content/uploads/2025/03/Alap-motor.jpg" alt="Motorrad">

<div id="counter">Anonyme Klicks: 0</div>
<p class="hinweis">Jeder Klick zählt als eine Person.</p>

<script>
let count = 0;
const motorrad = document.getElementById('motorrad');
const counter = document.getElementById('counter');

motorrad.addEventListener('click', () => {
count++;
counter.textContent = Anonyme Klicks: ${count};

// Motorrad umkippen lassen (Drehpunkt = untere Mitte)
motorrad.style.transform = "rotate(70deg)";
motorrad.style.transformOrigin = "center bottom";

// Nach 1 Sekunde zurücksetzen
setTimeout(() => {
motorrad.style.transform = "rotate(0deg)";
}, 1000);
});
</script>
</body>
</html>
