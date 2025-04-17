## GIT TP TEST
 GROUPE SAMUEL BRONES / ANDREAS CROUZILHAT / GUERLIN DUBRULLE


1. Je récupère le reposit

 ```bash 
 cd Documents/evalgit
 git clone https://github.com/Chizzy-mio/evalmasson.git
 git config user.name "mewgame"
 git config user.email "poke.brones@gmail.com"
 ```

2. je me mets dans le dossier et vérifie si il y a tout
```bash
cd evalmasson
ls
git branch
```

3. je me mets dans le css pour le modifier et ajouter un footer
```bash
cd css
nano style.css

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

4. ici je crée un branche et j'envoie tout vers le site avec un commentaire pour dire ce que j'ai fait
```bash
git add .
git branch csssamuel
git checkout csssamuel
git add .
git commit -m "modifcsssamuel"
git push -u origin csssamuel
```

5. Je me mets dans master pour ensuite fusionner et envoyer vers github
```bash
git checkout master
git merge csssamuel
git push -u origin master
```

6. je crée une branche html et rajoute une page
```bash
git branch htmlsamuel
git checkout htmlsamuel
git add .
```

7. J'ai ensuite rempli les pages html avec 3 sujets différents : page1, page2, page3 :
```bash
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Evaluation GIT 17/04/2025</title>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="../css/style.css">
    <link rel="stylesheet" href="../css/mobile.css">
</head>
<body>
    

    <header>
        <a href="../index.html"><img src="../images/image1.jpg"></a>
    </header>

    <nav>
        <a href="../pages/page1.html">Page1</a>
        <a href="../pages/page2.html">Page2</a>
        <a href="../pages/page3.html">Page3</a>
    </nav>

    <main>
        <h1>Princesse Mononoke</h1>
        <br>
        <p>Ashitaka, un jeune guerrier japonais, affronte un sanglier géant et furieux qui attaque son village. Il tue la bête, mais se retrouve atteint par un mal mystérieux. Sur le conseil des sages, il part vers l'Ouest, à la recherche de ce qui a transformé l'animal en démon. Au cours de son périple, il rencontre San, une jeune fille qui vit avec les loups. Ashitaka apprend que les humains sont à l'origine de tous ces maux, car ils détruisent la forêt, qu'ils exploitent pour alimenter leurs forges.</p>
</main>

    <aside>
        <img src="../images/mononoke.jpg" alt="mononoke ghibli">
    </aside>

    <footer>
        &copy; copyrigth
    </footer>

</body>
</html>
```
8. J'ai rajouté du css pour que ça soit plus jolie visuellement :
```bash
h1{
    text-align: center;
    font-size: 40px;
    margin-bottom: 20px;
    color: darkgreen;
    text-shadow: 1px 1px 2px;
  }

p{
    background-color: #fff;
    border-left: 6px solid green;
    padding: 25px;
    max-width: 700px;
    margin: auto;
    box-shadow: 0 4px 8px;
    line-height: 1.5;
    font-size: 18px;
    color: grey;
  }
```

9. Puis j'ai renvoyé vers master pour ensuite l'importer dans github : 
```bash
git checkout master
git add .
git commit -m "modifhtmletcsssamuel2"
git git merge htmlsamuel
git push -u origin master
```

### Pour récupérer les commandes
```bash
history
```