<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Landing Page</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      line-height: 1.6;
      color: black;
    }

    /* Header */
    header {
      background: black;
      color: white;
      padding: 15px 5%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    header h1 {
      font-size: 24px;
    }

    nav ul {
      list-style: none;
      display: flex;
      gap: 20px;
    }

    nav ul li a {
      text-decoration: none;
      color: white;
      font-weight: bold;
      transition: color 0.3s;
    }

    nav ul li a:hover {
      color: #f39c12;
    }

    /* Hero */
    .hero {
      height: 90vh;
      background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)),
                  url("/image/pexels-bri-schneiter-28802-346529.jpg") center/cover no-repeat;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: white;
      padding: 0 10%;
    }

    .hero h2 {
      font-size: 48px;
      margin-bottom: 15px;
    }

    .hero p {
      font-size: 18px;
      margin-bottom: 20px;
    }

    .btn {
      background: #f39c12;
      padding: 12px 25px;
      color: white;
      text-decoration: none;
      border-radius: 5px;
      font-weight: bold;
      transition: background 0.3s;
    }

    .btn:hover {
      background: #e67e22;
    }

    /* About */
    .about {
      padding: 60px 10%;
      text-align: center;
    }

    .about h2 {
      margin-bottom: 20px;
      font-size: 32px;
    }

    .about p {
      max-width: 800px;
      margin: auto;
    }

    /* Services */
    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      padding: 60px 10%;
      background: #f9f9f9;
    }

    .service {
      background: white;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      transition: transform 0.3s;
    }

    .service:hover {
      transform: translateY(-10px);
    }

    .service h3 {
      margin-bottom: 15px;
      font-size: 22px;
      color: #f39c12;
    }

    /* Footer */
    footer {
      background: #222;
      color: white;
      text-align: center;
      padding: 20px;
    }

    footer p {
      font-size: 14px;
    }

    /* Responsive */
    @media (max-width: 768px) {
      .hero h2 {
        font-size: 32px;
      }
      .hero p {
        font-size: 16px;
      }
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <h1>My Landing Page</h1>
    <nav>
      <ul>
        <li><a href="#hero">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="hero" id="hero">
    <h2>Welcome to My Landing Page</h2>
    <p>Create beautiful websites with HTML & CSS</p>
    <a href="#services" class="btn">Get Started</a>
  </section>

  <!-- About Section -->
  <section class="about" id="about">
    <h2>About Us</h2>
    <p>
      I’m a passionate Frontend Developer who loves turning ideas into interactive and visually appealing web experiences. With strong skills in HTML, CSS, and JavaScript, I focus on building responsive, user-friendly websites that combine clean design with smooth functionality. My goal is to create digital solutions that are not only functional but also leave a lasting impression on users.
  </section>

  <!-- Services Section -->
  <section class="services" id="services">
    <div class="service">
      <h3>Web Design</h3>
      <p>Creative and modern website design with responsive layouts.</p>
    </div>
    <div class="service">
      <h3>Development</h3>
      <p>Clean and efficient code using HTML, CSS, and JavaScript.</p>
    </div>
    <div class="service">
      <h3>SEO</h3>
      <p>Optimized websites for better ranking and visibility.</p>
    </div>
  </section>

  <!-- Footer -->
  <footer id="contact">
    <p>&copy; Contact:+918878251894 <br>
        Gmail:mohitdholkar6@gmail.com
    </p>
  </footer>

</body>
</html>
