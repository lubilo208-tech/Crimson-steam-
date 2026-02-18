# Crimson-steam-
Fast, modern anime discovery web app built with HTML and deployed on Vercel.
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>CrimsonStream</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;800&display=swap" rel="stylesheet">
<style>
:root {
  --charcoal: #121212;
  --dark-gray: #1e1e1e;
  --crimson: #b11226;
  --light: #f5f5f5;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}

body {
  background: var(--charcoal);
  color: var(--light);
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 5%;
  background: var(--dark-gray);
  position: sticky;
  top: 0;
}

.logo {
  font-size: 1.8rem;
  font-weight: 800;
  color: var(--crimson);
}

nav a {
  color: var(--light);
  margin-left: 20px;
  text-decoration: none;
  transition: 0.3s;
}

nav a:hover {
  color: var(--crimson);
}

.hero {
  text-align: center;
  padding: 80px 20px;
}

.hero h1 {
  font-size: 3rem;
  margin-bottom: 20px;
}

.search-bar {
  max-width: 500px;
  margin: auto;
  display: flex;
  background: var(--dark-gray);
  border-radius: 50px;
  overflow: hidden;
}

.search-bar input {
  flex: 1;
  padding: 15px;
  border: none;
  background: transparent;
  color: var(--light);
}

.search-bar button {
  padding: 15px 25px;
  background: var(--crimson);
  border: none;
  color: white;
  cursor: pointer;
}

.anime-grid {
  padding: 50px 5%;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
  gap: 25px;
}

.card {
  background: var(--dark-gray);
  border-radius: 15px;
  overflow: hidden;
  transition: 0.3s;
  cursor: pointer;
}

.card:hover {
  transform: scale(1.05);
  box-shadow: 0 0 20px var(--crimson);
}

.card img {
  width: 100%;
  height: 260px;
  object-fit: cover;
}

.card h3 {
  padding: 15px;
  font-size: 1rem;
}

footer {
  text-align: center;
  padding: 30px;
  background: var(--dark-gray);
  margin-top: 50px;
}
</style>
</head>

<body>

<header>
  <div class="logo">CRIMSON STREAM</div>
  <nav>
    <a href="#">Home</a>
    <a href="#">Trending</a>
    <a href="#">New</a>
    <a href="#">My List</a>
  </nav>
</header>

<section class="hero">
  <h1>Welcome to the Crimson Realm</h1>
  <div class="search-bar">
    <input type="text" placeholder="Search anime...">
    <button>Search</button>
  </div>
</section>

<section class="anime-grid">
  <div class="card">
    <img src="https://via.placeholder.com/300x400">
    <h3>Anime Title</h3>
  </div>
  <div class="card">
    <img src="https://via.placeholder.com/300x400">
    <h3>Another Title</h3>
  </div>
</section>

<footer>
  © 2026 CrimsonStream — Discover Anime Legally
</footer>

</body>
</html>