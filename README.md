<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MP CLOTH HANGERS</title>
    <style>
        /* Your CSS styles here */
        /* Existing styles remain unchanged */

        /* Smooth scrolling */
        html {
            scroll-behavior: smooth;
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
            <li><a href="#home" onclick="showSection('home')">Home</a></li>
            <li><a href="#products" onclick="showSection('products')">Products</a></li>
            <li><a href="#about" onclick="showSection('about')">About Us</a></li>
            <li><a href="#contact" onclick="showSection('contact')">Contact</a></li> <!-- Added Contact link -->
        </ul>
    </nav>

    <!-- Content Sections -->
    <section id="home">
        <h2>Welcome to MP Cloth Hangers</h2>
        <p>Explore our range of cloth hanger solutions designed to maximize vertical space in your home.</p>
    </section>

    <section id="products" class="products" style="display: none;">
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

    <section id="about" class="about" style="display: none;">
        <h2>About Us</h2>
        <p>At MP Cloth Hangers, we specialize in providing high-quality, space-saving cloth hanger solutions to our customers. Our ceiling-mounted cloth hangers are designed to maximize vertical space in your home, making it easier than ever to dry and store your clothes without taking up valuable floor space.</p>
        <p>Contact: 9133449704 (Mazhar), 8374166274 (Praveen)</p>
    </section>

    <section id="contact" class="contact" style="display: none;">
        <h2>Contact Us</h2>
        <p>For inquiries and support, please contact us at:</p>
        <ul>
            <li>Phone: 9133449704 (Mazhar)</li>
            <li>Phone: 8374166274 (Praveen)</li>
            <li>Email: example@example.com</li>
        </ul>
    </section>

    <!-- Footer -->
    <footer id="footer" style="display: none;">
        <p>Contact: 9133449704 (Mazhar), 8374166274 (Praveen)</p>
        <p>&copy; 2024 MP CLOTH HANGERS. All rights reserved.</p>
    </footer>

    <script>
        // Function to show section based on id
        function showSection(sectionId) {
            // Hide all sections and footer
            var sections = document.querySelectorAll('section');
            sections.forEach(function(section) {
                section.style.display = 'none';
            });
            var footer = document.getElementById('footer');
            footer.style.display = 'none';

            // Show selected section
            var selectedSection = document.getElementById(sectionId);
            if (selectedSection) {
                selectedSection.style.display = 'block';
            }
            if (sectionId === 'about' || sectionId === 'contact') {
                footer.style.display = 'block';
            }
        }
    </script>
</body>
</html>
