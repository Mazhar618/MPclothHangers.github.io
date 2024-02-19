<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MP CLOTH HANGERS</title>
    <style>
        /* Your CSS styles here */
        body {
            /* Dark mode styles */
            background-color: #000;
            color: #fff;
        }

        .dark-mode body {
            /* Light mode styles */
            background-color: #fff;
            color: #000;
        }
        
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
            cursor: pointer;
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
            background-color: #444;
            color: #fff;
        }

        td {
            background-color: #222;
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
            <li><a href="#" onclick="showProducts()">Products</a></li>
            <li><a href="#">About Us</a></li>
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
                    <td>₹2800</td>
                </tr>
                <tr>
                    <td>7 Feet 6 Rods</td>
                    <td>₹2700</td>
                </tr>
                <tr>
                    <td>6 Feet 6 Rods</td>
                    <td>₹2600</td>
                </tr>
                <tr>
                    <td>5 Feet 6 Rods</td>
                    <td>₹2500</td>
                </tr>
                <tr>
                    <td>4 Feet 6 Rods</td>
                    <td>₹2400</td>
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

    <section>
        <h2>About Us</h2>
        <p>At MP Cloth Hangers, we specialize in providing high-quality, space-saving cloth hanger solutions to our customers. Our ceiling-mounted cloth hangers are designed to maximize vertical space in your home, making it easier than ever to dry and store your clothes without taking up valuable floor space.</p>
    </section>

    <!-- Footer -->
    <footer id="footer">
        <p>Contact: 9133449704 (Mazhar), 8374166274 (Praveen)</p>
        <p>&copy; 2024 MP CLOTH HANGERS. All rights reserved.</p>
    </footer>

    <!-- Button to toggle dark mode -->
    <button onclick="toggleDarkMode()">Toggle Dark Mode</button>

    <script>
        // Array of products
        var products = [
            { category: 'Regular', name: '8 Feet 6 Rods', price: '₹2800', image: 'product1.jpg' },
            { category: 'Regular', name: '7 Feet 6 Rods', price: '₹2700', image: 'product2.jpg' },
            { category: 'Regular', name: '6 Feet 6 Rods', price: '₹2600', image: 'product3.jpg' },
            { category: 'Regular', name: '5 Feet 6 Rods', price: '₹2500', image: 'product4.jpg' },
            { category: 'Regular', name: '4 Feet 6 Rods', price: '₹2400', image: 'product5.jpg' },
            { category: 'Heavy', name: '8 Feet 6 Rods', price: '₹3100', image: 'product6.jpg' },
            { category: 'Heavy', name: '7 Feet 6 Rods', price: '₹3000', image: 'product7.jpg' },
            { category: 'Heavy', name: '6 Feet 6 Rods', price: '₹2900', image: 'product8.jpg' },
            { category: 'Heavy', name: '5 Feet 6 Rods', price: '₹2800', image: 'product9.jpg' },
            { category: 'Heavy', name: '4 Feet 6 Rods', price: '₹2700', image: 'product10.jpg' }
        ];

        // Function to display products
        function displayProducts() {
            var productList = document.getElementById('product-list');

            // Clear existing products
            productList.innerHTML = '';

            // Loop through products array
            products.forEach(function(product) {
                // Create list item for each product
                var listItem = document.createElement('li');

                // Create an image element
                var image = document.createElement('img');
                image.src = product.image;
                image.alt = product.name; // You can set alt text to the product name
                image.classList.add('product-image'); // Add a class for styling

                // Append image to list item
                listItem.appendChild(image);

                // Create paragraph for product details
                var details = document.createElement('p');
                details.textContent = product.category + ': ' + product.name + ' - ' + product.price;

                // Append details to list item
                listItem.appendChild(details);

                // Append list item to product list
                productList.appendChild(listItem);
            });
        }

        // Call the function to display products
        displayProducts();

        // Function to show products section
        function showProducts() {
            var productsSection = document.getElementById('products');
            productsSection.style.display = 'block';
        }

        // Hide footer when scrolling
        window.addEventListener('scroll', function() {
            const footer = document.getElementById('footer');
            if (window.scrollY > 100) {
                footer.classList.add('footer-hidden');
            } else {
                footer.classList.remove('footer-hidden');
            }
        });

        // Toggle dark mode
        function toggleDarkMode() {
            document.body.classList.toggle('dark-mode');
        }
    </script>
</body>
</html>
