<!DOCTYPE html><html lang="th">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ไพ่กำลังใจ - BY STUDIO iWAVE</title>
  <style>
    @font-face {
      font-family: 'HealingFont';
      src: url('200.ttf');
    }body {
  font-family: 'HealingFont', sans-serif;
  background: #fefdf9;
  color: #333;
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: column;
  align-items: center;
}

h1 {
  color: #444;
  margin-top: 30px;
}

.question {
  background: #ffffff;
  border-radius: 12px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.08);
  padding: 20px;
  width: 90%;
  max-width: 600px;
  margin: 20px 0;
}

.question h2 {
  font-size: 1.2em;
  color: #555;
}

.options label {
  display: block;
  margin: 10px 0;
}

button {
  background: #9cb4cc;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 8px;
  font-size: 1em;
  cursor: pointer;
  margin: 20px;
  transition: background 0.3s;
}

button:hover {
  background: #8ca3bd;
}

.card {
  background: #fff;
  border: 2px solid #d4dbe5;
  border-radius: 16px;
  padding: 30px;
  margin: 30px 0;
  width: 90%;
  max-width: 500px;
  text-align: center;
  box-shadow: 0 6px 16px rgba(0,0,0,0.1);
  background: linear-gradient(145deg, #fefefe, #f2f5fa);
}

.card h3 {
  font-size: 1.5em;
  margin-bottom: 10px;
}

.footer {
  margin-top: 50px;
  font-size: 0.9em;
  color: #aaa;
}

  </style>
</head>
<body>
  <h1>สุ่มไพ่กำลังใจ - BY STUDIO iWAVE</h1>  <audio autoplay loop>
    <source src="https://cdn.pixabay.com/audio/2022/03/25/audio_c11dcfcd65.mp3" type="audio/mpeg">
    เบราว์เซอร์ของคุณไม่รองรับเสียง
  </audio>  <form id="quizForm">
    <!-- คำถามทั้ง 5 ข้อ เหมือนเดิม -->
  </form>  <div id="cardResult" class="card" style="display:none;"></div>  <div class="footer">© BY STUDIO iWAVE</div>  <script>
    const cards = [
      { title: "The Light", text: "แม้วันนี้จะหม่น แต่เธอก็คือแสงเล็ก ๆ ที่ยังส่องออกมาได้เสมอ" },
      { title: "The Tree", text: "เธออาจไม่รู้ตัว แต่เธอยืนหยัดได้ดีมากแล้วนะ" },
      { title: "The Mirror", text: "มองดูตัวเองอีกครั้ง เธอไม่ได้แย่อย่างที่คิด" },
      { title: "The Hug", text: "บางที... เธอแค่ต้องการอ้อมกอดจากใครสักคน ไม่ใช่คำตอบ" },
      { title: "The Dreamer", text: "แม้ความฝันจะเบลอ แต่การที่ยังฝันได้ คือพลังอย่างหนึ่ง" },
      { title: "The Flame", text: "เธอมีไฟในใจ แม้จะเล็กแค่ไหน ก็ยังให้ความอบอุ่นได้" },
      { title: "The Silence", text: "ไม่ต้องอธิบายทุกอย่างก็ได้ ความเงียบก็มีความหมายของมัน" },
      { title: "The Cloud", text: "วันนี้อาจครึ้ม แต่ท้องฟ้าสีฟ้าจะกลับมาเสมอ" },
      { title: "The Voice", text: "เสียงของเธอสำคัญ ไม่ว่าจะมีคนฟังหรือไม่ก็ตาม" },
      { title: "The Bridge", text: "เธอกำลังเดินข้ามบางอย่างอยู่ ไม่ช้าก็ถึงอีกฝั่ง" }
    ];

    document.getElementById("quizForm").addEventListener("submit", function(e) {
      e.preventDefault();
      const result = cards[Math.floor(Math.random() * cards.length)];
      const cardDiv = document.getElementById("cardResult");
      cardDiv.innerHTML = `<h3>${result.title}</h3><p>${result.text}</p>`;
      cardDiv.style.display = 'block';
      cardDiv.scrollIntoView({ behavior: 'smooth' });
    });
  </script></body>
</html># STUDIO-IWAVE-
