# Evaluation GIT 17/04/2025

DUBRULLE Guerlin
B1CS1

### Commande effectué :

Création du Reposit : https://github.com/Chizzy-mio/evalmasson.git

Partie html :

```html
<body>
    

    <header>
        <img src="images/image1.jpg" alt="Logo">
    </header>

    <nav>
        <a href="pages/page1.html">Page1</a>
        <a href="pages/page2.html">Page2</a>
        <a href="pages/page3.html">Page3</a>
    </nav>

    <main>
        <h1>Accueil</h1>
</main>

    <aside>
        <img src="images/image1.jpg" alt="Pub">
    </aside>

    <footer>
        &copy; copyrigth
    </footer>

</body>
```

```bash
#push sur github
git init 
git remote add https://github.com/Chizzy-mio/evalmasson.git
git config user.name "Chizzy-mio"
git config user.email "mioochizzy@gmail"
```

Création de la branche master :
```bash
git add .
git commit -m "Page principale"
git push origin -u master
```

MobileCSS :

```bash
#Je reprend les modifs de mes camarades
git pull origin master
    #ou
git clone https://github.com/Chizzy-mio/evalmasson.git
git config user.name "Chizzy-mio"
git config user.email "mioochizzy@gmail"
```

-> Modif du mobile css : 

```css
* {
    margin: 0;
    padding: 0;
  
}
body{
    display: flex;
    flex-wrap: wrap;
}
header{
    background-color: lightblue;
    width: 100%;
    height: 10%;
    display: flex;
}   
header img{
    padding: 1%;
    width: 10%;
}
main{
    width: 50%;
}

nav{
    background: #575858;
    width: 25%;
}

nav a {
    display: block;
    text-decoration: none;
    width: 80%;
    margin: 1em auto;
    background: rgb(255, 255, 255);
    color: black;
    text-align: center;
    padding: 1em;
}
aside{
    background-color: rgb(231, 231, 224);
    width: 25%;
}
aside img{
    display: block;
    width: 100%;
    padding: 1em;
}
footer{
    background-color: brown;
    width: 100%;
    padding: 3%;
    text-align: center;
}
```

```bash
#je crée une branche avec que les modif du mobilecss
git branch mobilecssguerlin
git checkout mobilecssguerlin
#je push toute mes modif dans la branche
git add .
git commit -m "MobileCSS Guerlin"
git push origin Mobilecssguerlin

#je reviens dans la branche master pour fusionner avec mes modif car je suis sur d'utiliser ces paramètres
git checkout master
git merge mobilecssguerlin
git push origin master
```