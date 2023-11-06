# Flor
Site feito para testar comandos
<!DOCTYPE html>
<html>
<head>
    <title>Formulário de Dados</title>
    <link rel="stylesheet" href="style.css">
  <style>
    #flores {
    display: flex;
    justify-content: space-around;
}

img {
    width: 300px;
    height: 300px;
}
</style>
</head>
<body>
    <h1>Gerador de imagens</h1>
    <hr>
    <h2>Tipos de Flores</h2>
    <div id="flores">
        <label for="girasol" id="girassol">Girassol</label>
        <br>
        <br>
        <label for="rosa" id="rosa">Rosa</label>
        <br>
        <br>
        <label for="tulipa" id="tulipa">Tulipa</label>
    </div>
    <h3>Resultado</h3>

    <p id="resultado"></p>
    <script src="script.js">
    let girassol = document.getElementById("girassol")
let rosa = document.getElementById("rosa")
let tulipa = document.getElementById("tulipa")
let resultado = document.getElementById("resultado")

//
girassol.addEventListener("mouseover", function(){
    resultado.innerText = "O Girassol (Helianthus annuus L.) é uma planta anual originária da América do Norte e Central, pertencente à família das Asteráceas Caracterizam-se por serem plantas de caule grosso e robusto, de coloração esverdeada. Podem atingir alturas que variam de 2 a 3 metros, porém existem também espécies anãs de 40 centímetros de altura. Suas folhas são ovais, opostas, pecioladas, com nervuras visíveis e ásperas. As flores são bonitas e grandiosas, e seu nome científico 'Helianthus' que significa 'flor do sol', traduz perfeitamente a imponência e porte majestoso desta planta.\n"
    let img = document.createElement("img")
    img.src = "img/girassol (3).jpg"
    resultado.append(img)
})
girassol.addEventListener("mouseout", function(){
    resultado.innerText = ""
})

//
rosa.addEventListener("mouseover", function () {
    resultado.innerText = "A rosa vermelha é um símbolo tradicional do amor. Mas está também ligada à paixão e ao desejo. Significa ainda a coragem, o respeito e a adoração. Trata-se de uma flor com forte representação em diversas culturas, designadamente na cigana, onde é utilizada para fazer magia e onde é associada ao romantismo.\n"
    let img = document.createElement("img")
    img.src = "img/rosa vermelha.jpg"
    resultado.append(img)
})

rosa.addEventListener("mouseout", function() {
    resultado.innerText = ""
})

//
tulipa.addEventListener("mouseover", function () {
    resultado.innerText = "A tulipa é um vegetal que pertence à divisão das angiospermas, plantas que produzem florações, e à família das liliáceas. Encontrada no nosso Planeta em pelo menos cem espécies, ela apresenta folhagem alongada, ovalada ou no formato de lanças. Do núcleo destas folhas ergue-se um caule aprumado, no qual desponta uma única flor constituída de seis pétalas.\n"
    let img = document.createElement("img")
    img.src = "img/tulipa.jpg"
    resultado.append(img)
})

tulipa.addEventListener("mouseout", function() {
    resultado.innerText = ""
})
    </script>
</body>
</html>
