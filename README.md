<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>10 G</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
   
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap');
        
        body {
            font-family: 'Montserrat', sans-serif;
            margin: 0;
            padding: 0;
            
            background-color: #081426;
            color: #d0d5c2;
            
        }

        .navbar {
            
            background-color: #052a5e;
            padding: 20px 50px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            color: #a72b2b;
            margin-right: 670px;
        }

        .nav-links {
            list-style: none;
            display: flex;
            gap: 20px;
        }

        .nav-links li a {
            text-decoration: none;
            color: #a72b2b;
            font-size: 1.3rem;
            transition: color 0.3s ease, transform 0.3s ease;
        }

        .nav-links li a:hover {
            color: #d0d5c2;
            transform: scale(1.1);
        }

        .home, .about, .skills, .achievements, .future-job, .wishes {
            opacity: 0;
            transform: translateY(50px);
            transition: all 0.8s ease-in-out;
        }

        .show {
            opacity: 1;
            transform: translateY(0);
        }

        .home, .about, .achievements, .skills, .future-job, .wishes {
            text-align: center;
            padding: 50px 20px;
        }

        .achievements {
            background-color: #02214d;
            border-radius: 15px;
            margin: 40px auto;
            width: 80%;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.3);
        }

        .gg{
            display: flex;
            height: 90px;
        }

        

        
       
    </style>
</head>
<body>
   
    <nav class="navbar">
        <h1 class="gg"><img src="https://img.hhcdn.ru/employer-logo/2410370.png" alt=""></h1>
        <h2 class="logo"> 10 G(2024-2025)</h2>
        <ul class="nav-links">
            <li><a href="#about">Класс туралы ақпарат</a></li>
            <li><a href="#future-job">Оқушылар</a></li>
            <li><a href="#achievements">Жетістіктер</a></li>
        </ul>
    </nav>

    <section class="home text-center">
        <img src="data:image/jpeg;base64,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"  
             class="mx-auto d-block" 
             style="width: 50%; max-width: 300px; border-radius: 30px; margin-top: 20px;" 
             alt="..">
        <h1>____</h1>
        <h5>Класс туралы мәлімет</h5>
<h5>Біздің 10 G сынып РФММ керегесін 2021 жылы аттады.Мектепті бітіру жылымыз 2026 болып табылады.Қазіргі таңда сыныбымызда 27 оқушы бар.Оның ішінде 20 оқушы интернатта,ал 7 оқушы қалалық.
    </section>

    <section id="about" class="about">
        <div id="carouselExampleFade" class="carousel slide carousel-fade">
            <div class="carousel-inner">
                <div class="carousel-item active">
                    <img class="dff" src="https://i.postimg.cc/pX1Vx4Hk/images.jpg" class="d-block w-50 mx-auto" alt="НЗФМ">
                </div>
            </div>
        </div>
        <h1>_____</h1>
        <h2>Класстың тарихы</h2>
        <h1> ㅤ</h1>
        <h5>Алғаш мектепке келген кезде интернат тәрбиешісімен таныстық.Ермекова Гүлжан 7 класстан бері біздің тәрбиешіміз болып келеді.</h5>
<h5> 7 сыныпта сынып жетекшіміз болып Малика Жасталаповна тағайындалды,8 сыныпта жетекші ауысып,Малика апайдың орнына мектептің завучы Нурбану Кабулова келді.Уақытының тығыздығынан 9 сыныптан бері сынып жетекшіміз Динара Абилхасимова болып келеді</h5>
    </section>

    <section class="home text-center">
        <img src="https://i.postimg.cc/7ZSGbKh7/aa.jpg"  
             class="mx-auto d-block" 
             style="width: 300px; height: auto; border-radius: 30px; margin-top: 20px;" 
             alt="..">
             <h1>_____</h1>
        <h1>Мектеп мақтаныштары және олардың жетістіктері</h1>
        <h5 class="fg"><strong>Ерсұлтан</strong>.2023-2024 мектеп мақтанышы атағын алды.Мектептегі баскетбол командасының капитаны,оған қоса 2025 Республикалық информатика пәнінен олимпиаданың қола жүлдегері</h5>
 <h5 class="fg"><strong>Әділ</strong>.2023-2024 мектеп мақтанышы атағын алды.Қазақстан білім олимпиадасы (КБО), жаратылыстану ғылымдары бойынша республикалық олимпиаданың және Халықаралық жасөспірімдер жаратылыстану-ғылыми олимпиадасының (IJSO) жүлдегері</h5>

    </section>
   
    

    <section id="achievements" class="achievements">
        <h2>Олардын жетістіктері
        </h2>
        <h1>____</h1>
        <ul>
            <H4><li>🏆 Шахмат клубының президенті</li>
                <li>🏆 Яндекс лицей академиясының түлегі</li>
                <li>🏆 Халықаралық Жәутіков Олимпиадасы - күміс және қола медальдар</li>
                <li>🏆 Халықаралық геометрия олимпиадасында 2 орын </li>
                <li>🏆 "Астрофотография года" байқауында 1 орын</li>
                <li>🏆 "Мұқағали Мақатаев" өлеңдерінен қалалық Олимпиададан 1-орын</li>
                <li>🏆 Футболдан 1,2,3-орын иегерлері</li>
                <li>🏆 "QUARK" олимпиадасының ұйымдастырушыларының бірі</li>
                <li>🏆 Шамамен 100 сағат волонтерлік жұмыс</li></H4>
        </ul>
    </section>

    
    <script>
        const sections = document.querySelectorAll('.home, .about, .skills, .achievements, .wishes, .future-job');

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('show');
                } else {
                    entry.target.classList.remove('show');
                }
            });
        }, { threshold: 0.2 });

        sections.forEach(section => observer.observe(section));



        
    </script>

<section id="students" class="students text-center" style="display: none; padding: 30px; background-color: #081426;">
<h2 style="color: #d0d5c2;">Оқушылар</h2>
<div class="container">
<div class="row">
<script>
let students = [
{ name: "Жомарт", link: "https://zhomart7898.github.io/555/" },
{ name: "Айдана", link: "https://aidanaa286.github.io/aidana/" },
{ name: "Ерсұлтан", link: "https://ersultaaan.github.io/portfolio/" },
{ name: "Асылжан", link: "https://zhasyl.github.io/asyl/" },
{ name: "Айбол", link: "https://aibol0923.github.io/777/" },
{ name: "Ерназар", link: "https://zhasyl.github.io/ernazar/" },
{ name: "Асет", link: "https://aseeett.github.io/asefhj/" },
{ name: "Парасат", link: "https://parassattangirbergen.github.io/parassat/" },
{ name: "Альбина", link: "https://albinasamatova.github.io/port/" },
{ name: "Әділ", link: "https://zhienbaevadil.github.io/my-first-site/" },
{ name: "Ильяс", link: "https://nokrad070.github.io/ILYAS/" },
{ name: "Ерәлім", link: "https://01102008yaya.github.io/Era.github.io/" },
{ name: "Жадыра", link: "https://zhasyl.github.io/zhako/zhadyra1.htm" },
];

                students.forEach(student => {
                    document.write(
                        <div class="col-md-3 mb-3 student-card" style="opacity: 0; transform: translateY(30px); transition: all 0.6s ease;">
                            <div class="card p-3 text-center" style="background-color: #052a5e; color: #d0d5c2; border-radius: 10px; box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.3);">
                                <h5>
                                    <a href="${student.link}" target="_blank" style="color: #d0d5c2; text-decoration: none;">${student.name}</a>
                                </h5>
                            </div>
                        </div>
                    );
                });
</script>
</div>
</div>
</section>

<script>
    // Кнопка "Оқушылар" плавно скроллит к списку
    document.querySelector('.nav-links li a[href="#future-job"]').addEventListener('click', function(event) {
        event.preventDefault();
        let studentsSection = document.getElementById("students");
        studentsSection.style.display = "block";
        studentsSection.scrollIntoView({ behavior: "smooth" });
    });

    // Анимация появления карточек при скролле
    function revealOnScroll() {
        let cards = document.querySelectorAll('.student-card');
        let windowHeight = window.innerHeight;

        cards.forEach(card => {
            let cardTop = card.getBoundingClientRect().top;
            if (cardTop < windowHeight - 50) {
                card.style.opacity = "1";
                card.style.transform = "translateY(0)";
            }
        });
    }

    window.addEventListener('scroll', revealOnScroll);
</script>

</body>
</html>
