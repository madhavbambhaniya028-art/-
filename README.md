😚
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Valentine Question 💘</title>

<style>
body {
    margin: 0;
    height: 100vh;
    font-family: 'Segoe UI', sans-serif;
    background: radial-gradient(circle, #ff758c, #ff7eb3);
    display: flex;
    align-items: center;
    justify-content: center;
}

.box {
    background: white;
    width: 90%;
    max-width: 350px;
    padding: 30px;
    border-radius: 20px;
    text-align: center;
    box-shadow: 0 15px 30px rgba(0,0,0,0.25);
    animation: pop 1.2s ease;
}

h1 {
    color: #ff2e63;
}

p {
    color: #444;
    font-size: 16px;
}

button {
    padding: 12px 18px;
    margin: 10px;
    border: none;
    border-radius: 30px;
    font-size: 15px;
    cursor: pointer;
    transition: 0.3s;
}

.next {
    background: #ff2e63;
    color: white;
}

.next:hover {
    transform: scale(1.1);
}

@keyframes pop {
    from { transform: scale(0.8); opacity: 0; }
    to { transform: scale(1); opacity: 1; }
}
</style>
</head>

<body>

<div class="box" id="content">
    <h1>Hey You 💖</h1>
    <p>
        I have a small story to tell you…  
        Are you ready to hear it?
    </p>
    <button class="next" onclick="step1()">Yes, tell me 😊</button>
</div>

<script>
function step1(){
    content.innerHTML = `
    <h1>Once Upon a Time ✨</h1>
    <p>
        There was a girl who slowly became  
        the most important part of my life.
    </p>
    <button class="next" onclick="step2()">Go on 💕</button>
    `;
}

function step2(){
    content.innerHTML = `
    <h1>That Girl 💫</h1>
    <p>
        She made me smile without trying,  
        and my heart chose her without asking.
    </p>
    <button class="next" onclick="step3()">And then? ❤️</button>
    `;
}

function step3(){
    content.innerHTML = `
    <h1>So Today 💌</h1>
    <p>
        I want to ask you something  
        straight from my heart…
    </p>
    <button class="next" onclick="finalStep()">Tell me 😍</button>
    `;
}

function finalStep(){
    content.innerHTML = `
    <h1>Will You Be My Valentine? 💖</h1>
    <p>
        Not just for today,  
        but for all the smiles we’ll share.
    </p>
    <button class="next" onclick="yes()">YES 💕</button>
    `;
}

function yes(){
    document.body.innerHTML = `
    <div style="height:100vh;display:flex;align-items:center;justify-content:center;
    background:radial-gradient(circle,#ff758c,#ff7eb3);
    font-family:'Segoe UI',sans-serif;">
        <h1 style="color:white;font-size:38px;text-align:center;">
        You just made my heart dance 💃❤️<br>
        Happy Valentine’s Day 💘
        </h1>
    </div>
    `;
}
</script>

</body>
</html>
