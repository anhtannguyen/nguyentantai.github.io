<html lang="en">
    <head>
        <meta charset="utf-8">
        <meta http-equiv="X-UA-Compatible" content="IE-edge">
        <meta name="Vieport" content="width=device-width, initial-scale=1.0">
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.1/css/all.min.css">
        <title>THE3D</title>
    </head>
    <style>
        *{
            padding:0;
            margin:0;
            box-sizing: border-box;
        }
        body{
            height:100vh;
            display:flex;
            justify-content:center;
            align-items:center;
            background-color: rgba(0,80,89,1);
            perspective: 3000px;
        }
        :root{
            --width:460px;
            --height:640px;
            --de:80px;
        }
        .card{
            position:relative;
            width:var(--width);
            height:var(--height);
            border: 0.5px solid white;
            transform-style:preserve-3d;
            transition:0.9s;
        }
        .side{
            position:absolute;
            left:-1;
            top:-1;
            border:inherit;
        }
        .left{
            width:var(--de);
            height:var(--height);
            background-color: rgba(141,140,141,1);
            transform-origin:left;
            transform:translateX(var(--width)) rotateY(90deg);
        }
        .bottom{
            width:var(--width);
            height:var(--de);
            background-color:rgba(141,140,141,1);
            transform-origin:top;
            transform:translateY(var(--height)) rotateX(-90deg);
            display:flex;
            justify-content: space-around;
            align-items: center;
        }
        .fa-brands{
            cursor: pointer;
            width:60px;
            height:60px;
            border:inherit;
            display:flex;
            justify-content:center;
            align-items:center;
            color:rgb(2,2,2,1);
            transition:0.4s;
        }
        .fa-brands:hover{
            background-color:white;
            color:black;
            transition: 1s;
        }
        .fa-solid{
            cursor: pointer;
            width:60px;
            height:60px;
            border:inherit;
            display:flex;
            justify-content:center;
            align-items:center;
            color:rgb(2,2,2,1);
            transition:0.4s;
        }
        .fa-solid:hover{
            background-color:white;
            color:black;
            transition: 1s;
        }
        .main{
            width: var(--width);
            height: var(--height);
        }
        .main img{
            width:100%;
            height:100%;
        }
        .card:hover{
            transform:rotateX(60deg) rotateY(-20deg);
        }
        h3{
            writing-mode:vertical-rl;
            align-content: center;
            font-size: 3em;
        }
        a{
            width:60px;
            height:60px;
            box-sizing: border-box;
            border:0.5px solid white;
            text-decoration: none;
        }
    
    </style>
    <body>
        <div class="card">
            <div class="side left">
                <h3>NGUYỄN TẤN TÀI</h3>
            </div>
            <div class="side bottom">
                <a href="https://www.facebook.com/tainguyen.tai.9279"><i class="fa-brands fa-facebook"></i></a>
                <i class="fa-brands fa-instagram-square"></i>
                <i class="fa-brands fa-tiktok"></i>
                <i class="fa-solid fa-shield-cat"></i>
            </div>
            <div class="side main">
                <img src="https://i.pinimg.com/236x/39/c0/c1/39c0c1578166c69e8c3e4685dce30aad.jpg">
            </div>
        </div>
    </body>
</html>
