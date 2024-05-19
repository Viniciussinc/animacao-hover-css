# animacao-hover-css
Este é um projeto sobre animações em css, com o intuito de praticarmos o que apreendemos na aula de desenvolvimento web 1.
#Html:
# Meu Projeto

Aqui está na integra o código HTML:

###  HTML

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="estilo.css">
    <title>Document</title>
</head>
<body>
    <div class="card">
        <div class="img-box">
            <img src="images/f69f644acef0142bb0615587664b570e.jpg">
        </div>
        <div class="content">
            <h2>Sukuna</h2>
            <p>
                Sukuna é um feiticeiro antigo que nasceu no período Heian, que ocorreu há mais de 1000 anos atrás no Japão.
            </p>
            <a href="https://jujutsu-kaisen.fandom.com/wiki/Sukuna" class="read-more">
                Leia mais
            </a>
        </div>
    </div>
</body>
</html>
```
### Css
Css:
```@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

body {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background: linear-gradient(90deg, #c50805, #dd0202, #cf0101);
}

.card {
    display: flex;
    justify-content: center;
    width: 350px;
    height: 300px;
    position: relative;
    background-color: #ffa4a4;
    border-radius: 20px;
    box-shadow: 0px 35px 80px rgba(0, 0, 0, 0.15);
    transition: 0.5s;
}

.card:hover {
    height: 400px;
}

.card .img-box {
    position: absolute;
    width: 250px;
    height: auto;
    top: 0px;
    transition: 0.5s;
}

.card:hover .img-box {
    top: -100px;
    scale: 0.75;
}

.card .img-box img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.card .content {
    display: flex;
    flex-direction: column;
    gap: 18px;
    position: absolute;
    top: 250px;
    width: 100%;
    padding: 0px 30px;
    text-align: center;
    height: 30px;
    overflow: hidden;
    transition: 0.5s;
}

.card:hover .content {
    top: 130px;
    height: 250px;
}

.card .read-more {
   background: linear-gradient(90deg, #540303, #270200);
   padding: 12px;
   color: #fff;
   text-decoration: none;
   border-radius: 8px;
}
```
![Funcionamento do Projeto](https://github.com/Viniciussinc/animacao-hover-css/blob/main/sukuna.gif)



