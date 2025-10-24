<!DOCTYPE html>
<html lang="id">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Website Pribadi - Nanda Aditya</title>
    <link
      href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap"
      rel="stylesheet"
    />
    <style>
      body {
        font-family: "Roboto", sans-serif;
        margin: 0;
        padding: 0;
        background-color: #f8f9fa;
        color: #333;
        line-height: 1.6;
      }
      nav {
        background-color: #fff;
        box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        position: fixed;
        width: 100%;
        top: 0;
        z-index: 100;
      }
      nav ul {
        list-style: none;
        margin: 0;
        padding: 0;
        display: flex;
        justify-content: center;
      }
      nav li {
        margin: 0 20px;
      }
      nav a {
        color: #007bff;
        text-decoration: none;
        padding: 15px;
        display: block;
        transition: color 0.3s;
      }
      nav a:hover {
        color: #0056b3;
      }
      #hero {
        background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        color: white;
        text-align: center;
        padding: 150px 20px;
        animation: fadeIn 1s ease-in-out;
      }
      #hero h1 {
        font-size: 3em;
        margin: 0;
      }
      #hero p {
        font-size: 1.5em;
        margin: 10px 0;
      }
      .typing {
        border-right: 2px solid white;
        animation: blink 1s infinite;
      }
      @keyframes blink {
        0%,
        50% {
          border-color: transparent;
        }
        51%,
        100% {
          border-color: white;
        }
      }
      section {
        max-width: 1200px;
        margin: 80px auto;
        padding: 40px;
        background-color: white;
        border-radius: 10px;
        box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
        animation: fadeInUp 1.5s ease-in-out;
      }
      .profile-pic {
        width: 200px;
        height: 200px;
        border-radius: 50%;
        object-fit: cover;
        margin-bottom: 20px;
        transition: transform 0.3s;
      }
      .profile-pic:hover {
        transform: scale(1.05);
      }
      .skills {
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
      }
      .skill {
        text-align: center;
        margin: 20px;
      }
      .portfolio {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 20px;
      }
      .portfolio-item {
        background-color: #f8f9fa;
        padding: 20px;
        border-radius: 8px;
        text-align: center;
        transition: transform 0.3s;
      }
      .portfolio-item:hover {
        transform: translateY(-10px);
      }
      footer {
        background-color: #333;
        color: white;
        text-align: center;
        padding: 20px;
      }
      @keyframes fadeIn {
        from {
          opacity: 0;
        }
        to {
          opacity: 1;
        }
      }
      @keyframes fadeInUp {
        from {
          opacity: 0;
          transform: translateY(30px);
        }
        to {
          opacity: 1;
          transform: translateY(0);
        }
      }
    </style>
  </head>
  <body>
    <nav>
      <ul>
        <li><a href="#hero">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#portfolio">Portfolio</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>

    <section id="hero">
      <h1>Nanda Aditya</h1>
      <p class="typing">Web Developer & Designer</p>
    </section>

    <section id="about">
      <img
        src="Pantai.jpg.jpg"
        alt="Foto Profil Nanda Aditya"
        class="profile-pic"
      />
      <h2>About Me</h2>
      <p>
        Halo! Saya Nanda Aditya Pratama, Saya asal Makassar, Sulawesi Selatan,
        Indonesia. Hobi saya menonton, membaca, bermain game dan traveling.
      </p>
      <p>
        Deskripsi lebih lanjut: Saya kuliah di Universitas Negeri Makassar,
        Jurusan Pendidikan Teknik Elektronika, Prodi D4 Teknik Elektronika,
        Kegiatan saya sebagai mahasiwa itu belajar dan mencari hal hal baru di
        kampus yang saya tidak dapatkan di dunia sebelumnya.
      </p>
    </section>

    <section id="skills">
      <h2>Skills</h2>
      <div class="skills">
        <div class="skill">
          <h3>HTML & CSS</h3>
          <p>Expert in building responsive websites.</p>
        </div>
        <div class="skill">
          <h3>JavaScript</h3>
          <p>Proficient in ES6, React, and Node.js.</p>
        </div>
        <div class="skill">
          <h3>Python</h3>
          <p>Experienced in backend development with Flask/Django.</p>
        </div>
      </div>
    </section>

    <section id="portfolio">
      <h2>Portfolio</h2>
      <div class="portfolio">
        <div class="portfolio-item">
          <img
            src="graduiaton2.jpg"
            alt="Project 1"
            style="width: 100%; border-radius: 8px"
          />
          <h3>Photo 1: Graduation</h3>
          <p>photo together with friends from vocational school.</p>
        </div>
        <div class="portfolio-item">
          <img
            src="gradiation3.jpg"
            alt="Project 2"
            style="width: 100%; border-radius: 8px"
          />
          <h3>Photo 2: Graduation</h3>
          <p>photo together with friends from vocational school.</p>
        </div>
        <div class="portfolio-item">
          <img
            src="graduation.jpg."
            alt="Project 3"
            style="width: 100%; border-radius: 8px"
          />
          <h3>Photo 3: graduation medal presentation</h3>
          <p>receive a graduation medal</p>
        </div>
      </div>
    </section>

    <section id="contact">
      <h2>Contact</h2>
      <ul style="list-style: none; padding: 0">
        <li>
          Email:
          <a href="nandaadityapratama0711@gmail.com"
            >nandaadityapratama0711@gmail.com</a
          >
        </li>
        <li>
          LinkedIn:
          <a href="https://lynk.id/mountskuy" target="_blank"
            >https://lynk.id/mountskuy</a
          >
        </li>
        <li>
          Instagram:
          <a
            href="https://www.instagram.com/mountskuy?igsh=NGV3bWEybGVqMWdy"
            target="_blank"
            >https://www.instagram.com/mountskuy?igsh=NGV3bWEybGVqMWdy</a
          >
        </li>
      </ul>
    </section>

    <footer>
      <p>&copy; 2023 John Doe. All rights reserved.</p>
    </footer>

    <script>
      // Smooth scroll for navbar links
      document.querySelectorAll("nav a").forEach((anchor) => {
        anchor.addEventListener("click", function (e) {
          e.preventDefault();
          const target = document.querySelector(this.getAttribute("href"));
          target.scrollIntoView({ behavior: "smooth" });
        });
      });

      // Typing animation for hero subtitle
      const typingText = document.querySelector(".typing");
      const text = "Web Developer & Designer";
      let index = 0;
      function typeWriter() {
        if (index < text.length) {
          typingText.innerHTML = text.substring(0, index + 1);
          index++;
          setTimeout(typeWriter, 100);
        }
      }
      window.onload = typeWriter;
    </script>
  </body>
</html>

