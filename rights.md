<html><head><base href="https://filmrights.io/perfect%20now%20keep%20everything%20you%20already%20have%20but%20remove%20%C2%A8.io%C2%A8%20name%20it%20screnplayrights">
<title>ScreenplayRights - Revolutionary Blockchain Screenplay Platform</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="ScreenplayRights: A visionary blockchain-powered platform for screenwriters, reimagined through the artistic lenses of Virgil Abloh and Takashi Murakami. Experience the future of screenplay rights management with a fusion of streetwear aesthetics and contemporary Japanese art.">
<link href="https://fonts.googleapis.com/css2?family=Helvetica+Neue:wght@300;400;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<script src="https://unpkg.com/htmx.org@1.9.2"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.9.1/gsap.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.9.1/ScrollTrigger.min.js"></script>
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
    cursor: pointer;
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

  .content-section {
    background-color: var(--off-white);
    color: var(--primary-color);
    padding: 80px 0;
  }

  .content-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }

  .content-block {
    flex-basis: calc(33.33% - 20px);
    margin-bottom: 40px;
    padding: 20px;
    background-color: rgba(255, 255, 255, 0.1);
    border: 2px solid var(--accent-color);
    transition: all 0.3s ease;
  }

  .content-block:hover {
    transform: translateY(-10px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
  }

  .content-block h3 {
    color: var(--accent-color);
    font-size: 1.8em;
    margin-bottom: 15px;
  }

  .content-block p {
    font-size: 1.1em;
    line-height: 1.6;
  }

  .scroll-section {
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
  }

  .scroll-content {
    text-align: center;
    max-width: 800px;
    margin: 0 auto;
  }

  .scroll-indicator {
    position: absolute;
    bottom: 30px;
    left: 50%;
    transform: translateX(-50%);
    font-size: 2em;
    color: var(--accent-color);
    animation: bounce 2s infinite;
  }

  @keyframes bounce {
    0%, 20%, 50%, 80%, 100% {
      transform: translateY(0);
    }
    40% {
      transform: translateY(-30px);
    }
    60% {
      transform: translateY(-15px);
    }
  }

  .certificate-generator,
  .screenplay-register,
  .pricing-section,
  .subscription-section {
    background-color: var(--off-white);
    color: var(--primary-color);
    padding: 80px 0;
  }

  .certificate-form,
  .screenplay-form {
    max-width: 600px;
    margin: 0 auto;
    background-color: rgba(255, 255, 255, 0.1);
    padding: 40px;
    border: 2px solid var(--accent-color);
  }

  .form-group {
    margin-bottom: 20px;
  }

  .form-group label {
    display: block;
    margin-bottom: 5px;
    color: var(--primary-color);
    font-weight: bold;
  }

  .form-group input,
  .form-group textarea {
    width: 100%;
    padding: 10px;
    border: 1px solid var(--accent-color);
    background-color: rgba(255, 255, 255, 0.8);
    color: var(--primary-color);
  }

  .pricing-plans,
  .subscription-plans {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
  }

  .plan {
    flex-basis: calc(33.33% - 40px);
    background-color: rgba(255, 255, 255, 0.1);
    border: 2px solid var(--accent-color);
    padding: 40px;
    margin-bottom: 40px;
    text-align: center;
    transition: all 0.3s ease;
  }

  .plan:hover {
    transform: scale(1.05);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
  }

  .plan h3 {
    color: var(--accent-color);
    font-size: 2em;
    margin-bottom: 20px;
  }

  .plan-price {
    font-size: 3em;
    font-weight: bold;
    margin-bottom: 20px;
  }

  .plan-features {
    list-style-type: none;
    padding: 0;
    margin-bottom: 30px;
  }

  .plan-features li {
    margin-bottom: 10px;
  }

  /* New styles for expanded sections */
  .testimonials-section {
    background-color: var(--primary-color);
    color: var(--secondary-color);
    padding: 80px 0;
  }

  .testimonial {
    background-color: rgba(255, 255, 255, 0.1);
    padding: 30px;
    margin-bottom: 30px;
    border-radius: 10px;
    position: relative;
  }

  .testimonial::before {
    content: '\201C';
    font-size: 4em;
    position: absolute;
    top: -10px;
    left: 10px;
    color: var(--accent-color);
    opacity: 0.3;
  }

  .testimonial-author {
    font-style: italic;
    text-align: right;
    margin-top: 20px;
  }

  .faq-section {
    background-color: var(--off-white);
    color: var(--primary-color);
    padding: 80px 0;
  }

  .faq-item {
    margin-bottom: 30px;
  }

  .faq-question {
    font-weight: bold;
    cursor: pointer;
    padding: 15px;
    background-color: rgba(255, 255, 255, 0.1);
    border: 1px solid var(--accent-color);
    transition: all 0.3s ease;
  }

  .faq-question:hover {
    background-color: var(--accent-color);
    color: var(--secondary-color);
  }

  .faq-answer {
    padding: 15px;
    background-color: rgba(255, 255, 255, 0.05);
    border: 1px solid var(--accent-color);
    border-top: none;
    display: none;
  }

  .blog-section {
    background-color: var(--primary-color);
    color: var(--secondary-color);
    padding: 80px 0;
  }

  .blog-post {
    background-color: rgba(255, 255, 255, 0.1);
    padding: 30px;
    margin-bottom: 30px;
    border-radius: 10px;
  }

  .blog-post h3 {
    color: var(--accent-color);
  }

  .blog-post-meta {
    font-style: italic;
    margin-bottom: 15px;
  }

  .community-section {
    background-color: var(--off-white);
    color: var(--primary-color);
    padding: 80px 0;
  }

  .community-feature {
    text-align: center;
    margin-bottom: 40px;
  }

  .community-feature i {
    font-size: 3em;
    color: var(--accent-color);
    margin-bottom: 20px;
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

    .content-block,
    .plan {
      flex-basis: 100%;
    }

    .testimonial,
    .blog-post {
      padding: 20px;
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
    gsap.registerPlugin(ScrollTrigger);

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

    gsap.utils.toArray('.scroll-section').forEach((section, index) => {
      gsap.from(section, {
        opacity: 0,
        y: 50,
        duration: 1,
        ease: 'power3.out',
        scrollTrigger: {
          trigger: section,
          start: 'top 80%',
          end: 'bottom 20%',
          toggleActions: 'play none none reverse'
        }
      });
    });

    // Smooth scrolling for navigation
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href')).scrollIntoView({
          behavior: 'smooth'
        });
      });
    });

    // Responsive design
    window.addEventListener('resize', () => {
      camera.aspect = window.innerWidth / window.innerHeight;
      camera.updateProjectionMatrix();
      renderer.setSize(window.innerWidth, window.innerHeight);
    });

    // Certificate Generator
    const certificateForm = document.getElementById('certificate-form');
    if (certificateForm) {
      certificateForm.addEventListener('submit', (e) => {
        e.preventDefault();
        alert('Certificate generated successfully!');
        // Here you would typically send the form data to a server to generate the certificate
      });
    }

    // Screenplay Registration
    const screenplayForm = document.getElementById('screenplay-form');
    if (screenplayForm) {
      screenplayForm.addEventListener('submit', (e) => {
        e.preventDefault();
        alert('Screenplay registered successfully!');
        // Here you would typically send the form data to a server to register the screenplay
      });
    }

    // FAQ Accordion
    const faqQuestions = document.querySelectorAll('.faq-question');
    faqQuestions.forEach(question => {
      question.addEventListener('click', () => {
        const answer = question.nextElementSibling;
        answer.style.display = answer.style.display === 'block' ? 'none' : 'block';
      });
    });

    // Blog Post Preview
    const blogPosts = document.querySelectorAll('.blog-post');
    blogPosts.forEach(post => {
      const content = post.querySelector('p');
      const fullContent = content.textContent;
      const preview = fullContent.slice(0, 150) + '...';
      content.textContent = preview;

      const readMoreBtn = document.createElement('button');
      readMoreBtn.textContent = 'Read More';
      readMoreBtn.classList.add('cta-button');
      readMoreBtn.style.marginTop = '15px';

      readMoreBtn.addEventListener('click', () => {
        if (content.textContent === preview) {
          content.textContent = fullContent;
          readMoreBtn.textContent = 'Show Less';
        } else {
          content.textContent = preview;
          readMoreBtn.textContent = 'Read More';
        }
      });

      post.appendChild(readMoreBtn);
    });
  });
</script>
</head>
<body hx-boost="true">
  <div id="three-container"></div>
  
  <header>
    <nav class="container">
      <a href="#" class="logo">ScreenplayRights</a>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#features">Features</a></li>
        <li><a href="#how-it-works">How It Works</a></li>
        <li><a href="#generate-certificate">Generate Certificate</a></li>
        <li><a href="#register-screenplay">Register Screenplay</a></li>
        <li><a href="#pricing">Pricing</a></li>
        <li><a href="#subscriptions">Subscriptions</a></li>
        <li><a href="#testimonials">Testimonials</a></li>
        <li><a href="#faq">FAQ</a></li>
        <li><a href="#blog">Blog</a></li>
        <li><a href="#community">Community</a></li>
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
    <section id="home" class="scroll-section">
      <div class="scroll-content">
        <h1 class="hero-text">Secure Your Vision</h1>
        <p>Welcome to the future of screenplay rights management. Inspired by the innovative spirit of Virgil Abloh and the vibrant artistry of Takashi Murakami.</p>
        <a href="#register" class="cta-button">Register Your Screenplay</a>
      </div>
      <div class="scroll-indicator">
        <i class="fas fa-chevron-down"></i>
      </div>
    </section>

    <section id="features" class="scroll-section">
      <div class="scroll-content">
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
      <div class="scroll-indicator">
        <i class="fas fa-chevron-down"></i>
      </div>
    </section>

    <section id="how-it-works" class="scroll-section">
      <div class="scroll-content">
        <h2>How It Works</h2>
        <div class="feature">
          <h3>1. Upload Your Screenplay</h3>
          <p>Securely upload your screenplay to our platform, where it's immediately protected by blockchain technology.</p>
        </div>
        <div class="feature">
          <h3>2. Set Your Terms</h3>
          <p>Define your rights, royalties, and conditions using our intuitive smart contract system.</p>
        </div>
        <div class="feature">
          <h3>3. Connect with the Industry</h3>
          <p>Your work becomes visible to our network of verified producers, studios, and industry professionals.</p>
        </div>
        <div class="feature">
          <h3>4. Secure Deals</h3>
          <p>When interested parties want to option or purchase your screenplay, our platform facilitates secure, transparent transactions.</p>
        </div>
      </div>
      <div class="scroll-indicator">
        <i class="fas fa-chevron-down"></i>
      </div>
    </section>

    <section id="generate-certificate" class="scroll-section certificate-generator">
      <div class="scroll-content">
        <h2>Generate Certificate</h2>
        <form id="certificate-form" class="certificate-form">
          <div class="form-group">
            <label for="screenplay-title">Screenplay Title</label>
            <input type="text" id="screenplay-title" name="screenplay-title" required>
          </div>
          <div class="form-group">
            <label for="author-name">Author Name</label>
            <input type="text" id="author-name" name="author-name" required>
          </div>
          <div class="form-group">
            <label for="completion-date">Completion Date</label>
            <input type="date" id="completion-date" name="completion-date" required>
          </div>
          <button type="submit" class="cta-button">Generate Certificate</button>
        </form>
      </div>
      <div class="scroll-indicator">
        <i class="fas fa-chevron-down"></i>
      </div>
    </section>

    <section id="register-screenplay" class="scroll-section screenplay-register">
      <div class="scroll-content">
        <h2>Register Screenplay or Draft</h2>
        <form id="screenplay-form" class="screenplay-form">
          <div class="form-group">
            <label for="screenplay-title">Screenplay Title</label>
            <input type="text" id="screenplay-title" name="screenplay-title" required>
          </div>
          <div class="form-group">
            <label for="author-name">Author Name</label>
            <input type="text" id="author-name" name="author-name" required>
          </div>
          <div class="form-group">
            <label for="screenplay-synopsis">Synopsis (max 500 characters)</label>
            <textarea id="screenplay-synopsis" name="screenplay-synopsis" maxlength="500" required></textarea>
          </div>
          <div class="form-group">
            <label for="screenplay-file">Upload Screenplay (PDF only)</label>
            <input type="file" id="screenplay-file" name="screenplay-file" accept=".pdf" required>
          </div>
          <button type="submit" class="cta-button">Register Screenplay</button>
        </form>
      </div>
      <div class="scroll-indicator">
        <i class="fas fa-chevron-down"></i>
      </div>
    </section>

    <section id="pricing" class="scroll-section pricing-section">
      <div class="scroll-content">
        <h2>Pricing</h2>
        <div class="pricing-plans">
          <div class="plan">
            <h3>Basic</h3>
            <div class="plan-price">$9.99/mo</div>
            <ul class="plan-features">
              <li>Register up to 3 screenplays</li>
              <li>Basic blockchain protection</li>
              <li>Access to global marketplace</li>
            </ul>
            <button class="cta-button">Choose Plan</button>
          </div>
          <div class="plan">
            <h3>Pro</h3>
            <div class="plan-price">$24.99/mo</div>
            <ul class="plan-features">
              <li>Register unlimited screenplays</li>
              <li>Advanced blockchain protection</li>
              <li>Priority listing in marketplace</li>
              <li>Smart contract templates</li>
            </ul>
            <button class="cta-button">Choose Plan</button>
          </div>
          <div class="plan">
            <h3>Enterprise</h3>
            <div class="plan-price">$99.99/mo</div>
            <ul class="plan-features">
              <li>All Pro features</li>
              <li>Dedicated account manager</li>
              <li>Custom smart contract creation</li>
              <li>API access for integration</li>
            </ul>
            <button class="cta-button">Choose Plan</button>
          </div>
        </div>
      </div>
      <div class="scroll-indicator">
        <i class="fas fa-chevron-down"></i>
      </div>
    </section>

    <section id="subscriptions" class="scroll-section subscription-section">
      <div class="scroll-content">
        <h2>Subscriptions</h2>
        <div class="subscription-plans">
          <div class="plan">
            <h3>Monthly</h3>
            <div class="plan-price">$29.99/mo</div>
            <ul class="plan-features">
              <li>Full access to all features</li>
              <li>Cancel anytime</li>
              <li>Monthly blockchain security updates</li>
            </ul>
            <button class="cta-button">Subscribe Now</button>
          </div>
          <div class="plan">
            <h3>Annual</h3>
            <div class="plan-price">$299.99/year</div>
            <ul class="plan-features">
              <li>Full access to all features</li>
              <li>Two months free</li>
              <li>Priority support</li>
              <li>Exclusive industry events access</li>
            </ul>
            <button class="cta-button">Subscribe Now</button>
          </div>
        </div>
      </div>
      <div class="scroll-indicator">
        <i class="fas fa-chevron-down"></i>
      </div>
    </section>

    <section id="testimonials" class="scroll-section testimonials-section">
      <div class="scroll-content">
        <h2>What Our Users Say</h2>
        <div class="testimonial">
          <p>"ScreenplayRights has revolutionized how I manage my scripts. The blockchain security gives me peace of mind, and I've made incredible industry connections through their marketplace."</p>
          <p class="testimonial-author">- Sarah J., Screenwriter</p>
        </div>
        <div class="testimonial">
          <p>"As a producer, this platform has streamlined our acquisition process. The smart contracts make rights management a breeze, and we've discovered some amazing talent here."</p>
          <p class="testimonial-author">- Michael R., Production Company CEO</p>
        </div>
        <div class="testimonial">
          <p>"The certificate generation feature is a game-changer. It's so easy to prove my ownership, and the blockchain verification adds a level of legitimacy that's unmatched in the industry."</p>
          <p class="testimonial-author">- David L., Indie Filmmaker</p>
        </div>
      </div>
      <div class="scroll-indicator">
        <i class="fas fa-chevron-down"></i>
      </div>
    </section>

    <section id="faq" class="scroll-section faq-section">
      <div class="scroll-content">
        <h2>Frequently Asked Questions</h2>
        <div class="faq-item">
          <div class="faq-question">How does blockchain protect my screenplay?</div>
          <div class="faq-answer">Blockchain creates an immutable, time-stamped record of your screenplay registration. This serves as proof of your authorship and can be used to verify the originality of your work.</div>
        </div>
        <div class="faq-item">
          <div class="faq-question">Can I update my screenplay after registration?</div>
          <div class="faq-answer">Yes, you can upload new versions of your screenplay. Each version will be separately registered on the blockchain, creating a clear revision history.</div>
        </div>
        <div class="faq-item">
          <div class="faq-question">How do smart contracts work for screenplay rights?</div>
          <div class="faq-answer">Smart contracts automatically execute predefined terms when certain conditions are met. For screenplay rights, this could include automatic royalty payments when your screenplay is used, or transfer of rights upon payment.</div>
        </div>
        <div class="faq-item">
          <div class="faq-question">Is my screenplay visible to everyone on the platform?</div>
          <div class="faq-answer">No, you control the visibility of your work. You can choose to make it visible to all verified industry professionals, or limit access to specific individuals or companies.</div>
        </div>
      </div>
      <div class="scroll-indicator">
        <i class="fas fa-chevron-down"></i>
      </div>
    </section>

    <section id="blog" class="scroll-section blog-section">
      <div class="scroll-content">
        <h2>Latest from Our Blog</h2>
        <div class="blog-post">
          <h3>The Future of Screenplay Rights in the Blockchain Era</h3>
          <p class="blog-post-meta">Posted on May 15, 2023 by John Doe</p>
          <p>As we venture deeper into the digital age, the landscape of intellectual property rights is undergoing a radical transformation. Blockchain technology, with its promise of transparency and immutability, is at the forefront of this revolution. In the world of screenwriting, this means unprecedented levels of security and new opportunities for creators to protect and monetize their work.</p>
        </div>
        <div class="blog-post">
          <h3>5 Tips for Navigating the Digital Screenplay Marketplace</h3>
          <p class="blog-post-meta">Posted on May 10, 2023 by Jane Smith</p>
          <p>The digital marketplace for screenplays is a dynamic and competitive space. To stand out, writers need to do more than just create compelling stories. In this post, we'll explore five essential strategies for success in the online screenplay market, from optimizing your script's metadata to leveraging social proof and building your personal brand.</p>
        </div>
        <div class="blog-post">
          <h3>Smart Contracts: A Screenwriter's New Best Friend</h3>
          <p class="blog-post-meta">Posted on May 5, 2023 by Alex Johnson</p>
          <p>Smart contracts are revolutionizing how screenwriters manage their rights and royalties. These self-executing contracts with the terms of the agreement directly written into code are streamlining transactions and ensuring fair compensation. In this article, we'll dive into how smart contracts work, their benefits for screenwriters, and how to start implementing them in your career.</p>
        </div>
      </div>
      <div class="scroll-indicator">
        <i class="fas fa-chevron-down"></i>
      </div>
    </section>

    <section id="community" class="scroll-section community-section">
      <div class="scroll-content">
        <h2>Join Our Community</h2>
        <div class="community-feature">
          <i class="fas fa-users"></i>
          <h3>Writers' Forum</h3>
          <p>Connect with fellow screenwriters, share experiences, and get valuable feedback on your work.</p>
        </div>
        <div class="community-feature">
          <i class="fas fa-calendar-alt"></i>
          <h3>Virtual Events</h3>
          <p>Participate in online workshops, webinars, and Q&A sessions with industry professionals.</p>
        </div>
        <div class="community-feature">
          <i class="fas fa-handshake"></i>
          <h3>Collaboration Opportunities</h3>
          <p>Find writing partners, connect with producers, and explore co-creation possibilities.</p>
        </div>
        <div class="community-feature">
          <i class="fas fa-graduation-cap"></i>
          <h3>Learning Resources</h3>
          <p>Access our library of tutorials, guides, and courses on screenwriting and the business of film.</p>
        </div>
      </div>
      <div class="scroll-indicator">
        <i class="fas fa-chevron-down"></i>
      </div>
    </section>

    <section id="contact" class="scroll-section">
      <div class="scroll-content">
        <h2>Contact Us</h2>
        <form id="contact-form" class="contact-form">
          <div class="form-group">
            <label for="name">Name</label>
            <input type="text" id="name" name="name" required>
          </div>
          <div class="form-group">
            <label for="email">Email</label>
            <input type="email" id="email" name="email" required>
          </div>
          <div class="form-group">
            <label for="message">Message</label>
            <textarea id="message" name="message" required></textarea>
          </div>
          <button type="submit" class="cta-button">Send Message</button>
        </form>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">
      <div class="footer-content">
        <div class="footer-section">
          <h3>ScreenplayRights</h3>
          <p>Empowering screenwriters with blockchain technology and innovative rights management solutions.</p>
        </div>
        <div class="footer-section">
          <h3>Quick Links</h3>
          <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#features">Features</a></li>
            <li><a href="#pricing">Pricing</a></li>
            <li><a href="#blog">Blog</a></li>
          </ul>
        </div>
        <div class="footer-section">
          <h3>Connect With Us</h3>
          <div class="social-icons">
            <a href="https://twitter.com/screenplayrights" target="_blank"><i class="fab fa-twitter"></i></a>
            <a href="https://facebook.com/screenplayrights" target="_blank"><i class="fab fa-facebook"></i></a>
            <a href="https://instagram.com/screenplayrights" target="_blank"><i class="fab fa-instagram"></i></a>
            <a href="https://linkedin.com/company/screenplayrights" target="_blank"><i class="fab fa-linkedin"></i></a>
          </div>
        </div>
      </div>
      <div class="footer-bottom">
        <p>&copy; 2023 ScreenplayRights. All rights reserved.</p>
      </div>
    </div>
  </footer>

</body>
</html>
