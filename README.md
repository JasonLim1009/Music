# Music

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>music</title>
    <link rel="stylesheet" href="music.css">
</head>
<body>
<div class="container">
    <div class="navbar">
        <img src="media/music%20logo.png" class="logo" alt="">
        <ul>
            <li><a href="#">HOME</a></li>
            <li><a href="#">ABOUT</a></li>
            <li><a href="#">SPECIFICATIONS</a></li>
            <li><a href="#">PRODUCTS</a></li>
            <li><a href="#">CONNECT</a></li>
        </ul>
    </div>
    <div class="content">
        <div class="left-col">
            <h1>THE<br>REAL<br>SOUND</h1>
        </div>
        <div class="right-col">
            <p>Click Here To Listen</p>
            <img src="media/play.png" id="icon" alt="">
        </div>
    </div>
</div>

<audio id="mySong">
    <source src="media/music.mp3" type="audio/mp3">
</audio>

<script>
    let mySong = document.getElementById('mySong');
    let icon = document.getElementById('icon');

    icon.onclick = function (){
        if(mySong.paused){
            mySong.play();
            icon.src = 'media/play.png';
        }else {
            mySong.pause();
            icon.src = 'media/play.png';
        }
    }
</script>

</body>
</html>
