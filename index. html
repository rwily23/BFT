# BFT <!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>BFT - Blox Fruits Trading</title>

<style>
*{
    box-sizing:border-box;
    margin:0;
    padding:0;
    font-family:Arial, sans-serif;
}

body{
    background:
        radial-gradient(circle at top,#172554 0,#080b16 45%,#05060b 100%);
    color:white;
    min-height:100vh;
}

header{
    height:75px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:0 6%;
    background:rgba(5,8,18,.85);
    border-bottom:1px solid rgba(255,255,255,.08);
    position:sticky;
    top:0;
    z-index:10;
    backdrop-filter:blur(15px);
}

.logo{
    font-size:30px;
    font-weight:900;
    color:#ffb300;
    letter-spacing:2px;
}

nav{
    display:flex;
    gap:25px;
    align-items:center;
}

nav a{
    color:#ddd;
    text-decoration:none;
    cursor:pointer;
    transition:.2s;
}

nav a:hover{
    color:#ffb300;
}

.lang{
    border:1px solid #334155;
    background:#111827;
    color:white;
    padding:9px 14px;
    border-radius:10px;
    cursor:pointer;
}

.hero{
    min-height:430px;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    padding:60px 20px;
}

.hero-content{
    max-width:850px;
}

.badge{
    display:inline-block;
    background:rgba(255,179,0,.1);
    border:1px solid rgba(255,179,0,.3);
    color:#ffbf26;
    padding:8px 15px;
    border-radius:30px;
    margin-bottom:20px;
}

h1{
    font-size:clamp(45px,8vw,85px);
    font-weight:900;
    line-height:1;
    margin-bottom:20px;
}

.gradient{
    background:linear-gradient(90deg,#ffb300,#ff6b00,#ffd54a);
    -webkit-background-clip:text;
    color:transparent;
}

.hero p{
    color:#aeb8cc;
    font-size:19px;
    line-height:1.8;
    margin-bottom:30px;
}

.buttons{
    display:flex;
    gap:15px;
    justify-content:center;
    flex-wrap:wrap;
}

button{
    border:none;
    cursor:pointer;
    transition:.2s;
}

.primary{
    background:linear-gradient(135deg,#ffb300,#ff7200);
    color:#111;
    font-weight:bold;
    padding:14px 25px;
    border-radius:12px;
    font-size:16px;
    box-shadow:0 8px 25px rgba(255,150,0,.2);
}

.primary:hover{
    transform:translateY(-2px);
    box-shadow:0 12px 30px rgba(255,150,0,.35);
}

.secondary{
    background:#151b2d;
    color:white;
    border:1px solid #303a52;
    padding:14px 25px;
    border-radius:12px;
    font-size:16px;
}

.container{
    width:min(1150px,92%);
    margin:auto;
}

.section{
    padding:70px 0;
}

.section-title{
    text-align:center;
    margin-bottom:35px;
}

.section-title h2{
    font-size:32px;
    margin-bottom:10px;
}

.section-title p{
    color:#8490a7;
}

.trade-box{
    background:rgba(15,21,38,.9);
    border:1px solid #29344d;
    border-radius:20px;
    padding:30px;
    box-shadow:0 20px 60px rgba(0,0,0,.25);
}

.form-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:25px;
}

.field{
    margin-bottom:20px;
}

label{
    display:block;
    margin-bottom:9px;
    color:#cbd5e1;
    font-weight:bold;
}

input,textarea,select{
    width:100%;
    background:#080d1a;
    border:1px solid #303b55;
    color:white;
    border-radius:10px;
    padding:13px;
    outline:none;
}

input:focus,textarea:focus,select:focus{
    border-color:#ffb300;
}

textarea{
    min-height:100px;
    resize:vertical;
}

.fruit-list{
    display:flex;
    flex-wrap:wrap;
    gap:9px;
}

.fruit{
    background:#111827;
    border:1px solid #34415e;
    padding:9px 13px;
    border-radius:9px;
    color:#dce3ef;
    cursor:pointer;
    transition:.2s;
}

.fruit:hover{
    border-color:#ffb300;
}

.fruit.selected{
    background:rgba(255,179,0,.15);
    border-color:#ffb300;
    color:#ffc84d;
}

.trade-actions{
    margin-top:20px;
    text-align:center;
}

.search-area{
    display:flex;
    gap:12px;
    margin-bottom:25px;
}

.search-area input{
    flex:1;
}

.trades{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:18px;
}

.trade-card{
    background:#101728;
    border:1px solid #293650;
    border-radius:17px;
    padding:20px;
    transition:.2s;
}

.trade-card:hover{
    transform:translateY(-4px);
    border-color:#ffae00;
}

.player{
    color:#ffbd2e;
    font-weight:bold;
    margin-bottom:18px;
}

.trade-row{
    display:grid;
    grid-template-columns:1fr 40px 1fr;
    align-items:center;
    gap:8px;
}

.offer{
    background:#080e1c;
    border-radius:10px;
    padding:12px;
    text-align:center;
    min-height:70px;
}

.offer small{
    display:block;
    color:#71809a;
    margin-bottom:6px;
}

.arrow{
    text-align:center;
    font-size:20px;
    color:#ffb300;
}

.note{
    margin-top:15px;
    color:#8d99ae;
    font-size:13px;
}

.empty{
    text-align:center;
    color:#7d899e;
    padding:40px;
    background:#0e1525;
    border-radius:15px;
}

footer{
    border-top:1px solid #202a3e;
    margin-top:40px;
    padding:30px;
    text-align:center;
    color:#68758c;
}

.toast{
    position:fixed;
    bottom:25px;
    left:50%;
    transform:translateX(-50%) translateY(100px);
    background:#16a34a;
    color:white;
    padding:13px 22px;
    border-radius:10px;
    opacity:0;
    transition:.3s;
    z-index:50;
}

.toast.show{
    transform:translateX(-50%) translateY(0);
    opacity:1;
}

@media(max-width:800px){
    header{
        padding:0 4%;
    }

    nav a{
        display:none;
    }

    .form-grid{
        grid-template-columns:1fr;
    }

    .trades{
        grid-template-columns:1fr;
    }

    .hero{
        min-height:380px;
    }

    .trade-box{
        padding:20px;
    }
}
</style>
</head>

<body>

<header>
    <div class="logo">BFT</div>

    <nav>
        <a onclick="scrollToId('home')" data-ar="الرئيسية" data-en="Home">الرئيسية</a>
        <a onclick="scrollToId('create')" data-ar="أنشئ عرضك" data-en="Create Trade">أنشئ عرضك</a>
        <a onclick="scrollToId('trades')" data-ar="المقايضات" data-en="Trades">المقايضات</a>
    </nav>

    <button class="lang" onclick="toggleLanguage()">English</button>
</header>


<section class="hero" id="home">
    <div class="hero-content">

        <span class="badge" data-ar="منصة مقايضة فواكه Blox Fruits"
              data-en="Blox Fruits Trading Platform">
            منصة مقايضة فواكه Blox Fruits
        </span>

        <h1>
            <span class="gradient">BFT</span>
        </h1>

        <p data-ar="اعرض فواكهك، حدد ما تريده، وابحث عن أفضل المقايضات مع لاعبين آخرين."
           data-en="Offer your fruits, choose what you want, and discover trades with other players.">
            اعرض فواكهك، حدد ما تريده، وابحث عن أفضل المقايضات مع لاعبين آخرين.
        </p>

        <div class="buttons">
            <button class="primary" onclick="scrollToId('create')"
                    data-ar="➕ أنشئ عرضك"
                    data-en="➕ Create Trade">
                ➕ أنشئ عرضك
            </button>

            <button class="secondary" onclick="scrollToId('trades')"
                    data-ar="🔄 تصفح المقايضات"
                    data-en="🔄 Browse Trades">
                🔄 تصفح المقايضات
            </button>
        </div>

    </div>
</section>


<section class="section" id="create">
<div class="container">

    <div class="section-title">
        <h2 data-ar="أنشئ عرض مقايضتك"
            data-en="Create Your Trade">
            أنشئ عرض مقايضتك
        </h2>

        <p data-ar="حدد ما تملك وما تريد الحصول عليه."
           data-en="Choose what you offer and what you want.">
            حدد ما تملك وما تريد الحصول عليه.
        </p>
    </div>

    <div class="trade-box">

        <div class="field">
            <label data-ar="اسم اللاعب في Roblox"
                   data-en="Roblox Username">
                اسم اللاعب في Roblox
            </label>

            <input id="username"
                   placeholder="مثال: BFT_Player"
                   data-placeholder-ar="مثال: BFT_Player"
                   data-placeholder-en="Example: BFT_Player">
        </div>

        <div class="form-grid">

            <div class="field">
                <label data-ar="🍎 أنا أقدم"
                       data-en="🍎 I Offer">
                    🍎 أنا أقدم
                </label>

                <div class="fruit-list" id="offerFruits"></div>
            </div>

            <div class="field">
                <label data-ar="🎯 أطلب مقابلها"
                       data-en="🎯 I Want">
                    🎯 أطلب مقابلها
                </label>

                <div class="fruit-list" id="wantFruits"></div>
            </div>

        </div>

        <div class="field">
            <label data-ar="ملاحظة (اختياري)"
                   data-en="Note (Optional)">
                ملاحظة (اختياري)
            </label>

            <textarea id="note"
                      placeholder="مثال: قابل للتفاوض..."
                      data-placeholder-ar="مثال: قابل للتفاوض..."
                      data-placeholder-en="Example: Open to offers..."></textarea>
        </div>

        <div class="trade-actions">
            <button class="primary" onclick="publishTrade()"
                    data-ar="🚀 نشر المقايضة"
                    data-en="🚀 Publish Trade">
                🚀 نشر المقايضة
            </button>
        </div>

    </div>

</div>
</section>


<section class="section" id="trades">
<div class="container">

    <div class="section-title">
        <h2 data-ar="🔄 المقايضات"
            data-en="🔄 Trades">
            🔄 المقايضات
        </h2>

        <p data-ar="ابحث عن العرض الذي يناسبك."
           data-en="Find a trade that matches what you need.">
            ابحث عن العرض الذي يناسبك.
        </p>
    </div>

    <div class="search-area">
        <input id="search"
               oninput="renderTrades()"
               placeholder="ابحث عن فاكهة..."
               data-placeholder-ar="ابحث عن فاكهة..."
               data-placeholder-en="Search for a fruit...">

        <select id="filter" onchange="renderTrades()">
            <option value="all" data-ar="الكل" data-en="All">الكل</option>
            <option value="Dragon">Dragon</option>
            <option value="Dough">Dough</option>
            <option value="Kitsune">Kitsune</option>
            <option value="Leopard">Leopard</option>
            <option value="Buddha">Buddha</option>
        </select>
    </div>

    <div class="trades" id="tradeContainer"></div>

</div>
</section>


<footer>
    <strong>BFT</strong>
    <br><br>
    <span data-ar="منصة مقايضة فواكه Blox Fruits"
          data-en="Blox Fruits Trading Platform">
        منصة مقايضة فواكه Blox Fruits
    </span>
</footer>


<div class="toast" id="toast"></div>


<script>

const fruits = [
    "Dragon",
    "Dough",
    "Kitsune",
    "Leopard",
    "Buddha",
    "T-Rex",
    "Mammoth",
    "Spirit",
    "Venom",
    "Control",
    "Shadow",
    "Blizzard",
    "Rumble",
    "Portal",
    "Phoenix",
    "Magma",
    "Light",
    "Dark",
    "Ice",
    "Flame"
];

let language = "ar";

let selectedOffer = [];
let selectedWant = [];

let trades = JSON.parse(localStorage.getItem("bftTrades")) || [
    {
        username:"BFT_Trader",
        offer:["Dragon"],
        want:["Kitsune"],
        note:"مستعد للتفاوض"
    },
    {
        username:"FruitMaster",
        offer:["Dough","Buddha"],
        want:["Leopard"],
        note:""
    },
    {
        username:"TradeKing",
        offer:["Kitsune"],
        want:["Dragon"],
        note:"أفضل عرض"
    }
];


function createFruitButtons(){

    const offer = document.getElementById("offerFruits");
    const want = document.getElementById("wantFruits");

    offer.innerHTML="";
    want.innerHTML="";

    fruits.forEach(fruit=>{

        const a=document.createElement("button");
        a.className="fruit";
        a.textContent=fruit;

        if(selectedOffer.includes(fruit))
            a.classList.add("selected");

        a.onclick=()=>{
            if(selectedOffer.includes(fruit)){
                selectedOffer=selectedOffer.filter(x=>x!==fruit);
            }else{
                selectedOffer.push(fruit);
            }

            createFruitButtons();
        };

        offer.appendChild(a);


        const b=document.createElement("button");
        b.className="fruit";
        b.textContent=fruit;

        if(selectedWant.includes(fruit))
            b.classList.add("selected");

        b.onclick=()=>{
            if(selectedWant.includes(fruit)){
                selectedWant=selectedWant.filter(x=>x!==fruit);
            }else{
                selectedWant.push(fruit);
            }

            createFruitButtons();
        };

        want.appendChild(b);

    });
}


function publishTrade(){

    const username=document.getElementById("username").value.trim();
    const note=document.getElementById("note").value.trim();

    if(!username){
        showToast(language==="ar"
            ?"اكتب اسم لاعب Roblox أولاً"
            :"Enter your Roblox username first");
        return;
    }

    if(selectedOffer.length===0 || selectedWant.length===0){
        showToast(language==="ar"
            ?"اختر الفواكه التي تقدمها والتي تريدها"
            :"Choose both offer and wanted fruits");
        return;
    }

    trades.unshift({
        username,
        offer:[...selectedOffer],
        want:[...selectedWant],
        note
    });

    localStorage.setItem("bftTrades",JSON.stringify(trades));

    document.getElementById("username").value="";
    document.getElementById("note").value="";

    selectedOffer=[];
    selectedWant=[];

    createFruitButtons();
    renderTrades();

    showToast(language==="ar"
        ?"تم نشر مقايضتك بنجاح 🚀"
        :"Your trade was published 🚀");

    scrollToId("trades");
}


function renderTrades(){

    const container=document.getElementById("tradeContainer");

    const search=document.getElementById("search").value.toLowerCase();
    const filter=document.getElementById("filter").value;

    const filtered=trades.filter(trade=>{

        const allFruits=[...trade.offer,...trade.want];

        const matchesSearch =
            trade.username.toLowerCase().includes(search) ||
            allFruits.some(f=>f.toLowerCase().includes(search));

        const matchesFilter =
            filter==="all" ||
            allFruits.includes(filter);

        return matchesSearch && matchesFilter;
    });

    if(filtered.length===0){

        container.innerHTML=`
            <div class="empty" style="grid-column:1/-1">
                ${language==="ar"
                    ?"لا توجد مقايضات مطابقة 🔍"
                    :"No matching trades found 🔍"}
            </div>
        `;

        return;
    }

    container.innerHTML=filtered.map(trade=>`

        <div class="trade-card">

            <div class="player">
                🎮 ${escapeHTML(trade.username)}
            </div>

            <div class="trade-row">

                <div class="offer">
                    <small>${language==="ar"?"يقدم":"Offers"}</small>
                    ${trade.offer.map(x=>`<div>${x}</div>`).join("")}
                </div>

                <div class="arrow">⇄</div>

                <div class="offer">
                    <small>${language==="ar"?"يطلب":"Wants"}</small>
                    ${trade.want.map(x=>`<div>${x}</div>`).join("")}
                </div>

            </div>

            ${
                trade.note
                ? `<div class="note">💬 ${escapeHTML(trade.note)}</div>`
                : ""
            }

        </div>

    `).join("");
}


function escapeHTML(text){

    return text
        .replace(/&/g,"&amp;")
        .replace(/</g,"&lt;")
        .replace(/>/g,"&gt;")
        .replace(/"/g,"&quot;")
        .replace(/'/g,"&#039;");
}


function toggleLanguage(){

    language=language==="ar"?"en":"ar";

    document.documentElement.lang=language;
    document.documentElement.dir=language==="ar"?"rtl":"ltr";

    document.querySelector(".lang").textContent=
        language==="ar"?"English":"العربية";

    document.querySelectorAll("[data-ar]").forEach(el=>{
        el.textContent=language==="ar"
            ?el.dataset.ar
            :el.dataset.en;
    });

    document.querySelectorAll("[data-placeholder-ar]").forEach(el=>{
        el.placeholder=language==="ar"
            ?el.dataset.placeholderAr
            :el.dataset.placeholderEn;
    });

    renderTrades();
}


function scrollToId(id){

    document.getElementById(id).scrollIntoView({
        behavior:"smooth"
    });
}


function showToast(message){

    const toast=document.getElementById("toast");

    toast.textContent=message;
    toast.classList.add("show");

    setTimeout(()=>{
        toast.classList.remove("show");
    },2500);
}


createFruitButtons();
renderTrades();

</script>

</body>
</html>
