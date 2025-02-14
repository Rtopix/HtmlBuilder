<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HTML Builder</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    html, body { width: 100%; height: 100%; overflow-x: hidden; overscroll-behavior: none; transition: background 0.3s ease; }
    body { font-family: 'Poppins', sans-serif; color: #444; display: flex; flex-direction: column; align-items: center; justify-content: center; padding: 20px; transition: color 0.3s ease, background 0.3s ease; overflow-y: scroll; }
    h1 { font-size: 2.5rem; font-weight: 700; margin-bottom: 20px; color: #5e6b73; transition: color 0.3s ease; }
    p { font-size: 1.1rem; line-height: 1.6; margin: 10px 0; color: #666; }
    button, select, input[type="text"] {
      background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%);
      color: white;
      padding: 12px 24px;
      font-size: 1.1rem;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: all 0.3s ease;
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
    }
    button:hover, select:hover, input[type="text"]:hover {
      background: linear-gradient(135deg, #2575fc 0%, #6a11cb 100%);
      transform: translateY(-3px);
    }
#newBTN {

}

    button:active, select:active, input[type="text"]:active { transform: translateY(0); }
    .toolbar { display: flex; flex-wrap: wrap; gap: 15px; justify-content: center; margin-bottom: 30px; transition: opacity 0.3s ease; }
    .workspace { width: 100%; max-width: 900px; padding: 20px; background-color: #fff; border-radius: 15px; box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1); min-height: 200px; overflow-y: auto; position: relative; transition: background-color 0.3s ease; text-align: center; }
    .workspace img { max-width: 100%; height: auto; border-radius: 5px; margin-bottom: 15px; box-shadow: 0 4px 6px rgba(0,0,0,0.1); transition: transform 0.3s ease; }
    .workspace img:hover { transform: scale(1.05); }
    input[type="text"] { width: 100%; padding: 12px; border-radius: 10px; border: 1px solid #ddd; margin-bottom: 15px; font-size: 1rem; transition: border-color 0.3s ease; }
    input[type="text"]:focus { border-color: #2575fc; outline: none; }
    .btn-container { width: 100%; max-width: 300px; margin-top: 15px; }
    #desktopWarning { display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0, 0, 0, 0.8); color: white; text-align: center; flex-direction: column; justify-content: center; align-items: center; z-index: 9999; transition: opacity 0.3s ease; }
    #desktopWarning a { color: #fff; text-decoration: underline; font-weight: bold; }

    body.light-theme { background: #f5f7fb; color: #444; }
    .workspace.light-theme { background-color: #fff; }
    .toolbar.light-theme { opacity: 1; }
    button.light-theme, select.light-theme, input[type="text"].light-theme { background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%); color: white; }

    body.dark-theme { background: #121212; color: #f5f5f5; }
    .workspace.dark-theme { background-color: #1c1c1c; box-shadow: 0 10px 30px rgba(255, 255, 255, 0.2); }
    .toolbar.dark-theme { opacity: 0.9; }
    button.dark-theme, select.dark-theme, input[type="text"].dark-theme { background: linear-gradient(135deg, #f39c12 0%, #e74c3c 100%); color: white; }
    button.dark-theme:hover, select.dark-theme:hover, input[type="text"].dark-theme:hover { background: linear-gradient(135deg, #e74c3c 0%, #f39c12 100%); }

    @media (max-width: 768px) { .workspace { width: 100%; } }

    .menu { position: absolute; left: 20px; top: 20px; z-index: 100; cursor: pointer; transition: transform 0.3s ease; }
    .menu-bar { width: 25px; height: 3px; background-color: #444; margin: 5px 0; transition: 0.3s ease; }
    .menu-content { position: fixed; top: 0; left: 0; width: 250px; height: 100%; background-color: #fff; padding: 20px; box-shadow: 4px 0px 10px rgba(0, 0, 0, 0.3); display: none; flex-direction: column; gap: 20px; transition: transform 0.3s ease, opacity 0.3s ease; opacity: 0; justify-content: center; align-items: center; }
    .menu-content.active { display: flex; transform: translateX(0); opacity: 1; }
    .menu-content a, .menu-content button { font-size: 1.2rem; color: #2575fc; text-decoration: none; padding: 10px 0; background: none; border: none; text-align: center; cursor: pointer; transition: all 0.3s ease; }
    .menu-content a:hover, .menu-content button:hover { color: #fff; background-color: #2575fc; }

    .menu.open .menu-bar:nth-child(1) { transform: rotate(-45deg) translate(-5px, 6px); }
    .menu.open .menu-bar:nth-child(2) { opacity: 0; }
    .menu.open .menu-bar:nth-child(3) { transform: rotate(45deg) translate(-5px, -6px); }

    .workspace {
      overflow-y: visible;
      text-align: center;
    }

    body.menu-open .workspace {
      opacity: 0.2;
    }

    .toolbar button {
      opacity: 0;
      animation: fadeIn 0.5s forwards;
    }

    .toolbar button:nth-child(1) { animation-delay: 0.2s; }
    .toolbar button:nth-child(2) { animation-delay: 0.4s; }
    .toolbar button:nth-child(3) { animation-delay: 0.6s; }
    .toolbar button:nth-child(4) { animation-delay: 0.8s; }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    .fade-in { animation: fadeIn 0.5s ease-in; }
    .fade-out { animation: fadeOut 0.5s ease-out; }

    @keyframes fadeOut {
      from { opacity: 1; }
      to { opacity: 0; }
    }



  </style>
  <script>
    document.addEventListener("DOMContentLoaded", function(){
      if(window.innerWidth > 768){
        document.getElementById('desktopWarning').style.display = 'flex';
        document.getElementById('mainContent').style.display = 'none';
      }
      
      const savedTheme = localStorage.getItem('theme') || 'light';
      document.body.classList.add(savedTheme + '-theme');
    });

    function toggleTheme() {
      const currentTheme = document.body.classList.contains('light-theme') ? 'light' : 'dark';
      const newTheme = currentTheme === 'light' ? 'dark' : 'light';

      document.body.classList.remove(currentTheme + '-theme');
      document.body.classList.add(newTheme + '-theme');
      localStorage.setItem('theme', newTheme);
    }

    function toggleMenu() {
      const menu = document.querySelector('.menu');
      const menuContent = document.querySelector('.menu-content');
      menu.classList.toggle('open');
      menuContent.classList.toggle('active');
      document.body.classList.toggle('menu-open');
    }

    function closeBuilder() {
      document.getElementById('builder').classList.add('fade-out');
      setTimeout(() => {
        document.getElementById('builder').style.display = 'none';
        document.getElementById('homePage').style.display = 'block';
        document.getElementById('homePage').classList.add('fade-in');
        document.querySelector('.menu').style.display = 'block';
        toggleMenu();
      }, 500);
    }

    function openBuilder() {
  document.querySelector('.menu').classList.remove('open');
  document.querySelector('.menu-content').classList.remove('active'); 
  document.body.classList.remove('menu-open'); 

  document.getElementById('homePage').classList.add('fade-out');
  setTimeout(() => {
    document.getElementById('homePage').style.display = 'none';
    document.getElementById('builder').style.display = 'block';
    document.getElementById('builder').classList.add('fade-in');
    document.querySelector('.menu').style.display = 'none';
  }, 500);
}

function addPodtext() {
const textx = prompt("Введите текст для добавления:");
var cl = prompt("Введите цвет текста. HEХ или словом (к примеру: #123456 - hex, black - словом). Обычно у подтекстов цвет #979797");
var size = prompt("Введите размер шрифта в px");
var align = prompt("Введите позицию. center / left / right");
var fontw = prompt("Введите жирность шрифта");
var mb = prompt("Введите отступ в px");
if (textx) {
        const newPod = document.createElement("p");
        newPod.id = "newPODText";
        newPod.textContent = textx;
      newPod.style.marginTop = mb + "px";
     newPod.style.fontSize = size + "px";
     newPod.style.textAlign = align;
     newPod.style.fontWeight = fontw;
    newPod.style.color = cl;

document.getElementById('workspace').appendChild(newPod);
      }
    }


    function addText() {
      const text = prompt("Введите текст для добавления:");
  var cl = prompt("Введите цвет текста. HEХ или словом (к примеру: #123456 - hex, black - словом)");
var size = prompt("Введите размер шрифта в px")
var align = prompt("Введите позицию. center / left / right")
var fontw = prompt("Введите жирность шрифта")
var mb = prompt("Введите отступ в px");


      if (text) {
        const newText = document.createElement('p');
        newText.id = "newTEXT";
        newText.textContent = text;
        newText.style.marginTop = mb + "px";
     newText.style.fontSize = size + "px";
     newText.style.textAlign = align;
     newText.style.fontWeight = fontw;

    newText.style.color = cl;
     document.getElementById('workspace').appendChild(newText);
      }
    }

    function addImage() {
      const imgURL = prompt("Введите URL изображения:");
var widthZ = prompt("Введите ширину в px!");
var heightZ = prompt("Введите толщину в px!");
var br = prompt("Введите округление в px!")
      if (imgURL) {
        const newImage = document.createElement('img');
        newImage.src = imgURL;
        newImage.alt = 'Image';
        newImage.style.width = widthZ + "px";
        newImage.style.height = heightZ + "px";
        newImage.style.borderRadius = br + "px";
        newImage.style.marginBottom = '15px';
        document.getElementById('workspace').appendChild(newImage);
      }
    }

function addBtn() {
    const yourText = prompt("Введите название");
    const buttonText = prompt("Введите текст который будет в кнопке");
    var cl = prompt("Введите цвет текста в кнопке. HEХ или словом (к примеру: #123456 - hex, black - словом)");
    var widthZ = prompt("Введите ширину в px!");
    var heightZ = prompt("Введите толщину в px!");
    var fsize = prompt("Введите размер текста внутри кнопки в px.");
    var align = prompt("Введите позицию текста в кнопке (center / left / right)");
    var link = prompt("Введите ссылку");
var fw = prompt("Введите жирность шрифта")

    if (buttonText) {
        const az = document.createElement('a');
        az.setAttribute('href', link);

        const newButton = document.createElement('button');
        newButton.id = "newBTN";
        newButton.textContent = buttonText;
        newButton.style.width = widthZ + 'px';
        newButton.style.height = heightZ + 'px';
        newButton.style.fontSize = fsize + 'px';
        newButton.style.textAlign = align;
        newButton.style.color = cl;
        newButton.style.fontWeight = fw;
        newButton.style.marginBottom = '15px';

        az.appendChild(newButton); 
        document.getElementById('workspace').appendChild(az); 
    }
}

    function clearWorkspace() {
      document.getElementById('workspace').innerHTML = '';
    }

    function changeBackgroundColor() {
      const color = document.getElementById('bck').value;
      document.getElementById('workspace').style.backgroundColor = color;
    }

    function changeTextColor() {
      const color = document.getElementById('col').value;
      document.getElementById('newTEXT').style.color = color;
    }

    function saveHTML() {
      const workspaceContent = document.getElementById('workspace').innerHTML;
      const fullHTML = `
        <!DOCTYPE html>
        <html lang="ru">
        <head>
          <meta charset="UTF-8">
          <meta name="viewport" content="width=device-width, initial-scale=1.0">
          <title>By HTMLbuilder. t.me/ipabuilder</title>
          <style>
            body { font-family: 'Poppins', sans-serif; color: ${document.getElementById('workspace').style.color}; background-color: ${document.getElementById('workspace').style.backgroundColor}; padding: 20px; }
            img { max-width: 100%; height: auto; border-radius: 5px; margin-bottom: 15px; }
            button { background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%); color: white; padding: 12px 24px; font-size: 1.1rem; border: none; border-radius: 10px; cursor: pointer; margin-bottom: 15px; }
          </style>
        </head>
        <body>
          ${workspaceContent}
        </body>
        </html>
      `;
      navigator.clipboard.writeText(fullHTML).then(() => {
        alert("t.me/ipabuilder");
        alert('HTML-код успешно скопирован в буфер обмена!');
      }).catch(() => {
        alert('Не удалось скопировать HTML-код. Пожалуйста, скопируйте его вручную.');
      });
    }
  </script>
</head>
<body>
  <div id="desktopWarning">
    <h1>Сайт на ПК будет доступен позже</h1>
    <p>Перейдите в наш Telegram-канал.</p>
    <a href="https://t.me/ipabuilder" target="_blank">Перейти в Telegram</a>
  </div>

  <div id="mainContent">
    <div class="menu" onclick="toggleMenu()">
      <div class="menu-bar"></div>
      <div class="menu-bar"></div>
      <div class="menu-bar"></div>
    </div>

    <div class="menu-content">
      <button onclick="toggleTheme()">Переключить тему</button>
      <a href="https://t.me/ipabuilder" target="_blank">Открыть Telegram</a>
    </div>

    <div id="homePage">
      <h1>Добро пожаловать в HTML Builder</h1>
      <p>Создайте свой сайт: добавляйте текст, изображения, кнопки и меняйте их стиль.</p>
      <div class="btn-container">
        <button onclick="openBuilder()">Открыть редактор</button>
      </div>
    </div>

    <div id="builder" style="display:none;">
<h1>
HTMLBuilder
</h1>
      <div class="toolbar">
        <button onclick="addText()">Добавить текст</button>
        <button onclick="addPodtext()">Добавить подтекст</button>
        <button onclick="addImage()">Добавить изображение</button>
        <button onclick="addBtn()">Добавить кнопку</button>
        <button onclick="clearWorkspace()">Очистить</button>
 <input type="color" id="bck" onchange="changeBackgroundColor()" value="#ffffff">
<h>

</h>

         


      </div>
      <div class="workspace" id="workspace">

   


      </div>





      <div class="btn-container">

        <button onclick="saveHTML()">Сохранить HTML</button>
<p>
</p>
        <button onclick="closeBuilder()">Закрыть редактор</button>

      </div>
    </div>
  </div>

<script>
function tutorials() {
window.open("https://t.me/htmlbuilder_tutorials");
}
    function hhh() {
      let select = document.getElementById('colb');
      var body = document.getElementById('newBTN');

      select.addEventListener('change', (event) => {
        let color = event.target.value;
        body.style.width = color || '150px';
      });
    }

    function hh() {
      let select = document.getElementById('colbb');
      var body = document.getElementById('newTEXT');

      select.addEventListener('change', (event) => {
        let color = event.target.value;
        body.style.fontSize = color || '15px';
      });
    }

 function h() {
      let select = document.getElementById('pos');
      var body = document.getElementById('workspace');

      select.addEventListener('change', (event) => {
        let color = event.target.value;
        body.style.textAlign = color || 'center';
      });
    }

 function hz() {
      let select = document.getElementById('colbbb');
      var body = document.getElementById('newBTN');

      select.addEventListener('change', (event) => {
        let color = event.target.value;
        body.style.height = color || 'center';
      });
    }

 function hzz() {
      let select = document.getElementById('colbbbb');
      var body = document.getElementById('newBTN');

      select.addEventListener('change', (event) => {
        let color = event.target.value;
        body.style.fontSize = color || '15px';
      });
    }

 function hzzz() {
      let select = document.getElementById('colbbbbb');
      var body = document.getElementById('newBTN');

      select.addEventListener('change', (event) => {
        let color = event.target.value;
        body.style.textAlign = color || '15px';
      });
    }
</script>
</body>
</html>
