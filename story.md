<html><head><base href="https://filmrights.io/%20perfect%20now%20redesign%20it%20by%20virgil%20abloh%20and%20murakami">
<title>ScreenplayRights.io - Avant-Garde Blockchain Screenplay Platform</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="ScreenplayRights.io: A visionary blockchain-powered platform for screenwriters, reimagined through the artistic lenses of Virgil Abloh and Takashi Murakami. Experience the future of screenplay rights management with a fusion of streetwear aesthetics and contemporary Japanese art.">
<link href="https://fonts.googleapis.com/css2?family=Helvetica+Neue:wght@300;400;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<script src="https://unpkg.com/htmx.org@1.9.2"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.9.1/gsap.min.js"></script>
<style>
  :root {
    --primary-color: #000000;
    --secondary-color: #ffffff;
    --accent-color: #ff3366;
    --murakami-yellow: #ffff00;
    --murakami-blue: #00a0e9;
    --text-color: #ffffff;
    --off-white: #f5f5f5;
  }

  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body {
    font-family: 'Helvetica Neue', sans-serif;
    background-color: var(--primary-color);
    color: var(--text-color);
    line-height: 1.6;
    overflow-x: hidden;
  }

  .container {
    max-width: 1400px;
    margin: 0 auto;
    padding: 0 20px;
  }

  header {
    background-color: rgba(0, 0, 0, 0.8);
    padding: 20px 0;
    position: fixed;
    width: 100%;
    z-index: 1000;
    backdrop-filter: blur(10px);
  }

  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .logo {
    font-size: 2em;
    font-weight: bold;
    color: var(--secondary-color);
    text-decoration: none;
    text-transform: uppercase;
    letter-spacing: 2px;
  }

  nav ul {
    display: flex;
    list-style-type: none;
  }

  nav ul li {
    margin-left: 30px;
  }

  nav ul li a {
    color: var(--secondary-color);
    text-decoration: none;
    font-weight: bold;
    text-transform: uppercase;
    letter-spacing: 1px;
    position: relative;
    transition: color 0.3s ease;
  }

  nav ul li a::after {
    content: '';
    position: absolute;
    width: 100%;
    height: 2px;
    bottom: -5px;
    left: 0;
    background-color: var(--accent-color);
    transform: scaleX(0);
    transition: transform 0.3s ease;
  }

  nav ul li a:hover::after {
    transform: scaleX(1);
  }

  .section {
    padding: 120px 0;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
    overflow: hidden;
  }

  h1, h2, h3, h4, h5, h6 {
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 3px;
    margin-bottom: 20px;
  }

  .hero-text {
    font-size: 4.5em;
    font-weight: bold;
    text-transform: uppercase;
    letter-spacing: 5px;
    background: linear-gradient(45deg, var(--accent-color), var(--murakami-yellow), var(--murakami-blue));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    position: relative;
    display: inline-block;
  }

  .cta-button {
    display: inline-block;
    background-color: var(--accent-color);
    color: var(--secondary-color);
    padding: 15px 30px;
    text-decoration: none;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-weight: 700;
    border: 2px solid var(--accent-color);
    transition: all 0.3s ease;
    position: relative;
    overflow: hidden;
  }

  .cta-button::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(120deg, transparent, rgba(255, 255, 255, 0.3), transparent);
    transition: all 0.5s ease;
  }

  .cta-button:hover::before {
    left: 100%;
  }

  .cta-button:hover {
    background-color: transparent;
    color: var(--accent-color);
  }

  .feature {
    background-color: var(--off-white);
    padding: 30px;
    margin-bottom: 30px;
    border-radius: 0;
    position: relative;
    overflow: hidden;
    transition: all 0.3s ease;
  }

  .feature::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: conic-gradient(from 0deg at 50% 50%, var(--murakami-yellow) 0deg, var(--murakami-blue) 90deg, var(--accent-color) 180deg, var(--murakami-yellow) 270deg);
    opacity: 0.1;
    animation: rotate 20s linear infinite;
  }

  @keyframes rotate {
    0% {
      transform: rotate(0deg);
    }
    100% {
      transform: rotate(360deg);
    }
  }

  .feature h3 {
    color: var(--primary-color);
    font-size: 1.5em;
    position: relative;
    z-index: 1;
  }

  .feature p {
    color: var(--primary-color);
    position: relative;
    z-index: 1;
  }

  #three-container {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
  }

  @media (max-width: 768px) {
    .hero-text {
      font-size: 2.5em;
    }

    nav ul {
      display: none;
    }

    .hamburger {
      display: block;
      cursor: pointer;
    }

    .hamburger .line {
      width: 30px;
      height: 3px;
      background-color: var(--secondary-color);
      margin: 6px 0;
    }
  }
</style>
<script>
  document.addEventListener('DOMContentLoaded', () => {
    // Three.js background
    const scene = new THREE.Scene();
    const camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
    const renderer = new THREE.WebGLRenderer({ alpha: true });
    renderer.setSize(window.innerWidth, window.innerHeight);
    document.getElementById('three-container').appendChild(renderer.domElement);

    const geometry = new THREE.TorusKnotGeometry(10, 3, 100, 16);
    const material = new THREE.MeshBasicMaterial({ 
      color: 0xff3366,
      wireframe: true
    });
    const torusKnot = new THREE.Mesh(geometry, material);
    scene.add(torusKnot);

    camera.position.z = 30;

    function animate() {
      requestAnimationFrame(animate);
      torusKnot.rotation.x += 0.01;
      torusKnot.rotation.y += 0.01;
      renderer.render(scene, camera);
    }
    animate();

    // GSAP animations
    gsap.from('.hero-text', {
      duration: 1.5,
      opacity: 0,
      y: 50,
      ease: 'power3.out'
    });

    gsap.from('.cta-button', {
      duration: 1,
      opacity: 0,
      y: 30,
      ease: 'power3.out',
      delay: 0.5
    });

    gsap.from('.feature', {
      duration: 1,
      opacity: 0,
      y: 50,
      stagger: 0.2,
      ease: 'power3.out',
      scrollTrigger: {
        trigger: '.features',
        start: 'top 80%'
      }
    });

    // Responsive design
    window.addEventListener('resize', () => {
      camera.aspect = window.innerWidth / window.innerHeight;
      camera.updateProjectionMatrix();
      renderer.setSize(window.innerWidth, window.innerHeight);
    });
  });
</script>
</head>
<body hx-boost="true">
  <div id="three-container"></div>
  
  <header>
    <nav class="container">
      <a href="#" class="logo">ScreenplayRights.io</a>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#features">Features</a></li>
        <li><a href="#how-it-works">How It Works</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
      <div class="hamburger">
        <div class="line"></div>
        <div class="line"></div>
        <div class="line"></div>
      </div>
    </nav>
  </header>

  <main>
    <section id="home" class="section">
      <div class="container">
        <h1 class="hero-text">Secure Your Vision</h1>
        <p>Welcome to the future of screenplay rights management. Inspired by the innovative spirit of Virgil Abloh and the vibrant artistry of Takashi Murakami.</p>
        <a href="#register" class="cta-button">Register Your Screenplay</a>
      </div>
    </section>

    <section id="features" class="section">
      <div class="container">
        <h2>Features</h2>
        <div class="features">
          <div class="feature">
            <h3>Blockchain Security</h3>
            <p>Protect your intellectual property with cutting-edge blockchain technology.</p>
          </div>
          <div class="feature">
            <h3>Global Marketplace</h3>
            <p>Showcase your work to a worldwide network of producers and studios.</p>
          </div>
          <div class="feature">
            <h3>Smart Contracts</h3>
            <p>Automate royalties and rights management with intelligent contract systems.</p>
          </div>
        </div>
      </div>
    </section>

    <section id="how-it-works" class="section">
      <div class="container">
        <h2>How It Works</h2>
        <!-- Add content for How It Works section -->
      </div>
    </section>

    <section id="contact" class="section">
      <div class="container">
        <h2>Contact Us</h2>
        <!-- Add contact form or contact information -->
      </div>
    </section>
  </main>

  <footer>
    <div class="container">
      <p>&copy; 2023 ScreenplayRights.io. All rights reserved.</p>
    </div>
  </footer>
</body>
</html>
