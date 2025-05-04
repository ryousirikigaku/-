<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>量子占い - あなたの意識が未来を観測する</title>
  <style>
    body {
      background: radial-gradient(circle, #1a1a1a, #000000);
      color: #ffffff;
      font-family: 'Helvetica Neue', sans-serif;
      text-align: center;
      padding: 2rem;
    }
    h1 {
      font-size: 2.5rem;
      margin-bottom: 0.5rem;
    }
    p {
      font-size: 1.2rem;
      max-width: 600px;
      margin: 0 auto 2rem;
    }
    input, select, button {
      padding: 0.8rem;
      font-size: 1rem;
      margin: 0.5rem;
      border: none;
      border-radius: 5px;
    }
    button {
      background-color: #00c3ff;
      color: #fff;
      cursor: pointer;
    }
    .result {
      margin-top: 2rem;
      font-size: 1.4rem;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <h1>量子力学的意識占い</h1>
  <p>あなたの意識波動が、どんな未来を観測しているのか──簡単な質問に答えて診断してみよう。</p>

  <form id="quiz-form">
    <input type="text" id="name" placeholder="名前" required><br>
    <select id="focus">
      <option value="love">恋愛</option>
      <option value="career">仕事</option>
      <option value="growth">自己成長</option>
    </select><br>
    <button type="submit">診断する</button>
  </form>

  <div class="result" id="result"></div>

  <script>
    document.getElementById("quiz-form").addEventListener("submit", function(e) {
      e.preventDefault();
      const name = document.getElementById("name").value;
      const focus = document.getElementById("focus").value;

      let message = "";
      switch (focus) {
        case "love":
          message = `${name}さんの意識は、愛の共鳴波動に包まれています。観測することで、出会いの確率が高まるでしょう。`;
          break;
        case "career":
          message = `${name}さんの思考は、未来の成功をすでに収束させています。集中するほど、現実は好転します。`;
          break;
        case "growth":
          message = `${name}さんの波動は、変化と進化の縁にいます。自己観察を続けることで、可能性は無限に展開します。`;
          break;
      }

      document.getElementById("result").textContent = message;
    });
  </script>
</body>
</html>
