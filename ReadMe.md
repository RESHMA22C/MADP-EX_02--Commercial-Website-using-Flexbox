# Ex02 Commercial Website
## Date:

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
# HTML
~~~
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Reshma's Coffee Shop</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <nav class="navbar">
      <div class="logo">Reshma's Coffee</div>
      <ul class="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#menu">Menu</a></li>
        <li><a href="#about">About Us</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="home" class="hero">
    <h1>Welcome to Reshma's Coffee Shop</h1>
    <p>Freshly brewed coffee, every day.</p>
    <a href="#menu" class="btn">View Menu</a>
  </section>

  

  <section id="about" class="about">
    <h2>About Us</h2>
    <p>At Reshma's Coffee Shop, we serve the freshest coffee made from carefully selected beans. Come enjoy a warm atmosphere and delicious drinks.</p>
  </section>

    <section id="menu" class="menu">
  <h2>Our Menu</h2>
  <div class="menu-list">
    <div class="menu-item">
      <img src="https://images.unsplash.com/photo-1511920170033-f8396924c348?auto=format&fit=crop&w=400&q=80" alt="Espresso" />
      <h3>Espresso</h3>
      <p>Strong and bold, a classic favorite.</p>
    </div>
    <div class="menu-item">
      <img src="https://images.unsplash.com/photo-1509042239860-f550ce710b93?auto=format&fit=crop&w=400&q=80" alt="Cappuccino" />
      <h3>Cappuccino</h3>
      <p>Espresso with steamed milk and foam.</p>
    </div>
    <div class="menu-item">
      <img src="https://images.unsplash.com/photo-1529042410759-befb1204b468?auto=format&fit=crop&w=400&q=80" alt="Latte" />
      <h3>Latte</h3>
      <p>Smooth blend of espresso and steamed milk.</p>
    </div>
    <div class="menu-item">
      <h3>Mocha</h3>
      <p>Chocolate and espresso, a perfect mix.</p>
    </div>
  </div>
</section>

  <section id="contact" class="contact">
    <h2>Contact Us</h2>
    <p>Email: reshmascoffee@gmail.com</p>
    <p>Phone: +1 234 567 8900</p>
    <p>Address: 123 Coffee Lane, Cityville</p>
  </section>


  <footer>
    <p>Designed by Reshma | Register Number: 212223040168</p>
  </footer>
</body>
</html>

~~~

# CSS
~~~
/* Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background-color: #fff8f0;
  color: #4b2e05;
  line-height: 1.6;
}

/* Navbar */
.navbar {
  background-color: #6f4e37;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  color: white;
}

.logo {
  font-size: 1.8rem;
  font-weight: bold;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 1.5rem;
}

.nav-links a {
  color: white;
  text-decoration: none;
  font-weight: 600;
}

.nav-links a:hover {
  text-decoration: underline;
}

/* Hero Section */
.hero {
  background: url('https://images.unsplash.com/photo-1509042239860-f550ce710b93?auto=format&fit=crop&w=1350&q=80') no-repeat center center/cover;
  height: 400px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: #fff2e6;
  padding: 0 1rem;
}

.hero h1 {
  font-size: 3rem;
  margin-bottom: 1rem;
  text-shadow: 2px 2px 4px #3e2f15;
}

.hero p {
  font-size: 1.3rem;
  margin-bottom: 2rem;
  text-shadow: 1px 1px 3px #3e2f15;
}

.btn {
  background-color: #6f4e37;
  color: white;
  padding: 0.8rem 1.5rem;
  text-decoration: none;
  border-radius: 5px;
  font-weight: 600;
  transition: background-color 0.3s ease;
}

.btn:hover {
  background-color: #543d29;
}

/* Menu Section */
.menu {
  max-width: 900px;
  margin: 3rem auto;
  padding: 0 1rem;
}

.menu h2 {
  text-align: center;
  margin-bottom: 2rem;
  color: #6f4e37;
}

.menu-list {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  gap: 1.5rem;
}

.menu-item {
  background-color: #fff2e6;
  padding: 1.5rem;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgb(111 78 55 / 0.3);
  flex: 1 1 220px;
  text-align: center;
}

.menu-item h3 {
  margin-bottom: 1rem;
  color: #6f4e37;
}

/* About Section */
.about {
  background-color: #f7ede2;
  max-width: 700px;
  margin: 3rem auto;
  padding: 2rem 1rem;
  border-radius: 10px;
  text-align: center;
  color: #4b2e05;
}

.about h2 {
  margin-bottom: 1rem;
}

/* Contact Section */
.contact {
  max-width: 600px;
  margin: 3rem auto;
  padding: 0 1rem;
  text-align: center;
}

.contact h2 {
  margin-bottom: 1rem;
  color: #6f4e37;
}

.contact p {
  margin: 0.5rem 0;
}

/* Footer */
footer {
  background-color: #6f4e37;
  color: white;
  text-align: center;
  padding: 1rem;
  font-weight: 600;
  margin-top: 3rem;
}

/* Responsive */
@media (max-width: 768px) {
  .menu-list {
    flex-direction: column;
    align-items: center;
  }
}

.menu-item img {
  width: 100%;
  height: 180px;
  object-fit: cover;
  border-radius: 8px;
  margin-bottom: 0.8rem;
}

~~~

## OUTPUT

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/f065f7a6-2f26-4575-bb49-cb928ffabfa3" />

<img width="1312" height="766" alt="image" src="https://github.com/user-attachments/assets/73b0713a-174c-4eb7-827c-b5eff1d49d79" />

<img width="1392" height="375" alt="image" src="https://github.com/user-attachments/assets/443fce60-7f09-4eba-ad94-cba014555d3f" />

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
