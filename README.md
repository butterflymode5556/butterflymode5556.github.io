<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Capital Construction Limited</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <div class="logo">Capital Construction Ltd.</div>
    <nav>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="home" class="hero">
    <h1>Building Your Dreams</h1>
    <p>We specialize in quality construction and reliable project delivery.</p>
    <a href="#contact" class="btn">Get in Touch</a>
  </section>

  <section id="services">
    <h2>Our Services</h2>
    <div class="service-box">
      <div class="service">
        <h3>Residential Construction</h3>
        <p>Expert in homes, villas, and apartments.</p>
      </div>
      <div class="service">
        <h3>Commercial Projects</h3>
        <p>Offices, malls, plazas and more.</p>
      </div>
      <div class="service">
        <h3>Renovation</h3>
        <p>Top-to-bottom home and office makeovers.</p>
      </div>
    </div>
  </section>

  <section id="about">
    <h2>About Us</h2>
    <p>
      Capital Construction Limited has been providing top-quality construction
      services for over 15 years. Our team of experienced engineers and architects
      ensures every project is built with precision and excellence.
    </p>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <form>
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email" required />
      <textarea placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>

  <footer>
    <p>© 2025 Capital Construction Limited. All rights reserved.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Segoe UI', sans-serif;
}

body {
  background: #f8f8f8;
  color: #333;
}

header {
  background-color: #003366;
  color: white;
  padding: 1em 2em;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 1.5em;
  font-weight: bold;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 1.5em;
}

nav a {
  color: white;
  text-decoration: none;
  font-weight: 500;
}

.hero {
  background: url('https://via.placeholder.com/1500x500') no-repeat center center/cover;
  padding: 5em 2em;
  text-align: center;
  color: white;
  background-color: #004080;
}

.hero h1 {
  font-size: 3em;
  margin-bottom: 0.5em;
}

.btn {
  display: inline-block;
  margin-top: 1em;
  padding: 0.75em 1.5em;
  background: #0066cc;
  color: white;
  text-decoration: none;
  border-radius: 5px;
}

section {
  padding: 3em 2em;
  max-width: 1000px;
  margin: auto;
}

#services .service-box {
  display: flex;
  gap: 2em;
  flex-wrap: wrap;
}

.service {
  background: white;
  padding: 1.5em;
  flex: 1;
  box-shadow: 0 0 10px rgba(0,0,0,0.1);
  border-radius: 8px;
}

form {
  display: flex;
  flex-direction: column;
  gap: 1em;
}

input, textarea {
  padding: 0.75em;
  border: 1px solid #ccc;
  border-radius: 5px;
}

button {
  padding: 0.75em;
  background-color: #003366;
  color: white;
  border: none;
  border-radius: 5px;
}

footer {
  background-color: #003366;
  color: white;
  text-align: center;
  padding: 1em;
}// Show alert on form submit
document.querySelector("form").addEventListener("submit", function (e) {
  e.preventDefault();
  alert("Thank you! We'll get back to you soon.");
});