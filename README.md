<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Моё расширенное портфолио</title>
<!-- Подключение шрифтов Google -->
<link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet" />
<style>
  /* Общие стили */
  body {
    margin: 0;
    font-family: 'Roboto', sans-serif;
    background-color: #f4f4f4;
    color: #333;
  }

  /* Хедер */
  header {
    background-color: #222;
    color: #fff;
    padding: 30px 20px;
    text-align: center;
    position: relative;
  }

  header h1 {
    margin: 0;
    font-size: 2.5em;
  }

  /* Навигация */
  nav {
    display: flex;
    justify-content: center;
    background-color: #444;
    position: sticky;
    top: 0;
    z-index: 1000;
  }

  nav a {
    color: #fff;
    padding: 14px 20px;
    text-decoration: none;
    transition: background-color 0.3s;
  }

  nav a:hover {
    background-color: #555;
  }

  /* Разделы */
section {
    padding: 60px 20px;
    max-width: 1200px;
    margin: auto;
}

h2 {
    font-size: 2em;
    margin-bottom: 20px;
    border-bottom: 2px solid #ccc;
    padding-bottom:10px;
}

/* О себе */
.about {
    display:flex;
    flex-wrap: wrap;
    align-items:center;
}
.about-img {
    flex:1; 
    min-width:250px; 
}
.about-img img {
    width:100%;
    border-radius:10px; 
}
.about-text {
    flex:2; 
    padding-left:20px; 
}
.about-text p {
   line-height:1.6; 
}

/* Галерея проектов */
.projects-grid {
   display:grid; 
   grid-template-columns:minmax(250px,1fr) minmax(250px,1fr);
   gap:20px; 
}
.project-card {
   background:#fff; 
   border-radius:10px; 
   overflow:hidden; 
   box-shadow:0 4px 8px rgba(0,0,0,0.1); 
   transition:.3s transform; 
}
.project-card:hover {
   transform : translateY(-5px); 
}
.project-card img {
   width :100%; 
   display:block; 
}
.project-info {
   padding :15px; 
}

/* Контактная форма */
.contact-form {
   display:flex; 
   flex-direction :column; 
}
.contact-form input,
.contact-form textarea {
   padding :10px; 
   margin-bottom :15px; 
   border-radius :5px; 
   border :1px solid #ccc; 
}
.contact-form button {
   padding :12px; 
   background-color:#222; 
   color:#fff; 
   border:none; 
   border-radius :5px; 
   cursor:pointer; 
}
.contact-form button:hover{
background:#555;}
/* Анимации при прокрутке */
@keyframes fadeInUp {
 from {opacity:.3; transform : translateY(20px);}
 to {opacity :1 ; transform : translateY(0);}
}

.animate-fadeInUp{
 animation : fadeInUp .8s forwards ;
 opacity:.3 ;
}

/* Адаптивность */
@media(max-width :768px){
 header h1{
     font-size :2em;}
 .about{
     flex-direction :column;}
 .about-img,
 .about-text{
     flex :none ;
     width :'100%';}
 .projects-grid{
     grid-template-columns :1fr;}
}

</style>
</head>
<body>

<header>
<h1>Моё расширенное портфолио</h1>
</header>

<nav>
<a href="#about">О себе</a>
<a href="#projects">Работы</a>
<a href="#gallery">Галерея</a>
<a href="#contact">Контакты</a>
</nav>

<!-- О себе -->
<section id="about" class="about animate-fadeInUp">
<div class="about-img">
<img src="https://via.placeholder.com/400x300?text=О+себе" alt="Об изображении" />
</div>
<div class="about-text">
<p>Здравствуйте! Я — веб-разработчик и дизайнер с опытом создания современных сайтов и приложений. Люблю делать интерфейсы удобными и красивыми.</p>
<p>Обладаю навыками в HTML, CSS, JavaScript и популярных фреймворках. Постоянно учусь новому и развиваюсь в сфере IT.</p>
</div>
</section>

<!-- Мои работы -->
<section id="projects" class="projects animate-fadeInUp">
<h2>Мои работы</h2>
<div class="projects-grid">
<div class="project-card">
<img src="https://via.placeholder.com/400x200?text=Проект+1" alt="Проект 1" />
<div class="project-info">
<h3>Веб-сайт для бизнеса</h3>
<p>Современный сайт для компании с адаптивным дизайном и интеграцией с соцсетями.</p>
</div>
</div>

<div class="project-card">
<img src="https://via.placeholder.com/400x200?text=Проект+2" alt="Проект 2" />
<div class="project-info">
<h3>Личный блог</h3>
<p>Интерактивный блог с комментариями и системой управления контентом.</p>
</div>
</div>

<div class="project-card">
<img src="https://via.placeholder.com/400x200?text=Проект+3" alt="Проект 3" />
<div class="project-info">
<h3>Портфолио сайт</h3>
<p>Стильный сайт для демонстрации своих работ и навыков.</p>
</div>
</div>

<!-- Добавьте свои проекты сюда -->
</div>
</section>

<!-- Галерея -->
<section id="gallery" class="animate-fadeInUp">
<h2>Галерея работ</h2>
<div class="projects-grid">
<img src="https://via.placeholder.com/600x400?text=Галерея+1" alt="" style="width:auto;height:auto;border-radius:10px;">
<img src="https://via.placeholder.com/600x400?text=Галерея+2" alt="" style="width:auto;height:auto;border-radius:10px;">
<img src="https://via.placeholder.com/600x400?text=Галерея+3" alt="" style="width:auto;height:auto;border-radius:10px;">
<!-- Добавьте свои изображения -->
</div>
</section>

<!-- Контакты с формой -->
<section id='contact' class='animate-fadeInUp'>
<h2>Свяжитесь со мной</h2>
<form class='contact-form' id='contactForm'>
<input type='text' placeholder='Ваше имя' required />
<input type='email' placeholder='Ваш email' required />
<textarea rows='4' placeholder='Ваше сообщение' required></textarea>
<button type='submit'>Отправить сообщение</button>
<div id='formMessage'></div>
</form>
</section>

<!-- Подвал -->
<footer style='background:#222;color:#fff;text-align:center;padding:20px;margin-top:-40px'>
&copy;2024 Ваше имя. Все права защищены.
</footer>

<script>
// Обработка формы
document.getElementById('contactForm').addEventListener('submit', function(e){
 e.preventDefault();
 const messageDiv = document.getElementById('formMessage');
 messageDiv.innerHTML = 'Сообщение отправлено! Спасибо!';
 messageDiv.style.color = 'lightgreen';
 // Можно добавить отправку данных на сервер или очистку формы
 this.reset();
});
  
// Анимация при прокрутке
const animatedSections = document.querySelectorAll('.animate-fadeInUp');
window.addEventListener('scroll', () => {
 animatedSections.forEach(section => {
 if (section.getBoundingClientRect().top < window.innerHeight -50) {
 section.style.opacity = '1';
 section.style.transform = 'translateY(0)';
 }
 });
});
  
// Изначально скрываем секции
animatedSections.forEach(section => {
 section.style.opacity = '0';
 section.style.transform = 'translateY(20px)';
});
</script>

</body>
</html>
