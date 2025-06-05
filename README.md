# mypets

#html
```html
<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>My Pets</title>
</head>

<body>
    <!--O restante do cod HTML será inserido aqui-->

    <header id="cabecalho">
        <img src="./assets/logo.png" alt="Logo">
        <h1>MY PETS</h1>
        <nav>
            <ul>
                <li><a href="#banner">Home</a></li>
                <li><a href="#Sobre">Sobre</a></li>
                <li><a href="#contato">Contato</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="banner"></section>

        <section id="Sobre">
            <h2>Sobre o site</h2>
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ratione consectetur, quisquam mollitia esse
                officia amet deleniti quod praesentium odit dolorum? Corrupti accusamus rerum, autem aperiam cumque,
                explicabo id ipsa tempore suscipit quasi recusandae esse, tempora neque! Placeat quia eligendi sit
                cupiditate dolores ipsa eum minus, amet repellendus perspiciatis, sint laborum.</p>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Odit, iure consequuntur fuga nesciunt animi,
                magnam, sunt debitis laboriosam earum repellendus deleniti voluptatibus necessitatibus suscipit
                molestias quas amet. Quam quibusdam eligendi adipisci accusamus hic dolorum veniam quidem quod.
                Provident in laboriosam tempora at! Reiciendis maiores debitis provident eaque laudantium? Sed, eveniet!
            </p>

            <a href="#cabecalho"><img src="./assets/up.png" alt="subir"></a>

            <section>
                <h2>GALERIA DE FOTOS</h2>
                <div class="container">
                    <img src="./assets/dog1.jpg" alt="5">
                    <img src="./assets/dog2.jpg" alt="">
                    <img src="./assets/cat1.jpg" alt="">
                    <img src="./assets/cat2.jpg" alt="">
                </div>
            </section>
        </section>

        <section id="contato">
            <h2>Contate-nos</h2>
            <p>Estamos sempre prontos...</p>
            <div class="contatct-info">

                <div><strong>Email:</strong><a href="malito:contato@mypets.com"></a></div>
                <div><strong>Telefone:</strong>+55 11 1234-5678</div>
                <div><strong>WhatsApp:</strong><a href="htpps://wa.me/551112345678"target="_blanck">+55 11 1234-5678</a></div>

            </div>
        </section>

        <a href="#cabecalho"><img src="./assets/up.png" alt="subir"></a>

    </main>

    <footer>
        <a href="#"><img src="./assets/face.png" alt="Facebook"></a>
        <a href="#"><img src="./assets/insta.png" alt="Instagram"></a>
        <a href="#"><img src="./assets/tiktok.png" alt="TikTok"></a>
        <p>&copy;2023 My Pets</p>
    </footer>
</body>

</html>
```

#css
```css
body,
h1,
h2,
p,
ul,
li {
    margin: 0;
    padding: 0;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    background: linear-gradient(45deg, #c9c8c8 12%, #ac3939 21%, #4e0101 100%)
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 5%;
    color: rgb(6, 6, 6);
    background-color: whitesmoke;
    position: relative;
    z-index: 2;
}

header h1 {
    font-size: 2rem;
}

nav ul {
    list-style-type: none;
    display: flex;
    gap: 1rem;
}

nav a {
    text-decoration: none;
    color: black;
    background-color: #7c5454;
    padding: 15px;
    border-radius: 15px 0px;
    transition: 0.3 ease;
}
nav a:hover{
    color: white;
    text-decoration: none;
    background-color: #4e0101;
    padding: 15px;
    border-radius: 0px 15px;
}

/*estilizaçao das seçoes*/
#banner {
    position: relative;
    background-image: url(./assets/gatinho.jpg);
    height: 300px;
    background-position: center;
    background-size: cover;
    background-attachment: fixed;
    overflow: hidden;
    z-index: 1;
}

#banner::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.4);
}

main {
    padding: 2rem 5%;
}

section {
    margin: 50px;
    padding: 20px;
}

section p {
    text-align: justify;
    color: white;
    font-size: 14pt;
    padding: 20px;
}

section h2 {
    color: white;
    padding: 20px;
}

#contato {
    border: 2px solid black;
    background-color: #7c5454;
}

.contact-info {
    margin-top: 1rem;
}
.contact-info>div{
    margin-bottom: 0.5rem;
}
.contact-info a{
    color: #007bff;
}
.contact-info a:hover{
    text-decoration: underline;
}
.container{
    display: flex;
    justify-content: space-around;
    align-items: center;
    gap: 10px;
    flex-wrap: wrap;
}
.container img{
    width: 500px;
    height: 400px;
}
/*Estilização do footer*/
footer{
    height: 150px;
    background-color: #7c5454;
    padding: 1rem 5%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
footer img{
    width: 100px;
    margin-right: 1rem;
}

@media screen and(max-width: 768px){
    header, main, footer{
        padding: 1rem 2%;
    }
}
```
