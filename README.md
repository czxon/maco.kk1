<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>maco.kk — สั่งเครื่องดื่มและอาหารออนไลน์</title>
<link href="https://fonts.googleapis.com/css2?family=Anuphan:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<style>
:root{--bg:#f6f5f2;--card:#fff;--ink:#1f1e1a;--muted:#5d5b55;--line:#dad8d1;--wood:#a67c52;--wood-d:#7a5632;--matcha:#6f8145;--dark:#1f1e1a;--on-dark:#f6f5f2;--soft:#ebe9e3;
box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#171613;--card:#242320;--ink:#f3f1ec;--muted:#b0ada4;--line:#3a3833;--soft:#2c2a26;--wood:#c9a273;--wood-d:#d9b78c;--dark:#0f0e0c}}
:root[data-theme="dark"]{--bg:#171613;--card:#242320;--ink:#f3f1ec;--muted:#b0ada4;--line:#3a3833;--soft:#2c2a26;--wood:#c9a273;--wood-d:#d9b78c;--dark:#0f0e0c}
*,*::before,*::after{box-sizing:border-box}
html{scroll-behavior:smooth;height:100%}
body{margin:0;background:var(--bg);color:var(--ink);font:400 16px/1.65 'Anuphan','Noto Sans Thai',system-ui,sans-serif}
button{font:inherit;color:inherit;cursor:pointer}
:focus-visible{outline:3px solid var(--wood);outline-offset:2px}
.wrap{max-width:1080px;margin:0 auto;padding:0 20px}
.nav{position:sticky;top:env(safe-area-inset-top,0px);z-index:5;background:var(--bg);border-bottom:1px solid var(--line)}
.nav .wrap{display:flex;align-items:center;justify-content:space-between;height:60px;gap:12px}
.brand{font-weight:700;font-size:22px;letter-spacing:-.04em;text-decoration:none;color:var(--ink)}
.links{display:flex;gap:20px;font-size:14px;font-weight:500}
.links a{color:var(--muted);text-decoration:none}.links a:hover{color:var(--ink)}
.cartbtn{background:var(--ink);color:var(--bg);border:0;border-radius:99px;padding:8px 18px;font-weight:600;display:flex;gap:8px;align-items:center}
.cartbtn b{background:var(--wood);color:#1f1e1a;border-radius:99px;min-width:22px;height:22px;display:grid;place-items:center;font-size:13px;padding:0 6px}
@media(max-width:640px){.links{display:none}}

.hero{background:var(--dark);color:var(--on-dark);padding:64px 0 0;overflow:hidden}
.hero h1{margin:0;font-size:clamp(72px,18vw,200px);line-height:.9;letter-spacing:-.06em;font-weight:700;color:#fff}
.hero h1 i{color:#d9b78c;font-style:normal}
.hero .row{display:grid;grid-template-columns:1.3fr 1fr;gap:32px;margin-top:30px;align-items:end}
.hero p.pr{font-size:clamp(20px,3vw,30px);line-height:1.4;font-weight:500;margin:0;color:#fff}
.hero p.sm{margin:0 0 16px;color:#d5d2c9}
.btn{border:0;border-radius:99px;padding:12px 26px;font-weight:600;background:#d9b78c;color:#1f1e1a;text-decoration:none;display:inline-block}
.btn:hover{background:#e6c9a4}
.btn.dk{background:var(--ink);color:var(--bg)}
.btn.block{width:100%;text-align:center}
.strip{margin-top:48px;background:#3a3832;height:14px;background:linear-gradient(90deg,#a67c52,#c9a273 45%,#a67c52 70%,#8a6640)}
@media(max-width:700px){.hero .row{grid-template-columns:1fr}}

.perks{display:grid;grid-template-columns:repeat(4,1fr);gap:0;border-bottom:1px solid var(--line);background:var(--card)}
.perks div{padding:18px 16px;border-right:1px solid var(--line);font-size:14px;color:var(--muted)}
.perks b{display:block;color:var(--ink);font-size:15px}
.perks div:last-child{border-right:0}
@media(max-width:700px){.perks{grid-template-columns:1fr 1fr}}

section{padding:72px 0}
h2{font-size:clamp(28px,4.5vw,42px);letter-spacing:-.03em;line-height:1.2;margin:0 0 8px;font-weight:600}
.lead{color:var(--muted);margin:0 0 28px;max-width:56ch}
.tabs{display:flex;gap:8px;flex-wrap:wrap;margin-bottom:26px}
.tabs button{border:1.5px solid var(--line);background:var(--card);border-radius:99px;padding:6px 18px;font-weight:500}
.tabs button[aria-pressed=true]{background:var(--ink);color:var(--bg);border-color:var(--ink)}
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(230px,1fr));gap:18px}
.item{background:var(--card);border:1px solid var(--line);border-radius:16px;overflow:hidden;display:flex;flex-direction:column;text-align:left;padding:0;transition:transform .2s,box-shadow .2s}
.item:hover{transform:translateY(-3px);box-shadow:0 10px 24px rgba(0,0,0,.14)}
.pic{height:130px;display:grid;place-items:center;font-size:58px;position:relative}
.pic em{position:absolute;top:10px;left:10px;font-style:normal;font-size:12px;font-weight:600;background:#1f1e1a;color:#fff;border-radius:99px;padding:1px 10px}
.item .b{padding:14px 16px 16px;display:flex;flex-direction:column;gap:2px;flex:1}
.item h3{margin:0;font-size:17px;line-height:1.3}
.item small{color:var(--muted);line-height:1.4}
.item .pp{margin-top:auto;padding-top:10px;display:flex;justify-content:space-between;align-items:center;font-weight:600}
.item .pp span:last-child{background:var(--ink);color:var(--bg);width:32px;height:32px;border-radius:50%;display:grid;place-items:center;font-size:20px;line-height:1}

.about{background:var(--soft)}
.cols{display:grid;grid-template-columns:1fr 1fr;gap:40px}
.cols h3{margin:0 0 6px;font-size:15px;color:var(--wood-d)}
.cols p{margin:0 0 20px}
.steps{list-style:none;margin:32px 0 0;padding:0;display:grid;grid-template-columns:repeat(6,1fr);gap:12px}
.steps li{background:var(--card);border:1px solid var(--line);border-radius:12px;padding:12px;font-size:14px;font-weight:500;line-height:1.4}
.steps li b{display:block;color:var(--wood-d);font-size:13px}
@media(max-width:800px){.cols{grid-template-columns:1fr}.steps{grid-template-columns:1fr 1fr}}

.swatch{display:flex;gap:10px;margin-top:6px}.swatch i{width:36px;height:36px;border-radius:50%;border:1px solid var(--line)}
footer{background:var(--dark);color:#e8e5dd;padding:56px 0 32px}
footer .big{font-size:clamp(44px,11vw,110px);font-weight:700;letter-spacing:-.06em;line-height:1;margin:0 0 20px;color:#fff}
footer .r{display:flex;justify-content:space-between;flex-wrap:wrap;gap:16px;align-items:end}
footer small{display:block;margin-top:28px;color:#a9a69c}

/* dialogs & drawer */
dialog{border:0;border-radius:20px;padding:0;background:var(--card);color:var(--ink);width:min(460px,calc(100% - 24px));max-height:calc(100% - 24px);box-shadow:0 24px 70px rgba(0,0,0,.45)}
dialog::backdrop{background:rgba(20,18,14,.6);backdrop-filter:blur(3px)}
dialog[open]{animation:pop .25s cubic-bezier(.2,.8,.2,1)}
@keyframes pop{from{opacity:0;transform:translateY(16px) scale(.97)}}
.dh{height:120px;display:grid;place-items:center;font-size:64px;position:relative}
.x{position:absolute;top:10px;right:10px;width:36px;height:36px;border-radius:50%;border:0;background:rgba(255,255,255,.9);color:#1f1e1a;font-size:20px;line-height:1}
.dbody{padding:18px 22px 22px}
.dbody h3{margin:0;font-size:22px;line-height:1.3}
.dbody p{margin:2px 0 14px;color:var(--muted)}
fieldset{border:0;padding:0;margin:0 0 14px}
legend{font-weight:600;font-size:14px;margin-bottom:6px;padding:0}
.opts{display:flex;flex-wrap:wrap;gap:8px}
.opts label{position:relative}
.opts input{position:absolute;opacity:0;inset:0}
.opts span{display:block;border:1.5px solid var(--line);border-radius:99px;padding:4px 14px;font-size:14px;background:var(--bg)}
.opts input:checked+span{background:var(--ink);color:var(--bg);border-color:var(--ink)}
.opts input:focus-visible+span{outline:3px solid var(--wood);outline-offset:2px}
.qty{display:inline-flex;align-items:center;border:1.5px solid var(--line);border-radius:99px}
.qty button{border:0;background:none;width:38px;height:38px;font-size:20px;border-radius:50%}
.qty span{min-width:26px;text-align:center;font-weight:600}
.foot{display:flex;gap:14px;align-items:center;margin-top:8px}
.foot .btn{flex:1;background:var(--ink);color:var(--bg)}
input.t,textarea.t,select.t{width:100%;border:1.5px solid var(--line);border-radius:12px;padding:9px 12px;background:var(--bg);color:var(--ink);font:inherit;margin-bottom:12px}
label.f{display:block;font-size:14px;font-weight:600;margin-bottom:4px}

.drawer{position:fixed;inset:0;z-index:20;pointer-events:none}
.drawer .ov{position:absolute;inset:0;background:rgba(20,18,14,.55);opacity:0;transition:opacity .25s}
.drawer .pn{position:absolute;top:0;right:0;bottom:0;width:min(420px,100%);background:var(--card);transform:translateX(100%);transition:transform .3s cubic-bezier(.2,.8,.2,1);display:flex;flex-direction:column;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
.drawer.on{pointer-events:auto}.drawer.on .ov{opacity:1}.drawer.on .pn{transform:none}
.ph{display:flex;justify-content:space-between;align-items:center;padding:16px 20px;border-bottom:1px solid var(--line)}
.ph h3{margin:0;font-size:20px}
.ph .x{position:static;background:var(--soft);color:var(--ink)}
.lines{flex:1;overflow:auto;padding:8px 20px}
.ln{display:grid;grid-template-columns:48px 1fr auto;gap:12px;padding:12px 0;border-bottom:1px solid var(--line);align-items:center}
.ln .ic{width:48px;height:48px;border-radius:12px;display:grid;place-items:center;font-size:26px}
.ln b{display:block;line-height:1.3}.ln small{color:var(--muted);display:block;line-height:1.3}
.ln .qty{transform:scale(.85);transform-origin:right;margin-top:4px}
.empty{text-align:center;color:var(--muted);padding:60px 10px}
.sum{padding:16px 20px;border-top:1px solid var(--line);background:var(--soft)}
.sum div{display:flex;justify-content:space-between;font-size:15px}
.sum .tot{font-size:20px;font-weight:700;margin:6px 0 12px}
.disc{color:var(--matcha);font-weight:600}
[data-theme="dark"] .disc{color:#a9c27a}
.toast{position:fixed;left:50%;bottom:calc(20px + env(safe-area-inset-bottom,0px));transform:translate(-50%,120px);background:var(--ink);color:var(--bg);padding:10px 20px;border-radius:99px;font-weight:500;z-index:50;transition:transform .3s;box-shadow:0 8px 24px rgba(0,0,0,.3)}
.toast.on{transform:translate(-50%,0)}
.ok{text-align:center;padding:30px 24px}
.ok .ck{width:72px;height:72px;border-radius:50%;background:var(--matcha);color:#fff;display:grid;place-items:center;font-size:38px;margin:0 auto 12px}
.ok .no{font-size:34px;font-weight:700;letter-spacing:-.03em;margin:4px 0}
.ok ul{list-style:none;padding:12px 14px;margin:14px 0;background:var(--soft);border-radius:12px;text-align:left;font-size:14px}
@media(prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important}}
</style>
</head>
<body>
<header class="nav"><div class="wrap">
<a class="brand" href="#top">maco.kk</a>
<nav class="links" aria-label="เมนูหลัก"><a href="#menu">สั่งเมนู</a><a href="#story">เรื่องราว</a><a href="#visit">แวะมาหาเรา</a></nav>
<button class="cartbtn" id="openCart" aria-label="เปิดตะกร้า">🛒 ตะกร้า <b id="cnt">0</b></button>
</div></header>

<main id="top">
<div class="hero"><div class="wrap">
<h1>maco<i>.</i>kk</h1>
<div class="row">
<p class="pr">กาแฟดี บรรยากาศดี มีพื้นที่ให้ใช้ชีวิตและพบปะ ได้ทั้งกลางวันและกลางคืน</p>
<div><p class="sm">คาเฟ่ &amp; บาร์ไลฟ์สไตล์ ย่านกังสดาล จ.ขอนแก่น สั่งล่วงหน้าแล้วมารับที่ร้านได้เลย</p><a class="btn" href="#menu">เลือกเมนูเลย</a></div>
</div></div><div class="strip"></div></div>

<div class="perks"><div><b>Takeaway</b>สั่งก่อน รับที่หน้าร้าน</div><div><b>ซิกเนเจอร์</b>เมนูเฉพาะที่ maco.kk</div><div><b>Combo</b>เครื่องดื่ม + อาหาร ลด ฿20</div><div><b>เปิดกลางวัน–กลางคืน</b>เมนูบาร์หลังทุ่ม</div></div>

<section id="menu"><div class="wrap">
<h2>เมนูของ maco.kk</h2>
<p class="lead">แตะเมนูเพื่อเลือกตัวเลือกและใส่ตะกร้า สั่งเครื่องดื่มคู่กับอาหาร รับส่วนลด Combo อัตโนมัติ</p>
<div class="tabs" id="tabs" role="group" aria-label="หมวดเมนู"></div>
<div class="grid" id="grid"></div>
</div></section>

<section class="about" id="story"><div class="wrap">
<h2>เรื่องราวของ maco.kk</h2>
<p class="lead">คาเฟ่ &amp; บาร์ใกล้ มข. ที่ผสานกาแฟ อาหาร และพื้นที่พบปะ ในสเปซมินิมอล–โมเดิร์นเท่ๆ</p>
<div class="cols">
<div><h3>Promise</h3><p style="font-size:20px;font-weight:500;line-height:1.5">“กาแฟดี บรรยากาศดี มีพื้นที่ให้ใช้ชีวิตและพบปะ ได้ทั้งกลางวันและกลางคืน”</p><h3>บุคลิก</h3><p>เรียบเท่ • เป็นกันเอง • มีสไตล์ เหมาะกับนักศึกษา มข. Creator และกลุ่มเพื่อน</p></div>
<div><h3>โทนสีของร้าน</h3><div class="swatch"><i style="background:#f6f5f2"></i><i style="background:#d9d7d1"></i><i style="background:#1f1e1a"></i><i style="background:#a67c52"></i><i style="background:#6f8145"></i></div><p style="margin-top:12px">ขาว เทาคอนกรีต ดำ ไม้อ่อน และสีสดจากเครื่องดื่มและอาหาร</p><h3>ภาพลักษณ์</h3><p>แสงธรรมชาติ ปูนเปลือย ไม้ กระจก มุมบันได และ Rooftop</p></div>
</div>
<ol class="steps"><li><b>1</b>เห็นร้านผ่าน IG / TikTok</li><li><b>2</b>สนใจบรรยากาศและมุมถ่ายรูป</li><li><b>3</b>แวะมาลองกาแฟ / อาหาร</li><li><b>4</b>นั่งทำงานหรือพบเพื่อน</li><li><b>5</b>ถ่ายรูป + แชร์ลงโซเชียล</li><li><b>6</b>กลับมาใช้บริการซ้ำ</li></ol>
</div></section>
</main>

<footer id="visit"><div class="wrap">
<p class="big">maco.kk</p>
<div class="r"><div>คาเฟ่ &amp; บาร์ไลฟ์สไตล์<br>ย่านกังสดาล จ.ขอนแก่น<br>แชร์รูปแล้ว Tag #maco.kk รับสิทธิ์ลดครั้งถัดไป</div>
<a class="btn" href="https://www.google.com/maps/search/maco.kk+ขอนแก่น" target="_blank" rel="noopener">เปิดแผนที่</a></div>
<small>เว็บตัวอย่างสาธิตการสั่งซื้อ ยังไม่ได้เชื่อมระบบร้านจริงหรือระบบชำระเงิน</small>
</div></footer>

<dialog id="pd" aria-label="รายละเอียดเมนู"></dialog>
<dialog id="co" aria-label="ยืนยันคำสั่งซื้อ"></dialog>
<div class="drawer" id="drawer"><div class="ov" id="ov"></div>
<aside class="pn" role="dialog" aria-label="ตะกร้าสินค้า">
<div class="ph"><h3>ตะกร้าของคุณ</h3><button class="x" id="closeCart" aria-label="ปิด">×</button></div>
<div class="lines" id="lines"></div>
<div class="sum" id="sum"></div></aside></div>
<div class="toast" id="toast" role="status"></div>

<script>
const P=[
{id:1,c:'coffee',n:'Espresso',d:'ช็อตเข้ม หอม กลมกล่อม',p:60,e:'☕',bg:'#e2cdb3',t:'d'},
{id:2,c:'coffee',n:'Americano',d:'เบลนด์คั่วกลาง หวานติดผลไม้',p:65,e:'🧊',bg:'#d8c3a5',t:'d'},
{id:3,c:'coffee',n:'Cafe Latte',d:'เอสเปรสโซนมสดเนียนนุ่ม',p:75,e:'🥛',bg:'#efe1cc',t:'d'},
{id:4,c:'coffee',n:'maco Cloud Latte',d:'ซิกเนเจอร์ ฟองนมเข้มข้นราดคาราเมลเกลือ',p:95,e:'☁️',bg:'#e9d3b1',t:'d',tag:'ซิกเนเจอร์'},
{id:5,c:'nocoffee',n:'Matcha Latte',d:'มัทฉะเกรดพิธีชงกับนมสด',p:85,e:'🍵',bg:'#cfdcb0',t:'d'},
{id:6,c:'nocoffee',n:'Yuzu Soda',d:'ยูสุซ่าเปรี้ยวหวาน สดชื่น',p:70,e:'🍋',bg:'#f2e6a6',t:'d'},
{id:7,c:'nocoffee',n:'Cocoa Rich',d:'โกโก้เข้มข้นจากช็อกโกแลตแท้',p:75,e:'🍫',bg:'#d1b4a0',t:'d'},
{id:8,c:'food',n:'Croissant แฮมชีส',d:'ครัวซองต์อบสดใหม่ ไส้แฮมและชีสเยิ้ม',p:95,e:'🥐',bg:'#f0d9a8',t:'f'},
{id:9,c:'food',n:'Pesto Pasta',d:'เส้นพาสต้าซอสเพสโต้ ไก่ย่าง',p:149,e:'🍝',bg:'#cfe0b4',t:'f'},
{id:10,c:'food',n:'Truffle Fries',d:'เฟรนช์ฟรายส์ทรัฟเฟิลและพาร์เมซาน',p:99,e:'🍟',bg:'#f2dc9b',t:'f',tag:'ขายดี'},
{id:11,c:'food',n:'ข้าวไก่เทริยากิ',d:'ไก่เทริยากิ ไข่ออนเซ็น ผักย่าง',p:120,e:'🍚',bg:'#eed6b2',t:'f'},
{id:12,c:'dessert',n:'Basque Cheesecake',d:'ชีสเค้กหน้าไหม้ เนื้อครีมมี่',p:110,e:'🍰',bg:'#f1d8c2',t:'f'},
{id:13,c:'dessert',n:'Brownie เข้มข้น',d:'บราวนี่หน้ากรอบ เสิร์ฟอุ่นๆ',p:80,e:'🧁',bg:'#d3b7a3',t:'f'}];
const CATS={all:'ทั้งหมด',coffee:'กาแฟ',nocoffee:'ไม่ใช่กาแฟ',food:'อาหาร',dessert:'ของหวาน'};
const $=s=>document.querySelector(s);
const baht=n=>'฿'+n.toLocaleString('th-TH');
let cart=[],cat='all';
try{cart=JSON.parse(localStorage.getItem('makokk_cart')||'[]')}catch(e){cart=[]}
const save=()=>{try{localStorage.setItem('makokk_cart',JSON.stringify(cart))}catch(e){}};
let tt;const toast=m=>{const t=$('#toast');t.textContent=m;t.classList.add('on');clearTimeout(tt);tt=setTimeout(()=>t.classList.remove('on'),2000)};

function renderTabs(){$('#tabs').innerHTML=Object.entries(CATS).map(([k,v])=>`<button data-c="${k}" aria-pressed="${k===cat}">${v}</button>`).join('')}
function renderGrid(){$('#grid').innerHTML=P.filter(x=>cat==='all'||x.c===cat).map(x=>`<button class="item" data-id="${x.id}"><div class="pic" style="background:${x.bg}">${x.tag?`<em>${x.tag}</em>`:''}${x.e}</div><div class="b"><h3>${x.n}</h3><small>${x.d}</small><div class="pp"><span>${baht(x.p)}</span><span aria-hidden="true">+</span></div></div></button>`).join('')}
$('#tabs').onclick=e=>{const b=e.target.closest('button');if(!b)return;cat=b.dataset.c;renderTabs();renderGrid()};
$('#grid').onclick=e=>{const b=e.target.closest('.item');if(b)openProduct(+b.dataset.id)};

const pd=$('#pd');
function radios(name,arr,def){return `<div class="opts">${arr.map(([v,l],i)=>`<label><input type="radio" name="${name}" value="${v}" ${v===def?'checked':''}><span>${l}</span></label>`).join('')}</div>`}
function openProduct(id){
 const x=P.find(p=>p.id===id);let q=1;
 const dr=x.t==='d';
 pd.innerHTML=`<div class="dh" style="background:${x.bg}">${x.e}<button class="x" data-close aria-label="ปิด">×</button></div>
 <div class="dbody"><h3>${x.n}</h3><p>${x.d}</p>
 ${dr?`<fieldset><legend>รูปแบบ</legend>${radios('temp',[['ร้อน','ร้อน'],['เย็น','เย็น'],['ปั่น','ปั่น +฿10']],'เย็น')}</fieldset>
 <fieldset><legend>ระดับความหวาน</legend>${radios('sw',[['0%','0%'],['30%','30%'],['50%','50%'],['100%','100%']],'50%')}</fieldset>
 <fieldset><legend>ขนาด</legend>${radios('sz',[['M','M'],['L','L +฿10']],'M')}</fieldset>`
 :`<fieldset><legend>ตัวเลือก</legend>${radios('wm',[['ทานที่ร้าน','ทานที่ร้าน'],['อุ่นให้','อุ่นให้'],['ห่อกลับ','ห่อกลับ']],'ทานที่ร้าน')}</fieldset>`}
 <label class="f" for="nt">หมายเหตุ</label><input class="t" id="nt" placeholder="เช่น ไม่ใส่น้ำแข็ง แพ้ถั่ว">
 <div class="foot"><div class="qty"><button data-m aria-label="ลด">−</button><span id="q">1</span><button data-p aria-label="เพิ่ม">+</button></div><button class="btn" id="add"></button></div></div>`;
 const calc=()=>{let u=x.p;if(dr){if(pd.querySelector('[name=sz]:checked').value==='L')u+=10;if(pd.querySelector('[name=temp]:checked').value==='ปั่น')u+=10}return u};
 const upd=()=>{$('#q').textContent=q;$('#add').textContent=`ใส่ตะกร้า • ${baht(calc()*q)}`};
 pd.onchange=upd;
 pd.onclick=e=>{
  if(e.target.closest('[data-close]')||e.target===pd)return pd.close();
  if(e.target.closest('[data-m]')){q=Math.max(1,q-1);upd()}
  if(e.target.closest('[data-p]')){q=Math.min(20,q+1);upd()}
  if(e.target.closest('#add')){
   const o=dr?[pd.querySelector('[name=temp]:checked').value,'หวาน '+pd.querySelector('[name=sw]:checked').value,'ไซส์ '+pd.querySelector('[name=sz]:checked').value]:[pd.querySelector('[name=wm]:checked').value];
   const note=$('#nt').value.trim();if(note)o.push(note);
   const key=x.id+'|'+o.join(',');const ex=cart.find(l=>l.key===key);
   if(ex)ex.q+=q;else cart.push({key,id:x.id,opt:o.join(' • '),u:calc(),q});
   save();renderCart();pd.close();toast(`เพิ่ม ${x.n} ลงตะกร้าแล้ว`);
  }};
 upd();pd.showModal();
}

function totals(){
 const sub=cart.reduce((s,l)=>s+l.u*l.q,0);
 let dn=0,fd=0;cart.forEach(l=>{const p=P.find(x=>x.id===l.id);if(p.t==='d')dn+=l.q;else fd+=l.q});
 const disc=Math.min(dn,fd)*20;return{sub,disc,tot:sub-disc,n:cart.reduce((s,l)=>s+l.q,0),pairs:Math.min(dn,fd),dn,fd};
}
function renderCart(){
 const t=totals();$('#cnt').textContent=t.n;
 $('#lines').innerHTML=cart.length?cart.map((l,i)=>{const p=P.find(x=>x.id===l.id);return `<div class="ln"><div class="ic" style="background:${p.bg}">${p.e}</div><div><b>${p.n}</b><small>${l.opt}</small><div class="qty"><button data-d="${i}" aria-label="ลด">−</button><span>${l.q}</span><button data-i="${i}" aria-label="เพิ่ม">+</button></div></div><b>${baht(l.u*l.q)}</b></div>`}).join(''):`<div class="empty"><div style="font-size:48px">🛒</div>ตะกร้ายังว่างอยู่<br>เลือกเมนูที่ชอบได้เลย</div>`;
 let hint='';if(cart.length&&!t.pairs){hint=t.dn?'เพิ่มอาหารอีก 1 อย่าง รับส่วนลด Combo ฿20':'เพิ่มเครื่องดื่มอีก 1 แก้ว รับส่วนลด Combo ฿20'}
 $('#sum').innerHTML=cart.length?`<div><span>ยอดรวม</span><span>${baht(t.sub)}</span></div>${t.disc?`<div class="disc"><span>Combo × ${t.pairs}</span><span>−${baht(t.disc)}</span></div>`:''}${hint?`<div style="color:var(--muted);font-size:13px">${hint}</div>`:''}<div class="tot"><span>รวมสุทธิ</span><span>${baht(t.tot)}</span></div><button class="btn dk block" id="goCo">ไปหน้าชำระเงิน</button>`:'';
}
$('#lines').onclick=e=>{const d=e.target.closest('[data-d]'),i=e.target.closest('[data-i]');
 if(i)cart[+i.dataset.i].q++;
 if(d){const k=+d.dataset.d;cart[k].q--;if(cart[k].q<1)cart.splice(k,1)}
 save();renderCart()};
const dw=$('#drawer');
const openC=()=>{dw.classList.add('on')},closeC=()=>dw.classList.remove('on');
$('#openCart').onclick=openC;$('#closeCart').onclick=closeC;$('#ov').onclick=closeC;
document.addEventListener('keydown',e=>{if(e.key==='Escape')closeC()});

const co=$('#co');
$('#sum').onclick=e=>{if(!e.target.closest('#goCo'))return;closeC();checkout()};
function checkout(){
 const t=totals();
 co.innerHTML=`<div class="ph"><h3>ยืนยันคำสั่งซื้อ</h3><button class="x" data-close aria-label="ปิด">×</button></div>
 <div class="dbody"><label class="f" for="nm">ชื่อผู้สั่ง</label><input class="t" id="nm" placeholder="ชื่อเล่นก็ได้" autocomplete="name">
 <label class="f" for="ph">เบอร์โทร</label><input class="t" id="phn" inputmode="tel" placeholder="08x-xxx-xxxx" autocomplete="tel">
 <fieldset><legend>รูปแบบรับสินค้า</legend>${radios('mode',[['ทานที่ร้าน','ทานที่ร้าน'],['Takeaway','Takeaway (รับหน้าร้าน)']],'Takeaway')}</fieldset>
 <fieldset><legend>ชำระเงิน</legend>${radios('pay',[['PromptPay','PromptPay'],['เงินสดที่เคาน์เตอร์','เงินสดที่เคาน์เตอร์']],'PromptPay')}</fieldset>
 <p id="err" style="color:#b3261e;font-weight:600;margin:0 0 8px" role="alert"></p>
 <div class="sum" style="border-radius:12px;padding:12px 16px;margin-bottom:14px"><div class="tot" style="margin:0"><span>ยอดชำระ</span><span>${baht(t.tot)}</span></div></div>
 <button class="btn dk block" id="place">ยืนยันสั่งซื้อ</button></div>`;
 co.onclick=e=>{
  if(e.target.closest('[data-close]')||e.target===co)return co.close();
  if(e.target.closest('#place')){
   const nm=$('#nm').value.trim(),ph=$('#phn').value.replace(/\D/g,'');
   if(!nm)return $('#err').textContent='กรอกชื่อผู้สั่งก่อนยืนยัน';
   if(ph.length<9)return $('#err').textContent='กรอกเบอร์โทรอย่างน้อย 9 หลัก';
   const mode=co.querySelector('[name=mode]:checked').value,pay=co.querySelector('[name=pay]:checked').value;
   const no='MK-'+String(Math.floor(100+Math.random()*900));
   const items=cart.map(l=>`<li>${l.q}× ${P.find(x=>x.id===l.id).n}</li>`).join('');
   const tot=totals().tot;cart=[];save();renderCart();
   co.innerHTML=`<div class="ok"><div class="ck">✓</div><h3 style="margin:0">สั่งซื้อสำเร็จ</h3><div class="no">${no}</div><p style="margin:0;color:var(--muted)">คุณ ${nm} • ${mode} • ${pay}</p><ul>${items}<li><b>รวม ${baht(tot)}</b></li></ul><p style="color:var(--muted);font-size:14px;margin:0 0 16px">ร้านจะเตรียมออเดอร์ให้ใน 10–15 นาที แสดงเลขออเดอร์นี้ที่เคาน์เตอร์ แล้ว Tag #maco.kk ได้เลย</p><button class="btn dk block" data-close>กลับไปดูเมนู</button></div>`;
  }};
 co.showModal();
}

renderTabs();renderGrid();renderCart();
</script>
</body>
</html>
