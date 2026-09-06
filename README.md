# Ex.No:08 Responsive Web Design using Bootstrap
# Date:4/09/2026
# AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

## Step 5:
Create a HTML file and include the needed Bootstrap components.

## Step 6:
Publish the website in the LocalHost.

# PROGRAM :
~~~
<!DOCTYPE html>
<html>
<head>
    <title>Dribbble</title>

    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: #f5f5f5;
        }

        .navbar {
            display: flex;
            align-items: center;
            gap: 25px;
            padding: 18px 40px;
            background: #333;
            color: white;
        }

        .logo {
            font-size: 22px;
            font-weight: bold;
        }

        .navbar a {
            color: #bbb;
            text-decoration: none;
        }

        .navbar a:hover {
            color: white;
        }

        .search {
            margin-left: auto;
            padding: 8px;
            border: none;
            border-radius: 5px;
            background: #444;
            color: white;
        }

        button {
            padding: 9px 15px;
            border-radius: 5px;
            cursor: pointer;
        }

        .sign-up {
            border: none;
            background: #ea4c89;
            color: white;
        }

        .learn-more {
            border: 1px solid #666;
            background: transparent;
            color: white;
        }

        .hero {
            padding: 40px 20px;
            text-align: center;
            background: #444;
            color: white;
        }

        .hero p {
            color: #ccc;
        }

        .filters {
            display: flex;
            justify-content: space-between;
            padding: 15px 50px;
            background: white;
        }

        select {
            padding: 7px;
            border: 1px solid #ddd;
            border-radius: 5px;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 25px;
            padding: 40px;
        }

        .card img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            border-radius: 8px;
        }

        .info {
            display: flex;
            justify-content: space-between;
            padding: 10px 2px;
            font-size: 13px;
        }

        .author {
            font-weight: bold;
        }

        .stats {
            color: #888;
        }
    </style>
</head>

<body>
    <header class="navbar">
        <div class="logo">Dribbble</div>

        <a href="#">Inspiration</a>
        <a href="#">Find Work</a>
        <a href="#">Learn Design</a>
        <a href="#">Go Pro</a>

        <input class="search" type="text" placeholder="Search shots...">

        <a href="#">Sign in</a>
        <button class="sign-up">Sign up</button>
    </header>

    <section class="hero">
        <h1>Discover the world’s top designers & creatives</h1>
        <p>Find and showcase creative work.</p>

        <button class="sign-up">Sign up</button>
        <button class="learn-more">Learn more</button>
    </section>

    <section class="filters">
        <div>
            <select>
                <option>Popular</option>
                <option>Newest</option>
            </select>

            <select>
                <option>All Shots</option>
                <option>PC Setups</option>
                <option>Accessories</option>
            </select>
        </div>

        <select>
            <option>Now</option>
            <option>This Week</option>
            <option>This Month</option>
        </select>
    </section>

    <main class="grid">
        <div class="card">
            <img src="pc1.jpg" alt="Gaming PC">
            <div class="info">
                <span class="author">PC Master</span>
                <span class="stats">👁 4.2k ♥ 512</span>
            </div>
        </div>

        <div class="card">
            <img src="pc2.jpg" alt="Laptop">
            <div class="info">
                <span class="author">Tech Byte</span>
                <span class="stats">👁 3.6k ♥ 436</span>
            </div>
        </div>

        <div class="card">
            <img src="pc3.jpg" alt="Monitor">
            <div class="info">
                <span class="author">Pixel Setup</span>
                <span class="stats">👁 2.9k ♥ 312</span>
            </div>
        </div>

        <div class="card">
            <img src="pc4.jpg" alt="Keyboard">
            <div class="info">
                <span class="author">Keys & Clicks</span>
                <span class="stats">👁 3.2k ♥ 408</span>
            </div>
        </div>
    </main>
</body>
</html>
~~~

# OUTPUT:

![alt text](image.png)

# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
