<!doctype html>
<html lang="ru">
<head>
<meta charset="utf-8">
<meta content="width=device-width, initial-scale=1" name="viewport">
<title>Запись на тренировку — Мир тенниса</title>
<link rel="stylesheet" href="./css/my.css">
</head>
<body>
<div class="container">
<header><h5>Мир тенниса 🎾</h5></header>
<nav><ul><li><a href="./index.html">Главная</a></li>
<li><a class="active" aria-current="page" href="./form.html">Запись на тренировку</a></li>
<li><a href="./shop.html">Теннисный магазин</a></li>
<li><a href="./program.html">Образовательная программа</a></li></ul></nav>
<main><h5 id="top_of_page">Запись на тренировку</h5>
<a href="#section_1">На раздел 1</a> <a href="#section_2">На раздел 2</a>
<h6 id="section_1">Раздел 1. Анкета</h6>
<p>Заполните форму для записи на пробную тренировку.</p>
<form action="https://www.bing.com/search" method="get" target="_blank" onsubmit="return sendForm()">
<input type="hidden" name="q" id="search_query">
<label>Ваше имя <input type="text" name="student_name" value="Мария" required></label>
<label>Ваш возраст <input type="number" name="student_age" min="5" max="100" value="19" required></label>
<label>Электронная почта <input type="email" name="student_email" value="mglebedeva@edu.hse.ru" required></label>
<p>Уровень игры:</p>
<label><input type="radio" name="tennis_level" value="beginner" checked> Начинающий</label>
<label><input type="radio" name="tennis_level" value="experienced"> Есть опыт</label>
<button type="submit">Отправить</button>
</form>
<a href="#top_of_page">К началу страницы</a>
<h6 id="section_2">Раздел 2. О занятиях</h6>
<p>Для первой тренировки возьмите удобную спортивную одежду, кроссовки и воду. Инвентарь можно выбрать в разделе «Теннисный магазин».</p>
<a href="#top_of_page">К началу страницы</a></main>
<footer><p>© 2026 Мир тенниса · Лебедева Мария Георгиевна · БЮРЦЮ252</p></footer>
</div>

<script>
function sendForm() {
  let name = document.querySelector('[name="student_name"]').value;
  let age = document.querySelector('[name="student_age"]').value;
  let email = document.querySelector('[name="student_email"]').value;
  let level = document.querySelector('[name="tennis_level"]:checked').value;
  document.getElementById('search_query').value = name + ' ' + age + ' ' + email + ' ' + level;
  return true;
}
</script>
</body>
</html>