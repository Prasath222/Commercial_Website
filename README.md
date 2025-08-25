# Ex02 Commercial Website
## Date: 25/08/2025

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sweet Treats Bakery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #1ed21e;
            color: white;
            padding: 20px;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #1ed21e;
            padding: 10px;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            padding: 10px 15px;
        }
        nav a:hover {
            background-color: #1ed21e;
            border-radius: 5px;
        }
        .hero {
            display: flex;
            align-items: center;
            justify-content: center;
            background: url('bakery-hero.jpg') no-repeat center center/cover;
            height: 400px;
            color: white;
            text-align: center;
        }
        .hero h1 {
            font-size: 3rem;
            background: rgba(0, 0, 0, 0.5);
            padding: 20px;
        }
        .products {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 20px;
            gap: 20px;
        }
        .product {
            border: 1px solid #ddd;
            border-radius: 5px;
            overflow: hidden;
            width: 300px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            background: white;
        }
        .product img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        .product-details {
            padding: 15px;
        }
        .product-details h3 {
            margin: 0 0 10px;
        }
        .product-details p {
            margin: 0 0 15px;
            color: #555;
        }
        .product-details a {
            text-decoration: none;
            color: white;
            background-color: #1ed21e;
            padding: 10px 15px;
            border-radius: 5px;
        }
        .product-details a:hover {
            background-color: #1ed21e;
        }
        footer {
            background-color: #1ed21e;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Sweet Treats Bakery</h1>
    </header>
    <nav>
        <a href="#home">Home</a>
        <a href="#products">Menu</a>
        <a href="#about">About Us</a>
        <a href="#contact">Contact</a>
    </nav>
    <section id="home" class="home">
        <div style="text-align: center; padding: 50px;">
            <h2>Welcome to Sweet Treats Bakery</h2>
            <p>Freshly baked cakes, pastries, and breads made with love. Order online and enjoy our delicious treats delivered straight to your doorstep.</p>
            <a href="#products" style="text-decoration: none; color: white; background-color: #d2691e; padding: 10px 20px; border-radius: 5px;">View Menu</a>
        </div>
    </section>
    <section class="hero">
        <h1>Fresh. Delicious. Delivered.</h1>
    </section>
    <section id="products" class="products">
        <div class="product">
            <img src="cake.jpg" alt="Chocolate Cake">
            <div class="product-details">
                <h3>Chocolate Cake</h3>
                <p>₹450 - Rich and moist with creamy frosting</p>
                <a href="#">Order Now</a>
            </div>
        </div>
        <div class="product">
            <img src="croissant.jpg" alt="Croissant">
            <div class="product-details">
                <h3>Butter Croissant</h3>
                <p>₹320 - Flaky, buttery, and perfect for breakfast</p>
                <a href="#">Order Now</a>
            </div>
        </div>
        <div class="product">
            <img src="donut.webp" alt="Donuts">
            <div class="product-details">
                <h3>Glazed Donuts</h3>
                <p>₹200 - Soft, sweet, and irresistibly tasty</p>
                <a href="#">Order Now</a>
            </div>
        </div>
    </section>
    <section id="about" class="about" style="background-color: #f9f9f9; padding: 50px;">
        <div style="max-width: 800px; margin: auto; text-align: center;">
            <h2>About Us</h2>
            <p>At Sweet Treats Bakery, we believe every day deserves a little sweetness. Our bakers use only the finest ingredients to create mouthwatering cakes, breads, and pastries that delight every customer.</p>
            <p>From morning coffee companions to grand celebration cakes — we’ve got something for everyone.</p>
        </div>
    </section>
    <section id="contact" class="contact" style="padding: 50px;">
        <div style="max-width: 600px; margin: auto; text-align: center;">
            <h2>Contact Us</h2>
            <p>Want to place a custom order or have a question?</p>
            <p>Email: <a href="mailto:abc@sweettreats.com">sweet@sweettreats.com</a></p>
            <p>Phone: <a href="tel:+919876543210">+91 9876543210</a></p>
            <p>Address: 12 Bakery Street, Chennai</p>
            <form style="margin-top: 20px;">
                <input type="text" placeholder="Your Name" style="width: 100%; padding: 10px; margin-bottom: 10px; border: 1px solid #ddd; border-radius: 5px;">
                <input type="email" placeholder="Your Email" style="width: 100%; padding: 10px; margin-bottom: 10px; border: 1px solid #ddd; border-radius: 5px;">
                <textarea placeholder="Your Message" style="width: 100%; padding: 10px; margin-bottom: 10px; border: 1px solid #ddd; border-radius: 5px;"></textarea>
                <button type="submit" style="background-color: #2dd21e; color: white; padding: 10px 20px; border: none; border-radius: 5px;">Send Message</button>
            </form>
        </div>
    </section>
    <footer>
        <p>&copy; 2025 Sweet Treats Bakery. All rights reserved.</p>
    </footer>
</body>
</html>

## OUTPUT
<img width="1913" height="1055" alt="Screenshot 2025-08-25 100954" src="https://github.com/user-attachments/assets/06545ad3-09ce-42e7-baed-4c8d3447d3fb" />
<img width="1241" height="557" alt="Screenshot 2025-08-25 101233" src="https://github.com/user-attachments/assets/57f65fcc-4965-4c81-bafc-a000f9a58835" />
<img width="1586" height="945" alt="Screenshot 2025-08-25 101248" src="https://github.com/user-attachments/assets/9a0c870c-f502-486f-b902-14c1556bf064" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
