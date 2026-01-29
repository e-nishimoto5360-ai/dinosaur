<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <title>きょうりゅうってなに？</title>
  <style>
    body {
      margin: 0;
      font-family: "Rounded Mplus 1c", "Hiragino Maru Gothic ProN", Arial, sans-serif;
      background-color: #d6dce0;
      color: #333;
    }

    /* 背景（スクロールでゆっくり動く） */
    .bg {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 120%;
      background-image: url("dinosaur_bg.png");
      background-repeat: no-repeat;
      background-position: center top;
      background-size: cover;
      z-index: -1;
      transform: translateY(0);
    }

    header {
      text-align: center;
      padding: 50px 20px;
    }

    header h1 {
      background: rgba(255, 255, 255, 0.85);
      display: inline-block;
      padding: 18px 32px;
      border-radius: 22px;
    }

    section {
      max-width: 900px;
      margin: 40px auto;
      background: rgba(255, 255, 255, 0.9);
      border-radius: 22px;
      padding: 28px;
      box-shadow: 0 6px 10px rgba(0,0,0,0.1);
    }

    h2 {
      color: #4f6f7a;
    }

    .highlight {
      background-color: #eef4f6;
      border-left: 6px solid #7fa5b0;
      padding: 12px;
      border-radius: 8px;
      margin: 15px 0;
    }

    footer {
      text-align: center;
      padding: 20px;
      font-size: 0.9em;
      background: rgba(255,255,255,0.7);
    }
  </style>
</head>
<body>

  <div class="bg" id="bg"></div>

  <header>
    <h1>きょうりゅうってなに？</h1>
  </header>

  <section>
    <h2>きょうりゅうの しょうたい</h2>
    <p>
      恐竜（きょうりゅう）は、今からとてもむかし、
      地球の上でくらしていた大きなは虫類のなかまです。
    </p>
    <div class="highlight">
      約2億3000万年前から、長いあいだ地球の主役でした。
    </div>
  </section>

  <section>
    <h2>どんな しゅるいが いるの？</h2>
    <p>
      草を食べる恐竜や、肉を食べる恐竜、
      とても大きいものや、鳥のように小さいものもいました。
    </p>
  </section>

  <section>
    <h2>どうして 化石が 見つかるの？</h2>
    <p>
      恐竜が死んだあと、土や砂にうもれて、
      長い時間をかけて骨が石のように変わり、化石になりました。
    </p>
  </section>

  <section>
    <h2>どうして いなくなったの？</h2>
    <p>
      大きな隕石（いんせき）が地球にぶつかったことなどで、
      環境が急に変わり、多くの恐竜が絶滅したと考えられています。
    </p>
  </section>

  <footer>
    きょうりゅう学習サイト
  </footer>

  <script>
    const bg = document.getElementById("bg");
    window.addEventListener("scroll", () => {
      bg.style.transform = `translateY(${window.scrollY * 0.3}px)`;
    });
  </script>

