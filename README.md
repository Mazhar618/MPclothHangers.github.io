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
    </style>
</head>
<body>
    <!-- Your HTML content here -->

    <!-- Header -->
    <header>
        <h1>MP CLOTH HANGERS</h1>
        <p>Hang Right, Hang Tight</p>
    </header>

    <!-- Navigation Menu -->
    <nav>
        <ul>
            <li><a href="#" onclick="showProducts()">Products</a></li>
            <li><a href="#">About Us</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>

    <!-- Content Sections -->
    <section id="products" class="products">
        <h2>Products</h2>
        <ul id="product-list"></ul>
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
        // Array of products
        var products = [
            { category: 'Regular', name: '8 Feet 6 Rods', price: '₹2800', image: 'product1.jpg' },
            { category: 'Regular', name: '7 Feet 6 Rods', price: '₹2700', image: 'product2.jpg' },
            // Add more products with their image file names
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

    <!-- Button to toggle dark mode -->
    <button onclick="toggleDarkMode()">Toggle Dark Mode</button>
</body>
</html>
