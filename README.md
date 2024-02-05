<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        *{
            margin: 0;
            padding: 0;
        }
       .container{
        border: 4px solid black;
        background-color: beige;
        height: 100vh;
        width: 100vw;
        box-sizing: border-box;
       }
       #box1{
        border: 2px solid black;
        background-color: cyan;
        width: 200px;
        height: 75px;
        margin: 5px;
        border-radius: 10px;
        position: relative;
        /* animation-name: rightmovement; */
        /* animation-duration: 6s;
        animation-delay: none;
        animation-iteration-count: infinite;
        animation-direction: alternate; */
        /* animation-timing-function: cubic-bezier(0,0.07,0.01,0.02) ; */
        /* animation-timing-function: linear;
        animation-fill-mode: both;
        animation-play-state: running; */
        animation: rightmovement 7s ease-in-out 0s infinite alternate forwards;
       }
       @keyframes rightmovement{
        from{
            top:0;
            left:0;
        }
        to{
            top: 0;
            left: 1015px;
        }
       }
       #box2{
        border: 2px solid black;
        background-color: cyan;
        width: 200px;
        height: 75px;
        margin: 5px;
        border-radius: 10px;
        position: relative;
        animation: leftmovement 7s ease-in-out 0s infinite alternate forwards;
       }
       @keyframes leftmovement {
        from{
        top: 335px;
        left:1015px;
        }
        to{
         top:335px;
         left:0;
        }
       }
       #box3{
        border: 2px solid black;
        background-color: cyan;
        width: 20px;
        height: 20px;
        margin: 5px;
        border-radius: 200px;
        position: relative;
        animation: circlemovement 7s linear 0s infinite alternate forwards;
       }
       @keyframes circlemovement{
        0%{
            top:50vh;
            left:504px
        }
        25%{
            top:22vh;
            left: 0;
        }
        50%{
            top:22vh;
            left:1015px;
        }
        75%{
            top: 75vh;
            left: 0;
        }
        100%{
            top: 75vh;
            left: 1015px;
        }
       }
    </style>
</head>
<body>
    <div class="container">
        <div id="box1"></div>
        <div id="box3"></div>
        <div id="box2"></div>
    </div>
</body>
</html>
