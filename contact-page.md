---
layout: null
title: "Contact Me"
permalink: /contact-page
---

<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Contact Me</title>
<link rel="stylesheet" href="custom.css" />

<!-- Load Space Mono from Google Fonts -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Space+Mono:ital,wght@0,400;0,700;1,400;1,700&display=swap" rel="stylesheet">

<style>
/* Fonts */
.space-mono-regular {
  font-family: "Space Mono", monospace;
  font-weight: 400;
  font-style: normal;
}

.space-mono-bold {
  font-family: "Space Mono", monospace;
  font-weight: 700;
  font-style: normal;
}

.space-mono-regular-italic {
  font-family: "Space Mono", monospace;
  font-weight: 400;
  font-style: italic;
}

.space-mono-bold-italic {
  font-family: "Space Mono", monospace;
  font-weight: 700;
  font-style: italic;
}

/* Base */
body {
  margin: 0;
  padding: 0;
  background-color: #F9F4EE;
  font-family: "Space Mono", monospace;
  overflow-x: hidden; 
}

/* Contact page */
.contact-container {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 2rem;
  text-align: center;
}

.contact-title {
  font-size: 2.5rem;
  color: #1E1E1E;
  margin-bottom: 1.5rem;
  font-weight: 700; 
}

.contact-description {
  font-size: 1.1rem;
  max-width: 500px;
  margin-bottom: 2rem;
  color: #555;
}


.contact-links {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.contact-links a {
  display: inline-block;
  margin: 0.5rem 0.5rem;
  text-decoration: none;
  color: #1E1E1E;
  border: 1px solid #1E1E1E;
  padding: 0.5rem 1.2rem;
  border-radius: 25px;
  transition: all 0.3s ease;
  min-width: 120px;
  text-align: center;
}

.contact-links a:hover {
  background-color: #C7BEAF;
  color: #F9F4EE;
}

/* Contact form */
.form-wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  padding: 2rem;
  box-sizing: border-box;
}

form {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  width: 100%;
  max-width: 500px;
  background-color: #fff;
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.05);
}

input, textarea {
  padding: 0.8rem;
  border: 1px solid #ccc;
  border-radius: 8px;
  font-size: 1rem;
  font-family: inherit;
  background-color: #fff;
}

button {
  padding: 0.8rem 1.5rem;
  background-color: #C7BEAF;
  color: #F9F4EE;
  font-size: 1rem;
  border: none;
  border-radius: 25px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: #333;
}


@media (max-width: 600px) {
  .contact-title {
    font-size: 2rem;
  }

  .contact-description {
    font-size: 1rem;
    padding: 0 1rem;
  }

  form {
    padding: 1.5rem;
  }
}
</style>

{% include header.html %}

<div class="contact-container">
  <h1 class="contact-title">Let's Get in Touch</h1>
  <p class="contact-description">
    Feel free to reach out for collaborations, questions, or just to say hi! <br>
    (Psss, this is my email <b>hosanasacha@gmail.com</b>)
  </p>

  <div class="contact-links">
    <a href="mailto:hosanasacha@gmail.com">Email Me</a>
    <a href="https://www.linkedin.com/in/sacha-hosana/" target="_blank">LinkedIn</a>
    <a href="https://github.com/Hosana-sacha" target="_blank">GitHub</a>
    <a href="https://www.instagram.com/sacha_hosana/" target="_blank">Instagram</a>
  </div>

  <div class="form-wrapper">
    <form action="https://formspree.io/f/mpwpgyjw" method="POST">
      <input type="text" name="name" placeholder="Your Name" required><br>
      <input type="email" name="email" placeholder="Your Email" required><br>
      <textarea name="message" placeholder="Your Message" rows="5" required></textarea><br>
      <button type="submit">Send Message</button>
    </form>
  </div>
</div>
