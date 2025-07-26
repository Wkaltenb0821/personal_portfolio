# personal_portfolio
Responsive personal portfolio website styled with custom CSS, featuring dark theme, purple accents, and modern UI. 

:root {
  --bg-color: #000000;
  --text-color: #ffffff;
  --accent-color: #a259ff;
  --accent-hover: #c084fc;
  --card-bg: #1a1a1a;
  --shadow-color: rgba(162, 89, 255, 0.3);
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background-color: var(--bg-color);
  color: var(--text-color);
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

/* Navbar */
.navbar-name {
  font-size: 20px;
  padding-left: 30px;
  font-weight: bold;
  color: var(--accent-color);
  text-decoration: none;
}

.nav-link {
  font-size: 15px;
  padding: 20px;
  color: var(--text-color);
  background-color: transparent;
}

/* Icons */
.link-icons-1 {
  font-size: 40px;
  text-decoration: none;
}

.link-icons-1 i {
  padding: 15px;
  transition: color 0.3s ease;
}

.link-icons-1 i:hover {
  color: var(--accent-hover);
}

/* Resume Button */
.resumebtn {
  display: inline-block;
  margin: 40px 0 0 0;
  padding: 10px 30px;
  font-size: 18px;
  color: white;
  background: linear-gradient(45deg, #7f00ff, #e100ff);
  border: none;
  border-radius: 30px;
  text-decoration: none;
  transition: background 0.3s ease;
}

.resumebtn:hover {
  background: linear-gradient(45deg, #e100ff, #7f00ff);
}

/* About Section */
.about {
  display: flex;
  flex-wrap: wrap;
  gap: 40px;
  padding: 60px;
  justify-content: center;
  text-align: left;
}

.about img:hover {
  transform: scale(1.05);
  cursor: pointer;
  transition: transform 0.3s ease;
}

.abt2 {
  max-width: 600px;
  font-size: 1.1rem;
  line-height: 1.8rem;
}

/* Cards */
.card {
  background-color: var(--card-bg);
  border: 1px solid transparent;
  box-shadow: 0 0 10px var(--shadow-color);
  transition: all 0.3s ease;
}

.card:hover {
  border-color: var(--accent-color);
  box-shadow: 0 0 15px var(--shadow-color);
}

.card-header {
  text-align: center;
  font-weight: bold;
  color: var(--accent-color);
  background-color: var(--bg-color);
}

/* Carousel */
.carousel-item img {
  border: 2px solid transparent;
  animation: neon-border 2s linear infinite alternate;
  box-shadow: 0 0 10px var(--shadow-color);
}

@keyframes neon-border {
  0% {
    border-color: transparent;
    box-shadow: 0 0 10px var(--shadow-color);
  }
  100% {
    border-color: var(--accent-hover);
    box-shadow: 0 0 20px var(--shadow-color);
  }
}

/* Responsive */
@media (max-width: 768px) {
  .navbar-name {
    font-size: 18px;
    padding-left: 10px;
  }
  .nav-link {
    font-size: 14px;
    padding: 15px;
  }
  .about {
    padding: 30px;
  }
  .abt2 {
    font-size: 1rem;
    padding: 0;
  }
  .resumebtn {
    font-size: 16px;
    padding: 8px 20px;
  }
  .card {
    margin-bottom: 20px;
  }
}

