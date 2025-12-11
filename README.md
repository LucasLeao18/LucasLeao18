👋 Olá! Eu sou o Lucas Leão

Desenvolvedor apaixonado por tecnologia, automações, IA e soluções que realmente fazem diferença.
Aqui você encontra meus projetos, experimentos e muita criatividade.

🎮 Joguinhos Interativos no Terminal

Aperte as setas ⬆️⬇️ para mover e tente capturar o emoji certo!

👉 Mini-Game: Catch the Emoji

(Copia e cola este bloco no seu README — o jogo funciona usando Markdown + JS no GitHub Pages ou no Codespaces.)

<!-- Mini Game simples em HTML + JS para usar no GitHub Pages -->
<div id="game" style="font-size:30px; text-align:center;">
  <p id="emoji">🎯</p>
  <p>Use as setas do teclado para mover o alvo: <span id="cursor">⬇️</span></p>
  <p>Pontuação: <span id="score">0</span></p>
</div>

<script>
let score = 0;
const emojis = ["🔥","⭐","🍀","⚡","🎯","💎"];
const cursor = document.getElementById("cursor");
const scoreBox = document.getElementById("score");
const emojiBox = document.getElementById("emoji");

document.addEventListener("keydown", (e) => {
  if (["ArrowUp","ArrowDown","ArrowLeft","ArrowRight"].includes(e.key)) {
    cursor.textContent = e.key.replace("Arrow","") + "️";
    const target = emojis[Math.floor(Math.random() * emojis.length)];
    if (target === "🎯") score++;
    emojiBox.textContent = target;
    scoreBox.textContent = score;
  }
});
</script>

🧑‍💻 Sobre mim

🎓 Bacharelando em Sistemas de Informação — UPE

🤖 Focado em IA, automações e desenvolvimento full-stack

🚀 Crio bots, ferramentas úteis e interfaces modernas

🧠 Amante de desafios e aprendizado constante

📫 Entre em contato

LinkedIn: https://www.linkedin.com/in/lucasleão18/

GitHub: https://github.com/LucasLeao18
