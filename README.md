<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MP CLOTH HANGERS</title>
    <style>
        /* Resetting default margin and padding */
        body, h1, h2, p, ul, li {
            margin: 0;
            padding: 0;
        }

        /* Global styles */
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            background-color: #000;
            color: #fff;
        }

        /* Header styles */
        header {
            background-color: #333;
            padding: 20px;
            text-align: center;
        }

        header h1 {
            font-size: 24px;
        }

        /* Navigation menu styles */
        nav {
            background-color: #444;
            padding: 10px;
        }

        nav ul {
            list-style-type: none;
            text-align: center;
        }

        nav ul li {
            display: inline;
            margin-right: 20px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
        }

        /* Content section styles */
        section {
            padding: 20px;
            margin: 20px 0;
            background-color: #222;
        }

        section h2 {
            font-size: 20px;
            margin-bottom: 10px;
        }

        /* Footer styles */
        footer {
            background-color: #333;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
            transition: transform 0.3s ease;
        }

        .footer-hidden {
            transform: translateY(100%);
        }

        /* Flash styles */
        .flash {
            background-color: #ff0000;
            color: #fff;
            padding: 5px 10px;
            display: inline-block;
            margin-bottom: 10px;
            animation: flashAnimation 1s ease infinite alternate;
        }

        @keyframes flashAnimation {
            0% { opacity: 1; }
            100% { opacity: 0.5; }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <h1>MP CLOTH HANGERS</h1>
        <p>Hang Right, Hang Tight</p>
    </header>

    <!-- Navigation Menu -->
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">Products</a></li>
            <li><a href="#">About Us</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>

    <!-- Content Sections -->
    <section>
        <h2>Products</h2>
        <ul>
            <li>Regular <span class="flash">₹200 OFF!</span></li>
            <ul>
                <li>8 Feet 6 Rods - ₹2800</li>
                <li>7 Feet 6 Rods - ₹2700</li>
                <li>6 Feet 6 Rods - ₹2600</li>
                <li>5 Feet 6 Rods - ₹2500</li>
                <li>4 Feet 6 Rods - ₹2400</li>
            </ul>
            <li>Heavy <span class="flash">₹500 OFF!</span></li>
            <ul>
                <li>8 Feet 6 Rods - ₹3100</li>
                <li>7 Feet 6 Rods - ₹3000</li>
                <li>6 Feet 6 Rods - ₹2900</li>
                <li>5 Feet 6 Rods - ₹2800</li>
                <li>4 Feet 6 Rods - ₹2700</li>
            </ul>
        </ul>
    </section>

    <section>
        <h2>About Us</h2>
        <p>At MP Cloth Hangers, we specialize in providing high-quality, space-saving cloth hanger solutions to our customers. Our ceiling-mounted cloth hangers are designed to maximize vertical space in your home, making it easier than ever to dry and store your clothes without taking up valuable floor space.</p>
    </section>

    <!-- Footer -->
    <footer id="footer">
        <p>Contact: 9133449704 (Mazhar), 8374166274 (Praveen)</p>
        <p>&copy; 2024 MP CLOTH HANGERS. All rights reserved.</p>
    </footer>

    <script>
        window.addEventListener('scroll', function() {
            const footer = document.getElementById('footer');
            if (window.scrollY > 100) {
                footer.classList.add('footer-hidden');
            } else {
                footer.classList.remove('footer-hidden');
            }
        });
    </script>
</body>
</html>
