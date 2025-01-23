/* General styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

body {
    background: #000;
    background-image: url('background-small.jpg'); /* Replace with the correct path */
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    min-height: 200vh;
}

/* Header styling */
header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 40px 100px;
    transition: padding 0.6s, background 0.6s;
    z-index: 10;
}

header.sticky {
    padding: 5px 100px;
    background: #fff;
}

header .logo {
    font-weight: 700;
    color: #fff;
    text-decoration: none;
    font-size: 2em;
    text-transform: uppercase;
    letter-spacing: 2px;
    transition: color 0.6s;
}

header.sticky .logo {
    color: #000;
}

header ul {
    display: flex;
    justify-content: center;
}

header ul li {
    list-style: none;
}

header ul li a {
    margin: 0 15px;
    text-decoration: none;
    color: #fff;
    letter-spacing: 2px;
    font-weight: 500;
    transition: color 0.6s;
}

header.sticky ul li a {
    color: #000;
}

header nav ul {
    list-style: none;
    display: flex;
    gap: 15px;
}

header nav ul li a:hover {
    color: #f39c12;
}

/* Navbar for mobile screens */
@media (max-width: 768px) {
    header {
        padding: 20px;
    }

    header ul {
        flex-direction: column;
        gap: 10px;
    }
}

/* Hero section */
.hero {
    width: 100%;
    height: 100vh;
    background: url('bg.jpg'); /* Replace with the correct path */
    background-size: cover;
    color: white;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
}

.hero h1 {
    font-size: 3em;
}

/* Images */
img {
    max-width: 100%;
    height: auto;
    display: block;
}

.card-img-top {
    height: 200px;
    object-fit: cover;
}

.gallery img {
    border-radius: 5px;
}

/* Footer */
footer {
    background-color: #343a40;
    color: white;
    padding: 20px 0;
    text-align: center;
}

/* Sticky Navbar */
.navbar {
    background-color: #343a40;
}

.navbar.sticky-top {
    position: sticky;
    top: 0;
    z-index: 1000;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

/* Navbar Links */
.navbar-nav .nav-item .nav-link {
    color: white;
    font-size: 16px;
    padding: 10px 20px;
    transition: color 0.3s;
}

.navbar-nav .nav-item .nav-link:hover {
    color: #f8f9fa;
}

.navbar-toggler-icon {
    background-color: white;
}

/* Adjustments for mobile */
@media (max-width: 768px) {
    .navbar {
        background-color: #343a40;
    }
}

/* Price styling */
.original-price {
    text-decoration: line-through;
    color: #888;
    margin-right: 10px;
}

.discounted-price {
    font-weight: bold;
    color: #e74c3c;
    font-size: 1.2em;
}
