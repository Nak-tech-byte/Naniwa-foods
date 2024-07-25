
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Naniwa Foods</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <!-- Styling of website, this section of code adds aesthetics to the website -->
    <style>
        /* General styles */
        body {
            background-image: url("cooking.jpeg");
            background-size: cover;
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 20px;
            transition: background-color 0.5s, color 0.5s;
        }

        body.dark-theme {
            background-color: #11418a;
            color: #000000;
        }

        /* Navigation menu styles */
        nav ul {
            list-style-type: none;
            padding: 0;
            margin: 0;
            background-color: rgba(106, 9, 126, 0.5);
            display: flex;
            justify-content: space-around;
            backdrop-filter: blur(5px);
            border-radius: 10px;
            animation: fadeIn 1s ease-in-out;
        }

        nav ul li {
            margin: 0;
            padding: 10px;
        }

        nav ul li a {
            display: block;
            padding: 10px 20px;
            color: inherit;
            text-decoration: none;
            background-color: #199743;
            transition: background-color 0.3s, color 0.3s;
            border-radius: 5px;
        }

        nav ul li a:hover {
            background-color: #555;
            color: rgb(55, 137, 192);
        }

        /* Styles for elements in the dark theme */
        body.dark-theme nav ul {
            background-color: rgba(86, 97, 194, 0.1);
        }

        body.dark-theme nav ul li a {
            background-color: #350e7e;
            color: #1c9462;
        }

        body.dark-theme nav ul li a:hover {
            background-color: #666;
            color: rgb(68, 226, 108);
        }

        /* Additional styles for restaurant aesthetics */
        h1, h2, h3 {
            text-align: center;
            margin: 20px 0;
        }

        p {
            text-align: center;
        }

        #makeReservations {
            display: block;
            margin: 20px auto;
            padding: 10px 20px;
            background-color: #333;
            color: #28e617;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s, color 0.3s;
        }

        #makeReservations:hover {
            background-color: #555;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.8);
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            animation: slideIn 1s ease-in-out;
        }

        .menu-section img {
            display: block;
            margin: 0 auto;
            max-width: 100%;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(8, 167, 145, 0.2);
        }

        .menu-section {
            margin: 20px 0;
        }

        .menu-section h2 {
            margin-bottom: 10px;
        }

        .food-gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .food-gallery img {
            max-width: 300px;
            margin: 10px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(195, 216, 5, 0.2);
            transition: transform 0.3s;
        }

        .food-gallery img:hover {
            transform: scale(1.1);
        }

        /* Carousel styles */
        .carousel-inner img {
            width: 100%;
            height: 100%;
        }

        /* Social media icons */
        .social-icons {
            display: flex;
            justify-content: center;
            margin-top: 20px;
        }

        .social-icons a {
            margin: 0 10px;
            color: #333;
            font-size: 24px;
            transition: color 0.3s;
        }

        .social-icons a:hover {
            color: #555;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }

        @keyframes slideIn {
            from {
                transform: translateY(20px);
                opacity: 0;
            }
            to {
                transform: translateY(0);
                opacity: 1;
            }
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav>
        <ul>
            <li><a href="#makeReservations">Make Reservations</a></li>
            <li><a href="#Address">Address</a></li>
            <li><a href="#Menu">Menu</a></li>
            <li><a href="#Drinks">Drinks</a></li>
            <li><a href="#Gallery">Gallery</a></li>
            <li><a href="#Contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Dark theme toggle button -->
    <button id="themeButton">Naniwa foods</button>

    <!-- Welcome Section -->
    <div class="container" id="Address">
        <h1>Welcome to Naniwa Foods</h1>
        <p>1020 Lavida St, Lala Land<br>
            Opening Hours: Everyday: 11 AM - 12 AM
        </p>
        <div class="Team shape">
            <img src="team-shape.svg" alt="Team shape">
        </div>
    </div>

    <!-- Carousel Section -->
    <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
        <ol class="carousel-indicators">
            <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
            <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
            <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
        </ol>
        <div class="carousel-inner">
            <div class="carousel-item active">
                <img class="d-block w-100" src="menu-item-4.png" alt="First slide">
            </div>
            <div class="carousel-item">
                <img class="d-block w-100" src="menu-item-6.png" alt="Second slide">
            </div>
            <div class="carousel-item">
                <img class="d-block w-100" src="menu-item-1.png" alt="Third slide">
            </div>
        </div>
        <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Previous</span>
        </a>
        <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Next</span>
        </a>
    </div>

    <!-- Menu Section -->
    <div class="container menu-section" id="Menu">
        <h2>Menu</h2>
        <h3>Lunch</h3>
        <h3>Dinner</h3>
        <p>Consuming Raw or Undercooked Meats, Poultry, Seafood, Shellfish, or Eggs May increase your risk of Foodborne Illness.</p>
        <div class="food-gallery">
            <img src="menu-item-2.png" alt="Menu item 1">
            <img src="OIP.jpeg" alt="Menu item 2">
            <img src="menu-item-3.png" alt="Menu item 3">
        </div>
    </div>

    <!-- Drinks Section -->
    <div class="container menu-section" id="Drinks">
        <h2>Drinks</h2>
        <h3>Beer</h3>
        <h3>Wine</h3>
        <h3>Cocktails</h3>
        <h3>Spirits</h3>
        <p>There are a variety of drinks available in our restaurant.</p>
        <div class="food-gallery">
            <img src="drink 2.jpeg" alt="Drink item 1">
            <img src="drink.jpeg" alt="Drink item 2">
        </div>
    </div>

    <!-- Gallery Section -->
    <div class="container menu-section" id="Gallery">
        <h2>Gallery</h2>
        <div class="food-gallery">
            <img src="gallery-8.jpg" alt="Gallery item 1">
            <img src="gallery-7.jpg" alt="Gallery item 2">
            <img src="gallery-6.jpg" alt="Gallery item 3">
            <img src="gallery-5.jpg" alt="Gallery item 4">
        </div>
    </div>

    <!-- Contact Section -->
    <div class="container menu-section" id="Contact">
        <h2>Contact</h2>
        <p>For reservations, please call (123) 456-7890 or email us at reservations@naniwafoods.com.</p>
        <div class="social-icons">
            <a href="#"><i class="fab fa-facebook-f"></i></a>
            <a href="#"><i class="fab fa-twitter"></i></a>
            <a href="#"><i class="fab fa-instagram"></i></a>
            <a href="#"><i class="fab fa-linkedin-in"></i></a>
        </div>
    </div>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.2/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
    <script>
        document.getElementById("themeButton").addEventListener("click", function() {
            document.body.classList.toggle("dark-theme");
        });
    </script>
</body>
</html>
