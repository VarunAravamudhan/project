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
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <style>
        body {
            margin: 0;
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            background: #f5f5f5;
        }

        .navbar {
            background: #333;
            padding: 12px 40px;
            min-height: 70px;
        }

        .logo {
            color: white;
            font-size: 22px;
            font-weight: 800;
            letter-spacing: -0.5px;
            margin-right: 40px;
        }

        .nav-links {
            display: flex;
            list-style: none;
            margin: 0;
            padding: 0;
            align-items: center;
        }

        .nav-links li {
            margin-right: 25px;
        }

        .nav-links a {
            color: #bbb;
            text-decoration: none;
            font-size: 14px;
            font-weight: 500;
        }

        .nav-links a:hover {
            color: white;
            text-decoration: none;
        }

        .nav-links a.active {
            color: white;
            font-weight: bold;
        }

        .auth {
            margin-left: auto;
            display: flex;
            align-items: center;
            gap: 20px;
        }

        .auth a {
            color: #bbb;
            text-decoration: none;
            font-size: 14px;
            font-weight: 500;
        }

        .auth a:hover {
            color: white;
        }

        .search {
            width: 180px;
            height: 38px;
            border: none;
            padding: 6px 14px;
            border-radius: 6px;
            background: #444;
            color: white;
            font-size: 14px;
        }

        .search::placeholder {
            color: #888;
        }

        .sub-header {
            background: #444;
            padding: 40px 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            color: white;
            text-align: center;
        }

        .sub-header h1 {
            font-size: 28px;
            font-weight: 700;
            margin-bottom: 10px;
        }

        .sub-header p {
            margin: 0 0 20px 0;
            font-size: 15px;
            color: #ccc;
        }

        .sub-header-actions {
            display: flex;
            gap: 10px;
        }

        .learn-more {
            padding: 10px 18px;
            border: 1px solid #666;
            background: transparent;
            border-radius: 6px;
            color: white;
            font-size: 14px;
            font-weight: 500;
        }

        .sign-up {
            padding: 10px 18px;
            border: none;
            border-radius: 6px;
            background: #ea4c89;
            color: white;
            font-size: 14px;
            font-weight: 500;
        }

        .filter-bar {
            background: white;
            height: 60px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 50px;
            border-bottom: 1px solid #e7e7e7;
        }

        .filter-dropdowns {
            display: flex;
            gap: 10px;
        }

        .filter-bar select {
            border: 1px solid #e7e7e7;
            background: white;
            padding: 6px 12px;
            border-radius: 6px;
            font-weight: 600;
            font-size: 13px;
            color: #333;
        }

        .grid {
            padding: 40px 40px;
        }

        .card {
            background: transparent;
            border: none;
            margin-bottom: 30px;
        }

        .card-image {
            background: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 2px 8px rgba(0,0,0,0.04);
        }

        .card-image img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            display: block;
        }

        .card-footer-info {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-top: 10px;
            padding: 0 2px;
        }

        .author {
            display: flex;
            align-items: center;
            font-size: 13px;
            font-weight: 600;
            color: #333;
        }

        .author-circle {
            display: inline-flex;
            width: 24px;
            height: 24px;
            border-radius: 50%;
            background: #333;
            color: white;
            align-items: center;
            justify-content: center;
            font-size: 11px;
            font-weight: bold;
            margin-right: 8px;
        }

        .stats {
            display: flex;
            gap: 12px;
            color: #999;
            font-size: 12px;
            font-weight: 500;
        }

        .stat-item {
            display: flex;
            align-items: center;
            gap: 4px;
        }
    </style>
</head>
<body>

<header class="navbar">
    <div class="logo">
        Dribbble
    </div>
    <nav>
        <ul class="nav-links">
            <li><a href="#" class="active">Inspiration</a></li>
            <li><a href="#">Find Work</a></li>
            <li><a href="#">Learn Design</a></li>
            <li><a href="#">Go Pro</a></li>
            <li><a href="#">Hire Designers</a></li>
        </ul>
    </nav>
    <div class="auth">
        <input type="text" class="search" placeholder="Search shots...">
        <a href="#">Sign in</a>
        <a href="#" class="btn btn-sm sign-up">Sign up</a>
    </div>
</header>

<section class="sub-header">
    <h1>Discover the world’s top designers & creatives</h1>
    <p>Dribbble is the leading destination to find & showcase creative work and home to the world's best design professionals.</p>
    <div class="sub-header-actions">
        <button class="sign-up">Sign up</button>
        <button class="learn-more">Learn more</button>
    </div>
</section>

<section class="filter-bar">
    <div class="filter-dropdowns">
        <select>
            <option>Popular</option>
            <option>Newest</option>
        </select>
        <select>
            <option>All Shots</option>
            <option>PC Setups</option>
            <option>Components</option>
            <option>Accessories</option>
        </select>
    </div>
    <select>
        <option>Now</option>
        <option>This Week</option>
        <option>This Month</option>
        <option>All Time</option>
    </select>
</section>

<main class="grid">
    <div class="container-fluid">
        <div class="row">
            
            <!-- Card 1 -->
            <div class="col-12 col-sm-6 col-md-4 col-lg-3">
                <div class="card">
                    <div class="card-image">
                        <img src="pc1.jpg" alt="Gaming PC">
                    </div>
                    <div class="card-footer-info">
                        <div class="author">
                            <span class="author-circle">P</span>
                            PC Master
                        </div>
                        <div class="stats">
                            <span class="stat-item">👁 4.2k</span>
                            <span class="stat-item">♥ 512</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Card 2 -->
            <div class="col-12 col-sm-6 col-md-4 col-lg-3">
                <div class="card">
                    <div class="card-image">
                        <img src="pc2.jpg" alt="Laptop">
                    </div>
                    <div class="card-footer-info">
                        <div class="author">
                            <span class="author-circle">T</span>
                            Tech Byte
                        </div>
                        <div class="stats">
                            <span class="stat-item">👁 3.6k</span>
                            <span class="stat-item">♥ 436</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Card 3 -->
            <div class="col-12 col-sm-6 col-md-4 col-lg-3">
                <div class="card">
                    <div class="card-image">
                        <img src="pc3.jpg" alt="Monitor">
                    </div>
                    <div class="card-footer-info">
                        <div class="author">
                            <span class="author-circle">P</span>
                            Pixel Setup
                        </div>
                        <div class="stats">
                            <span class="stat-item">👁 2.9k</span>
                            <span class="stat-item">♥ 312</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Card 4 -->
            <div class="col-12 col-sm-6 col-md-4 col-lg-3">
                <div class="card">
                    <div class="card-image">
                        <img src="pc4.jpg" alt="Keyboard">
                    </div>
                    <div class="card-footer-info">
                        <div class="author">
                            <span class="author-circle">K</span>
                            Keys & Clicks
                        </div>
                        <div class="stats">
                            <span class="stat-item">👁 3.2k</span>
                            <span class="stat-item">♥ 408</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Card 5 -->
            <div class="col-12 col-sm-6 col-md-4 col-lg-3">
                <div class="card">
                    <div class="card-image">
                        <img src="pc5.jpg" alt="Mouse">
                    </div>
                    <div class="card-footer-info">
                        <div class="author">
                            <span class="author-circle">G</span>
                            Gear Lab
                        </div>
                        <div class="stats">
                            <span class="stat-item">👁 3.7k</span>
                            <span class="stat-item">♥ 298</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Card 6 -->
            <div class="col-12 col-sm-6 col-md-4 col-lg-3">
                <div class="card">
                    <div class="card-image">
                        <img src="pc14.jpg" alt="Motherboard">
                    </div>
                    <div class="card-footer-info">
                        <div class="author">
                            <span class="author-circle">B</span>
                            Board Builder
                        </div>
                        <div class="stats">
                            <span class="stat-item">👁 2.3k</span>
                            <span class="stat-item">♥ 243</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Card 7 -->
            <div class="col-12 col-sm-6 col-md-4 col-lg-3">
                <div class="card">
                    <div class="card-image">
                        <img src="pc16.jpg" alt="Gaming Chair">
                    </div>
                    <div class="card-footer-info">
                        <div class="author">
                            <span class="author-circle">C</span>
                            Comfort Gear
                        </div>
                        <div class="stats">
                            <span class="stat-item">👁 2.1k</span>
                            <span class="stat-item">♥ 187</span>
                        </div>
                    </div>
                </div>
            </div>

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
