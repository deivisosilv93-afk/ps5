<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>PS5 Game Selector</title>

<link href="https://fonts.googleapis.com/css2?family=Rajdhani:wght@500;700&display=swap" rel="stylesheet"/>

<style>
*{
  box-sizing:border-box;
  margin:0;
  padding:0;
  cursor:none !important;
}

html,body{
  height:100%;
  overflow:hidden;
  font-family:'Rajdhani',sans-serif;
}

/* CURSOR */
#cursor{
  position:fixed;
  width:10px;
  height:10px;
  background:#00d4ff;
  border-radius:50%;
  pointer-events:none;
  transform:translate(-50%,-50%);
  z-index:9999;
}

#cursor-ring{
  position:fixed;
  width:28px;
  height:28px;
  border:1.5px solid rgba(0,212,255,.55);
  border-radius:50%;
  pointer-events:none;
  transform:translate(-50%,-50%);
  z-index:9998;
}

/* FUNDO */
.bg-fixed{
  position:fixed;inset:0;z-index:-3;
  background-image:url('https://tse1.mm.bing.net/th/id/OIP.u5utXeHNafAKv_teT8aEEgHaEK');
  background-size:cover;
  background-position:center;
}

.bg-overlay{
  position:fixed;inset:0;
  background:rgba(0,0,0,0.35);
  z-index:-2;
}

.bg-shine{
  position:fixed;inset:0;
  z-index:-1;
  background:
    radial-gradient(circle at 20% 50%, rgba(0,212,255,.18), transparent 60%),
    radial-gradient(circle at 80% 30%, rgba(120,80,255,.15), transparent 60%);
}

/* TOPO */
.topbar{
  position:fixed;
  top:0;
  width:100%;
  display:flex;
  justify-content:space-between;
  padding:10px 20px;
  background:rgba(0,0,0,.55);
}

.menu span{color:#fff;margin-right:20px;opacity:.5;}
.menu .active{opacity:1;color:#00d4ff;}

/* 🔥 NOVO - ÍCONES */
.top-right{
  display:flex;
  align-items:center;
  gap:18px;
  color:white;
}

.icon{
  width:22px;
  height:22px;
  opacity:0.7;
  transition:0.25s;
}

.icon:hover{
  opacity:1;
  transform:scale(1.15);
  filter:drop-shadow(0 0 6px #00d4ff);
}

/* CONTEÚDO */
.scene{
  position:absolute;
  top:60px;
  left:20px;
  right:0;
  bottom:0;
  display:flex;
  flex-direction:column;
  justify-content:center;
}

.game-title{font-size:32px;color:#fff;}
.game-sub{font-size:14px;color:#00d4ff;margin-bottom:20px;}

.grid{
  display:flex;
  gap:10px;
  transition:.4s;
}

.card{
  width:80px;
  height:80px;
  border-radius:10px;
  overflow:hidden;
  filter:brightness(.5);
  transition:.4s;
}

.card img{
  width:100%;
  height:100%;
  object-fit:cover;
}

.card.selected{
  width:160px;
  height:160px;
  filter:brightness(1.1);
  box-shadow:0 0 25px rgba(0,212,255,0.9);
}
</style>
</head>

<body>

<div id="cursor"></div>
<div id="cursor-ring"></div>

<div class="bg-fixed"></div>
<div class="bg-overlay"></div>
<div class="bg-shine"></div>

<div class="topbar">
  <div class="menu">
    <span class="active">Games</span>
    <span>Media</span>
  </div>

  <!-- 🔥 ÍCONES ADICIONADOS -->
  <div class="top-right">

    <!-- LUPA -->
    <svg class="icon" viewBox="0 0 24 24">
      <circle cx="11" cy="11" r="7" stroke="white" stroke-width="2" fill="none"/>
      <line x1="16.5" y1="16.5" x2="21" y2="21" stroke="white" stroke-width="2"/>
    </svg>

    <!-- CONFIG -->
    <svg class="icon" viewBox="0 0 24 24">
      <circle cx="12" cy="12" r="3" stroke="white" stroke-width="2" fill="none"/>
      <path d="M19 12a7 7 0 0 0-.1-1l2-1.5-2-3.5-2.3 1a7 7 0 0 0-1.7-1l-.3-2.5h-4l-.3 2.5a7 7 0 0 0-1.7 1l-2.3-1-2 3.5 2 1.5a7 7 0 0 0 0 2l-2 1.5 2 3.5 2.3-1a7 7 0 0 0 1.7 1l.3 2.5h4l.3-2.5a7 7 0 0 0 1.7-1l2.3 1 2-3.5-2-1.5c.1-.3.1-.7.1-1z"
        stroke="white" stroke-width="1.5" fill="none"/>
    </svg>

    <!-- PERFIL -->
    <svg class="icon" viewBox="0 0 24 24">
      <circle cx="12" cy="8" r="4" stroke="white" stroke-width="2" fill="none"/>
      <path d="M4 20c0-4 4-6 8-6s8 2 8 6" stroke="white" stroke-width="2" fill="none"/>
    </svg>

    <span id="clock"></span>
  </div>
</div>

<div class="scene">
  <div class="game-title" id="gtitle"></div>
  <div class="game-sub" id="gsub"></div>
  <div class="grid" id="grid"></div>
</div>

<script>
const games = [
{ name:"Demon's Souls", genre:"RPG de Ação", img:"https://th.bing.com/th/id/R.a9e89a6fc9245db5a76c4c6581e2342c?rik=9y7yPa3TcXIXLw&pid=ImgRaw&r=0" },
{ name:"Returnal", genre:"Roguelike / Ação", img:"https://upload.wikimedia.org/wikipedia/pt/5/51/Returnal_capa.png" },
{ name:"Horizon Forbidden West", genre:"Mundo Aberto", img:"https://mods.store.gx.me/mods/a94eb028-50a3-4bad-85cd-4cb83e106a9c/ebdd972a-fc6a-4643-87f2-041edf018a14/fe854c70-a5fb-4d6a-8f71-0bc2e836338f/contents/icon_512.png" },
{ name:"God of War Ragnarök", genre:"Ação / Aventura", img:"https://tse2.mm.bing.net/th/id/OIP.RTHPTOjbijTpXH9RWUrOhwHaHa" },
{ name:"Spider-Man 2", genre:"Ação", img:"https://image.api.playstation.com/vulcan/ap/rnd/202306/1219/1c7b75d8ed9271516546560d219ad0b22ee0a263b4537bd8.png" },
{ name:"Elden Ring", genre:"RPG", img:"https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/8a156873-a830-43b1-9b31-3becb2f788fb/dfidn59-0aa07c30-b68a-4188-8a24-3a5276d81ead.png/v1/fill/w_512,h_512,strp/elden_ring_logo_by_firzecrescent_dfidn59-fullview.png?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOjdlMGQxODg5ODIyNjQzNzNhNWYwZDQxNWVhMGQyNmUwIiwiaXNzIjoidXJuOmFwcDo3ZTBkMTg4OTgyMjY0MzczYTVmMGQ0MTVlYTBkMjZlMCIsIm9iaiI6W1t7ImhlaWdodCI6Ijw9NTEyIiwicGF0aCI6IlwvZlwvOGExNTY4NzMtYTgzMC00M2IxLTliMzEtM2JlY2IyZjc4OGZiXC9kZmlkbjU5LTBhYTA3YzMwLWI2OGEtNDE4OC04YTI0LTNhNTI3NmQ4MWVhZC5wbmciLCJ3aWR0aCI6Ijw9NTEyIn1dXSwiYXVkIjpbInVybjpzZXJ2aWNlOmltYWdlLm9wZXJhdGlvbnMiXX0.7oRtpdc_X2l8zA6hqLN9hb1xeSkZzBXz5PR_DX0b0vU" },
{ name:"GTA V", genre:"Mundo Aberto", img:"https://upload.wikimedia.org/wikipedia/en/a/a5/Grand_Theft_Auto_V.png" },
{ name:"Cyberpunk 2077", genre:"RPG", img:"https://upload.wikimedia.org/wikipedia/en/9/9f/Cyberpunk_2077_box_art.jpg" }
];

const grid = document.getElementById("grid");
let sel = 0, cards = [];

games.forEach((g,i)=>{
  const c = document.createElement("div");
  c.className="card";

  const img=document.createElement("img");
  img.src=g.img;

  c.appendChild(img);
  c.onclick=()=>{sel=i;update();};

  grid.appendChild(c);
  cards.push(c);
});

function update(){
  cards.forEach((c,i)=>c.classList.toggle("selected",i===sel));
  grid.style.transform=`translateX(-${sel*90}px)`;
  gtitle.textContent=games[sel].name;
  gsub.textContent=games[sel].genre;
}
update();

document.addEventListener("keydown", e=>{
  if(e.repeat) return;

  if(e.key==="ArrowRight"){
    sel=(sel+1)%games.length;
    update();
  }

  if(e.key==="ArrowLeft"){
    sel=(sel-1+games.length)%games.length;
    update();
  }

  if((e.key===" " || e.code==="Space") && games[sel].name==="GTA V"){
    e.preventDefault();
    window.open("https://sites.google.com/view/rockstarspms/gtav","_blank");
  }
});

const cursor = document.getElementById("cursor");
const cursorRing = document.getElementById("cursor-ring");

let mx=0,my=0,rx=0,ry=0;

document.addEventListener("mousemove",e=>{
  mx=e.clientX;
  my=e.clientY;
  cursor.style.left=mx+"px";
  cursor.style.top=my+"px";
});

function loop(){
  rx+=(mx-rx)*0.1;
  ry+=(my-ry)*0.1;

  cursorRing.style.left=rx+"px";
  cursorRing.style.top=ry+"px";

  requestAnimationFrame(loop);
}
loop();

setInterval(()=>{
  const d=new Date();
  clock.textContent=
    d.getHours().toString().padStart(2,"0")+":"+
    d.getMinutes().toString().padStart(2,"0");
},1000);
</script>

</body>
</html>
