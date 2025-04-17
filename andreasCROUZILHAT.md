# registre exam de git


## andreas



```bash
#apres avoir cree mon dossier je fais un 
git init

```

2.
```bash
git clone https://github.com/Chizzy-mio/evalmasson.git
```

3.
```bash
cd evalmasson
```

4.
```bash
git pull origin master 
#je viens de recupérer l'html ainsi que tous les dossiers
```
5.
```bash
#je me connecte a mon github
git config user.name "midasLas"
git config user.email "crouzilhatandreas"
```

6.
```bash
#je cree une branch
git branch cssandreas
git checkout cssandreas
```
7.
```bash
#j'envoie mon css
git add .
git commit -m "cssandreas"
git push -u origin cssandreas
```

# ccs:
```bash
* {
    margin: 0;
    padding: 0;
  
}
body{
    display: flex;
    flex-wrap: wrap;
}
header{
    background-color:#545657;
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
    color: rgb(246, 248, 249);
    text-align: center;

}
aside{
    background-color: rgb(231, 231, 224);
    width: 25%;
}
aside img{
    display: block;
    width: 100%;
}
```

