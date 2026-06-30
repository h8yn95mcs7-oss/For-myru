<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>for myru.</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500&display=swap');

*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:Poppins;
}

body{
  background:#0b0b0f;
  color:#fff;
  overflow-x:hidden;
}

/* soft background glow */
.glow{
  position:fixed;
  width:400px;
  height:400px;
  background:#ffffff10;
  filter:blur(120px);
  border-radius:50%;
  top:20%;
  left:30%;
  animation:float 6s infinite ease-in-out;
}

@keyframes float{
  0%,100%{transform:translateY(0px);}
  50%{transform:translateY(-30px);}
}

/* landing */
.center{
  height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  flex-direction:column;
  text-align:center;
}

.title{
  font-size:28px;
  letter-spacing:1px;
}

.subtitle{
  opacity:0.6;
  margin-top:5px;
  font-size:14px;
}

button{
  margin-top:20px;
  padding:10px 25px;
  border:none;
  border-radius:20px;
  background:#ffffff15;
  color:white;
  backdrop-filter:blur(10px);
  cursor:pointer;
}

/* glass card */
.card{
  margin:80px auto;
  width:90%;
  max-width:500px;
  padding:20px;
  background:#ffffff10;
  border-radius:20px;
  backdrop-filter:blur(15px);
  text-align:center;
}

/* images */
img{
  width:100%;
  border-radius:15px;
  margin-top:10px;
}

/* video */
video{
  width:100%;
  border-radius:15px;
  margin-top:10px;
}

/* hidden hearts */
.heart{
  position:absolute;
  color:white;
  opacity:0.08;
  font-size:20px;
  animation:fall 10s linear infinite;
}

@keyframes fall{
  from{transform:translateY(-10vh);}
  to{transform:translateY(110vh);}
}
</style>
</head>

<body>

<div class="glow"></div>

<!-- floating hearts -->
<div class="heart" style="left:10%">🤍</div>
<div class="heart" style="left:30%">🤍</div>
<div class="heart" style="left:50%">🤍</div>
<div class="heart" style="left:70%">🤍</div>

<!-- landing -->
<div class="center">
  <div class="title">for myru.</div>
  <div class="subtitle">from abhay.</div>
  <button onclick="document.getElementById('main').scrollIntoView({behavior:'smooth'})">
    open
  </button>
</div>

<!-- content -->
<div id="main">

<div class="card">
  <h3>myru</h3>
  <p style="opacity:0.7;margin-top:10px;">
    soryyy na myruuuuuu babyyy yrr mujhe pta h apko nhi pasand hattt pee glti se boldia thaaaa ajkee bad pakka nhi bolungaaa is bari maf krdooo bassss plizzzzzzzzz naraz mt rho babyyy🥺
  </p>
  <p style="margin-top:10px;">— abhay</p>
</div>

<div class="card">
  <h3>photos</h3>
  <img src="photo1.jpg">
  <img src="photo2.jpg">
  <img src="photo3.jpg">
  <img src="photo4.jpg">
  <img src="photo5.jpg">
  <img src="photo6.jpg">
</div>

<div class="card">
  <h3>video</h3>
  <video controls>
    <source src="myru.mp4" type="video/mp4">
  </video>
</div>

</div>

</body>
</html>