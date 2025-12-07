<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Skyline Inc.</title>

    <!-- overall -->
    <style>

        /* basics */
        body {
            font-family: courier,monospace ;
            margin: 0px;
            padding: 0;
            background-image: url("https://i.imgur.com/ikbeP4Y.jpeg");
            background-size: cover;          
            background-position: center;     
            background-repeat: no-repeat;   
            background-attachment: fixed;   
        }
        
        /* header */
        header {
            background-image: url("https://i.imgur.com/KrreuWh.png"); 
            background-size: cover;      
            background-position: center;  
            background-repeat: no-repeat;  
            height: 200px;                 
            color: rgb(255, 255, 255);                  
            display: flex;
            flex-direction: column;
            justify-content: center;       
            align-items: center;           
            text-align: center;
            padding: 0px;
        }
        header h1,
        header p {
            background: rgba(229, 122, 122, 0.7);
            padding: 10px 20px;
            border-radius: 8px;
            display: inline-block;
        }

        /* nav bar */
        nav {
            background: rgb(229, 122, 122, 0.7);
            padding: 10px;
        }
        nav a {
            color: white;
            margin-right: 20px;
            text-decoration: underline;
        }

        /* tab buttons */
        .gallery-selector {
            text-align: center;
            margin: 20px 0;
        }
        .tab-btn {
            background: #a0d9ff;
            color: #fff;
            border: none;
            padding: 10px 20px;
            margin: 0 5px;
            border-radius: 6px;
            cursor: pointer;
        }
        .tab-btn:hover {
            background: #2980b9;
        }
        /* active tab highlight */
        .tab-btn.active {
            background: #1e90ff; /* brighter blue */
        }

        /* sections */
        .section, .section1 {
            background: white;
            padding: 20px;
            margin: 20px;
            border-radius: 8px;      
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        .section1 { padding: 20px; margin: 20px; }

        /* button */
        .btn {
            background: #3498db;  
            color: rgb(255, 255, 255);
            padding: 10px 20px;
            border: none;
            border-radius: 6px;
            cursor: pointer;
        }
        .btn:hover { background: #2980b9; }
        .btn:active { transform: scale(0.33); }

        /* footer */
        footer {
            text-align: center;
            padding: 15px;
            background: rgb(229, 122, 122, 0.7);
            color: white;
            margin-top: 40px;
        }

    </style>
</head>

<body>

    <!-- title+captions -->
    <header>
        <h1>Skyline Inc.</h1>
        <p>The Sun Sets in the West</p>
    </header>

    <!-- navigation -->
    <nav>
        <a href="https://www.louvre.fr/en/">Louvre</a>
        <a href="https://www.museivaticani.va/content/museivaticani/en.html">Vatican Museums</a>
        <a href="https://www.britishmuseum.org/">British Museum</a>
        <a href="https://www.metmuseum.org/">The Met Museum of Art</a>
        <a href="https://www.tate.org.uk/visit/tate-modern">Tate Modern</a>
        <a href="https://www.shanghaimuseum.net/mu/frontend/pg/en/service/visit-east">Shanghai Museum East</a>
        <a href="https://www.nga.gov/">U.S.- National Gallery of Art</a>
    </nav>

    <!-- Gallery selector -->
    <div class="gallery-selector">
        <button class="tab-btn active" data-target="overview-tab">About Us</button>
        <button class="tab-btn" data-target="artworks-tab">Featured Artworks</button>
    </div>

    <!-- About Us tab -->
    <div id="overview-tab" class="tab-content">
        <!-- 1-->
        <div class="section">
            <h2>Art</h2>
            <p>
                Art is a diverse range of cultural activity centered around 
                works utilizing creative or imaginative talents, which are expected 
                to evoke a worthwhile experience, generally through an expression of emotional 
                power, conceptual ideas, technical proficiency, or beauty. 
            </p>
            <img src="https://i.imgur.com/yIhxe7s.jpeg" width="200">
        </div>

        <!-- 2-->
        <div class="section">
            <h2>Our gallery</h2>
            <ul>
                <li>Features 7 famous art galleries.</li>
                <li>Contains high quality descriptions.</li>
                <li>Dedicated to all types of art</li>
            </ul>
            <img src="https://i.imgur.com/C8tpgcq.jpeg" width="200">
        </div>
    </div>

    <!-- Featured Artworks tab -->
    <div id="artworks-tab" class="tab-content" style="display:none;">
        <!-- 3-->
        <div class="section1">
            <h2>The Starry Night</h2>
            <p>
                The Starry Night, often called simply Starry Night, 
                is an oil-on-canvas painting by the Dutch Post-Impressionist 
                painter Vincent van Gogh. Painted in June 1889, 
                it depicts the view from the east-facing window of his 
                asylum room at Saint-Rémy-de-Provence, just before sunrise, 
                with the addition of an imaginary village. 
            </p>
            <img src="https://i.imgur.com/CreY35j.jpeg" width="200">
            <button class="btn">♥</button>
        </div>

        <!-- 4-->
        <div class="section1">
            <h2>Mona Lisa</h2>
            <p>
                The Mona Lisa is a half-length portrait painting by 
                the Italian artist Leonardo da Vinci. Considered an archetypal 
                masterpiece of the Italian Renaissance, it has been described as 
                "the best known, the most visited, the most written about, the most sung about, 
                [and] the most parodied work of art in the world."
            </p>
            <img src="https://i.imgur.com/fXUtq2F.jpeg" width="200">
            <button class="btn">♥</button>
        </div>

        <!-- 5-->
        <div class="section1">
            <h2>The Scream</h2>
            <p>
                The Scream is an art composition created by Norwegian 
                artist Edvard Munch in 1893. The Norwegian name of the piece is Skrik, 
                and the German title under which it was first exhibited is Der Schrei der Natur. 
                The agonized face in the painting has become one of the most iconic images in art, 
                seen as representing a profound experience of existential dread related to the human 
                condition.
            </p>
            <img src="https://i.imgur.com/yXJZeWV.jpeg" width="200">
            <button class="btn">♥</button>
        </div>
    </div>

    <!-- footer -->
    <footer>
        © 2025 Skyline Inc. — All Rights Reserved
    </footer>

    <!-- Confetti + Tabs -->
    <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>
    <script>
        document.addEventListener("DOMContentLoaded", () => {
            // Confetti for all buttons
            const buttons = document.querySelectorAll(".btn");
            buttons.forEach(button => {
                button.addEventListener("click", () => {
                    for (let i = 0; i < 5; i++) {
                        confetti({
                            particleCount: 150,
                            spread: 160,
                            startVelocity: 40,
                            origin: { x: Math.random(), y: Math.random() * 0.8 }
                        });
                    }
                });
            });

            // Tabs for overview / artworks
            const tabButtons = document.querySelectorAll(".tab-btn");
            const tabContents = document.querySelectorAll(".tab-content");

            tabButtons.forEach(btn => {
                btn.addEventListener("click", () => {
                    const target = btn.getAttribute("data-target");
                    tabContents.forEach(content => content.style.display = "none");
                    document.getElementById(target).style.display = "block";

                    // Highlight active tab
                    tabButtons.forEach(b => b.classList.remove("active"));
                    btn.classList.add("active");
                });
            });
        });
    </script>
</body>
</html>
