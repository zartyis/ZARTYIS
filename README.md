<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Échange de services entre particuliers">
    <title>Échange de Services</title>
    <link rel="webside icon" type="jpg"
    href="https://img.freepik.com/premium-vector/customer-service-icon-vector-full-customer-care-service-hand-with-persons-vector-illustration_399089-2810.jpg?w=2000">
    <style>
        body { 
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
        }
        header {
            background-color: #4CAF50;
            color: white;
            padding: 10px 0;
            text-align: center;
        }
        nav {
            background-color: #333;
            color: white;
            padding: 10px;
            display: flex;
            justify-content: center;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
        }
        .container {
            max-width: 1200px;
            margin: 20px auto;
            padding: 20px;
        }
        h1, h2 {
            text-align: center;
        }
        .service-list, .offer-form {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
        }
        .service-card, .form-card {
            background-color: white;
            padding: 20px;
            margin: 10px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            flex-basis: 30%;
            box-sizing: border-box;
        }
        .service-card h3 {
            margin-top: 0;
        }
        .offer-form input, .offer-form textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 4px;
        
        }
        .button {
            background-color: #4CAF50;
            color: white;
            border: none;
            padding: 10px 20px;
            cursor: pointer;
            border-radius: 4px;
            text-align: center;
        }
        .button:hover {
            background-color: #45a049;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            margin-top: 30px;
        }
        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        
    </style>
</head>
<body>

    <header>
        <h1>Échange de Services</h1>
        <p>Proposez un service et échangez-le avec un autre membre !</p>
    </header>

    <nav>
        <a href="#home">Accueil</a>
        <a href="#services">Services</a>
        <a href="#offer">Proposer un Service</a>
        <a href="#contact">Contact</a>
    </nav>

    <div class="container" id="home">
        <h2>Bienvenue sur la plateforme d'échange de services</h2>
        <p>Rejoignez notre communauté et commencez à échanger des services gratuitement ! Vous pouvez offrir vos compétences et recevoir des services en retour. Trouvez des solutions locales et simplifiez votre quotidien.</p>
    </div>

                <div class="service-card">
                <h3>Nettoyage de maison</h3>
                <p>Proposez un nettoyage complet de maison, cuisine, salle de bain, etc.</p>
                <button class="button" onclick="rediriger()">Demander ce service</button></div>
                </div>
            <div class="service-card">
                <h3>Cours de guitare</h3>
                <p>Vous avez une passion pour la musique ? Proposez des cours particuliers de guitare !</p>
                <button class="button" onclick="demanderService('Cours de guitare')">Demander ce service</button>
            </div>
            <div class="service-card">
                <h3>Jardinage</h3>
                <p>Besoin d'aide pour entretenir votre jardin ? Proposez des services de jardinage et d'aménagement paysager.</p>
                <button class="button" onclick="demanderService('Jardinage')">Demander ce service</button>
            </div>
            <div class="service-card">
                <h3>Aide aux devoirs</h3>
                <p>Aidez les étudiants avec leurs devoirs dans diverses matières : mathématiques, langues, sciences.</p>
                <button class="button" onclick="demanderService('Aide aux devoirs')">Demander ce service</button>
            </div>
            <div class="service-card">
                <h3>Réparations diverses</h3>
                <p>Proposez des services pour réparer des objets dans la maison : électroménager, meubles, petits appareils.</p>
                <button class="button" onclick="demanderService('Réparations diverses')">Demander ce service</button>
            </div>
            <div class="service-card">
                <h3>Livraison locale</h3>
                <p>Proposez des services de livraison pour des petits colis ou des courses locales.</p>
                <button class="button" onclick="demanderService('Livraison locale')">Demander ce service</button>
            </div>
            <div class="service-card">
                <h3>Design graphique</h3>
                <p>Vous êtes créatif ? Proposez des services de design pour logos, cartes de visite, affiches et plus.</p>
                <button class="button" onclick="demanderService('Design graphique')">Demander ce service</button>
            </div>
            <div class="service-card">
                <h3>Cuisine à domicile</h3>
                <p>Proposez vos talents culinaires pour préparer des repas à domicile pour des événements ou des particuliers.</p>
                <button class="button" onclick="demanderService('Cuisine à domicile')">Demander ce service</button>
            </div>
            <!-- Nouveaux services ajoutés -->
            <div class="service-card">
                <h3>Assistance informatique</h3>
                <p>Proposez votre aide pour résoudre des problèmes informatiques, installer des logiciels ou dépanner des appareils.</p>
                <button class="button" onclick="demanderService('Assistance informatique')">Demander ce service</button>
            </div>
            <div class="service-card">
                <h3>Photographie</h3>
                <p>Services de photographie pour événements, portraits ou même des shootings photo personnalisés.</p>
                <button class="button" onclick="demanderService('Photographie')">Demander ce service</button>
            </div>
            <div class="service-card">
                <h3>Traduction</h3>
                <p>Proposez des services de traduction pour divers documents ou conversations dans plusieurs langues.</p>
                <button class="button" onclick="demanderService('Traduction')">Demander ce service</button>
            </div>
            <div class="service-card">
                <h3>Coaching sportif</h3>
                <p>Proposez des séances de coaching sportif, de fitness ou même des conseils nutritionnels.</p>
                <button class="button" onclick="demanderService('Coaching sportif')">Demander ce service</button>
            </div>
            <div class="service-card">
                <h3>Massage bien-être</h3>
                <p>Offrez des services de massage bien-être ou de relaxation à domicile pour soulager le stress et la fatigue.</p>
                <button class="button" onclick="demanderService('Massage bien-être')">Demander ce service</button>
            </div>
            <div class="service-card">
                <h3>Consultation en développement personnel</h3>
                <p>Offrez des services de coaching en développement personnel pour aider les gens à mieux gérer leur vie.</p>
                <button class="button" onclick="demanderService('Consultation en développement personnel')">Demander ce service</button>
            </div>
            <div class="service-card">
                <h3>Organisation d'événements</h3>
                <p>Proposez des services pour organiser des événements comme des mariages, des fêtes d'anniversaire, des séminaires, etc.</p>
                <button class="button" onclick="demanderService('Organisation d\'événements')">Demander ce service</button>
            </div>
            <div class="service-card">
                <h3>Consultation juridique</h3>
                <p>Proposez des conseils juridiques pour des contrats, des litiges ou des questions liées au droit.</p>
                <button class="button" onclick="demanderService('Consultation juridique')">Demander ce service</button>
            </div>
            <div class="service-card">
                <h3>Services de réparation automobile</h3>
                <p>Proposez des services de réparation automobile comme le changement de pneus, révision moteur, ou entretien général des véhicules.</p>
                <button class="button" onclick="demanderService('Services de réparation automobile')">Demander ce service</button>
            </div>
            
        </div>
    </div>

    <div class="container" id="contact">
        <h2>Contactez-nous</h2>
        <form class="contact-form" id="contactForm" onsubmit="return envoyerMessage(event)">
            <label for="name">Votre Nom :</label>
            <input type="text" id="name" name="name" required>

            <label for="email">Votre Email :</label>
            <input type="email" id="email" name="email" required>

            <label for="message">Votre Message :</label>
            <textarea id="message" name="message" rows="4" required></textarea>

            <input class="button" type="submit" value="Envoyer Message">
        </form>
    </div>
    <script>
        // Fonction pour demander un service et rediriger vers la page du service
        function demanderService(service) {
            // Vous pouvez définir ici les pages de redirection spécifiques pour chaque service
            let pageURL = '';
            
            switch (service) {
                case 'Nettoyage de maison':
                    pageURL = ''; 
                    break;
                case 'Cours de guitare':
                    pageURL = '';  
                    break;
                case 'Jardinage':
                    pageURL = '';    
                    break;
                case 'Aide aux devoirs':
                    pageURL = '';
                    break;
                case 'Réparations diverses':
                    pageURL = '';  
                    break;
                case 'Livraison locale':
                    pageURL = '';  
                    break;
                case 'Design graphique':
                    pageURL = '';   
                    break;
                case 'Cuisine à domicile':
                    pageURL = '';     
                    break;
                case 'Assistance informatique':
                    pageURL = '';  
                    break;
                case 'Photographie':
                    pageURL = '';  
                    break;
                case 'Traduction':
                    pageURL = '';  
                    break;
                case 'Coaching sportif':
                    pageURL = '';  
                case 'Massage bien-être':
                    pageURL = '';  
                    break;
                case 'Consultation en développement personnel':
                    pageURL = '';  
                    break; 
                case 'Organisation d"événements':
                    pageURL = '';  
                    break;  
                case 'Consultation juridique':
                    pageURL = '';  
                    break;  
                case 'Services de réparation automobile':
                    pageURL = ''; 
                    break;
                
            }
    
            // Effectuer la redirection vers la page du service
            window.location.href =pageURL;
        }
    </script>
    
       
    
     
    <footer>
        <p>&copy; 2025 Échange de Services - Tous droits réservés</p>
    </footer>

    <script>
            // Fonction pour demander un service
            function demanderService(service) {
            alert("Vous avez demandé le service : " + service);
        }

        // Fonction pour soumettre une annonce
        function soumettreAnnonce(event) {
            event.preventDefault();  // Empêche l'envoi classique du formulaire

            // Récupération des valeurs du formulaire
            const serviceName = document.getElementById('service-name').value;
            const description = document.getElementById('description').value;
            const location = document.getElementById('location').value;
            const availability = document.getElementById('availability').value;

            // Vous pouvez ajouter ici la logique pour soumettre l'annonce (par exemple, sauvegarder dans une base de données ou envoyer par email)

            // Pour l'instant, affichons les valeurs dans une alerte
            alert("Annonce soumise !\n\nService : " + serviceName + "\nDescription : " + description + "\nLocalisation : " + location + "\nDisponibilité : " + availability);

            // Réinitialiser le formulaire après la soumission
            document.getElementById('serviceForm').reset();
        }

        // Fonction pour envoyer un message via le formulaire de contact
        function envoyerMessage(event) {
            event.preventDefault();  // Empêche l'envoi classique du formulaire

            // Récupération des valeurs du formulaire de contact
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            const message = document.getElementById('message').value;

            // Vous pouvez ajouter ici la logique pour soumettre le message (par exemple, envoyer l'email ou sauvegarder dans une base de données)

            // Pour l'instant, affichons les valeurs dans une alerte
            alert("Message envoyé !\n\nNom : " + name + "\nEmail : " + email + "\nMessage : " + message);

            // Réinitialiser le formulaire de contact après la soumission
            document.getElementById('contactForm').reset();
        }
     
