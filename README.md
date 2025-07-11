# Prodigytask1
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Responsive Landing Page</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(to right, #2980b9, #6dd5fa);
      color: white;
    }

    header {
      position: fixed;
      top: 0;
      width: 100%;
      background-color: rgba(0, 0, 0, 0.7);
      padding: 15px 0;
      text-align: center;
      transition: background-color 0.3s;
      z-index: 1000;
    }

    header.scrolled {
      background-color: rgba(0, 0, 0, 0.9);
    }

    nav a {
      margin: 0 15px;
      text-decoration: none;
      color: white;
      font-weight: bold;
      transition: color 0.3s;
    }

    nav a:hover {
      color: #ffcc00;
    }

    .hero {
      padding: 150px 20px 100px;
      text-align: center;
    }

    .hero h1 {
      font-size: 3rem;
      margin-bottom: 20px;
    }

    .hero p {
      font-size: 1.2rem;
    }

    @media (max-width: 768px) {
      .hero h1 {
        font-size: 2rem;
      }

      nav a {
        display: block;
        margin: 10px 0;
      }
    }
  </style>
</head>
<body>

  <header id="navbar">
    <nav>
      <a href="#">Home</a>
      <a href="#">About</a>
      <a href="#">Services</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  <div class="hero">
    <h1>Welcome to My Landing Page</h1>
    <p>This is a simple and responsive landing page created using HTML, CSS, and JavaScript.</p>
  </div>

  <script>
    const navbar = document.getElementById('navbar');
    window.addEventListener('scroll', () => {
      if (window.scrollY > 50) {
        navbar.classList.add('scrolled');
      } else {
        navbar.classList.remove('scrolled');
      }
    });
  </script>

</body>
</html>
