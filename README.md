<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>中文练习 — Китайский язык</title>

<style>
:root {
--peach: #f4b99e;
--peach-dark: #c9785c;
--peach-light: #fff0e8;
--cream: #fffaf6;
--pink: #f8d9d0;
--brown: #704b40;
--text: #493a35;
--muted: #927b72;
--white: #ffffff;
--green: #6c9879;
}

* {
box-sizing: border-box;
}

html {
scroll-behavior: smooth;
}

body {
margin: 0;
background: var(--cream);
color: var(--text);
font-family: Arial, "Noto Sans SC", sans-serif;
line-height: 1.65;
}

header {
padding: 45px 20px 35px;
text-align: center;
color: white;
background: linear-gradient(135deg, #d98d70, #f2b99f, #f7d5c5);
}

header h1 {
margin: 0;
font-size: clamp(30px, 5vw, 46px);
letter-spacing: 2px;
}

header p {
margin: 8px 0 0;
font-size: 17px;
}

.header-chinese {
font-family: "Noto Serif SC", "Songti SC", serif;
font-size: 27px;
letter-spacing: 5px;
}

nav {
position: sticky;
top: 0;
z-index: 20;
display: flex;
justify-content: center;
flex-wrap: wrap;
gap: 9px;
padding: 13px;
background: #fffaf6ee;
border-bottom: 1px solid #f1d9ce;
backdrop-filter: blur(10px);
}

nav a {
padding: 8px 15px;
border-radius: 25px;
background: var(--peach-light);
color: var(--peach-dark);
text-decoration: none;
font-size: 14px;
font-weight: bold;
transition: .2s;
}

nav a:hover {
background: var(--peach);
color: white;
}

main {
width: min(1050px, 94%);
margin: 30px auto 60px;
}

section {
margin-bottom: 28px;
padding: clamp(20px, 4vw, 35px);
background: white;
border: 1px solid #f2ded5;
border-radius: 22px;
box-shadow: 0 8px 25px #a66e5410;
scroll-margin-top: 85px;
}

h2 {
margin-top: 0;
color: var(--peach-dark);
font-size: 27px;
}

h3 {
color: var(--brown);
}

.intro {
color: var(--muted);
margin-top: -5px;
}

.video-box {
width: 100%;
max-width: 760px;
margin: 22px auto;
padding: 12px;
background: var(--peach-light);
border-radius: 18px;
}

.video-box video,
.video-box iframe {
display: block;
width: 100%;
aspect-ratio: 16 / 9;
border: 0;
border-radius: 12px;
background: #302722;
}

.video-note {
padding: 10px 12px;
color: var(--muted);
font-size: 13px;
}

.video-actions {
display: flex;
flex-wrap: wrap;
gap: 10px;
align-items: center;
margin-top: 12px;
}

.video-actions input {
max-width: 100%;
}

button,
.file-label {
display: inline-block;
padding: 10px 17px;
border: 0;
border-radius: 12px;
background: var(--peach);
color: white;
font-size: 15px;
font-weight: bold;
cursor: pointer;
transition: .2s;
}

button:hover,
.file-label:hover {
background: var(--peach-dark);
}

button.secondary {
color: var(--peach-dark);
background: var(--peach-light);
}

input[type="file"] {
display: none;
}

.song {
max-width: 720px;
margin: 35px auto;
padding: 30px 20px;
text-align: center;
background: linear-gradient(145deg, #fff8f3, #fff0e8);
border: 1px solid #f4d7ca;
border-radius: 20px;
}

.song-title {
margin-bottom: 24px;
color: var(--peach-dark);
font-size: 20px;
letter-spacing: 4px;
}

.song-line {
margin: 20px 0;
}

.song-chinese {
color: #744b3d;
font-family: "Noto Serif SC", "Songti SC", serif;
font-size: clamp(24px, 4vw, 34px);
font-weight: bold;
letter-spacing: 3px;
}

.song-pinyin {
margin-top: 3px;
color: #b47d69;
font-size: 15px;
letter-spacing: 1px;
}

.translation-card {
margin-top: 20px;
padding: 20px;
background: #fff8f3;
border-radius: 15px;
}

.explanation {
display: grid;
grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
gap: 13px;
margin-top: 15px;
}

.explanation-card {
padding: 17px;
background: #fff8f3;
border: 1px solid #f4e0d7;
border-radius: 14px;
}

.explanation-card .chinese {
color: var(--peach-dark);
font-size: 23px;
font-weight: bold;
}

.explanation-card .pinyin {
color: var(--muted);
font-size: 14px;
}

.example {
padding: 12px;
margin-top: 10px;
background: white;
border-radius: 10px;
}

.flashcard-area {
max-width: 650px;
margin: 25px auto;
}

.flashcard {
display: flex;
justify-content: center;
align-items: center;
min-height: 310px;
padding: 30px;
text-align: center;
background: linear-gradient(145deg, #fff1e9, #f8d9cc);
border: 2px solid #efc2b0;
border-radius: 25px;
box-shadow: 0 10px 25px #a66e541c;
cursor: pointer;
perspective: 1000px;
user-select: none;
transition: background .25s;
}

.flashcard:hover {
background: linear-gradient(145deg, #ffe8dc, #f5cbbb);
}

.flashcard-inner {
width: 100%;
}

.flashcard-label {
color: #a87b6b;
font-size: 13px;
letter-spacing: 2px;
text-transform: uppercase;
}

.flashcard-word {
margin: 20px 0;
color: #704b40;
font-family: "Noto Serif SC", "Songti SC", serif;
font-size: clamp(48px, 9vw, 76px);
font-weight: bold;
line-height: 1.3;
}

.flashcard-pinyin {
color: #a97867;
font-size: 18px;
}

.flashcard-translation {
color: #704b40;
font-size: clamp(25px, 5vw, 36px);
font-weight: bold;
}

.flashcard-hint {
margin-top: 22px;
color: #a87b6b;
font-size: 13px;
}

.card-controls {
display: flex;
justify-content: center;
flex-wrap: wrap;
gap: 9px;
margin-top: 17px;
}

.progress {
margin: 16px auto;
color: var(--muted);
text-align: center;
}

.progress-bar {
width: 100%;
height: 9px;
overflow: hidden;
background: #f8e8e0;
border-radius: 10px;
}

.progress-fill {
height: 100%;
width: 0;
background: var(--peach-dark);
transition: width .3s;
}

.category-filter {
display: flex;
justify-content: center;
flex-wrap: wrap;
gap: 8px;
margin: 15px 0;
}

.category-filter button {
padding: 8px 13px;
font-size: 13px;
}

.category-filter button.active {
background: var(--peach-dark);
}

.word-count {
color: var(--muted);
text-align: center;
font-size: 14px;
}

footer {
padding: 30px;
color: var(--muted);
text-align: center;
}

@media(max-width: 600px) {
nav {
position: static;
}

nav a {
padding: 7px 11px;
font-size: 13px;
}

.flashcard {
min-height: 260px;
}

section {
padding: 18px;
}

.song {
padding: 23px 10px;
}
}
</style>
</head>

<body>

<header>
<div class="header-chinese">中文学习时间</div>
<h1>Китайский язык</h1>
<p>Практика произношения и повторение лексики</p>
</header>

<nav>
<a href="#speed">速度练习 · Скорость речи</a>
<a href="#vocabulary">词汇卡片 · Карточки</a>
</nav>

<main>

<!-- ПЕРВЫЙ РАЗДЕЛ -->
<section id="speed">
<h2>第一部分 · Практика скорости речи</h2>
<p class="intro">
Слушай, следи за текстом и повторяй за исполнителем.
Сначала попробуй произнести текст медленно, затем постепенно увеличивай скорость.
</p>

<h3>🎬 Видео для тренировки</h3>

<div class="video-box">

<div class="video-box">
<video id="localVideo"
controls
playsinline
webkit-playsinline
controlsList="nofullscreen"
preload="metadata">
</video>

<div class="video-actions">
<label class="file-label" for="videoFile">Выбрать видеофайл</label>
<input type="file" id="videoFile" accept="video/*">
<button class="secondary" onclick="clearVideo()">Очистить</button>
</div>
<div class="video-note">
</div>
</div>

<h3>🎵 Текст для повторения</h3>

<div class="song">
<div class="song-title">吃吃吃</div>

<div class="song-line">
<div class="song-chinese">吃吃吃　什么都吃</div>
<div class="song-pinyin">chī chī chī　shénme dōu chī</div>
</div>

<div class="song-line">
<div class="song-chinese">吃惊吃亏也要吃</div>
<div class="song-pinyin">chījīng chīkuī yě yào chī</div>
</div>

<div class="song-line">
<div class="song-chinese">想吃就吃　慢慢吃</div>
<div class="song-pinyin">xiǎng chī jiù chī　mànman chī</div>
</div>

<div class="song-line">
<div class="song-chinese">每天三餐不够吃</div>
<div class="song-pinyin">měitiān sān cān bú gòu chī</div>
</div>

<div class="song-title" style="margin-top:35px">再唱一次 · Ещё раз</div>

<div class="song-line">
<div class="song-chinese">吃吃吃　什么都吃</div>
<div class="song-pinyin">chī chī chī　shénme dōu chī</div>
</div>

<div class="song-line">
<div class="song-chinese">吃惊吃亏也要吃</div>
<div class="song-pinyin">chījīng chīkuī yě yào chī</div>
</div>

<div class="song-line">
<div class="song-chinese">想吃就吃　慢慢吃</div>
<div class="song-pinyin">xiǎng chī jiù chī　mànman chī</div>
</div>

<div class="song-line">
<div class="song-chinese">每天三餐不够吃</div>
<div class="song-pinyin">měitiān sān cān bú gòu chī</div>
</div>
</div>

<h3>📖 Общий смысл текста</h3>

<div class="translation-card">
<p>
Текст построен вокруг иероглифа 吃 — «есть».
В нём используется игра слов: выражения со словом 吃
могут обозначать не только приём пищи, но и разные жизненные ситуации.
</p>
<p>
Герой текста с юмором говорит о том, что любит есть всё подряд,
не отказывается от еды, хочет есть тогда, когда хочется,
и даже трёх приёмов пищи в день ему недостаточно.
</p>
<p>
Это шуточный текст, в котором повтор слова 吃 помогает тренировать
скорость речи, произношение и узнавание устойчивых выражений.
</p>
</div>

<h3>💡 Полезные выражения и идиомы</h3>

<div class="explanation">

<div class="explanation-card">
<div class="chinese">吃惊</div>
<div class="pinyin">chījīng</div>
<p><b>Удивляться, быть поражённым.</b></p>
<p>Буквально: «есть удивление», но это устойчивое выражение.</p>
<div class="example">
<div class="chinese">听到这个消息，我很吃惊。</div>
<div class="pinyin">Tīngdào zhège xiāoxi, wǒ hěn chījīng.</div>
<p>Услышав эту новость, я очень удивился.</p>
</div>
</div>

<div class="explanation-card">
<div class="chinese">吃亏</div>
<div class="pinyin">chīkuī</div>
<p><b>Потерпеть неудачу, оказаться в невыгодном положении, пострадать от ситуации.</b></p>
<p>Устойчивое выражение, которое не следует переводить буквально как «есть убыток».</p>
<div class="example">
<div class="chinese">不听别人的建议，自己容易吃亏。</div>
<div class="pinyin">Bù tīng biérén de jiànyì, zìjǐ róngyì chīkuī.</div>
<p>Если не слушать советы других, можно оказаться в невыгодном положении.</p>
</div>
</div>

<div class="explanation-card">
<div class="chinese">想吃就吃</div>
<div class="pinyin">xiǎng chī jiù chī</div>
<p><b>Хочешь есть — ешь.</b></p>
<p>Конструкция 想……就…… означает: «если хочешь…, то…», «делай…, когда хочешь…».</p>
<div class="example">
<div class="chinese">想去就去。</div>
<div class="pinyin">Xiǎng qù jiù qù.</div>
<p>Хочешь пойти — иди.</p>
</div>
</div>

<div class="explanation-card">
<div class="chinese">慢慢吃</div>
<div class="pinyin">mànman chī</div>
<p><b>Ешь не спеша, приятного аппетита.</b></p>
<p>慢慢 — повтор наречия 慢, который означает «медленно», «не торопясь».</p>
<div class="example">
<div class="chinese">别着急，慢慢吃。</div>
<div class="pinyin">Bié zháojí, mànman chī.</div>
<p>Не торопись, ешь спокойно.</p>
</div>
</div>

</div>

<h3>🔍 Грамматика: 什么都</h3>

<div class="translation-card">
<div class="chinese" style="font-size:28px">什么都</div>
<div class="pinyin">shénme dōu</div>
<p><b>Значение: всё, что угодно; всё без исключения.</b></p>

<p>
什么 означает «что», а 都 добавляет значение обобщения —
«всё», «все», «без исключения».
</p>

<p>
В утвердительном предложении 什么都 обычно переводится как «всё».
</p>

<div class="example">
<div class="chinese">我什么都吃。</div>
<div class="pinyin">Wǒ shénme dōu chī.</div>
<p>Я ем всё.</p>
</div>

<div class="example">
<div class="chinese">她什么都知道。</div>
<div class="pinyin">Tā shénme dōu zhīdào.</div>
<p>Она всё знает.</p>
</div>

<div class="example">
<div class="chinese">我什么都喜欢。</div>
<div class="pinyin">Wǒ shénme dōu xǐhuan.</div>
<p>Мне всё нравится.</p>
</div>

<p><b>Важно:</b> при отрицании используется конструкция 什么都不 / 什么都没.
Она означает «ничего не…».</p>

<div class="example">
<div class="chinese">我什么都不想吃。</div>
<div class="pinyin">Wǒ shénme dōu bù xiǎng chī.</div>
<p>Я совсем ничего не хочу есть.</p>
</div>

<div class="example">
<div class="chinese">他什么都不知道。</div>
<div class="pinyin">Tā shénme dōu bù zhīdào.</div>
<p>Он ничего не знает.</p>
</div>
</div>

<h3>✏️ Мини-практика</h3>

<div class="explanation-card">
<p><b>1. Выбери правильный перевод: 我什么都吃。</b></p>
<label><input type="radio" name="songq1" value="a"> Я ничего не ем.</label><br>
<label><input type="radio" name="songq1" value="b"> Я ем всё.</label><br>
<label><input type="radio" name="songq1" value="c"> Я хочу есть.</label>

<hr>

<p><b>2. Что означает 吃亏?</b></p>
<label><input type="radio" name="songq2" value="a"> Быстро есть.</label><br>
<label><input type="radio" name="songq2" value="b"> Быть удивлённым.</label><br>
<label><input type="radio" name="songq2" value="c"> Оказаться в невыгодном положении.</label>

<hr>

<p><b>3. Как перевести 什么都不想吃?</b></p>
<label><input type="radio" name="songq3" value="a"> Хочу всё съесть.</label><br>
<label><input type="radio" name="songq3" value="b"> Ничего не хочу есть.</label><br>
<label><input type="radio" name="songq3" value="c"> Ем очень медленно.</label>

<button onclick="checkSongQuiz()">Проверить ответы</button>
<p id="songFeedback" class="video-note"></p>
</div>
</section>

<!-- ВТОРОЙ РАЗДЕЛ -->
<section id="vocabulary">
<h2>第二部分 · Карточки для повторения слов</h2>
<p class="intro">
Нажми на карточку, чтобы увидеть перевод.
Сначала попробуй вспомнить значение самостоятельно.
</p>

<div class="category-filter" id="categoryFilters">
<button class="active" data-category="all">Все слова</button>
<button data-category="pronouns">Местоимения</button>
<button data-category="family">Семья</button>
<button data-category="actions">Действия</button>
<button data-category="clothes">Одежда</button>
<button data-category="colors">Цвета</button>
<button data-category="countries">Страны и языки</button>
<button data-category="adjectives">Прилагательные</button>
</div>

<div class="flashcard-area">
<div class="flashcard" id="flashcard" role="button"
tabindex="0" aria-label="Перевернуть карточку">
<div class="flashcard-inner">
<div class="flashcard-label" id="cardLabel">Китайское слово</div>
<div class="flashcard-word" id="cardWord">你好</div>
<div class="flashcard-pinyin" id="cardPinyin"></div>
<div class="flashcard-hint" id="cardHint">Нажми, чтобы увидеть перевод</div>
</div>
</div>

<div class="progress">
<div id="cardProgressText">Карточка 1 из 1</div>
<div class="progress-bar">
<div class="progress-fill" id="cardProgress"></div>
</div>
</div>

<div class="card-controls">
<button class="secondary" onclick="previousCard()">← Назад</button>
<button onclick="flipCard()">Перевернуть</button>
<button onclick="nextCard()">Следующая →</button>
</div>

<div class="card-controls">
<button class="secondary" onclick="shuffleCards()">🔀 Перемешать</button>
<button class="secondary" onclick="restartCards()">↺ Сначала</button>
</div>

<p class="word-count" id="wordCount"></p>
</div>
</section>

</main>

<footer>
中文学习时间 · Учим китайский с удовольствием
</footer>

<script>
/* ВИДЕОФАЙЛ */
const videoInput = document.getElementById("videoFile");
const localVideo = document.getElementById("localVideo");
let localVideoURL = null;

videoInput.addEventListener("change", function() {
const file = this.files[0];
if (!file) return;

if (localVideoURL) {
URL.revokeObjectURL(localVideoURL);
}

localVideoURL = URL.createObjectURL(file);
localVideo.src = localVideoURL;
localVideo.load();
});

function clearVideo() {
localVideo.pause();
localVideo.removeAttribute("src");
localVideo.load();
videoInput.value = "";

if (localVideoURL) {
URL.revokeObjectURL(localVideoURL);
localVideoURL = null;
}
}

/* ПРОВЕРКА МИНИ-ТЕСТА */
function checkSongQuiz() {
const answers = {
songq1: "b",
songq2: "c",
songq3: "b"
};

let score = 0;
let answered = 0;

Object.keys(answers).forEach(name => {
const selected = document.querySelector(
'input[name="' + name + '"]:checked'
);

if (selected) {
answered++;
if (selected.value === answers[name]) score++;
}
});

const feedback = document.getElementById("songFeedback");

if (answered < 3) {
feedback.textContent = "Ответь на все три вопроса.";
return;
}

feedback.textContent = "Правильных ответов: " + score + " из 3.";
}

/* СЛОВАРЬ КАРТОЧЕК */
const vocabulary = [
// МЕСТОИМЕНИЯ
{word:"你", pinyin:"nǐ", translation:"ты", category:"pronouns"},
{word:"你们", pinyin:"nǐmen", translation:"вы", category:"pronouns"},
{word:"我", pinyin:"wǒ", translation:"я", category:"pronouns"},
{word:"我们", pinyin:"wǒmen", translation:"мы", category:"pronouns"},
{word:"她", pinyin:"tā", translation:"она", category:"pronouns"},
{word:"他", pinyin:"tā", translation:"он", category:"pronouns"},
{word:"他们", pinyin:"tāmen", translation:"они (мужчины или смешанная группа)", category:"pronouns"},
{word:"您", pinyin:"nín", translation:"Вы (вежливая форма)", category:"pronouns"},

// СЕМЬЯ
{word:"妈妈", pinyin:"māma", translation:"мама", category:"family"},
{word:"爸爸", pinyin:"bàba", translation:"папа", category:"family"},
{word:"奶奶", pinyin:"nǎinai", translation:"бабушка по отцу", category:"family"},
{word:"爷爷", pinyin:"yéye", translation:"дедушка по отцу", category:"family"},
{word:"老婆", pinyin:"lǎopo", translation:"жена (разговорное)", category:"family"},
{word:"老公", pinyin:"lǎogōng", translation:"муж (разговорное)", category:"family"},
{word:"姐姐", pinyin:"jiějie", translation:"старшая сестра", category:"family"},
{word:"妹妹", pinyin:"mèimei", translation:"младшая сестра", category:"family"},
{word:"哥哥", pinyin:"gēge", translation:"старший брат", category:"family"},
{word:"弟弟", pinyin:"dìdi", translation:"младший брат", category:"family"},

// ДЕЙСТВИЯ
{word:"做作业", pinyin:"zuò zuòyè", translation:"делать домашнее задание", category:"actions"},
{word:"看书", pinyin:"kàn shū", translation:"читать книгу", category:"actions"},
{word:"看电视", pinyin:"kàn diànshì", translation:"смотреть телевизор", category:"actions"},
{word:"看电影", pinyin:"kàn diànyǐng", translation:"смотреть фильм", category:"actions"},
{word:"起床", pinyin:"qǐchuáng", translation:"вставать с кровати", category:"actions"},
{word:"睡觉", pinyin:"shuìjiào", translation:"спать, ложиться спать", category:"actions"},
{word:"游泳", pinyin:"yóuyǒng", translation:"плавать", category:"actions"},
{word:"跑步", pinyin:"pǎobù", translation:"бегать", category:"actions"},
{word:"做饭", pinyin:"zuò fàn", translation:"готовить еду", category:"actions"},
{word:"做运动", pinyin:"zuò yùndòng", translation:"заниматься спортом", category:"actions"},
{word:"上学", pinyin:"shàngxué", translation:"ходить в школу / на учёбу", category:"actions"},
{word:"放学", pinyin:"fàngxué", translation:"заканчивать занятия", category:"actions"},
{word:"休息", pinyin:"xiūxi", translation:"отдыхать", category:"actions"},
{word:"散步", pinyin:"sànbù", translation:"гулять пешком", category:"actions"},
{word:"学习汉语", pinyin:"xuéxí Hànyǔ", translation:"учить китайский язык", category:"actions"},
{word:"写汉字", pinyin:"xiě Hànzì", translation:"писать китайские иероглифы", category:"actions"},
{word:"吃早饭", pinyin:"chī zǎofàn", translation:"завтракать", category:"actions"},
{word:"刷手机", pinyin:"shuā shǒujī", translation:"листать телефон", category:"actions"},
{word:"晚饭", pinyin:"wǎnfàn", translation:"ужин", category:"actions"},

// ОДЕЖДА
{word:"穿上", pinyin:"chuān shàng", translation:"надеть (одежду, обувь)", category:"clothes"},
{word:"脱掉", pinyin:"tuō diào", translation:"снять (одежду, обувь)", category:"clothes"},
{word:"T恤", pinyin:"T-xù", translation:"футболка", category:"clothes"},
{word:"鞋子", pinyin:"xiézi", translation:"обувь, туфли", category:"clothes"},
{word:"包", pinyin:"bāo", translation:"сумка", category:"clothes"},
{word:"外套", pinyin:"wàitào", translation:"верхняя одежда, куртка", category:"clothes"},
{word:"毛衣", pinyin:"máoyī", translation:"свитер", category:"clothes"},
{word:"围巾", pinyin:"wéijīn", translation:"шарф", category:"clothes"},
{word:"短裤", pinyin:"duǎnkù", translation:"шорты", category:"clothes"},
{word:"裤子", pinyin:"kùzi", translation:"брюки, штаны", category:"clothes"},
{word:"牛仔裤", pinyin:"niúzǎikù", translation:"джинсы", category:"clothes"},
{word:"衬衫", pinyin:"chènshān", translation:"рубашка", category:"clothes"},
{word:"连衣裙", pinyin:"liányīqún", translation:"платье", category:"clothes"},
{word:"裙子", pinyin:"qúnzi", translation:"юбка", category:"clothes"},

// ЦВЕТА
{word:"灰色", pinyin:"huīsè", translation:"серый цвет", category:"colors"},
{word:"红色", pinyin:"hóngsè", translation:"красный цвет", category:"colors"},
{word:"黄色", pinyin:"huángsè", translation:"жёлтый цвет", category:"colors"},
{word:"绿色", pinyin:"lǜsè", translation:"зелёный цвет", category:"colors"},
{word:"蓝色", pinyin:"lánsè", translation:"синий цвет", category:"colors"},
{word:"白色", pinyin:"báisè", translation:"белый цвет", category:"colors"},
{word:"黑色", pinyin:"hēisè", translation:"чёрный цвет", category:"colors"},
{word:"棕色", pinyin:"zōngsè", translation:"коричневый цвет", category:"colors"},
{word:"紫色", pinyin:"zǐsè", translation:"фиолетовый цвет", category:"colors"},
{word:"粉红色", pinyin:"fěnhóngsè", translation:"розовый цвет", category:"colors"},
{word:"橙色", pinyin:"chéngsè", translation:"оранжевый цвет", category:"colors"},

// СТРАНЫ И ЯЗЫКИ
{word:"中国", pinyin:"Zhōngguó", translation:"Китай", category:"countries"},
{word:"中文", pinyin:"Zhōngwén", translation:"китайский язык", category:"countries"},
{word:"日本", pinyin:"Rìběn", translation:"Япония", category:"countries"},
{word:"英国", pinyin:"Yīngguó", translation:"Великобритания", category:"countries"},
{word:"美国", pinyin:"Měiguó", translation:"США, Америка", category:"countries"},
{word:"德国", pinyin:"Déguó", translation:"Германия", category:"countries"},
{word:"法国", pinyin:"Fǎguó", translation:"Франция", category:"countries"},
{word:"俄罗斯", pinyin:"Éluósī", translation:"Россия", category:"countries"},

// ПРИЛАГАТЕЛЬНЫЕ
{word:"开心", pinyin:"kāixīn", translation:"радостный, счастливый", category:"adjectives"},
{word:"漂亮", pinyin:"piàoliang", translation:"красивый", category:"adjectives"},
{word:"忙", pinyin:"máng", translation:"занятый", category:"adjectives"},
{word:"累", pinyin:"lèi", translation:"уставший", category:"adjectives"},
{word:"好吃", pinyin:"hǎochī", translation:"вкусный (о еде)", category:"adjectives"},
{word:"好喝", pinyin:"hǎohē", translation:"вкусный (о напитке)", category:"adjectives"}
];

/* ПЕРЕМЕШИВАНИЕ */
function shuffleArray(array) {
const copy = [...array];

for (let i = copy.length - 1; i > 0; i--) {
const j = Math.floor(Math.random() * (i + 1));
[copy[i], copy[j]] = [copy[j], copy[i]];
}

return copy;
}

let activeCategory = "all";
let cards = shuffleArray(vocabulary);
let currentIndex = 0;
let isFlipped = false;

const flashcard = document.getElementById("flashcard");
const cardWord = document.getElementById("cardWord");
const cardPinyin = document.getElementById("cardPinyin");
const cardLabel = document.getElementById("cardLabel");
const cardHint = document.getElementById("cardHint");

function getFilteredCards() {
if (activeCategory === "all") return cards;
return cards.filter(card => card.category === activeCategory);
}

function renderCard() {
const filtered = getFilteredCards();

if (filtered.length === 0) return;

if (currentIndex >= filtered.length) currentIndex = 0;
if (currentIndex < 0) currentIndex = filtered.length - 1;

const card = filtered[currentIndex];

isFlipped = false;
cardLabel.textContent = "Китайское слово";
cardWord.textContent = card.word;
cardPinyin.textContent = card.pinyin;
cardHint.textContent = "Нажми, чтобы увидеть перевод";

document.getElementById("cardProgressText").textContent =
"Карточка " + (currentIndex + 1) + " из " + filtered.length;

document.getElementById("cardProgress").style.width =
((currentIndex + 1) / filtered.length * 100) + "%";

document.getElementById("wordCount").textContent =
"Всего слов в выбранной категории: " + filtered.length;
}

function flipCard() {
const filtered = getFilteredCards();
if (!filtered.length) return;

const card = filtered[currentIndex];

if (!isFlipped) {
cardLabel.textContent = "Перевод";
cardWord.textContent = card.translation;
cardPinyin.textContent = "";
cardHint.textContent = "Нажми ещё раз, чтобы вернуться к иероглифу";
cardWord.className = "flashcard-translation";
isFlipped = true;
} else {
cardWord.className = "flashcard-word";
renderCard();
}
}

function nextCard() {
const filtered = getFilteredCards();
currentIndex = (currentIndex + 1) % filtered.length;
renderCard();
}

function previousCard() {
const filtered = getFilteredCards();
currentIndex = (currentIndex - 1 + filtered.length) % filtered.length;
renderCard();
}

function shuffleCards() {
cards = shuffleArray(cards);
currentIndex = 0;
renderCard();
}

function restartCards() {
currentIndex = 0;
renderCard();
}

flashcard.addEventListener("click", flipCard);

flashcard.addEventListener("keydown", function(event) {
if (event.key === "Enter" || event.key === " ") {
event.preventDefault();
flipCard();
}
});

/* ФИЛЬТРЫ */
document.querySelectorAll("#categoryFilters button").forEach(button => {
button.addEventListener("click", function() {
document.querySelectorAll("#categoryFilters button")
.forEach(item => item.classList.remove("active"));

this.classList.add("active");
activeCategory = this.dataset.category;
currentIndex = 0;
renderCard();
});
});

/* ПЕРВЫЙ ПОКАЗ */
renderCard();
</script>

</body>
</html>

