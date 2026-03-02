<index html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Colony Brew | Faizabad</title>
    <style>
        /* --- CSS STYLES --- */
        :root {
            --primary: #6F4E37; /* Coffee Brown */
            --secondary: #C0A080; /* Latte */
            --dark: #2c2c2c;
            --light: #f9f9f9;
            --white: #ffffff;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--light);
            color: var(--dark);
            line-height: 1.6;
        }

        /* Navigation */
        nav {
            background: var(--white);
            padding: 1rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--primary);
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--dark);
            margin-left: 2rem;
            font-weight: 500;
            transition: 0.3s;
        }

        .nav-links a:hover {
            color: var(--primary);
        }

        /* Hero Section */
        .hero {
            height: 80vh;
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('https://images.unsplash.com/photo-1509042239860-f550ce710b93?ixlib=rb-1.2.1&auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: var(--white);
            padding: 0 20px;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            max-width: 600px;
        }

        .btn {
            padding: 12px 30px;
            background-color: var(--primary);
            color: var(--white);
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
            transition: 0.3s;
        }

        .btn:hover {
            background-color: var(--secondary);
        }

        /* Sections General */
        section {
            padding: 4rem 5%;
            text-align: center;
        }

        h2 {
            color: var(--primary);
            margin-bottom: 3rem;
            font-size: 2.5rem;
        }

        /* Menu Section */
        .menu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .menu-item {
            background: var(--white);
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s;
        }

        .menu-item:hover {
            transform: translateY(-5px);
        }

        .price {
            color: var(--primary);
            font-weight: bold;
            font-size: 1.2rem;
            display: block;
            margin-top: 10px;
        }

        /* About Section */
        .about-container {
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            justify-content: center;
            gap: 2rem;
        }

        .about-img {
            flex: 1;
            min-width: 300px;
        }

        .about-img img {
            width: 100%;
            border-radius: 10px;
        }

        .about-text {
            flex: 1;
            min-width: 300px;
            text-align: left;
        }

        /* Gallery */
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1rem;
        }

        .gallery-grid img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            border-radius: 8px;
            transition: 0.3s;
        }

        .gallery-grid img:hover {
            opacity: 0.8;
        }

        /* Contact Section */
        .contact-info {
            background-color: var(--white);
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            max-width: 600px;
            margin: 0 auto;
        }

        .map-btn {
            display: inline-block;
            margin-top: 1rem;
            background-color: #db4437;
            color: white;
            padding: 10px 20px;
            text-decoration: none;
            border-radius: 4px;
        }

        /* Footer */
        footer {
            background-color: var(--dark);
            color: var(--white);
            text-align: center;
            padding: 2rem;
            margin-top: 2rem;
        }

        /* Mobile Responsive */
        @media (max-width: 768px) {
            .hero h1 { font-size: 2.5rem; }
            .nav-links { display: none; } /* Simple hide for mobile example */
        }
    </style>
</head>
<body>

    <!-- Navigation -->
    <nav>
        <div class="logo">Colony Brew</div>
        <div class="nav-links">
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#menu">Menu</a>
            <a href="#gallery">Gallery</a>
            <a href="#contact">Contact</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <h1>Colony Brew</h1>
        <p>The best coffee and snacks in Tilak Nagar Colony, Faizabad. A cozy place to hang out with friends.</p>
        <a href="#menu" class="btn">View Menu</a>
    </section>

    <!-- About Section -->
    <section id="about">
        <h2>About Us</h2>
        <div class="about-container">
            <div class="about-img">
                <img src="https://images.unsplash.com/photo-1554118811-1e0d58224f24?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Cafe Interior">
            </div>
            <div class="about-text">
                <h3>Welcome to Colony Brew</h3>
                <p>Located in the heart of Tilak Nagar Colony, Janoura, we serve the finest coffee, authentic Indian chai, and delicious snacks. Whether you are looking for a quiet corner to work or a lively space to catch up with friends, Colony Brew is the perfect spot.</p>
            </div>
        </div>
    </section>

    <!-- Menu Section -->
    <section id="menu" style="background-color: #f0f0f0;">
        <h2>Our Menu</h2>
        <div class="menu-grid">
            <div class="menu-item">
                <h3>Masala Chai</h3>
                <p>Traditional Indian spiced tea.</p>
                <span class="price">₹20</span>
            </div>
            <div class="menu-item">
                <h3>Hot Coffee</h3>
                <p>Rich and creamy filter coffee.</p>
                <span class="price">₹40</span>
            </div>
            <div class="menu-item">
                <h3>Cappuccino</h3>
                <p>Espresso with steamed milk foam.</p>
                <span class="price">₹80</span>
            </div>
            <div class="menu-item">
                <h3>Veg Sandwich</h3>
                <p>Toasted bread with fresh veggies.</p>
                <span class="price">₹50</span>
            </div>
            <div class="menu-item">
                <h3>Samosa</h3>
                <p>Crispy pastry with spiced potatoes.</p>
                <span class="price">₹30</span>
            </div>
            <div class="menu-item">
                <h3>Chocolate Lava Cake</h3>
                <p>Warm cake with melted chocolate center.</p>
                <span class="price">₹90</span>
            </div>
        </div>
    </section>

    <!-- Gallery Section -->
    <section id="gallery">
        <h2>Gallery</h2>
        <div class="gallery-grid">
            <img src="https://images.unsplash.com/photo-1495474472287-4d71bcdd2085?ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=80" alt="Coffee 1">
            <img src="https://images.unsplash.com/photo-1511920170033-f8396924c348?ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=80" alt="Cafe Seating">
            <img src="https://images.unsplash.com/photo-1521017432531-fbd92d768814?ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=80" alt="Pastries">
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2>Contact & Location</h2>
        <div class="contact-info">
            <h3>Visit Us</h3>
            <p><strong>Address:</strong><br>
            Tilak Nagar Colony, Janoura, Karaundia,<br>
            Faizabad, Uttar Pradesh 224001</p>
            
            <br>
            <p><strong>Hours:</strong><br>
            Open Daily: 8:00 AM - 10:00 PM</p>

            <br>
            <a href="https://maps.google.com/?q=Tilak+Nagar+Colony+Janoura+Karaundia+Faizabad" target="_blank" class="map-btn">Get Directions</a>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2023 Colony Brew. All Rights Reserved.</p>
    </footer>

    <script>
        // Simple smooth scrolling script
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
