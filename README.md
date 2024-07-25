!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
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
    <title>Naniwa Foods</title>
</head>
<body>
    <nav>
        <ul>
            <li><a href="#makeReservations">Make Reservations</a></li>
            <li><a href="#Address">Address</a></li>
            <li><a href="#Menu">Menu</a></li>
            <li><a href="#Drinks">Drinks</a></li>
            <li><a href="#Gallery">Gallery</a></li>
        </ul>
    </nav>

    <button id="themeButton">Naniwa Foods</button>

    <div class="container" id="Address">
        <h1>Welcome to Naniwa Foods</h1>
        <p>1020 Lavida St, Lala Land</p>
        <div class="Team shape">
            <img src="team-shape.svg" alt="Team shape">
    </div>

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

    <div class="container menu-section" id="Drinks">
        <h2>Drinks</h2>
        <h3>Beer</h3>
        <h3>Wine</h3>
        <h3>Cocktails</h3>
        <h3>Spirits</h3>
        <p>There are a variety of drinks available in our restaurant.</p>
        <div class="Drinks">
            <img src="drink 2.jpeg" alt="Menu item 1">
            <img src="drink.jpeg" alt="Menu item 2">
    </div>

    <div class="container menu-section" id="Gallery">
        <h2>Gallery</h2>
        <div class="food-gallery">
            <img src="gallery-8.jpg" alt="gallery 1">
            <img src="gallery-7.jpg" alt="gallery 2">
            <img src="events-4.jpg" alt="about"
        </div>
    </div>

    <script>
        document.getElementById('themeButton').addEventListener('click', function() {
            document.body.classList.toggle('dark-theme');
        });
    </script>
</body>
</html>
