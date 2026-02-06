function floatingHearts(){
let heart = document.createElement("div");
heart.innerHTML="💖";
heart.style.position="fixed";
heart.style.left=Math.random()*100+"vw";
heart.style.top="100vh";
heart.style.fontSize="20px";
heart.style.animation="float 4s linear";

document.body.appendChild(heart);

setTimeout(()=>heart.remove(),4000);
}

setInterval(floatingHearts,700);
