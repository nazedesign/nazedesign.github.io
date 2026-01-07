<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Kelvin | Creative Portfolio</title>
    
    <!-- Favicon (K Minimalista) -->
    <link rel="icon" href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22 fill=%22white%22 font-family=%22serif%22 font-style=%22italic%22>K</text></svg>">

    <!-- GSAP para interações fluidas -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/ScrollTrigger.min.js"></script>
    <style>
        :root {
            --white: #FFFFFF;
            --black: #000000;
            --gray: #1a1a1a;
            --serif: "Times New Roman", Times, serif;
            --sans: "Helvetica", Arial, sans-serif;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            -webkit-tap-highlight-color: transparent;
        }

        /* Esconder barra de rolagem mas manter funcionalidade */
        html {
            scrollbar-width: none;
            -ms-overflow-style: none;
            overflow-x: hidden;
        }

        html::-webkit-scrollbar {
            display: none;
        }

        body {
            background-color: var(--black);
            color: var(--white);
            font-family: var(--sans);
            overflow-x: hidden;
            width: 100%;
            transition: background-color 0.6s cubic-bezier(0.23, 1, 0.32, 1), color 0.6s ease;
        }

        .noise {
            position: fixed;
            top: 0; left: 0;
            width: 100vw; height: 100vh;
            z-index: 9999;
            pointer-events: none;
            opacity: 0.12;
            background: url('https://grainy-gradients.vercel.app/noise.svg');
        }

        .nav-link {
            position: fixed;
            top: 20px;
            z-index: 10001;
            mix-blend-mode: difference;
        }

        .social-link {
            left: 20px;
        }

        .lang-wrapper {
            right: 20px;
            display: flex;
            align-items: center;
        }

        .btn-ui {
            background: none;
            border: 1px solid currentColor;
            color: inherit;
            padding: 6px 10px;
            cursor: pointer;
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 6px;
            font-family: var(--sans);
            font-size: 0.7rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: all 0.3s ease;
        }

        .btn-ui:hover { background: var(--white); color: var(--black); }

        .lang-dropdown {
            position: absolute;
            top: 100%;
            right: 0;
            background: var(--black);
            border: 1px solid var(--white);
            display: none;
            flex-direction: column;
            min-width: 120px;
            margin-top: 5px;
        }

        .lang-dropdown.active { display: flex; }

        .lang-option {
            padding: 10px 15px;
            color: var(--white);
            text-decoration: none;
            font-size: 0.7rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            border-bottom: 1px solid #333;
            cursor: pointer;
        }

        #hero {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            background: var(--black);
            position: relative;
            z-index: 100;
            touch-action: pan-y;
        }

        .hero-text-container {
            font-family: var(--serif);
            font-size: 8vw;
            font-style: italic;
            height: 1.5em;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            width: 90%;
        }

        .warp-line {
            position: absolute;
            opacity: 0;
            transform: translateY(60px);
            filter: blur(10px);
            transition: opacity 0.8s, transform 0.8s, filter 0.8s;
            pointer-events: none;
            white-space: nowrap;
        }

        .warp-line.active {
            opacity: 1;
            transform: translateY(0);
            filter: blur(0px);
            pointer-events: auto;
        }

        .warp-line.exit {
            opacity: 0;
            transform: translateY(-60px);
            filter: blur(10px);
        }

        #gallery-wrapper {
            background: var(--white);
            color: var(--black);
            overflow: hidden;
            height: 100vh;
            width: 100%;
            position: relative;
        }

        .horizontal-container {
            height: 100vh;
            display: flex;
            align-items: center;
            width: fit-content;
            padding-left: 15vw;
            padding-right: 15vw;
            will-change: transform;
        }

        .gallery-item, .outro-item {
            position: relative;
            flex-shrink: 0;
            width: 70vw;
            height: 50vh;
            margin-right: 15vw;
            background-color: #eee;
            background-size: cover;
            background-position: center;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .outro-item {
            background: white;
            flex-direction: column;
            border: 1px solid rgba(0,0,0,0.1);
        }

        .gallery-label {
            position: absolute;
            bottom: -40px;
            left: 0;
            font-family: var(--sans);
            text-transform: uppercase;
            font-size: 0.65rem;
            letter-spacing: 2px;
            color: black;
        }

        #lightbox {
            position: fixed;
            top: 0; left: 0;
            width: 100vw; height: 100vh;
            background: rgba(0,0,0,0.95);
            z-index: 200000;
            display: none; 
            align-items: center;
            justify-content: center;
            opacity: 0;
            transition: opacity 0.4s ease;
        }

        #lightbox.active {
            display: flex;
            opacity: 1;
        }

        .lightbox-content {
            position: relative;
            width: 90vw;
            max-width: 1000px;
            aspect-ratio: 4 / 5;
            background: var(--white);
            padding: 10px;
            transform: scale(0.9);
            transition: transform 0.5s cubic-bezier(0.16, 1, 0.3, 1);
        }

        #lightbox.active .lightbox-content {
            transform: scale(1);
        }

        #lightbox-target {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        @media (min-width: 1024px) {
            .hero-text-container { font-size: 6vw; }
            .gallery-item, .outro-item { width: 45vw; height: 65vh; margin-right: 20vw; }
            .horizontal-container { padding-left: 27.5vw; }
            .lightbox-content { aspect-ratio: 16 / 10; width: 80vw; }
        }
    </style>
</head>
<body>

    <div class="noise"></div>

    <div class="nav-link social-link">
        <a href="https://instagram.com" target="_blank" class="btn-ui">
            <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="2" width="20" height="20" rx="5" ry="5"></rect><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"></path><line x1="17.5" y1="6.5" x2="17.51" y2="6.5"></line></svg>
            Instagram
        </a>
    </div>

    <div class="nav-link lang-wrapper">
        <button class="btn-ui" id="lang-btn">
            <span id="current-lang-label">EN</span>
        </button>
        <div class="lang-dropdown" id="lang-dropdown">
            <div class="lang-option" onclick="changeLang('en')">English</div>
            <div class="lang-option" onclick="changeLang('pt')">Português</div>
            <div class="lang-option" onclick="changeLang('es')">Español</div>
        </div>
    </div>

    <div id="lightbox" onclick="closeLightbox()">
        <div class="lightbox-content" onclick="event.stopPropagation()">
            <img id="lightbox-target" src="" alt="Project View">
        </div>
    </div>

    <section id="hero">
        <div class="hero-text-container">
            <div class="warp-line active" data-key="hero-1">Hello</div>
            <div class="warp-line" data-key="hero-2">I'm Kelvin</div>
            <div class="warp-line" data-key="hero-3">I'm not a designer</div>
            <div class="warp-line" data-key="hero-4">nor a programmer</div>
            <div class="warp-line" data-key="hero-5">but I know both</div>
            <div class="warp-line" data-key="hero-6">Scroll Down</div>
        </div>
    </section>

    <div id="gallery-wrapper">
        <div class="horizontal-container" id="scroll-content">
            <!-- Dinâmico -->
        </div>
    </div>

    <script>
        gsap.registerPlugin(ScrollTrigger);

        const translations = {
            en: { label: "EN", "hero-1": "Hello", "hero-2": "I'm Kelvin", "hero-3": "I'm not a designer", "hero-4": "nor a programmer", "hero-5": "but I know both", "hero-6": "Scroll Down", "project": "Project", "close": "Close" },
            pt: { label: "PT", "hero-1": "Olá", "hero-2": "Eu sou o Kelvin", "hero-3": "Não sou designer", "hero-4": "nem programador", "hero-5": "mas entendo de ambos", "hero-6": "Role para baixo", "project": "Projeto", "close": "Fechar" },
            es: { label: "ES", "hero-1": "Hola", "hero-2": "Soy Kelvin", "hero-3": "No soy diseñador", "hero-4": "ni programador", "hero-5": "pero entiendo ambos", "hero-6": "Desliza abaixo", "project": "Projeto", "close": "Cerrar" }
        };

        let currentLang = 'en';
        const lines = document.querySelectorAll('.warp-line');
        let currentIdx = 0;
        let isTransitioning = false;
        const chars = "01";

        function scrambleFull(element) {
            if (!element || element.dataset.isScrambling === "true") return;
            element.dataset.isScrambling = "true";
            const originalText = translations[currentLang][element.dataset.key];
            let iteration = 0;
            const interval = setInterval(() => {
                element.innerText = originalText.split("").map((l, i) => i < iteration ? originalText[i] : chars[Math.floor(Math.random()*2)]).join("");
                if (iteration >= originalText.length) { clearInterval(interval); element.dataset.isScrambling = "false"; }
                iteration += 1;
            }, 20);
        }

        function renderGallery() {
            const container = document.getElementById('scroll-content');
            const imgs = [
                "https://images.unsplash.com/photo-1478760329108-5c3ed9d495a0?w=1200",
                "https://images.unsplash.com/photo-1449247704656-13621df5ee70?w=1200",
                "https://images.unsplash.com/photo-1494438639946-1ebd1d20bf85?w=1200",
                "https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?w=1200"
            ];
            let html = '';
            imgs.forEach((src, i) => {
                html += `
                    <div class="gallery-item" style="background-image: url('${src}')" onclick="openLightbox('${src}')">
                        <span class="gallery-label">${translations[currentLang].project} 0${i+1}</span>
                    </div>
                `;
            });
            html += `<div class="outro-item"><h2>Kelvin</h2><p>kelvindesign@proton.me</p></div>`;
            container.innerHTML = html;
        }

        function transitionTo(nextIdx) {
            if (isTransitioning || nextIdx < 0 || nextIdx >= lines.length) return;
            isTransitioning = true;
            lines[currentIdx].classList.replace('active', 'exit');
            currentIdx = nextIdx;
            lines[currentIdx].classList.add('active');
            scrambleFull(lines[currentIdx]);
            setTimeout(() => {
                document.querySelectorAll('.exit').forEach(el => el.classList.remove('exit'));
                isTransitioning = false;
            }, 800);
        }

        // Scroll do Hero (Lógica de troca de frases)
        window.addEventListener('wheel', (e) => {
            if (window.scrollY < 10) {
                if (e.deltaY > 0 && currentIdx < lines.length - 1) transitionTo(currentIdx + 1);
                else if (e.deltaY < 0 && currentIdx > 0) transitionTo(currentIdx - 1);
            }
        });

        // Suporte a Touch para o Hero
        let touchStartY = 0;
        window.addEventListener('touchstart', e => touchStartY = e.touches[0].clientY);
        window.addEventListener('touchmove', e => {
            if (window.scrollY < 10) {
                const touchEndY = e.touches[0].clientY;
                if (touchStartY - touchEndY > 50 && currentIdx < lines.length - 1) transitionTo(currentIdx + 1);
                else if (touchEndY - touchStartY > 50 && currentIdx > 0) transitionTo(currentIdx - 1);
            }
        });

        function updateEffects() {
            const items = document.querySelectorAll('.gallery-item, .outro-item');
            const centerX = window.innerWidth / 2;
            items.forEach(item => {
                const rect = item.getBoundingClientRect();
                const dist = Math.abs(centerX - (rect.left + rect.width / 2));
                const norm = Math.min(dist / (window.innerWidth * 0.8), 1);
                gsap.set(item, {
                    filter: `blur(${norm * 8}px)`,
                    scale: 1.1 - (norm * 0.2),
                    opacity: 1 - (norm * 0.6)
                });
            });
        }

        function initScrollAnimations() {
            const content = document.getElementById('scroll-content');
            const wrapper = document.getElementById('gallery-wrapper');

            // Scroll Horizontal
            gsap.to(content, {
                x: () => -(content.scrollWidth - window.innerWidth),
                ease: "none",
                scrollTrigger: {
                    trigger: wrapper,
                    start: "top top",
                    end: () => "+=" + content.scrollWidth,
                    pin: true,
                    scrub: 1,
                    anticipatePin: 1,
                    onUpdate: updateEffects,
                    invalidateOnRefresh: true
                }
            });

            // Troca de Cor de Fundo
            ScrollTrigger.create({
                trigger: wrapper,
                start: "top 60%",
                onEnter: () => { document.body.style.backgroundColor = "white"; document.body.style.color = "black"; },
                onLeaveBack: () => { document.body.style.backgroundColor = "black"; document.body.style.color = "white"; }
            });
        }

        window.openLightbox = (src) => {
            const lb = document.getElementById('lightbox');
            document.getElementById('lightbox-target').src = src;
            lb.style.display = 'flex';
            setTimeout(() => lb.classList.add('active'), 10);
            document.body.style.overflow = 'hidden';
        };

        window.closeLightbox = () => {
            const lb = document.getElementById('lightbox');
            lb.classList.remove('active');
            setTimeout(() => { lb.style.display = 'none'; document.body.style.overflow = ''; }, 400);
        };

        window.changeLang = (lang) => {
            currentLang = lang;
            document.getElementById('current-lang-label').textContent = translations[lang].label;
            document.querySelectorAll('.warp-line').forEach(el => el.textContent = translations[lang][el.dataset.key]);
            renderGallery();
            document.getElementById('lang-dropdown').classList.remove('active');
        };

        document.getElementById('lang-btn').onclick = (e) => {
            e.stopPropagation();
            document.getElementById('lang-dropdown').classList.toggle('active');
        };

        window.onload = () => {
            renderGallery();
            initScrollAnimations();
            scrambleFull(lines[0]);
        };

        window.addEventListener('resize', () => {
            ScrollTrigger.refresh();
        });
    </script>
</body>
</html>
