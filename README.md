<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>E.E.A.C Pain de Vie - Site Officiel</title>
    
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

    <style>
        /* --- CSS INTÉGRÉ --- */
        :root {
            --primary-color: #2c3e50;
            --secondary-color: #e67e22;
            --text-light: #ffffff;
            --bg-light: #f4f4f4;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        html { scroll-behavior: smooth; }

        body { line-height: 1.6; color: #333; }

        /* Navigation */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 5%;
            background: var(--primary-color);
            color: white;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .logo { font-weight: 700; font-size: 1.5rem; }

        .nav-links { display: flex; list-style: none; }

        .nav-links li a {
            color: white;
            text-decoration: none;
            margin-left: 20px;
            transition: 0.3s;
        }

        .nav-links li a:hover { color: var(--secondary-color); }

        /* Hero Section */
        .hero {
            height: 100vh;
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), 
                        url('https://images.unsplash.com/photo-1544427928-c49cdcd8533d?q=80&w=2000') no-repeat center center/cover;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            padding: 0 20px;
        }

        .hero h1 { font-size: 3rem; margin-bottom: 1rem; }
        .hero p { font-size: 1.2rem; margin-bottom: 2rem; }

        /* Sections */
        section { padding: 100px 10%; text-align: center; }
        .bg-light { background: var(--bg-light); }
        h2 { margin-bottom: 30px; position: relative; padding-bottom: 10px; }
        h2::after {
            content: '';
            width: 50px; height: 3px; background: var(--secondary-color);
            position: absolute; bottom: 0; left: 50%; transform: translateX(-50%);
        }

        /* Grille Réalisations */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
        }

        .card {
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        /* Tableau Programme */
        .table-container { overflow-x: auto; }
        table { width: 100%; border-collapse: collapse; margin-top: 20px; background: white; }
        th, td { padding: 15px; border: 1px solid #ddd; text-align: left; }
        th { background: var(--primary-color); color: white; }

        /* Formulaire */
        form { max-width: 600px; margin: auto; display: grid; gap: 15px; }
        input, textarea { padding: 12px; border: 1px solid #ccc; border-radius: 5px; width: 100%; }
        
        .btn {
            background: var(--secondary-color);
            color: white;
            padding: 12px 25px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
            transition: 0.3s;
        }
        .btn:hover { background: #d35400; }

        /* Footer */
        footer { background: #1a252f; color: white; padding: 20px; text-align: center; }

        /* Responsive */
        @media (max-width: 768px) {
            .nav-links { display: none; }
            .hero h1 { font-size: 2rem; }
        }
    </style>
</head>
<body>

    <nav>
        <div class="logo">E.E.A.C Pain de Vie</div>
        <ul class="nav-links">
            <li><a href="#accueil">Accueil</a></li>
            <li><a href="#apropos">À Propos</a></li>
            <li><a href="#historique">Historique</a></li>
            <li><a href="#realisation">Réalisations</a></li>
            <li><a href="#programme">Programme</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <header id="accueil" class="hero">
        <h1>E.E.A.C Pain de Vie</h1>
        <p>Une communauté de foi, d'espoir et d'amour.</p>
        <a href="#programme" class="btn">Nos Programmes</a>
    </header>

    <section id="apropos">
        <h2>À Propos de Nous</h2>
        <p>L'Église Évangélique de l'Alliance Chrétienne (E.E.A.C) "Pain de Vie" est un lieu de rencontre avec Dieu. Nous croyons en la puissance de la parole transformatrice de Jésus-Christ.</p>
    </section>

    <section id="historique" class="bg-light">
        <h2>Notre Historique</h2>
        <p>Depuis sa création, l'église a œuvré pour l'épanouissement spirituel de ses membres. Née d'une vision d'évangélisation profonde, elle continue de croître par la grâce de Dieu.</p>
    </section>

    <section id="realisation">
        <h2>Nos Réalisations</h2>
        <div class="grid">
            <div class="card">
                <h3>Temple Moderne</h3>
                <p>Achèvement des travaux de rénovation de notre sanctuaire principal.</p>
            </div>
            <div class="card">
                <h3>Actions Sociales</h3>
                <p>Distribution de vivres et soutien scolaire aux enfants du quartier.</p>
            </div>
            <div class="card">
                <h3>École de Dimanche</h3>
                <p>Mise en place d'un programme éducatif biblique pour les plus jeunes.</p>
            </div>
        </div>
    </section>

    <section id="programme" class="bg-light">
        <h2>Programme du Culte</h2>
        <div class="table-container">
            <table>
                <thead>
                    <tr>
                        <th>Jour</th>
                        <th>Heure</th>
                        <th>Activité</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Dimanche</td>
                        <td>08h30 - 11h30</td>
                        <td>Culte Dominical</td>
                    </tr>
                    <tr>
                        <td>Mercredi</td>
                        <td>17h00 - 18h30</td>
                        <td>Enseignements Bibliques</td>
                    </tr>
                    <tr>
                        <td>Vendredi</td>
                        <td>16h30 - 18h30</td>
                        <td>Prière de Puissance</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </section>

    <section id="contact">
        <h2>Contactez-nous</h2>
        <form id="church-contact">
            <input type="text" placeholder="Votre Nom complet" required>
            <input type="email" placeholder="Votre Email" required>
            <textarea rows="5" placeholder="Votre message ou demande de prière" required></textarea>
            <button type="submit" class="btn">Envoyer le message</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2024 E.E.A.C Pain de Vie - Tous droits réservés.</p>
    </footer>

    <script>
        // --- JS INTÉGRÉ ---
        document.getElementById('church-contact').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Merci ! Votre message a été envoyé à l\'administration de l\'église Pain de Vie.');
            this.reset();
        });

        // Animation de scroll douce pour les liens
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
