<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Эврен | Кандидат в инженеры-программисты</title>
<style>
:root {
  --bg:#ffffff; --card:rgba(20,22,30,0.85);
  --text:#1a1a1a; --muted:#555555; --accent:#c1121f;
}
*{box-sizing:border-box;margin:0;padding:0;}
html{scroll-behavior:smooth;}
body{
  font-family:'Times New Roman', Times, serif;
  font-size:20px;line-height:1.8;letter-spacing:0.5px;
  margin-bottom:16px;background:var(--bg);color:var(--text);
}
.fade{opacity:0;transform:translateY(40px);transition:all 0.9s ease;}
.fade.show{opacity:1;transform:translateY(0);}
.header-lang{
  position:fixed;top:20px;right:20px;z-index:999;
}
.header-lang button{
  background:none;border:none;margin-left:8px;font-weight:600;
  cursor:pointer;color:var(--accent);
}
.hero{
  min-height:100vh;display:flex;justify-content:center;
  align-items:center;text-align:center;padding:40px 20px;
  background:linear-gradient(135deg,#fefefe 0%,#f7f7f7 100%);
}
.hero img{
  width:300px;height:300px;border-radius:50%;object-fit:cover;
  border:3px solid var(--accent);box-shadow:0 0 30px rgba(193,18,31,0.45);
  margin-bottom:26px;transition:transform 0.4s ease;
}
.hero img:hover{transform:scale(1.04);}
.hero h1{font-size:clamp(34px,5vw,50px);font-weight:600;letter-spacing:0.5px;margin-bottom:14px;}
.hero h1 span{color:var(--accent);}
.hero p{max-width:700px;margin:0 auto;font-size:17px;line-height:1.75;color:var(--muted);}
section{max-width:1000px;margin:auto;padding:80px 20px;position:relative;}
.section-title{font-size:30px;font-weight:600;margin-bottom:40px;position:relative;}
.section-title::after{
  content:"";position:absolute;left:0;bottom:-14px;width:60px;height:6px;
  background:url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 60 6"><path d="M0 3 Q15 0 30 3 T60 3" stroke="%23c1121f" stroke-width="2" fill="transparent"/></svg>') no-repeat;
}
.timeline{display:flex;flex-direction:column;gap:60px;}
.timeline-item{display:flex;flex-wrap:wrap;align-items:center;gap:30px;position:relative;border-radius:12px;background-image:url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="200" height="200"><circle cx="100" cy="100" r="5" fill="%23c1121f"/><circle cx="50" cy="50" r="3" fill="%23c1121f"/><circle cx="150" cy="150" r="3" fill="%23c1121f"/></svg>');background-repeat:repeat;background-position:center;background-size:50px;}
.timeline-item:nth-child(even){flex-direction:row-reverse;}
.timeline-item img{width:400px;height:300px;object-fit:cover;border-radius:12px;flex-shrink:0;box-shadow:0 8px 25px rgba(0,0,0,0.2);transition:transform 0.4s ease;}
.timeline-item img:hover{transform:scale(1.05);}
.timeline-item .text{background:rgba(255,255,255,0.95);padding:28px;border-radius:14px;flex:1;box-shadow:0 8px 25px rgba(0,0,0,0.15);}
.text p{font-size:16px;line-height:1.8;color:var(--text);}

/* PROJECTS */
.projects-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:35px;margin-top:30px;}
.project-card{background:rgba(255,255,255,0.95);border-radius:16px;padding:28px;box-shadow:0 10px 30px rgba(0,0,0,0.12);transition:transform 0.35s ease,box-shadow 0.35s ease;}
.project-card:hover{transform:translateY(-8px);box-shadow:0 25px 50px rgba(0,0,0,0.2);}
.project-card h3{font-size:20px;margin-bottom:12px;font-weight:600;}
.project-card p{font-size:16px;color: var(--muted);margin-bottom:16px;}
.project-tags{display:flex;flex-wrap:wrap;gap:10px;}
.project-tags span{font-size:13px;padding:6px 12px;border-radius:999px;background: rgba(193,18,31,0.1); color: var(--accent); font-weight:500;}
footer{text-align:center;padding:55px 20px;font-size:14px;color:var(--muted);opacity:0.8;}
</style>
</head>
<body>

<div class="header-lang">
  <button data-lang="tr">TR</button>
  <button data-lang="en">EN</button>
  <button data-lang="ru">RU</button>
</div>

<!-- HERO -->
<div class="hero fade">
  <div>
    <img src="https://i.hizliresim.com/97lswqu.jpg" alt="Evren">
    <h1 id="hero-name">Хасаноглу <span>Эврен</span></h1>
    <p id="hero-desc">Учится в России, студент подготовительного курса УрФУ. Сосредоточен на развитии навыков в области программной инженерии и русского языка, любит работать дисциплинированно.</p>
  </div>
</div>

<!-- Образование и мой путь -->
<section>
  <h2 class="section-title" id="edu-title">Образование и мой путь</h2>
  <div class="timeline">
    <div class="timeline-item fade">
      <img src="https://i.hizliresim.com/jyz9nxt.jpg" alt="Вид Екатеринбурга">
      <div class="text" id="edu-text1">
        Россия страна, которую я люблю с детства. Одной из главных причин моего интереса к этой стране является её богатая культура и ощущение бесконечных возможностей как в истории, так и в моей области. Поэтому я сознательно выбрал Россию для обучения и личного развития. Поступление в УрФУ и переезд в Россию стали для меня важным шагом не только в академическом, но и в личностном плане. Привыкать к новой стране, языку и образовательной системе было очень увлекательно и помогло мне стать более дисциплинированным, ответственным и целеустремлённым.
      </div>
    </div>
    <div class="timeline-item fade">
      <img src="https://i.hizliresim.com/1cs25go.jpg" alt="Архитектура Екатеринбурга">
      <div class="text" id="edu-text2">
        Раньше я не всегда был примерным учеником, но сегодня я ясно понимаю свои прошлые ошибки и воспринимаю их как ценный опыт. Сейчас я делаю всё возможное, чтобы не повторять прежние сожаления. Я работаю над собой каждый день, потому что стремление к своим целям для меня так же естественно, как дыхание.
      </div>
    </div>
  </div>
</section>

<!-- Почему инженерия программного обеспечения -->
<section>
  <h2 class="section-title" id="why-title">Почему инженерия программного обеспечения</h2>
  <div class="timeline">
    <div class="timeline-item fade">
      <img src="https://i.hizliresim.com/rim8zbw.jpg" alt="Программный проект">
      <div class="text" id="why-text">
        Программная инженерия, потому что особенно меня привлекает веб разработка; мне нравится создавать визуально понятные и функциональные продукты. Я интересуюсь сочетанием веб-технологий с искусственным интеллектом. С момента приезда в Россию у меня сильная мотивация стать успешным инженером программистом, постоянно развиваться и делиться своими знаниями с другими. Моя цель стать дисциплинированным и компетентным специалистом, способным вносить значимый вклад в современные технологические проекты.
      </div>
    </div>
  </div>
</section>


<!-- TOOLS / NASIL YAPTIM -->
<section>
  <h2 class="section-title" id="tools-title">Используемые инструменты</h2>
  <div class="timeline">
    <div class="timeline-item fade">
      <div class="text" id="tools-text">
        Этот веб-сайт создан с использованием HTML, CSS и JavaScript. Для анимаций и многоязычной системы была разработана JavaScript-основанная реализация. Дизайн и пользовательский опыт полностью принадлежат мне; также искусственный интеллект помог сделать тексты более плавными.
      </div>
    </div>
  </div>
</section>

<footer>© 2026 Эврен — Кандидат в инженеры-программисты</footer>

<script>
const translations = {
  tr:{
    "hero-name":"Hasanoğlu <span>Evren</span>",
    "hero-desc":"Rusya’da, UrFU hazırlık sınıfı öğrencisi olarak eğitim görüyor. Yazılım mühendisliği ve Rusça becerilerini geliştirmeye odaklanmış, disiplinli çalışmayı seven biri.",
    "edu-title":"Eğitim ve Yolculuğum",
    "edu-text1":"Rusya, çocukluğumdan beri sevdiğim bir ülke. Bu ülkeye olan ilgimin başlıca nedenlerinden biri, zengin kültürü ve hem tarih hem de kendi alanım açısından sonsuz fırsatlar sunmasıdır. Bu yüzden eğitim ve kişisel gelişimim için bilinçli olarak Rusya’yı seçtim. UrFU’ya kabul edilmek ve Rusya’ya taşınmak, benim için sadece akademik değil, kişisel açıdan da önemli bir adımdı. Yeni bir ülkeye, dile ve eğitim sistemine alışmak çok keyifliydi ve bana daha disiplinli, sorumlu ve hedef odaklı olmayı öğretti.",
    "edu-text2":"Eskiden her zaman örnek bir öğrenci değildim, ama bugün geçmişteki hatalarımı net bir şekilde anlıyor ve onları değerli bir deneyim olarak görüyorum. Şu anda, geçmiş pişmanlıkları tekrar etmemek için elimden geleni yapıyorum. Her gün kendim üzerinde çalışıyorum, çünkü hedeflerime ulaşma arzusu benim için nefes almak kadar doğal.",
    "why-title":"Neden Yazılım Mühendisliği",
    "why-text":"Yazılım mühendisliği, çünkü özellikle web geliştirme ilgimi çekiyor; görsel olarak anlaşılır ve işlevsel ürünler yaratmayı seviyorum. Web teknolojilerini yapay zeka ile birleştirmekle ilgileniyorum. Rusya’ya geldiğimden beri başarılı bir yazılım mühendisi olma, sürekli gelişme ve bilgimi başkalarıyla paylaşma konusunda güçlü bir motivasyona sahibim. Amacım, modern teknolojik projelere anlamlı katkılarda bulunabilecek, disiplinli ve yetkin bir uzman olmaktır.",
    "projects-title":"Projeler",
    "bot-title":"Telegram Bot",
    "bot-desc":"Kullanıcıyla sohbet arayüzü üzerinden etkileşim sağlayan ve görevleri otomatikleştiren işlevsel bir Telegram botu.",
    "tools-title":"Kullandığım Araçlar",
    "tools-text":"Bu web sitesi, HTML, CSS ve JavaScript kullanılarak oluşturuldu. Animasyonlar ve çokdilli sistem için JavaScript tabanlı çözüm geliştirildi. Tasarım ve kullanıcı deneyimi tamamen bana ait; ayrıca metinlerin akıcı hâle gelmesinde yapay zeka yardımcı oldu."
  },
  en:{
    "hero-name":"Hasanoglu <span>Evren</span>",
    "hero-desc":"Studying in Russia as a preparatory course student at UrFU. Focused on developing skills in software engineering and the Russian language, and enjoys working in a disciplined manner.",
    "edu-title":"Education & Journey",
    "edu-text1":"Russia is a country I have loved since childhood. One of the main reasons for my interest in this country is its rich culture and the sense of limitless opportunities, both in history and in the field of software engineering. That is why I consciously chose Russia for my education and personal development. Being admitted to UrFU and moving to Russia was an important step for me not only academically but also personally. Adapting to a new country, language, and educational system was very exciting and helped me become more disciplined, responsible, and goal-oriented.",
    "edu-text2":"I wasn’t always an exemplary student in the past, but today I clearly understand my previous mistakes and see them as valuable experience. Now, I do everything possible to avoid repeating past regrets. I work on myself every day, because striving for my goals is as natural to me as breathing.",
    "why-title":"Why Software Engineering",
    "why-text":"Software engineering, because I am especially interested in web development; I enjoy creating visually clear and functional products. I am interested in combining web technologies with artificial intelligence. Since coming to Russia, I have had a strong motivation to become a successful software engineer, to continuously improve myself, and to share my knowledge with others. My goal is to become a disciplined and competent professional, capable of making meaningful contributions to modern technological projects.",
    "projects-title":"Projects",
    "bot-title":"Telegram Bot",
    "bot-desc":"A functional Telegram bot that interacts with users via chat interface and automates tasks.",
    "tools-title":"Tools Used",
    "tools-text":"This website was built using HTML, CSS, and JavaScript. Animations and the multilingual system were implemented using JavaScript. Design and user experience are entirely my own; AI assisted in refining the text for readability."
  }
};

// RU texts stay the same
translations.ru = {};
for(const key in translations.en){
  translations.ru[key] = translations.ru[key] || document.getElementById(key)?.innerHTML || translations.en[key];
}

document.querySelectorAll(".header-lang button").forEach(btn=>{
  btn.addEventListener("click", ()=>{
    const lang = btn.dataset.lang;
    for(const id in translations[lang]){
      if(document.getElementById(id)) document.getElementById(id).innerHTML = translations[lang][id];
    }
  });
});

// IntersectionObserver fade
const observer = new IntersectionObserver(entries=>{
  entries.forEach(entry=>{
    if(entry.isIntersecting) entry.target.classList.add("show");
  });
},{threshold:0.2});
document.querySelectorAll(".fade").forEach(el=>observer.observe(el));
</script>

</body>
</html>
