<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MP CLOTH HANGERS</title>
    <style>
        /* Your CSS styles here */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            color: #333; /* Default text color */
            background-color: #f3f3f3; /* Default background color */
            transition: background-color 0.5s, color 0.5s; /* Smooth transition for background and text color */
        }

        /* Dark mode styles */
        body.dark-mode {
            color: #fff; /* Text color in dark mode */
            background-color: #333; /* Background color in dark mode */
        }

        /* Table text color in dark mode */
        body.dark-mode table td {
            color: #fff;
        }

        /* Other styles remain unchanged */
        header {
            background-color: #333;
            color: #fff;
            padding: 20px 0;
            text-align: center;
        }

        h1, h2, h3 {
            margin: 0;
        }

        nav ul {
            list-style-type: none;
            margin: 0;
            padding: 0;
            text-align: center;
        }

        nav ul li {
            display: inline;
            margin: 0 10px;
        }

        nav ul li a {
            text-decoration: none;
            color: #333;
            padding: 10px 15px;
            background-color: #fff;
            border-radius: 5px;
            transition: background-color 0.3s;
        }

        nav ul li a:hover {
            background-color: #555;
            color: #fff;
        }

        section {
            padding: 50px 20px;
            text-align: center;
        }

        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 20px 0;
            position: fixed;
            bottom: 0;
            width: 100%;
            display: none; /* Hide footer by default */
        }

        /* Product Table */
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }

        th, td {
            padding: 10px;
            border-bottom: 1px solid #ddd;
        }

        th {
            background-color: #555;
            color: #fff;
            text-align: left;
        }

        /* Flash Sale */
        .flash {
            background-color: #ff0000;
            color: #fff;
            padding: 5px 10px;
            display: inline-block;
            margin-bottom: 10px;
            border-radius: 5px;
            animation: flashAnimation 1s ease infinite alternate;
        }

        @keyframes flashAnimation {
            0% { opacity: 1; }
            100% { opacity: 0.5; }
        }

        /* Responsive */
        @media screen and (max-width: 768px) {
            nav ul li {
                display: block;
                margin: 10px 0;
            }
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
            <li><a href="#home">Home</a></li>
            <li><a href="#products">Products</a></li>
            <li><a href="#about">About Us</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Dark Mode Button -->
    <button onclick="toggleDarkMode()">Toggle Dark Mode</button>

    <!-- Content Sections -->
    <section id="home">
        <h2>Welcome to MP Cloth Hangers</h2>
        <p>Explore our range of cloth hanger solutions designed to maximize vertical space in your home.</p>
    </section>

    <section id="products">
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

    <section id="about">
        <h2>About Us</h2>
        <p>At MP Cloth Hangers, we specialize in providing high-quality, space-saving cloth hanger solutions to our customers. Our ceiling-mounted cloth hangers are designed to maximize vertical space in your home, making it easier than ever to dry and store your clothes without taking up valuable floor space.</p>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <p>For inquiries and support, please contact us at:</p>
        <p>Phone: 9133449704 (Mazhar), 8374166274 (Praveen)</p>
    </section>

    <!-- Footer -->
    <footer>
        <p>Contact: 9133449704 (Mazhar), 8374166274 (Praveen)</p>
        <p>&copy; 2024 MP CLOTH HANGERS. All rights reserved.</p>
    </footer>

    <script>
        // Function to toggle dark mode
        function toggleDarkMode() {
            document.body.classList.toggle('dark-mode');
        }
    </script>
</body>
</html>
body.dark-mode table td {
    color: #fff;
}

