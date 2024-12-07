# Ex04 Places Around Me
# Date: 29/11/2024
# AIM
To develop a website to display details about the places around my house.

# DESIGN STEPS
## STEP 1
Create a Django admin interface.

## STEP 2
Download your city map from Google.

## STEP 3
Using <map> tag name the map.

## STEP 4
Create clickable regions in the image using <area> tag.

## STEP 5
Write HTML programs for all the regions identified.

## STEP 6
Execute the programs and publish them.

# CODE

```
map.html
<!DOCTYPE html>
<html>
    <body>
        <div style="text-align: center;">
        <h1> SHOPS NEAR NEXUS MALL</h1>
        <h2> click the shop to know more about it</h2>
        
            <div style="text-align: center;">
            <img src="nexus mall.png" alt="Not found" style="width: fit-content;" usemap="#Landmark" >
            </div>
        <map name="Landmark">
            <area shape="circle" coords="913,555,8" alt="NEXUS VIJAYA MALL" href="hotel.html">
            <area shape="circle" coords="964,639,12" alt="VAN HEUSEN" href="vanheusen.html">
            <area shape="circle" coords="454,715,7" title="FORUM MALL" href="forummall.html">   
        
        </map>
        </div>
    </body>
</html>

forummall.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Forum Mall - Shopping, Dining & Entertainment</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            color: #333;
        }
        header {
            background-color: #6200EA;
            color: #fff;
            padding: 1.5rem 0;
            text-align: center;
        }
        nav {
            background-color: #3700B3;
            display: flex;
            justify-content: center;
            padding: 0.5rem 0;
        }
        nav a {
            color: #fff;
            text-decoration: none;
            margin: 0 1.5rem;
            font-weight: bold;
        }
        nav a:hover {
            text-decoration: underline;
        }
        .hero {
            background-image: url('mall-hero.jpg');
            background-size: cover;
            background-position: center;
            height: 60vh;
            display: flex;
            justify-content: center;
            align-items: center;
            color: #fff;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.7);
        }
        .hero h1 {
            font-size: 3.5rem;
            margin: 0;
        }
        .content {
            padding: 2rem;
        }
        .categories {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }
        .category {
            border: 1px solid #ddd;
            border-radius: 8px;
            overflow: hidden;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .category img {
            max-width: 100%;
            height: auto;
        }
        .category h3 {
            background-color: #6200EA;
            color: #fff;
            margin: 0;
            padding: 0.5rem;
        }
        footer {
            background-color: #6200EA;
            color: #fff;
            text-align: center;
            padding: 1rem 0;
            margin-top: 2rem;
        }
    </style>
</head>
<body>
    <header>
        <h1>Forum Mall</h1>
        <p>Your Destination for Shopping, Dining & Entertainment</p>
    </header>
    <nav>
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#stores">Stores</a>
        <a href="#dining">Dining</a>
        <a href="#contact">Contact</a>
    </nav>
    <section class="hero">
        <h1>Welcome to Forum Mall</h1>
    </section>
    <section class="content">
        <h2 id="stores">Explore Our Categories</h2>
        <div class="categories">
            <div class="category">
                <img src="https://www.shutterstock.com/image-photo/men-elegant-clothing-260nw-585751172.jpg" alt="Fashion">
                <h3>Fashion</h3>
            </div>
            <div class="category">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSdNoL2l6dvOS0O3nx9px2QLEZivfk_Z8YCxg&s" alt="Electronics">
                <h3>Electronics</h3>
            </div>
            <div class="category">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQscw4sOXi0BcwVS9MhILBm-GWczPhOp8B09A&s" alt="Dining">
                <h3>Dining</h3>
            </div>
            <div class="category">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRqZQEieucPRzLNZbMNhROX8InDo9uFoIjHIw&s" alt="Entertainment">
                <h3>Entertainment</h3>
            </div>
        </div>
    </section>
    <footer>
        <p>&copy; 2024 Forum Mall. All Rights Reserved.</p>
    </footer>
</body>
</html>

hotel.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Welcome to One8 Restaurant - Delight in Exquisite Cuisines.">
    <title>Tempting kitchen</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #d80e0e;
        }

        header {
            background-color: #5f0808;
            color: rgb(182, 217, 41);
            padding: 15px 0;
            text-align: center;
        }

        nav ul {
            list-style: none;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            background-color: #051345;
        }

        nav ul li {
            margin: 0 15px;
        }

        nav ul li a {
            color: rgb(208, 232, 26);
            text-decoration: none;
            padding: 14px 20px;
            display: block;
        }

        nav ul li a:hover {
            background-color: #e31212;
        }

        section {
            padding: 20px;
            margin: 20px;
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }

        footer {
            background-color: #434040;
            color: white;
            text-align: center;
            padding:1px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }

        h1 {
            color: #e1d7d7;
        }

        .menu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            padding: 20px;
        }

        .menu-item {
            background-color: #e70f0f;
            padding: 20px;
            border-radius: 8px;
            text-align: center;
            box-shadow: 0 0 10px rgba(6, 3, 3, 0.1);
        }

        .menu-item h3,h4{
            margin: 0 0 10px 0;
        }

        .menu-item p {
            color: #080808;
        }
    </style>
</head>
<body>

<header>
    <h1>TEMPTING KITCHEN</h1>
    <p>SATISFY YOUR SENSES</p>
    <img src="c:\Users\monis\AppData\Local\Packages\5319275A.WhatsAppDesktop_cv1g1gvanyjgm\TempState\7BFA32686D200C64CB46DE03AC2EAC0D\WhatsApp Image 2024-12-07 at 10.20.36_df746a11.jpg"width="15%">
 </header>

<nav>
    <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#menu">Menu</a></li>
        <li><a href="#administration">Administration</a></li>
        <li><a href="#about">About Us</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>

<section id="home">
    <h2>Welcome to TEMPTING KITCHEN</h2>
    <p>Where every bite is a celebration of flavor! Our menu is a culinary adventure, crafted with fresh, locally sourced ingredients that tantalize your taste buds. Whether you're here for a cozy dinner or a special celebration, our warm atmosphere and dedicated staff ensure a memorable dining experience. Indulge in our signature dishes and discover why we’re a beloved destination for food lovers. Come savor the magic at Tempting Kitchen!</p>
</section>

<section id="menu">
    <h2>Our Menu</h2>
    <div class="menu-grid">
        <div class="menu-item">
            <h3>Parotta</h3>
            <img src="c:\Users\monis\Downloads\pexels-prabal-9609857.jpg"width="100%">
            <p><strong>RS.30</strong></p>
        </div>
        <div class="menu-item">
            <h3>Chicken biriyani</h3>
            <img src="c:\Users\monis\Downloads\pexels-mumtahina-tanni-1080117-6260921.jpg"width="100%">
            <p><strong>RS.200</strong></p>
        
    </div>
        <div class="menu-item">
            <h3>Chicken full grill</h3>
            <img src="c:\Users\monis\Downloads\pexels-mouktik-joshi-98936055-9646843.jpg"width="50%">
            <p><strong>RS.300</strong></p>
        </div>
        <div class="menu-item">
            <h3>Hot chicken gravy</h3>
            <img src="c:\Users\monis\Downloads\pexels-sahersuthriwala-6599106.jpg"width="100%">
            <p><strong>RS.190</strong></p>
        </div>
        <div class="menu-item">
            <h3>Chicken fried rice</h3>
            <img src="c:\Users\monis\Downloads\pexels-nadim-shaikh-2923533-7758253.jpg"width="100%">
            <p><strong>RS.180</strong></p>
        </div>
        <div class="menu-item">
            <h3>Chicken noodles</h3>
            <img src="c:\Users\monis\Downloads\Sichuan-Chilli-Chicken-Noodles-04.jpg"width="80%">
            <p><strong>RS.180</strong></p>
        </div>
        <div class="menu-item">
            <h3>Malai chicken</h3>
            <img src="c:\Users\monis\Downloads\pexels-harry-dona-2338407.jpg"width="100%">
            <p><strong>RS.250</strong></p>
        </div>
        <div class="menu-item">
            <h3>Fried Chicken</h3>
            <img src="c:\Users\monis\Downloads\Instant-Pot-Fried-Chicken.jpg"width="100%">
            <p><strong>RS.210</strong></p>
        </div>
        <div class="menu-item">
            <h3>Chicken burger</h3>
            <img src="c:\Users\monis\Downloads\pexels-k-patel-1100389468-20722066.jpg"width="80%">
            <p><strong>RS.210</strong></p>
        </div>
        <div class="menu-item">
            <h3>Chicken shawerma</h3>
            <img src="c:\Users\monis\Downloads\pexels-rajdeepcraft-17119248-6416559.jpg"width="80%">
            <p><strong>RS.180</strong></p>
        </div>
        <div class="menu-item">
            <h3>Mint mojito</h3>
            <img src="c:\Users\monis\Downloads\pexels-anilsharma65-10927828.jpg"width="100%">
            <p><strong>RS.160</strong></p>
        </div>
        <div class="menu-item">
            <h3>Black current Ice Cream</h3>
            <img src="c:\Users\monis\Downloads\pexels-alisha-mishra-579430-1343504.jpg"width="100%">
            <p><strong>RS.150</strong></p>
        </div>
    </div>
</section>
<section id="administration">
    <h2>Administration</h2>
    <div class="menu-grid">
        <div class="menu-item">
            <img src="c:\Users\monis\AppData\Local\Packages\5319275A.WhatsAppDesktop_cv1g1gvanyjgm\TempState\31839B036F63806CBA3F47B93AF8CCB5\WhatsApp Image 2024-11-23 at 11.45.19_932b052c.jpg"width="60%">
            <h3>FOUNDER</h3>
        </div>
        <div class="menu-item">
            <img src="c:\Users\monis\AppData\Local\Packages\5319275A.WhatsAppDesktop_cv1g1gvanyjgm\TempState\3B5DCA501EE1E6D8CD7B905F4E1BF723\WhatsApp Image 2024-11-23 at 11.45.51_c8e2881c.jpg"width="50%">
            <h3>MANAGER</h3>
        </div>
        <div class="menu-item">
            <img src="c:\Users\monis\AppData\Local\Packages\5319275A.WhatsAppDesktop_cv1g1gvanyjgm\TempState\E2A2DCC36A08A345332C751B2F2E476C\WhatsApp Image 2024-11-23 at 11.46.17_10b82e73.jpg"width="50%">
            <h3>BRAND AMBASSADOR</h3>
        </div>
    </div>
</section>

<section id="about">
    <h2>About Us</h2>
    <p>Tempting Kitchen is a popular restaurant known for its diverse menu and inviting atmosphere. It typically features a mix of cuisines, emphasizing fresh ingredients and bold flavors. Many locations focus on creating a warm, welcoming environment, making it a great spot for casual dining or special occasions.

        If you’re looking for specifics about its offerings, ambiance, or any signature dishes, let me know!
        We are in this field since 2006. Served 25000+ customers</p>
</section>

<section id="contact">
    <h2>Contact Us</h2>
    <p>Anna nagar, Chennai- 600001</p>
    <p>Phone: 9876543213</p>
    <p>Email: temptingkitchen@gmail.com</p>
</section>
<footer>
    <p>@Owned by MONISH.S</p>
</footer>

</body>
</html>

vanheusan.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Van Heusen - Premium Apparel</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            color: #333;
        }
        header {
            background-color: #000;
            color: #fff;
            padding: 1rem 0;
            text-align: center;
        }
        nav {
            background-color: #333;
            display: flex;
            justify-content: center;
            padding: 0.5rem 0;
        }
        nav a {
            color: #fff;
            text-decoration: none;
            margin: 0 1rem;
            font-weight: bold;
        }
        nav a:hover {
            text-decoration: underline;
        }
        .hero {
            background-image: url('hero-image.jpg');
            background-size: cover;
            background-position: center;
            height: 60vh;
            display: flex;
            justify-content: center;
            align-items: center;
            color: #fff;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.7);
        }
        .hero h1 {
            font-size: 3rem;
            margin: 0;
        }
        .content {
            padding: 2rem;
        }
        .products {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
        }
        .product {
            border: 1px solid #ddd;
            padding: 1rem;
            text-align: center;
        }
        .product img {
            max-width: 100%;
            height: auto;
        }
        footer {
            background-color: #000;
            color: #fff;
            text-align: center;
            padding: 1rem 0;
            margin-top: 2rem;
        }
    </style>
</head>
<body>
    <header>
        <h1>Van Heusen</h1>
        <p>Style Meets Comfort</p>
    </header>
    <nav>
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#products">Products</a>
        <a href="#contact">Contact</a>
    </nav>
    <section class="hero">
        <h1>Experience Luxury Clothing</h1>
    </section>
    <section class="content">
        <h2 id="products">Our Products</h2>
        <div class="products">
            <div class="product">
                <img src="https://trybuy.in/cdn/shop/files/TB_83_vD9e4AmWF_1200x1200.jpg?v=1706939606" alt="Men's Shirt">
                <h3>Men's Shirt</h3>
                <p>Premium Cotton - $49.99</p>
            </div>
            <div class="product">
                <img src="https://www.alamodelabel.in/cdn/shop/products/WhatsAppImage2022-12-16at11.18.57AM_600x.jpg?v=1717497743" alt="Women's Blazer">
                <h3>Women's Blazer</h3>
                <p>Elegant Style - $89.99</p>
            </div>
            <div class="product">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS5iOBGGDk6Ido6M19hObJ3iL5BPGknjcIzIw&s" alt="Accessories">
                <h3>Accessories</h3>
                <p>Finishing Touch - $19.99</p>
            </div>
        </div>
    </section>
    <footer>
        <p>&copy; 2024 Van Heusen. All Rights Reserved.</p>
    </footer>
</body>
</html>

```
# OUTPUT
![alt text](<Screenshot 2024-12-07 175415.png>)
![alt text](<Screenshot 2024-12-07 175621.png>)
![alt text](<Screenshot 2024-12-07 175714.png>)
![alt text](<Screenshot 2024-12-07 175819.png>)
# RESULT
The program for implementing image maps using HTML is executed successfully.
