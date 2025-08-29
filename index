<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Manoir d'Exception à Allinges - 1 400 000 €</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Georgia', serif;
            line-height: 1.6;
            color: #333;
            background: #fafafa;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        header {
            background: linear-gradient(135deg, rgba(0,0,0,0.7), rgba(0,0,0,0.5)), url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><rect fill="%23d4a574" width="1200" height="600"/></svg>');
            background-size: cover;
            background-position: center;
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            position: relative;
            overflow: hidden;
        }

        .hero-content {
            z-index: 2;
            animation: fadeInUp 1s ease-out;
        }

        .hero-title {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
            letter-spacing: 2px;
        }

        .hero-subtitle {
            font-size: 1.5rem;
            margin-bottom: 2rem;
            opacity: 0.9;
        }

        .price {
            font-size: 2.5rem;
            color: #d4a574;
            font-weight: bold;
            margin-bottom: 2rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
        }

        .btn {
            display: inline-block;
            padding: 15px 40px;
            background: #d4a574;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            transition: all 0.3s ease;
            font-size: 1.1rem;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .btn:hover {
            background: #c19960;
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        /* Navigation */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(255,255,255,0.95);
            backdrop-filter: blur(10px);
            z-index: 1000;
            padding: 15px 0;
            transition: all 0.3s ease;
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            gap: 40px;
        }

        nav a {
            text-decoration: none;
            color: #333;
            font-weight: 500;
            transition: color 0.3s ease;
        }

        nav a:hover {
            color: #d4a574;
        }

        /* Sections */
        section {
            padding: 80px 0;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
            color: #333;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 80px;
            height: 3px;
            background: #d4a574;
            margin: 20px auto;
        }

        /* Property Info */
        .property-info {
            background: white;
            padding: 80px 0;
        }

        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
            margin-top: 50px;
        }

        .info-card {
            background: #f8f8f8;
            padding: 30px;
            border-radius: 10px;
            text-align: center;
            transition: transform 0.3s ease;
        }

        .info-card:hover {
            transform: translateY(-5px);
        }

        .info-icon {
            font-size: 3rem;
            color: #d4a574;
            margin-bottom: 20px;
        }

        .info-value {
            font-size: 2rem;
            font-weight: bold;
            color: #333;
            margin-bottom: 10px;
        }

        .info-label {
            color: #666;
            font-size: 1.1rem;
        }

        /* Gallery */
        .gallery {
            background: #f5f5f5;
        }

        .image-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin-top: 50px;
        }

        .gallery-item {
            position: relative;
            height: 300px;
            overflow: hidden;
            border-radius: 10px;
            cursor: pointer;
            transition: transform 0.3s ease;
        }

        .gallery-item:hover {
            transform: scale(1.05);
        }

        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.3s ease;
        }

        .gallery-overlay {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0,0,0,0.7);
            display: flex;
            align-items: center;
            justify-content: center;
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .gallery-item:hover .gallery-overlay {
            opacity: 1;
        }

        .gallery-title {
            color: white;
            font-size: 1.5rem;
            text-align: center;
        }

        /* Description */
        .description {
            background: white;
            padding: 80px 0;
        }

        .description-content {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
            font-size: 1.2rem;
            line-height: 1.8;
            color: #555;
        }

        .highlight {
            color: #d4a574;
            font-weight: bold;
        }

        /* Features */
        .features {
            background: #f5f5f5;
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }

        .feature-item {
            display: flex;
            align-items: center;
            background: white;
            padding: 20px;
            border-radius: 10px;
            transition: transform 0.3s ease;
        }

        .feature-item:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .feature-icon {
            font-size: 2rem;
            color: #d4a574;
            margin-right: 15px;
        }

        /* Contact */
        .contact {
            background: #333;
            color: white;
            text-align: center;
        }

        .contact-info {
            max-width: 600px;
            margin: 0 auto;
        }

        .contact-item {
            margin: 20px 0;
            font-size: 1.2rem;
        }

        /* Footer */
        footer {
            background: #222;
            color: white;
            text-align: center;
            padding: 40px 0;
        }

        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.6s ease;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero-title {
                font-size: 2.5rem;
            }
            
            .hero-subtitle {
                font-size: 1.2rem;
            }
            
            .price {
                font-size: 2rem;
            }
            
            nav ul {
                flex-direction: column;
                gap: 20px;
            }
            
            .info-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <nav>
        <div class="container">
            <ul>
                <li><a href="#accueil">Accueil</a></li>
                <li><a href="#propriete">Propriété</a></li>
                <li><a href="#galerie">Galerie</a></li>
                <li><a href="#caracteristiques">Caractéristiques</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </nav>

    <header id="accueil">
        <div class="hero-content">
            <h1 class="hero-title">Manoir d'Exception</h1>
            <p class="hero-subtitle">Allinges - Proche Genève et Lac Léman</p>
            <div class="price">1 400 000 €</div>
            <a href="#contact" class="btn">Nous Contacter</a>
        </div>
    </header>

    <section id="propriete" class="property-info">
        <div class="container">
            <h2 class="section-title">Informations Générales</h2>
            <div class="info-grid">
                <div class="info-card fade-in">
                    <div class="info-icon">🏠</div>
                    <div class="info-value">400 m²</div>
                    <div class="info-label">Surface Habitable</div>
                </div>
                <div class="info-card fade-in">
                    <div class="info-icon">🚪</div>
                    <div class="info-value">10 Pièces</div>
                    <div class="info-label">Chambres & Salons</div>
                </div>
                <div class="info-card fade-in">
                    <div class="info-icon">🌳</div>
                    <div class="info-value">7000 m²</div>
                    <div class="info-label">Parc Arboré</div>
                </div>
                <div class="info-card fade-in">
                    <div class="info-icon">📅</div>
                    <div class="info-value">XIXème</div>
                    <div class="info-label">Siècle</div>
                </div>
            </div>
        </div>
    </section>

    <section id="galerie" class="gallery">
        <div class="container">
            <h2 class="section-title">Galerie Photos</h2>
            <div class="image-grid">
                <div class="gallery-item fade-in">
                    <img src="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 400 300'><rect fill='%23d4a574' width='400' height='300'/><text x='200' y='150' text-anchor='middle' fill='white' font-size='20'>Façade Principale</text></svg>" alt="Façade du manoir">
                    <div class="gallery-overlay">
                        <div class="gallery-title">Façade Principale</div>
                    </div>
                </div>
                <div class="gallery-item fade-in">
                    <img src="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 400 300'><rect fill='%238b7355' width='400' height='300'/><text x='200' y='150' text-anchor='middle' fill='white' font-size='18'>Salon de Réception</text></svg>" alt="Salon de réception">
                    <div class="gallery-overlay">
                        <div class="gallery-title">Salon de Réception</div>
                    </div>
                </div>
                <div class="gallery-item fade-in">
                    <img src="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 400 300'><rect fill='%23a68b5b' width='400' height='300'/><text x='200' y='150' text-anchor='middle' fill='white' font-size='20'>Salle à Manger</text></svg>" alt="Salle à manger">
                    <div class="gallery-overlay">
                        <div class="gallery-title">Salle à Manger</div>
                    </div>
                </div>
                <div class="gallery-item fade-in">
                    <img src="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 400 300'><rect fill='%23c19960' width='400' height='300'/><text x='200' y='150' text-anchor='middle' fill='white' font-size='20'>Chambres Mansardées</text></svg>" alt="Chambres">
                    <div class="gallery-overlay">
                        <div class="gallery-title">Chambres Mansardées</div>
                    </div>
                </div>
                <div class="gallery-item fade-in">
                    <img src="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 400 300'><rect fill='%236b8e23' width='400' height='300'/><text x='200' y='150' text-anchor='middle' fill='white' font-size='20'>Parc de 7000 m²</text></svg>" alt="Parc">
                    <div class="gallery-overlay">
                        <div class="gallery-title">Parc de 7000 m²</div>
                    </div>
                </div>
                <div class="gallery-item fade-in">
                    <img src="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 400 300'><rect fill='%23556b2f' width='400' height='300'/><text x='200' y='150' text-anchor='middle' fill='white' font-size='18'>Vue sur le Domaine</text></svg>" alt="Vue domaine">
                    <div class="gallery-overlay">
                        <div class="gallery-title">Vue sur le Domaine</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section class="description">
        <div class="container">
            <h2 class="section-title">La Propriété</h2>
            <div class="description-content fade-in">
                <p>
                    <span class="highlight">Proche Genève et Lac Léman</span>, à 25 minutes de la frontière d'Anières, cette propriété de charme saura séduire les amoureux de la nature, du calme et des grands espaces.
                </p>
                <br>
                <p>
                    Elle date du <span class="highlight">19ème siècle</span>, est complètement rénovée (1990) et habitable. Sur environ <span class="highlight">400 m² de surface habitable</span> hors dépendances et annexes, toutes les pièces aux surfaces généreuses vous invitent à profiter au maximum de leurs destinations qui peuvent varier aux grés de vos envies et choix.
                </p>
                <br>
                <p>
                    Sur plus de <span class="highlight">7000 m² de terrain plat et majestueusement arboré</span>, la tranquillité sera votre alliée. Une annexe en entrée de la propriété d'environ 90 m² offre un joli potentiel de rénovation.
                </p>
            </div>
        </div>
    </section>

    <section id="caracteristiques" class="features">
        <div class="container">
            <h2 class="section-title">Caractéristiques</h2>
            <div class="features-grid">
                <div class="feature-item fade-in">
                    <div class="feature-icon">🏛️</div>
                    <div>
                        <h3>Architecture Historique</h3>
                        <p>Manoir du XIXème siècle entièrement rénové</p>
                    </div>
                </div>
                <div class="feature-item fade-in">
                    <div class="feature-icon">🔥</div>
                    <div>
                        <h3>Cheminées d'Époque</h3>
                        <p>Authentiques cheminées en pierre</p>
                    </div>
                </div>
                <div class="feature-item fade-in">
                    <div class="feature-icon">🌲</div>
                    <div>
                        <h3>Poutres Apparentes</h3>
                        <p>Charpente traditionnelle préservée</p>
                    </div>
                </div>
                <div class="feature-item fade-in">
                    <div class="feature-icon">🏞️</div>
                    <div>
                        <h3>Parc Paysager</h3>
                        <p>7000 m² de terrain plat et arboré</p>
                    </div>
                </div>
                <div class="feature-item fade-in">
                    <div class="feature-icon">🚗</div>
                    <div>
                        <h3>Proximité Genève</h3>
                        <p>25 minutes de la frontière suisse</p>
                    </div>
                </div>
                <div class="feature-item fade-in">
                    <div class="feature-icon">🔧</div>
                    <div>
                        <h3>Annexe 90 m²</h3>
                        <p>Potentiel de rénovation supplémentaire</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="contact" class="contact">
        <div class="container">
            <h2 class="section-title" style="color: white;">Contact</h2>
            <div class="contact-info">
                <div class="contact-item">
                    <strong>Prix :</strong> 1 400 000 €
                </div>
                <div class="contact-item">
                    📧 contact@immobilier-allinges.fr
                </div>
                <div class="contact-item">
                    📞 +33 (0)4 XX XX XX XX
                </div>
                <div class="contact-item">
                    📍 Allinges, Haute-Savoie, France
                </div>
                <br>
                <a href="mailto:contact@immobilier-allinges.fr" class="btn">Demander une Visite</a>
            </div>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2025 Manoir d'Allinges. Tous droits réservés.</p>
        </div>
    </footer>

    <script>
        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Fade in animation on scroll
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.fade-in').forEach(el => {
            observer.observe(el);
        });

        // Nav background on scroll
        window.addEventListener('scroll', () => {
            const nav = document.querySelector('nav');
            if (window.scrollY > 100) {
                nav.style.background = 'rgba(255,255,255,0.98)';
            } else {
                nav.style.background = 'rgba(255,255,255,0.95)';
            }
        });
    </script>
</body>
</html>
