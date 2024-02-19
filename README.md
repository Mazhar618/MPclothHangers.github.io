<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MP CLOTH HANGERS</title>
    <style>
        /* Your CSS styles here */
        body {
            /* Dark mode styles */
            background-color: #0c0c0c;
            color: #f2f2f2;
            font-family: Arial, sans-serif;
        }

        /* Header styles */
        header {
            background-color: #333;
            padding: 20px;
            text-align: center;
            color: #fff;
        }

        header h1 {
            font-size: 36px;
            margin-bottom: 10px;
        }

        header p {
            font-size: 18px;
            margin-bottom: 20px;
        }

        /* Navigation menu styles */
        nav {
            background-color: #444;
            padding: 10px;
            text-align: center;
        }

        nav ul {
            list-style-type: none;
            display: inline;
        }

        nav ul li {
            display: inline-block;
            margin-right: 20px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            padding: 10px;
            transition: all 0.3s ease;
        }

        nav ul li a:hover {
            background-color: #555;
            border-radius: 5px;
        }

        /* Content sections styles */
        section {
            padding: 20px;
            margin: 20px 0;
            background-color: #222;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
            animation: fadeIn 1s ease;
        }

        section h2 {
            font-size: 24px;
            margin-bottom: 10px;
            color: #fff;
        }

        section p {
            color: #ccc;
        }

        /* Footer styles */
        footer {
            background-color: #333;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
            color: #fff;
            display: none;
            animation: slideInUp 1s ease;
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

        /* Product list styles */
        .products {
            display: none;
        }

        /* Product image styles */
        .product-image {
            width: 100px; /* Adjust width as needed */
            height: auto; /* Maintain aspect ratio */
            margin-bottom: 10px;
        }

        /* Table styles */
        table {
            width: 100%;
            border-collapse: collapse;
            margin-bottom: 20px;
        }

        th, td {
            border: 1px solid #fff;
            padding: 8px;
            text-align: left;
        }

        th {
            background-color: #555;
            color: #fff;
        }

        td {
            background-color: #444;
            color: #ccc;
        }

        /* Keyframe animations */
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes slideInUp {
            from { transform: translateY(100px); }
            to { transform: translateY(0); }
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
            <li><a href="#" onclick="showHome()">Home</a></li>
            <li><a href="#" onclick="showProducts()">Products</a></li>
            <li><a href="#" onclick="showAbout()">About Us</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>

    <!-- Content Sections -->
    <section id="home">
        <h2>Welcome to MP Cloth Hangers</h2>
        <p>Explore our range of cloth hanger solutions designed to maximize vertical space in your home.</p>
    </section>

    <section id="products" class="products">
        <h2>Products</h2>
        <div class="flash">Flash Sale</div>
        <table>
            <thead>
                <tr>
                    <th>Category</th>
                    <th>Name</th>
                    <th>Price</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td rowspan="5">Regular</td>
                    <td>8 Feet 6 Rods</td>
                    <td>₹2600</td>
                </tr>
                <tr>
                    <td>7 Feet 6 Rods</td>
                    <td>₹2500</td>
                </tr>
                <tr>
                    <td>6 Feet 6 Rods</td>
                    <td>₹2400</td>
                </tr>
                <tr>
                    <td>5 Feet 6 Rods</td>
                    <td>₹2300</td>
                </tr>
                <tr>
                    <td>4 Feet 6 Rods</td>
                    <td>₹2200</td>
                </tr>
                <tr>
                    <td rowspan="5">Heavy</td>
                    <td>8 Feet 6 Rods</td>
                    <td>₹3100</td>
                </tr>
                <tr>
                    <td>7 Feet 6 Rods</td>
                    <td>₹3000</td>
                </tr>
                <tr>
                    <td>6 Feet 6 Rods</td>
                    <td>₹2900</td>
                </tr>
                <tr>
                    <td>5 Feet 6 Rods</td>
                    <td>₹2800</td>
                </tr>
                <tr>
                    <td>4 Feet 6 Rods</td>
                    <td>₹2700</td>
                </tr>
            </tbody>
        </table>
    </section>

    <!-- About Us Section -->
    <section id="about" class="about" style="display: none;">
        <h2>About Us</h2>
        <p>At MP Cloth Hangers, we specialize in providing high-quality, space-saving cloth hanger solutions to our customers. Our ceiling-mounted cloth hangers are designed to maximize vertical space in your home, making it easier than ever to dry and store your clothes without taking up valuable floor space.</p>
        <p>Contact: 9133449704 (Mazhar), 8374166274 (Praveen)</p>
    </section>

    <!-- Footer -->
    <footer id="footer">
        <p>Contact: 9133449704 (Mazhar), 8374166274 (Praveen)</p>
        <p>&copy; 2024 MP CLOTH HANGERS. All rights reserved.</p>
    </footer>

    <script>
        // Function to show home section
        function showHome() {
            var homeSection = document.getElementById('home');
            var productsSection = document.getElementById('products');
            var aboutSection = document.getElementById('about');
            var footer = document.getElementById('footer');

            homeSection.style.display = 'block';
            productsSection.style.display = 'none';
            aboutSection.style.display = 'none';
            footer.style.display = 'none';
        }

        // Function to show products section
        function showProducts() {
            var productsSection = document.getElementById('products');
            productsSection.style.display = 'block';
            var footer = document.getElementById('footer');
            footer.style.display = 'block';
        }

        // Function to show about us section
        function showAbout() {
            var aboutSection = document.getElementById('about');
            aboutSection.style.display = 'block';
            var footer = document.getElementById('footer');
            footer.style.display = 'block';
        }
    </script>
</body>
</html>
