# solo-rush1

-> HTML :

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Elite Shushi</title>
</head>
    <header>
        <nav>
            <img src="./image.png/logo-mobile.png" alt="logo" id="logo">
            <ul>
                <li><a href="#">Acceuil</a></li>
                <li><a href="#">Nos magasin</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    <section>
        <h1>Elite Sushi</h1>
    </section>
    </header>
<body>
    <main id="main-container">
        <section>
            <h2 id="acceuil">Acceuil</h2>
            <div class="articles">
                <article>
                    <img src="./image.png/Photo 5.webp" alt="">
                    <h3>Bawls</h3>
                    <h4>Prix: 19,99$</h4>
                    <button type="button">Acheter</button>
                </article>
                <article>
                    <img src="./image.png/Photo 7.webp" alt="">
                    <h3>Sushi</h3>
                    <h4>Prix: 11,99$</h4>
                    <button type="button">Acheter</button>
                </article>
                <article>
                    <img src="./image.png/Photo 8.webp" alt="">
                    <h3>Mocchi</h3>
                    <h4>Prix: 7,99$</h4>
                    <button type="button">Acheter</button>
                </article>
            </div>
        </section>
        <section class="magasin">
            <div class="image-container">
                <img src="./image.png/Devanture.jpg" alt="Devanture du restaurant Elite Sushi">
            </div>
            <div class="text-container">
                <h2>Bienvenue chez Elite Sushi</h2>
                <p>Plongez dans un univers où la gastronomie japonaise rencontre l'élégance. Chez <strong>Elite Sushi</strong>, nous mettons un point d'honneur à vous offrir des plats raffinés, préparés avec des ingrédients d'exception. Venez découvrir une ambiance unique et un voyage culinaire inoubliable.</p>
                <p><strong> Adresse :</strong> 4 rue boulevard de paris</p>
                <p><strong> Réservation :</strong> 03.XX.XX.XX.XX</p>
            </div>
        </section>
    </main>
    <footer>
        <section>
            <div class="contact">
                <h2>contacter-nous</h2>
                <h3>Tel:</h3>
                <h4>03.XX.XX.XX.XX</h4>
                <h3>Email:</h3>
                <h4>Elite.Sushi@gmail.com</h4>
            </div>
        </section>
        © 2025 wilders
    </footer>
</body>
</html>

-> CSS 

:root {
    --primary: #aaaaaa; 
    --secondary: #000000; 
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    width: 100%;
    min-height: 100vh;
}

header {
    background-color: var(--secondary);
    padding: 1rem;
}

header > nav {
    display: flex;
    align-items: center;
    flex-direction: column;
    text-align: center;

    @media screen and (min-width: 992px) {
        flex-direction: row;
        justify-content: space-between;
    
    }

}


header > h1 {
    color: white;
}

#logo {
    width: 100px;
    padding: 10px;
}

header > nav > ul {
    display: flex;
    flex-direction: row;
    list-style: none;

    @media screen and (min-width: 768px) {
        flex-direction: row;
    }
}


header > nav > ul > li > a {
    color: white;
    text-decoration: none;
    padding: 10px;
    display: block;
}

header > section {
    display: flex;
    align-items: center;
    flex-direction: column;
    padding: 1rem;
    text-align: center;
}

main {
    background-color: var(--primary);
    padding: 1rem;
}

#acceuil {
    color: transparent;
}

#articles {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1rem;
    justify-content: center;
    padding: 1rem;

}



article {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
    max-width: 400px;
    margin: 0 auto;
    padding: 10px;
    border-radius: 8px;

}

article img {
    width: 100%;
    max-width: 250px;
    height: auto;
}

article h4 {
    padding: 5px;
    text-align: center;
}

article button {
    background-color: var(--secondary);
    color: white;
    border: none;
    padding: 0.5rem 2.5rem;
    text-transform: uppercase;
    border-radius: 25px;
    margin: 0.5rem;
}

#main-container h2 {
    text-align: center;
}

.magasin {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 50px;
    background-color: white;
    max-width: 800px;
    margin: 30px auto;
    border-radius: 8px;
    text-align: center;
}

.image-container {
    width: 100%;
    margin-top: 20px;
}

.image-container > img {
    width: 100%;
    height: auto;
    border-radius: 10px;
}

.text-container {
    padding: 18px;
    color: black;
}

.text-container > h2 {
    font-size: 28px;
    margin-bottom: 15px;
}

.text-container > p {
    font-size: 18px;
    color: var(--secondary);
    line-height: 1.5;
}

.text-container > a {
    text-decoration: none;
    font-weight: bold;
}

.text-container > a:hover {
    text-decoration: underline;
}

.contact {
    display: flex;
    flex-direction: column;
    padding: 20px;
    background-color: black;
    max-width: 800px;
    text-align: center;
    color: white;
    border-radius: 8px;
    margin: auto;
}

.contact > h2 {
    padding: 8px;
}

.contact h3 {
    padding: 5px;
}

footer {
    text-align: center;
    background-color: black;
    color: white;
    padding: 1rem;
}
