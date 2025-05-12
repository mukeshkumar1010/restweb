# Ex.07 Restaurant Website
## Date: 12-05-2025

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
### home.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MARAN PAROTTA KADAI</title>
    <style>
      
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: #054c04;
            color: #333;
            padding: 10px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        header img {
            height: 40px;
        }

        header nav a {
            text-decoration: none;
            color: #f9f9f9;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ff5722;
        }

        .banner {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 30px 20px;
            /* background: url('bg.jpg') no-repeat center center/cover; */
            /* background-color: aqua; */
            color: white;
            height: 300px;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.8);
        }

        .banner-content {
            max-width: 50%;
        }

        .banner-content h1 {
            font-family: Georgia, 'Times New Roman', Times, serif;
            font-size: 2.5rem;
            margin-bottom: 10px;
            color: gold;
            text-align: center;
        }

        .banner-content p {
            font-size: 1rem;
            margin-bottom: 15px;
            color: black;
        }

        .banner-content a {
            background: #ff5722;
            color: white;
            padding: 8px 15px;
            text-decoration: none;
            font-weight: bold;
            border-radius: 5px;
            transition: background 0.3s ease;
        }

        .banner-content a:hover {
            background: #e64a19;
        }

        .features {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            padding: 20px;
            gap: 15px;
            background: #f9f9f9;
        }

        .feature {
            background: white;
            border-radius: 10px;
            padding: 15px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            flex: 1;
            text-align: center;
        }

        .feature img {
            width: 100%;
            border-radius: 10px;
            margin-bottom: 10px;
        }

        .feature h3 {
            font-size: 1.2rem;
            margin-bottom: 10px;
            color: #1f1714;
        }

        .feature p {
            font-size: 0.9rem;
            color: white;
        }

        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
            margin-top: 10px;
        }

        footer a {
            color: #ff5722;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #ffdd57;
        }

        @media (max-width: 768px) {
            .banner {
                flex-direction: column;
                height: auto;
                text-align: center;
            }

            .banner-content {
                max-width: 100%;
            }

            .features {
                flex-direction: column;
                gap: 20px;
            }

            .feature {
                flex: none;
            }

            header nav a {
                margin: 0 5px;
            }
        }
    </style>
</head>
<body>
      <header>
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQTK8YL9ek9TnidVUMIlW3C8djO35FLc2CJaw&s">
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="admin.html">Administration</a>
        </nav>
    </header>

    <div class="banner">
        <div class="banner-content">
            <h1>Welcome to Maran Parotta Kadai</h1>
            <p>A genuine fine-dining experience awaits.. We serve happiness on a plate!</p>
            <a href="#features">Explore Now</a>
        </div>
    </div>

    <section id="features" class="features">
        <div class="feature">
            <img src="https://plus.unsplash.com/premium_photo-1671379086168-a5d018d583cf?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Fresh Ingredients">
            <h3>Fresh Ingredients</h3>
            <p>Freshness Focused: "Taste the freshness, enjoy the flavor".</p>
        </div>
        <div class="feature">
            <img src="https://images.unsplash.com/photo-1635975206435-934b1ca3b421?q=80&w=1976&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Cozy Ambiance">
            <h3>Cozy Ambiance</h3>
            <p>The Perfect Place to Relax and Reconnect.</p>
        </div>
        <div class="feature">
            <img src="https://images.unsplash.com/photo-1632657583981-938d58b18b09?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="Easy Reservations">
            <h3>Easy Reservations</h3>
            <p>Book your table in seconds and guarantee yourself an unforgettable experience.</p>
        </div>
    </section>

    <footer>
        <p>&copy; Designed and developed by MUKESH KUMAR S | <a href="#">Privacy Policy</a></p>
    </footer>

</body>
</html>
```

### menu.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MARAN PAROTTA KADAI - Menu</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: #054c04;
            color: #fff;
            padding: 10px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        header nav a {
            text-decoration: none;
            color: #f9f9f9;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ffdd57;
        }

        header h1 {
            font-size: 1.5rem;
        }

        .menu-container {
            padding: 10px;
            background: #f9f9f9;
            text-align: center;
        }

        .menu-container h1 {
            font-size: 2rem;
            color: #054c04;
            margin-bottom: 15px;
        }

        .menu-items {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            justify-content: center;
        }

        .menu-item {
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            width: 280px;
            overflow: hidden;
            transition: transform 0.3s ease;
        }

        .menu-item img {
            width: 100%;
            height: 180px;
            object-fit: cover;
        }

        .menu-item:hover {
            transform: scale(1.05);
        }

        .menu-details {
            padding: 10px;
        }

        .menu-details h3 {
            font-size: 1.2rem;
            color: #054c04;
            margin-bottom: 8px;
        }

        .menu-details p {
            font-size: 0.9rem;
            color: #555;
            margin-bottom: 10px;
        }

        .menu-details .price {
            font-weight: bold;
            font-size: 1rem;
            color: #ff5722;
        }

        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
            margin-top: 10px;
        }

        footer a {
            color: #ff5722;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #ffdd57;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.2rem;
            }

            .menu-items {
                flex-direction: column;
                gap: 20px;
            }

            .menu-item {
                width: 100%;
            }

            header nav a {
                margin: 0 5px;
            }
        }
    </style>
</head>
<body>

    <header>
        <h1>Maran Parotta Kadai</h1>
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">contact</a>
            <a href="admin.html">Administration</a>
        </nav>
    </header>

    <div class="menu-container">
        <h1>Our Menu</h1>
        <div class="menu-items">
            <div class="menu-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRVxMDZ89fmuKlbqzOdXvFvhLA89V4J_klI3Q&s" alt="Biryani">
                <div class="menu-details">
                    <h3> Pani Puri</h3>
                    <p>Crispy puris filled with spicy, tangy water, mashed potatoes, chickpeas, and chutneys – an explosion of flavors in every bite! Served fresh for that authentic street food experience.</p>
                    <p class="price">₹170/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="https://upload.wikimedia.org/wikipedia/commons/4/4a/Bambayya_Pav_bhaji.jpg" alt="Curd rice">
                <div class="menu-details">
                    <h3> Pav Bhaji</h3>
                    <p>Spicy buttered vegetable mash served with toasted pav, onions, lemon, and extra butter.</p>
                    <p class="price">₹150/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="data:image/jpeg;base64,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" alt="Brownie">
                <div class="menu-details">
                    <h3>Brownie</h3>
                    <p>Brownie topped with coffee chip ice cream, chocolate sauce, and your favorite sundae toppings.</p>
                    <p class="price">₹100/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTSSe5VHZHhDB6_qQ0GpHFQk52BvSW-K1Ns5Q&s" alt="Dosa">
                <div class="menu-details">
                    <h3>Crispy dosa</h3>
                    <p>Crispy dosa with yummy taste.</p>
                    <p class="price">₹150/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR2lXVGVK8Ocz3LAjIHK1cGoRx01fRkkfiBlg&s" alt="falooda">
                <div class="menu-details">
                    <h3>Falooda</h3>
                    <p> Chilled dessert drink with rose milk, vermicelli, basil seeds, jelly, and ice cream.</p>
                    <p class="price">₹150/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcToiLbR1sOiQvyOkZQX-l11i3V9tHxquE2O6g&s" alt="gulab">
                <div class="menu-details">
                    <h3>Custard Gulab Jamun</h3>
                    <p>Soft gulab jamuns served chilled with creamy custard for a rich, delightful treat.</p>
                    <p class="price">₹180/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSyz_FpCbmjnIvVgqa36hec1mDDqSSQLtXVpQ&s" alt="">
                <div class="menu-details">
                    <h3>White Sauce Pasta</h3>
                    <p>Creamy, cheesy pasta tossed in rich white sauce with veggies and Italian herbs.</p>
                    <p class="price">₹180/-</p>
                </div>
            </div>


            <div class="menu-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQnDvCK23Qed0RKVa4oPv38sIaFV9ZOm5plnQ&s" alt="Idly">
                <div class="menu-details">
                    <h3>Idly</h3>
                    <p>Idly is a soft & fluffy steamed cake made with fermented rice & lentil batter. </p>
                    <p class="price">₹70/-</p>
                </div>
            </div>


            <div class="menu-item">
                <img src="https://www.thespruceeats.com/thmb/UnVh_-znw7ikMUciZIx5sNqBtTU=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/steamed-momos-wontons-1957616-hero-01-1c59e22bad0347daa8f0dfe12894bc3c.jpg" alt="momos">
                <div class="menu-details">
                    <h3>Momos</h3>
                    <p>Steamed or fried dumplings filled with veggies or meat, served with spicy dipping sauce.</p>
                    <p class="price">₹180/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQQmQSUfoESF1ewfjvcckKbjjfWmlboub454A&s" alt="cutlet">
                <div class="menu-details">
                    <h3>Cutlet</h3>
                    <p>Crispy, golden-fried patties filled with spiced vegetables or meat, served with tangy chutney.</p>
                    <p class="price">₹180/-</p>
                </div>
            </div>
         </div>
    </div>

    <footer>
        <p>&copy; designed and developed by MUKESH KUMAR S| <a href="home.html">Back to Home</a></p>
    </footer>

</body>
</html>
```

### contact.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Maran Parotta Kadai - Contact Us</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: #054c04;
            color: #333;
            padding: 15px 30px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        header img {
            height: 50px;
        }

        header nav a {
            text-decoration: none;
            color: #f9f9f9;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ff5722;
        }

        .contact-banner {
            display: flex;
            align-items: center;
            justify-content: center;
            background: url('contacts.jpg') no-repeat center center/cover;
            height: 300px;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.8);
        }

        .contact-banner h1 {
            font-family: Georgia, 'Times New Roman', Times, serif;
            font-size: 2.5rem;
            color: #f9f9f9;
        }

        .contact-section {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 30px 15px;
            background: #f9f9f9;
            gap: 20px;
        }

        .contact-details, .contact-form {
            flex: 1;
            max-width: 500px;
            margin: 10px;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        .contact-details h2, .contact-form h2 {
            font-size: 1.8rem;
            margin-bottom: 15px;
            color: #1f1714;
            text-align: center;
        }

        .contact-details p {
            margin: 10px 0;
            font-size: 1rem;
            color: #555;
        }

        .contact-details img {
            max-width: 100%;
            border-radius: 10px;
            margin-bottom: 20px;
        }

        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 1rem;
        }

        .contact-form textarea {
            height: 100px;
        }

        .contact-form button {
            width: 100%;
            padding: 10px;
            background: #ff5722;
            color: white;
            font-size: 1.1rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s ease;
        }

        .contact-form button:hover {
            background: #e64a19;
        }

        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 15px 0;
        }

        footer a {
            color: #ff5722;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #ffdd57;
        }

        @media (max-width: 768px) {
            .contact-details, .contact-form {
                max-width: 100%;
            }

            .contact-banner h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>

    <header>
        <img src="logo.jpg">
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="admin.html">Administration</a>
        </nav>
    </header>

    <div class="contact-banner">
     
    </div>

    <section class="contact-section">
        <div class="contact-details">
            <h2>Get in Touch</h2>
            <!-- <img src="contact.jpeg" alt="Contact Us"> -->
            <p><strong>Address:</strong> Maran Parotta Kadai, Chennai, Tamilnadu, India</p>
            <p><strong>Phone:</strong> +91 1234567890</p>
            <p><strong>Email:</strong> contact@maran.com</p>
            <p><strong>Hours:</strong> Mon-Sun: 12:00 am -12:00 pm</p>
        </div>

        <div class="contact-form">
            <h2>Send Us a Message</h2>
            <form action="/submit-contact" method="POST">
                <label for="name">Full Name</label>
                <input type="text" id="name" name="name" placeholder="Enter your full name" required>

                <label for="email">Email Address</label>
                <input type="email" id="email" name="email" placeholder="Enter your email address" required>
         
                <label for="phone no">Phone Number</label>
                <input type="phone no" id="phone no" name="phone no" placeholder="Enter your phone number" required>

                <label for="message">Message</label>
                <textarea id="message" name="message" placeholder="Your message" required></textarea>

                <button type="submit">Send Message</button>
            </form>
        </div>
    </section>

    <footer>
        <p>&copy; designed and by developed by MUKESH KUMAR S | <a href="#">Privacy Policy</a></p>
    </footer>

</body>
</html>
```

### admin.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MARAN PAROTTA KADAI - Administration</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: #054c04;
            color: #fff;
            padding: 10px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        header nav a {
            text-decoration: none;
            color: #f9f9f9;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ffdd57;
        }

        header h1 {
            font-size: 1.5rem;
        }

        .admin-container {
            padding: 20px;
            background: #f9f9f9;
            text-align: center;
        }

        .admin-container h1 {
            font-size: 2rem;
            color: #054c04;
            margin-bottom: 20px;
        }

        .admin-items {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }

        .admin-item {
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            width: 300px;
            overflow: hidden;
            transition: transform 0.3s ease;
            text-align: left;
        }

        .admin-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .admin-item:hover {
            transform: scale(1.05);
        }

        .admin-details {
            padding: 15px;
        }

        .admin-details h3 {
            font-size: 1.2rem;
            color: #054c04;
            margin-bottom: 8px;
        }

        .admin-details p {
            font-size: 0.9rem;
            color: #555;
            margin-bottom: 10px;
        }

        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
            margin-top: 10px;
        }

        footer a {
            color: #ff5722;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s ease;
        }

        footer a:hover {
            color: #ffdd57;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.2rem;
            }

            .admin-items {
                flex-direction: column;
                gap: 20px;
            }

            .admin-item {
                width: 100%;
            }

            header nav a {
                margin: 0 5px;
            }
        }
    </style>
</head>
<body>

    <header>
        <h1>Maran Parotta Kadai - Admin</h1>
        <nav>
            <a href="home.html">Home</a>
            <a href="menu.html">Menu</a>
            <a href="contact.html">Contact</a>
            <a href="admin.html">Administration</a>
        </nav>
    </header>

   <div class="admin-container">
      <h1>Our Leadership Team</h1>
      <div class="admin-items">
          <div class="admin-item">
              <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS_DZ5p7zmynNPrC1oODZOeKNTWs6y5m0SyQg&s" alt="Mary - Chief Executive Officer">
              <div class="admin-details">
                  <h3>Mary</h3>
                  <p>Chief Executive Officer - With over 15 years of experience in the hospitality industry, Mary leads Golden Cuisine with a strategic vision focused on guest satisfaction, business growth, and culinary innovation.</p>
              </div>
          </div>

          <div class="admin-item">
              <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQnHywKKifssBpak21VZNzozzCAtRfrvIOoLg&s" alt="John - Operations Manager">
              <div class="admin-details">
                  <h3>John</h3>
                  <p>Operations Manager - John brings a strong background in hotel management and front-of-house operations. He ensures daily activities run smoothly, from staff coordination to customer service quality. </p>
              </div>
          </div>

          <div class="admin-item">
              <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQHyhGLvUk1Z1DgloeWY-n6Tl9cTlKQke8KxQ&s" alt="Williams - Executive Chef">
              <div class="admin-details">
                  <h3>Williams</h3>
                  <p>Executive Chef - A culinary artist with international training, Williams specializes in fusing classic techniques with modern flavors. He curates the restaurant’s signature menu, supervises kitchen operations.</p>
              </div>
          </div>

          <div class="admin-item">
              <img src="https://media.licdn.com/dms/image/v2/D5603AQGnszVc36CJ6Q/profile-displayphoto-shrink_200_200/profile-displayphoto-shrink_200_200/0/1699882666140?e=2147483647&v=beta&t=OpuUElXeYFvpKug-CUZi_0IgYPTmdDeDiaDFAsmJv_Q" alt="Sofia - Deputy Director">
              <div class="admin-details">
                  <h3>Sofia</h3>
                  <p>Deputy Director - With expertise in business administration and hospitality services, Sofia supports strategic planning, staff training, and customer engagement programs.</p>
             </div>
          </div>
      </div>
  </div>
     <footer>
        <p>&copy; designed and developed by MUKESH KUMAR S | <a href="home.html">Back to Home</a></p>
    </footer>

</body>
</html>
```


## OUTPUT:
![Screenshot (26)](https://github.com/user-attachments/assets/d75c7ba2-8f7c-4ffd-86cc-1604788386c6)
![Screenshot (27)](https://github.com/user-attachments/assets/5d4b7655-b1d6-45b2-8318-5823cf018a32)
![Screenshot (28)](https://github.com/user-attachments/assets/57461f35-75c5-4d66-8f7a-4139da5cb465)
![Screenshot (29)](https://github.com/user-attachments/assets/26ce9b7d-510e-4b8a-8f53-6279e6c24536)


## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
