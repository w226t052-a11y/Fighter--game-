<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<title>ピクセル戦闘機ゲーム</title>
<style>
body{
margin:0;
background:black;
overflow:hidden;
color:white;
text-align:center;
font-family:sans-serif;
}
canvas{
background:#111;
display:block;
margin:auto;
border:3px solid white;
}
</style>
</head>
<body>

<h2>ピクセル戦闘機ゲーム</h2>
<p>← → 移動 / SPACE 攻撃</p >
<p>スコア: <span id="score">0</span></p >

<canvas id="game" width="400" height="600"></canvas>

<script>
const canvas=document.getElementById("game");
const ctx=canvas.getContext("2d");

let score=0;
let gameOver=false;

const player={
x:180,
y:520,
w:40,
h:40,
speed:5
};

const bullets=[];
const enemies=[];
const keys={};

document.addEventListener("keydown",e=>{
keys[e.key]=true;

if(e.code==="Space"){
bullets.push({
x:player.x+18,
y:player.y,
w:4,
h:10
});
}
});

document.addEventListener("keyup",e=>{
keys[e.key]=false;
});

function spawnEnemy(){
enemies.push({
x:Math.random()*360,
y:-40,
w:40,
h:40,
speed:2+Math.random()*2
});
}

function update(){

if(keys["ArrowLeft"]&&player.x>0){
player.x-=player.speed;
}

if(keys["ArrowRight"]&&player.x<360){
player.x+=player.speed;
}

bullets.forEach(b=>{
b.y-=8;
});

enemies.forEach(e=>{
e.y+=e.speed;

if(e.y>600){
gameOver=true;
}
});

bullets.forEach((b,bi)=>{
enemies.forEach((e,ei)=>{

if(
b.x<e.x+e.w&&
b.x+b.w>e.x&&
b.y<e.y+e.h&&
b.y+b.h>e.y
){
bullets.splice(bi,1);
enemies.splice(ei,1);

score+=10;
document.getElementById("score").textContent=score;
}

});
});

enemies.forEach(e=>{

if(
player.x<e.x+e.w&&
player.x+player.w>e.x&&
player.y<e.y+e.h&&
player.y+player.h>e.y
){
gameOver=true;
}

});
}

function draw(){

ctx.clearRect(0,0,400,600);

ctx.fillStyle="cyan";
ctx.fillRect(player.x,player.y,player.w,player.h);

ctx.fillStyle="yellow";
bullets.forEach(b=>{
ctx.fillRect(b.x,b.y,b.w,b.h);
});

ctx.fillStyle="red";
enemies.forEach(e=>{
ctx.fillRect(e.x,e.y,e.w,e.h);
});

if(gameOver){
ctx.fillStyle="white";
ctx.font="40px sans-serif";
ctx.fillText("GAME OVER",70,300);
}
}

function loop(){

if(!gameOver){
update();
draw();
requestAnimationFrame(loop);
}else{
draw();
}

}

setInterval(spawnEnemy,1000);

loop();
</script>

</body>
</html>
