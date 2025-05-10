# Ex.07 Restaurant Website
## Date: 03/05/2025
## Name: vasanthan .N
## Regno: 212224240180

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:

### HTML
```

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Delicious Bites</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <!-- HEADER: ONLY contains the title and nav -->
  <header>
    <h1>Delicious Bites</h1>
    <nav>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#menu">Menu</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- HERO -->
  <section id="home" class="hero">
    <div class="hero-content">
      <h2>Welcome to Delicious Bites</h2>
      <p>Experience the taste of joy with every bite!</p>
      <a href="#menu" class="btn">View Menu</a>
    </div>
  </section>

  <!-- MENU -->
  <section id="menu" class="menu-section">
    <h2>Our Menu</h2>
    <div class="menu-items">
      <div class="menu-card">
        <img src="images/pizza.png" alt="Pizza" />
        <h3>Margherita Pizza</h3>
        <p>Classic delight with fresh tomatoes, mozzarella, and basil.</p>
        <span>$8.99</span>
      </div>
  
      <div class="menu-card">
        <img src="images/burger.jpg" alt="Burger" />
        <h3>Cheese Burger</h3>
        <p>Juicy grilled patty with cheddar cheese and fresh veggies.</p>
        <span>$6.49</span>
      </div>
  
      <div class="menu-card">
        <img src="images/pasta.png" alt="Pasta" />
        <h3>Italian Pasta</h3>
        <p>Rich and creamy Alfredo pasta topped with parmesan.</p>
        <span>$7.99</span>
      </div>
  
      <!-- NEW MENU ITEMS -->
      <div class="menu-card">
        <img src="images/salad.jpg" alt="Salad" />
        <h3>Caesar Salad</h3>
        <p>Crisp romaine lettuce, croutons, and parmesan with Caesar dressing.</p>
        <span>$5.49</span>
      </div>
  
      <div class="menu-card">
        <img src="images/sushi.jpg" alt="Sushi" />
        <h3>California Sushi</h3>
        <p>Fresh avocado, crab, and cucumber wrapped in nori and rice.</p>
        <span>$9.99</span>
      </div>
  
      <div class="menu-card">
        <img src="images/steak.jpg" alt="Steak" />
        <h3>Grilled Steak</h3>
        <p>Succulent beef steak, grilled to perfection and served with sides.</p>
        <span>$14.99</span>
      </div>
  
      <div class="menu-card">
        <img src="images/dessert.jpg" alt="Dessert" />
        <h3>Chocolate Cake</h3>
        <p>Decadent chocolate cake layered with rich cream frosting.</p>
        <span>$4.99</span>
      </div>
    </div>
  </section>
  

  <!-- ABOUT -->
  <section id="about" class="about-section">
    <div class="about-content">
      <h2>About Us</h2>
      <p>
        At Delicious Bites, we believe in serving happiness through every dish.
        Founded in 2020, our restaurant blends passion with flavor to give you an
        unforgettable dining experience.
      </p>
      <p>
        From Italian classics to American favorites, our chefs use only the
        freshest ingredients to craft your meals with love.
      </p>
    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact" class="contact-section">
    <h2>Contact Us</h2>
    <form class="contact-form">
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email" required />
      <textarea rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>

  <!-- FOOTER -->
  <footer>
    <p>&copy; 2025 Delicious Bites. All rights reserved.</p>
  </footer>

  <!-- SCRIPT -->
  <script src="script.js"></script>

</body>
</html>

```

### CSS
```

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Segoe UI', sans-serif;
}

body {
  background-color: #fff8f0;
  color: #333;
}

/* Header */
header {
  background-color: #ff7f50;
  padding: 20px;
  text-align: center;
  color: white;
}

header h1 {
  margin-bottom: 10px;
}

nav ul {
  list-style: none;
  display: flex;
  justify-content: center;
  gap: 20px;
}

nav a {
  color: white;
  text-decoration: none;
  font-weight: bold;
}

nav a:hover {
  text-decoration: underline;
}

/* Hero Section */
.hero {
  background: url('images/res.png') no-repeat center center/cover;
  height: 90vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  color: white;
}

.hero-content {
  background-color: rgba(0, 0, 0, 0.6);
  padding: 40px;
  border-radius: 10px;
}

.btn {
  display: inline-block;
  margin-top: 20px;
  padding: 10px 25px;
  background-color: #ff7f50;
  color: white;
  text-decoration: none;
  border-radius: 5px;
}

.btn:hover {
  background-color: #e2673b;
}
.menu-section {
    padding: 60px 20px;
    text-align: center;
    background-color: #fff1e6;
  }
  
  .menu-section h2 {
    font-size: 2.5em;
    margin-bottom: 40px;
  }
  
  .menu-items {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 30px;
  }
  
  .menu-card {
    background-color: white;
    padding: 20px;
    width: 250px;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    transition: transform 0.2s;
  }
  
  .menu-card:hover {
    transform: translateY(-5px);
  }
  
  .menu-card img {
    width: 100%;
    height: 160px;
    object-fit: cover;
    border-radius: 10px;
  }
  
  .menu-card h3 {
    margin: 15px 0 10px;
  }
  
  .menu-card span {
    display: block;
    margin-top: 10px;
    font-weight: bold;
    color: #ff7f50;
  }
  .about-section {
    background-color: #fff;
    padding: 60px 20px;
    text-align: center;
  }
  
  .about-content {
    max-width: 700px;
    margin: auto;
  }
  
  .about-content h2 {
    font-size: 2.5em;
    margin-bottom: 20px;
  }
  
  .about-content p {
    margin-bottom: 15px;
    line-height: 1.6;
  }
  
  /* Contact Section */
  .contact-section {
    background-color: #fff1e6;
    padding: 60px 20px;
    text-align: center;
  }
  
  .contact-section h2 {
    font-size: 2.5em;
    margin-bottom: 30px;
  }
  
  .contact-form {
    max-width: 500px;
    margin: auto;
    display: flex;
    flex-direction: column;
    gap: 15px;
  }
  
  .contact-form input,
  .contact-form textarea {
    padding: 12px;
    border: 1px solid #ccc;
    border-radius: 8px;
    font-size: 1em;
  }
  
  .contact-form button {
    padding: 12px;
    background-color: #ff7f50;
    color: white;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    font-size: 1em;
  }
  
  .contact-form button:hover {
    background-color: #e2673b;
  }
  
  /* Footer */
  footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 20px 10px;
  }

/* Keyframes for fade-in animation */
@keyframes fadeIn {
    0% {
      opacity: 0;
      transform: translateY(20px);
    }
    100% {
      opacity: 1;
      transform: translateY(0);
    }
  }
  
  /* Class to apply fade-in effect */
  .menu-card {
    opacity: 0; /* Start with hidden items */
    animation: fadeIn 0.8s forwards;
  }
  
  /* Delay each menu card slightly for a staggered effect */
  .menu-card:nth-child(1) {
    animation-delay: 0.1s;
  }
  
  .menu-card:nth-child(2) {
    animation-delay: 0.2s;
  }
  
  .menu-card:nth-child(3) {
    animation-delay: 0.3s;
  }
  
  .menu-card:nth-child(4) {
    animation-delay: 0.4s;
  }
  
  .menu-card:nth-child(5) {
    animation-delay: 0.5s;
  }
  
  .menu-card:nth-child(6) {
    animation-delay: 0.6s;
  }
  
  .menu-card:nth-child(7) {
    animation-delay: 0.7s;
  }
  
  .menu-card:nth-child(8) {
    animation-delay: 0.8s;
  }
  
  /* Hover effect for menu cards */
.menu-card {
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }
  
  .menu-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
  }
  ```


## OUTPUT:


![Screenshot 2025-05-10 142327](https://github.com/user-attachments/assets/e4b0d036-6376-40d2-97b7-54297a7e6e36)


![Screenshot 2025-05-10 142419](https://github.com/user-attachments/assets/0fb58bb0-db9d-490b-99cb-52650bbfa3d0)



## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
