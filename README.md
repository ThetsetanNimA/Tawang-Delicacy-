# Tawang-Delicacy-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tawang Delicacy - Authentic Tibetan Cuisine</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="icon" href="https://i.ibb.co/0jQYh8L/tawang-logo.png" type="image/png">
    <style>
        /* Basic styling to make it work without external CSS */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 2rem;
            background-color: #f8f8f8;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        .logo {
            display: flex;
            align-items: center;
        }
        .logo img {
            height: 50px;
            margin-right: 1rem;
        }
        .nav-links {
            display: flex;
            list-style: none;
        }
        .nav-links li a {
            padding: 0.5rem 1rem;
            text-decoration: none;
            color: #333;
        }
        .nav-links li a.active {
            font-weight: bold;
            color: #d14031;
        }
        .burger {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
        }
        .hero {
            background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), 
                        url('https://i.ibb.co/5K4ZxJX/tibetan-restaurant.jpg');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            color: white;
            text-align: center;
            padding: 8rem 1rem;
        }
        .btn {
            display: inline-block;
            padding: 0.8rem 1.5rem;
            margin: 0.5rem;
            border-radius: 4px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s ease;
        }
        .btn-primary {
            background-color: #d14031;
            color: white;
        }
        .btn-primary:hover {
            background-color: #b53528;
            transform: translateY(-2px);
        }
        .btn-secondary {
            background-color: white;
            color: #d14031;
            border: 1px solid #d14031;
        }
        .btn-secondary:hover {
            background-color: #d14031;
            color: white;
        }
        .btn-small {
            padding: 0.5rem 1rem;
            font-size: 0.9rem;
        }
        section {
            padding: 4rem 1rem;
            max-width: 1200px;
            margin: 0 auto;
        }
        h2 {
            text-align: center;
            margin-bottom: 3rem;
            color: #d14031;
            font-size: 2.5rem;
        }
        .dishes {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 2rem;
        }
        .dish {
            width: 350px;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }
        .dish:hover {
            transform: translateY(-10px);
        }
        .dish img {
            width: 100%;
            height: 250px;
            object-fit: cover;
        }
        .dish-info {
            padding: 1.5rem;
            background: white;
        }
        .dish-info h3 {
            font-size: 1.5rem;
            margin-bottom: 0.5rem;
            color: #d14031;
        }
        .dish-info p {
            margin-bottom: 1rem;
        }
        footer {
            background-color: #333;
            color: white;
            padding: 3rem 1rem;
            text-align: center;
        }
        .footer-content {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            max-width: 1200px;
            margin: 0 auto 2rem;
        }
        .footer-section {
            margin: 1rem;
            min-width: 200px;
        }
        .footer-section h3 {
            font-size: 1.3rem;
            margin-bottom: 1rem;
            color: #d14031;
        }
        .footer-section p {
            margin-bottom: 0.5rem;
        }
        .social-icons a {
            color: white;
            margin: 0 0.5rem;
            font-size: 1.5rem;
            transition: color 0.3s ease;
        }
        .social-icons a:hover {
            color: #d14031;
        }
        .copyright {
            border-top: 1px solid #444;
            padding-top: 1rem;
        }
        @media (max-width: 768px) {
            .nav-links {
                display: none;
                flex-direction: column;
                width: 100%;
                position: absolute;
                top: 80px;
                left: 0;
                background-color: #f8f8f8;
                padding: 1rem;
            }
            .nav-links.active {
                display: flex;
            }
            .burger {
                display: block;
            }
            .hero {
                padding: 6rem 1rem;
            }
            .hero-content h1 {
                font-size: 2.5rem;
            }
            .hero-content p {
                font-size: 1.2rem;
            }
            .footer-content {
                flex-direction: column;
                align-items: center;
            }
        }
        @media (max-width: 480px) {
            .hero-content h1 {
                font-size: 2rem;
            }
            .featured h2 {
                font-size: 2rem;
            }
            .dish {
                width: 100%;
            }
        }
    </style>
</head>
<body>
    <!-- Navigation Bar -->
    <nav>
        <div class="logo">
            <img src="https://i.ibb.co/0jQYh8L/tawang-logo.png" alt="Tawang Delicacy Logo">
            <h1>Tawang Delicacy</h1>
        </div>
        <ul class="nav-links">
            <li><a href="index.html" class="active">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="about.html">About</a></li>
            <li><a href="contact.html">Contact</a></li>
        </ul>
        <div class="burger">
            <i class="fas fa-bars"></i>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-content">
            <h1>Authentic Tibetan Flavors</h1>
            <p>Experience the taste of the Himalayas</p>
            <div class="cta-buttons">
                <a href="menu.html" class="btn btn-primary">Order Now</a>
                <a href="tel:+1234567890" class="btn btn-secondary">
                    <i class="fas fa-phone"></i> Call Us
                </a>
            </div>
        </div>
    </section>

    <!-- Featured Dishes -->
    <section class="featured">
        <h2>Our Specialties</h2>
        <div class="dishes">
            <div class="dish">
                <img src="https://i.ibb.co/7YfG1qy/tibetan-momos.jpg" alt="Tibetan Momos">
                <div class="dish-info">
                    <h3>Tibetan Momos</h3>
                    <p>Steamed dumplings with savory fillings</p>
                    <a href="menu.html#momos" class="btn btn-small btn-primary">View Details</a>
                </div>
            </div>
            <div class="dish">
                <img src="https://i.ibb.co/6nLJQqF/thukpa-noodle-soup.jpg" alt="Thukpa">
                <div class="dish-info">
                    <h3>Thukpa</h3>
                    <p>Hearty noodle soup with vegetables</p>
                    <a href="menu.html#thukpa" class="btn btn-small btn-primary">View Details</a>
                </div>
            </div>
            <div class="dish">
                <img src="https://i.ibb.co/9HqJZ0Q/tibetan-laphing.jpg" alt="Laphing">
                <div class="dish-info">
                    <h3>Laphing</h3>
                    <p>Spicy cold mung bean noodle dish</p>
                    <a href="menu.html#laphing" class="btn btn-small btn-primary">View Details</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="footer-content">
            <div class="footer-section">
                <h3>Hours</h3>
                <p>Monday - Sunday</p>
                <p>11:00 AM - 10:00 PM</p>
            </div>
            <div class="footer-section">
                <h3>Contact</h3>
                <p><i class="fas fa-phone"></i> +1 (234) 567-890</p>
                <p><i class="fas fa-envelope"></i> info@tawangdelicacy.com</p>
                <p><i class="fas fa-map-marker-alt"></i> 123 Himalayan St, Tawang</p>
            </div>
            <div class="footer-section">
                <h3>Follow Us</h3>
                <div class="social-icons">
                    <a href="#" aria-label="Facebook"><i class="fab fa-facebook"></i></a>
                    <a href="#" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
                    <a href="#" aria-label="WhatsApp"><i class="fab fa-whatsapp"></i></a>
                </div>
            </div>
        </div>
        <div class="copyright">
            <p>&copy; <span id="year"></span> Tawang Delicacy. All rights reserved.</p>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        document.querySelector('.burger').addEventListener('click', function() {
            document.querySelector('.nav-links').classList.toggle('active');
        });

        // Update copyright year
        document.getElementById('year').textContent = new Date().getFullYear();

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth'
                    });
                }
            });
        });
    </script>
</body>
</html>
