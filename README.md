# Ex.07 Restaurant Website
# Date:09/05/2025
# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
Validate the layout in various browsers.

## Step 6:
Validate the HTML code.

## Step 7:
Publish the website in the given URL.

# PROGRAM:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Cozy Bites</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #fffaf0;
      color: #333;
    }

    header {
      background-color: #b22222;
      color: white;
      padding: 1em;
      text-align: center;
    }

    nav a {
      color: white;
      margin: 0 10px;
      text-decoration: none;
      font-weight: bold;
    }

    nav a:hover {
      text-decoration: underline;
    }

    .tabs {
      display: flex;
      justify-content: center;
      margin-top: 1em;
    }

    .tab-button {
      background: #b22222;
      color: white;
      border: none;
      padding: 10px 20px;
      margin: 0 5px;
      cursor: pointer;
      font-size: 1em;
    }

    .tab-button.active {
      background: #8b0000;
    }

    .tab-content {
      display: none;
    }

    .tab-content.active {
      display: block;
    }

    .hero {
      padding: 2em;
      background-color: #ffe4c4;
      text-align: center;
    }

    .section {
      padding: 2em;
      max-width: 1000px;
      margin: auto;
    }

    .menu-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 20px;
    }

    .menu-item {
      background-color: #fff;
      border: 1px solid #ddd;
      border-radius: 8px;
      padding: 1em;
      text-align: center;
    }

    .menu-item img {
      width: 100%;
      height: 150px;
      object-fit: cover;
      border-radius: 6px;
    }

    .menu-item strong {
      display: block;
      margin-top: 10px;
      font-size: 1.1em;
    }

    footer {
      background-color: #b22222;
      color: white;
      text-align: center;
      padding: 1em;
      margin-top: 2em;
    }
  </style>
</head>
<body>
  <header>
    <h1>Cozy Bites</h1>
    <nav>
      <a href="#" onclick="showTab('home')">Home</a>
      <a href="#" onclick="showTab('menu')">Menu</a>
    </nav>
  </header>

  <div class="tabs">
    <button class="tab-button active" onclick="showTab('home')">Home</button>
    <button class="tab-button" onclick="showTab('menu')">Menu</button>
  </div>

  <main>
    <!-- Home Tab -->
    <section id="home" class="tab-content active">
      <div class="hero">
        <h2>Welcome to Cozy Bites</h2>
        <p>Your friendly neighborhood restaurant serving delicious meals daily!</p>
      </div>
      <div class="section">
        <h3>About Us</h3>
        <p>At Cozy Bites, we believe in comfort food made with love and fresh ingredients.</p>
      </div>
    </section>

    <!-- Menu Tab -->
    <section id="menu" class="tab-content">
      <div class="section">
        <h2>Our Menu</h2>
        <div class="menu-grid">
          <div class="menu-item">
            <img src="https://cdn.pixabay.com/photo/2016/03/05/19/02/hamburger-1238246_1280.jpg" alt="Burger">
            <strong>Classic Burger</strong>
            $9.99
          </div>
          <div class="menu-item">
            <img src="https://cdn.pixabay.com/photo/2017/12/09/08/18/pizza-3007395_1280.jpg" alt="Pizza">
            <strong>Pepperoni Pizza</strong>
            $12.99
          </div>
          <div class="menu-item">
            <img src="saled.jpg" alt="Salad">
            <strong>Caesar Salad</strong>
            $7.99
          </div>
          <div class="menu-item">
            <img src="double burger.jpg" alt="Double Burger">
            <strong>Double Burger</strong>
            $11.99
          </div>
          <div class="menu-item">
            <img src="burgur.jpg" alt="Cheese Burger">
            <strong>Cheese Burger</strong>
            $10.49
          </div>
          <div class="menu-item">
            <img src="doner kebab.jpg" alt="Veggie Wrap">
            <strong>doner kebab</strong>
            $8.49
          </div>
          <div class="menu-item">
            <img src="sushi.jpg" alt="Grilled Chicken">
            <strong>sushi</strong>
            $10.99
          </div>
          <div class="menu-item">
            <img src="icecream.jpg" alt="Spicy Burger">
            <strong>Ice cream</strong>
            $10.99
          </div>
          <div class="menu-item">
            <img src="sandwich.jpg" alt="Fried Chicken">
            <strong>Sandwich
            </strong>
            $499
          </div>
          <div class="menu-item">
            <img src="tomoto.jpg" alt="Chicken Pizza">
            <strong>tomoto soup</strong>
            $13.99
          </div>
          <div class="menu-item">
            <img src="hotdog.jpg" alt="Cheesecake">
            <strong>HOT DOG</strong>
            $599
          </div>
          <div class="menu-item">
            <img src="https://cdn.pixabay.com/photo/2014/10/23/18/05/cake-500054_1280.jpg" alt="Lava Cake">
            <strong>Chocolate Lava Cake</strong>
            $5.49
          </div>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Cozy Bites. All rights reserved.</p>
  </footer>

  <script>
    function showTab(tabId) {
      const contents = document.querySelectorAll('.tab-content');
      const buttons = document.querySelectorAll('.tab-button');

      contents.forEach(c => c.classList.remove('active'));
      buttons.forEach(b => b.classList.remove('active'));

      document.getElementById(tabId).classList.add('active');
      const activeButton = Array.from(buttons).find(b => b.textContent.toLowerCase() === tabId);
      if (activeButton) activeButton.classList.add('active');
    }
  </script>
</body>
</html>



```
# OUTPUT:
![alt text](<Screenshot 2025-05-09 142651.png>)
![alt text](<Screenshot 2025-05-09 142714.png>)
![alt text](<Screenshot 2025-05-09 142730.png>)

# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
