# index.html
<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <title>جاري الاختراق...</title>
  <style>
    body {
      margin: 0;
      background-color: black;
      color: lime;
      font-family: monospace;
      font-size: 1.5em;
      text-align: center;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      flex-direction: column;
    }
    .hidden {
      display: none;
    }
  </style>
</head>
<body>
  <div id="msg1">🔐 جاري اختراق جهازك...</div>
  <div id="msg2" class="hidden">💣 حذف جميع ملفاتك...</div>
  <div id="msg3" class="hidden">🔥 تم تعطيل النظام...</div>
  <div id="final" class="hidden" style="color: red;">😂 عليه ياقواد
  <audio id="sound" src="https://www.myinstants.com/media/sounds/windows-error.mp3" autoplay></audio>

  <script>
    setTimeout(() => {
      document.getElementById('msg2').classList.remove('hidden');
    }, 2000);
    setTimeout(() => {
      document.getElementById('msg3').classList.remove('hidden');
    }, 4000);
    setTimeout(() => {
      document.getElementById('msg1').classList.add('hidden');
      document.getElementById('msg2').classList.add('hidden');
      document.getElementById('msg3').classList.add('hidden');
      document.getElementById('final').classList.remove('hidden');
    }, 6000);
  </script>
</body>
</html>
