<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cafe Adam</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }
        header {
            background-color: #8B4513; /* Brown for cafe theme */
            color: white;
            padding: 1rem;
            text-align: center;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 100;
        }
        nav ul {
            list-style: none;
            padding: 0;
            margin: 0;
        }
        nav ul li {
            display: inline;
            margin: 0 1rem;
        }
        nav a {
            color: white;
            text-decoration: none;
        }
        .hero {
            background-image: url('https://images.unsplash.com/photo-1509042239860-f550ce710b93?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80'); /* Cafe interior */
            background-size: cover;
            background-position: center;
            height: 60vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            margin-top: 80px; /* Account for fixed header */
        }
        .hero h1 {
            font-size: 3rem;
            margin: 0;
        }
        .menu {
            padding: 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }
        .menu h2 {
            text-align: center;
            margin-bottom: 2rem;
        }
        .menu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1rem;
        }
        .menu-item {
            background: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            text-align: center;
            transition: transform 0.3s;
        }
        .menu-item:hover {
            transform: scale(1.05);
        }
        .menu-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        .menu-item h3 {
            margin: 1rem 0;
        }
        .menu-item p {
            margin: 0 1rem 1rem;
            font-weight: bold;
        }
        /* Category-based colors */
        .drinks-hot { border-top: 5px solid #D2691E; background: linear-gradient(to bottom, #FFF8DC, white); } /* Warm for hot drinks */
        .drinks-cold { border-top: 5px solid #4682B4; background: linear-gradient(to bottom, #E0F6FF, white); } /* Cool for cold drinks */
        .food-savory { border-top: 5px solid #32CD32; background: linear-gradient(to bottom, #F0FFF0, white); } /* Green for savory food */
        .food-dessert { border-top: 5px solid #FF69B4; background: linear-gradient(to bottom, #FFF0F5, white); } /* Pink for desserts */
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1rem;
        }
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2rem;
            }
            .menu-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Cafe Adam</h1>
        <nav>
            <ul>
                <li><a href="#hero">Home</a></li>
                <li><a href="#menu">Menu</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero" id="hero">
        <div>
            <h1>Welcome to Cafe Adam</h1>
            <p>Enjoy the finest coffee, tea, and more in a cozy atmosphere.</p>
        </div>
    </section>

    <section class="menu" id="menu">
        <h2>Our Menu</h2>
        <div class="menu-grid">
            <div class="menu-item drinks-hot">
                <img src="https://images.unsplash.com/photo-1497935586351-b67a49e012bf?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80" alt="Espresso">
                <h3>Espresso</h3>
                <p>$3.50</p>
            </div>
            <div class="menu-item drinks-hot">
                <img src="https://images.unsplash.com/photo-1572442388796-11668a67e53d?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80" alt="Cappuccino">
                <h3>Cappuccino</h3>
                <p>$4.00</p>
            </div>
            <div class="menu-item drinks-cold">
                <img src="https://images.unsplash.com/photo-1461023058943-07fcbe16d735?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80" alt="Iced Coffee">
                <h3>Iced Coffee</h3>
                <p>$3.75</p>
            </div>
            <div class="menu-item drinks-hot">
                <img src="https://images.unsplash.com/photo-1544787219-7f47ccb76574?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80" alt="Green Tea">
                <h3>Green Tea</h3>
                <p>$2.50</p>
            </div>
            <div class="menu-item drinks-cold">
                <img src="https://images.unsplash.com/photo-1622483767028-3f66f32aef97?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80" alt="Pepsi">
                <h3>Pepsi</h3>
                <p>$2.00</p>
            </div>
            <div class="menu-item drinks-cold">
                <img src="https://images.unsplash.com/photo-1600271886742-f049cd451bba?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80" alt="Orange Juice">
                <h3>Orange Juice</h3>
                <p>$3.00</p>
            </div>
            <div class="menu-item food-savory">
                <img src="https://images.unsplash.com/photo-1565299624946-b28f40a0ca4b?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80" alt="Club Sandwich">
                <h3>Club Sandwich</h3>
                <p>$8.00</p>
            </div>
            <div class="menu-item food-savory">
                <img src="https://images.unsplash.com/photo-1568901346375-23c9450c58cd?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80" alt="Cheeseburger">
                <h3>Cheeseburger</h3>
                <p>$9.50</p>
            </div>
            <div class="menu-item food-savory">
                <img src="https://images.unsplash.com/photo-1512621776951-a57141f2eefd?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80" alt="Caesar Salad">
                <h3>Caesar Salad</h3>
                <p>$7.00</p>
            </div>
            <div class="menu-item food-dessert">
                <img src="https://images.unsplash.com/photo-1551024506-0bccd828d307?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80" alt="Chocolate Cake">
                <h3>Chocolate Cake</h3>
                <p>$5.00</p>
            </div>
            <div class="menu-item food-dessert">
                <img src="https://images.unsplash.com/photo-1551106652-a5bcf4b29ab6?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80" alt="Glazed Donut">
                <h3>Glazed Donut</h3>
                <p>$2.50</p>
            </div>
            <div class="menu-item drinks-cold">
                <img src="https://images.unsplash.com/photo-1544148103-0773bf10d330?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80" alt="Berry Smoothie">
                <h3>Berry Smoothie</h3>
                <p>$4.50</p>
            </div>
        </div>
    </section>

    <footer id="contact">
        <p>Contact Us: 123 Cafe Street, City, State | Phone: (123) 456-7890 | Email: info@cafeadam.com</p>
        <p>&copy; 2023 Cafe Adam. All rights reserved.</p>
    </footer>

    <script>
        // Simple scroll animation for menu items
        const menuItems = document.querySelectorAll('.menu-item');
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = 1;
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        });
        menuItems.forEach(item => {
            item.style.opacity = 0;
            item.style.transform = 'translateY(20px)';
            item.style.transition = 'opacity 0.5s, transform 0.5s';
            observer.observe(item);
        });
    </script>
</body>
</html>
