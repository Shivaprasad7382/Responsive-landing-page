Responsive landing page
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Website Title</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
        }

        #navbar {
            position: fixed;
            top: 0;
            width: 100%;
            background: linear-gradient(to right, #007bff, #0056b3);
            /* Blue gradient */
            padding: 10px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            z-index: 1000;
            transition: background 0.3s ease-in-out;
        }

        #navbar a {
            color: white;
            text-decoration: none;
            padding: 10px 20px;
            margin: 0 10px;
            border-radius: 5px;
            transition: background 0.3s ease-in-out, color 0.3s ease-in-out;
        }

        #navbar a:hover {
            background: white;
            color: #007bff;
        }

        #section-01 {
            height: 100vh;
            background: linear-gradient(to right, #007bff, #0056b3);
            /* Blue gradient */
            color: white;
            text-align: center;
            padding-top: 50px;
        }

        /* Additional styling for your content sections */
        .content-section {
            padding: 50px;
            text-align: center;
        }
    </style>
</head>

<body>

    <div id="navbar">
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Services</a>
        <a href="#">Contact</a>
    </div>

    <div id="section-01">
        <h1>PRODIGY INFOTECH</h1>
        <h2>Task-01</h2>

        <h3>Responsive Landing Page</h3>
    </div>

    <div class="content-section">
        <!-- Your page content goes here -->
    </div>

    <script>
        document.addEventListener("DOMContentLoaded", function() {
            var navbar = document.getElementById("navbar");

            // Change the background color of the navbar on scroll
            window.addEventListener("scroll", function() {
                if (window.scrollY > 50) {
                    navbar.style.background = "white";
                    navbar.style.color = "#007bff";
                } else {
                    navbar.style.background = "linear-gradient(to right, #007bff, #0056b3)";
                    navbar.style.color = "white";
                }
            });
        });
    </script>

</body>

</html>

