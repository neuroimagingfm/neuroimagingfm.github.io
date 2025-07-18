---
layout: default
title: Foundation Models for Neuroimaging @ NeurIPS 2025
---

<style>
  .site-header {
    display: none
  };

  body {
    font-family: 'Segoe UI', sans-serif;
    background: #f9f9fc;
    color: #333;
    line-height: 1.6;
    margin: 0;
    padding: 0;
  }

  html {
    scroll-behavior: smooth;
  }

  footer {
    display: none;
  }

  .site-header {
    padding-left: 30px;
    padding-right: 30px;
  }

  .page-content {
    padding: 0px;
  }

  .wrapper {
    max-width: unset;
    margin-right: auto;
    margin-left: auto;
    padding-right: 0px;
    padding-left: 0px;
  }

  .hero {
    width: 100vw;
    height: 100vh;
    background: linear-gradient(to right, #1e3c72, #2a5298);
    background-size: cover;
    color: white;
    padding: 4rem 1rem;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    position: relative;
  }

  .hero h1 {
    font-size: 3rem;
    margin-bottom: 0.5rem;
    animation: fadeInDown 1s ease-out;
  }

  .hero p {
    font-size: 1.3rem;
    max-width: 700px;
    margin: 0.5rem auto;
    animation: fadeInUp 1.2s ease-out;
  }

  .tagline {
    font-size: 1.4em;
    font-style: italic;
    color: #e0e0e0;
  }

  .hero-nav {
    position: fixed;
    top: 0;
    right: 0;
    width: 100%;
    background: transparent;
    padding: 15px 30px;
    z-index: 1000;
    display: flex;
    justify-content: flex-end;
    align-items: center;
    transition: background 0.3s ease, box-shadow 0.3s ease;
  }

  .hero-nav.scrolled {
    background: rgba(30, 60, 114, 0.95);
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  }

  .hero-nav ul {
    list-style: none;
    display: flex;
    gap: 15px;
    margin: 0;
    padding: 0;
  }

  .hero-nav ul li {
    position: relative;
  }

  .hero-nav ul li:not(:last-child)::after {
    content: "|";
    margin-left: 15px;
    color: #ffffff99;
  }

  .hero-nav ul li a {
    color: #ffffff;
    font-weight: bold;
    text-decoration: none;
    font-size: 0.95em;
    text-transform: uppercase;
    transition: color 0.3s ease, background 0.3s ease;
    padding: 4px 8px;
    border-radius: 4px;
  }

  .hero-nav ul li a:hover {
    background: #ffffff33;
    color: #ffffff;
  }

  /* Mobile hamburger menu */
  .mobile-menu-toggle {
    display: none;
    flex-direction: column;
    cursor: pointer;
    padding: 5px;
    z-index: 1001;
  }

  .mobile-menu-toggle span {
    width: 25px;
    height: 3px;
    background: white;
    margin: 3px 0;
    transition: 0.3s;
    border-radius: 2px;
  }

  .mobile-menu-toggle.active span:nth-child(1) {
    transform: rotate(-45deg) translate(-5px, 6px);
  }

  .mobile-menu-toggle.active span:nth-child(2) {
    opacity: 0;
  }

  .mobile-menu-toggle.active span:nth-child(3) {
    transform: rotate(45deg) translate(-5px, -6px);
  }

  .section {
    max-width: 960px;
    margin: 60px auto;
    padding: 0 20px;
    background: white;
    border-radius: 12px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.05);
    padding: 2rem;
  }

  .section h2 {
    color: #2a5298;
    border-bottom: 2px solid #ddd;
    padding-bottom: 0.3em;
  }

  ul {
    padding-left: 20px;
  }

  ul li {
    margin-bottom: 10px;
  }

  a {
    color: #2a5298;
    text-decoration: none;
    font-weight: 500;
  }

  a:hover {
    text-decoration: underline;
  }

  @keyframes fadeInDown {
    0% { opacity: 0; transform: translateY(-20px); }
    100% { opacity: 1; transform: translateY(0); }
  }

  @keyframes fadeInUp {
    0% { opacity: 0; transform: translateY(20px); }
    100% { opacity: 1; transform: translateY(0); }
  }

  .organizers-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 30px;
    margin-top: 20px;
  }

  .organizer-card {
    background: white;
    border-radius: 12px;
    padding: 20px;
    text-align: center;
    box-shadow: 0 4px 12px rgba(0,0,0,0.05);
    transition: transform 0.2s ease;
  }

  .organizer-card:hover {
    transform: translateY(-5px);
  }

  .organizer-card img {
    width: 100px;
    height: 100px;
    object-fit: cover;
    border-radius: 50%;
    margin-bottom: 15px;
    border: 3px solid #2a5298;
  }

  /* Mobile responsive styles */
  @media (max-width: 768px) {
    .hero h1 {
      font-size: 2.2em;
    }

    .hero p {
      font-size: 1.1em;
    }

    .tagline {
      font-size: 1.1em;
    }

    .hero-nav {
      padding: 15px 20px;
    }

    .mobile-menu-toggle {
      display: flex;
    }

    .hero-nav ul {
      position: fixed;
      top: 0;
      right: -100%;
      height: 100vh;
      width: 280px;
      background: rgba(30, 60, 114, 0.98);
      flex-direction: column;
      justify-content: center;
      align-items: center;
      gap: 30px;
      transition: right 0.3s ease;
      backdrop-filter: blur(10px);
    }

    .hero-nav ul.active {
      right: 0;
    }

    .hero-nav ul li {
      margin: 0;
    }

    .hero-nav ul li:not(:last-child)::after {
      display: none;
    }

    .hero-nav ul li a {
      font-size: 1.2em;
      padding: 12px 20px;
      display: block;
      border-radius: 8px;
      transition: all 0.3s ease;
    }

    .hero-nav ul li a:hover {
      background: #ffffff22;
      transform: translateX(5px);
    }

    .section {
      margin: 40px 20px;
      padding: 1.5rem;
    }

    .organizers-grid {
      grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
      gap: 20px;
    }

    .organizer-card {
      padding: 15px;
    }

    .organizer-card img {
      width: 80px;
      height: 80px;
    }
  }

  @media (max-width: 480px) {
    .hero {
      padding: 3rem 1rem;
    }

    .hero h1 {
      font-size: 1.8em;
    }

    .hero p {
      font-size: 1em;
    }

    .tagline {
      font-size: 1em;
    }

    .hero-nav ul {
      width: 100%;
    }

    .section {
      margin: 30px 15px;
      padding: 1.2rem;
    }

    .organizers-grid {
      grid-template-columns: 1fr;
      gap: 15px;
    }
  }
</style>

<header class="hero">
  <nav class="hero-nav">
    <div class="mobile-menu-toggle">
      <span></span>
      <span></span>
      <span></span>
    </div>
    <ul>
      <li><a href="#about">ABOUT</a></li>
      <li><a href="#topics">TOPICS</a></li>
      <li><a href="#speakers">SPEAKERS</a></li>
      <li><a href="#program">PROGRAM</a></li>
      <li><a href="#organizers">ORGANIZERS</a></li>
    </ul>
  </nav>
  <h1>Foundation Models for Neuroimaging</h1>
  <p class="tagline">Promises, pitfalls, and the imperative need for domain knowledge from cognitive and clinical neuroscience</p>
  <p>Submitted at NeurIPS 2025</p>
</header>

<section class="section" id="about">
  <h2>About</h2>
  <p>
    Recent progress in foundation models has transformed many areas of machine learning,
    yet their application to brain data remains in its infancy. The complexity, diversity,
    and multimodal nature of neuroimaging present unique challenges and opportunities
    for building general-purpose models of the brain.
  </p>
  <p>
    This workshop brings together researchers from neuroscience, machine learning,
    and clinical disciplines to advance brain foundation models—large-scale, pre-trained models
    that learn meaningful representations of brain anatomy and function.
  </p>
</section>

<section class="section" id="topics">
  <h2>Topics</h2>
  <ul>
    <li>Foundation models for structural, functional, and diffusion imaging</li>
    <li>Large-scale and multimodal neuroimaging datasets</li>
    <li>Biomarker discovery and model interpretability</li>
    <li>Brain decoding across modalities (fMRI, EEG, MEG)</li>
    <li>Multimodal representation learning and structure-function alignment</li>
  </ul>
</section>

<section class="section" id="speakers">
  <h2>Speakers</h2>
  <ul>
    <li>Russell Poldrack (Stanford University)</li>
    <li>Gaël Varoquaux (INRIA)</li>
    <li>Christos Davatzikos (University of Pennsylvania)</li>
    <li>Anqi Qiu (Hong Kong Polytechnic University)</li>
    <li>Hubert Banville (Meta, FAIR)</li>
    <li>Paul Thompson (University of Southern California)</li>
  </ul>
</section>

<section class="section" id="program">
  <h2>Program Schedule</h2>
  <p>See the full schedule <a href="#">here</a>. The workshop will include invited talks, spotlight presentations, poster sessions, and a closing panel discussion.</p>
</section>

<section class="section">
  <h2>Call for Papers</h2>
  <p>We welcome submissions on all topics related to large-scale modeling and brain representation learning. Details and submission links coming soon.</p>
</section>

<section class="section">
  <h2>Diversity and Inclusion</h2>
  <p>
    We actively encourage participation from underrepresented groups in AI and neuroscience.
    We aim to create an inclusive and collaborative environment for all attendees.
  </p>
</section>

<section class="section" id="organizers">
  <h2>Organizers</h2>
  <div class="organizers-grid">
    <div class="organizer-card">
      <img src="assets/images/organizers/carlo.jpg" alt="Carlo Alberto Barbano">
      <h3>Carlo Alberto Barbano</h3>
      <p>University of Turin</p>
    </div>
    <div class="organizer-card">
      <img src="assets/images/organizers/benoit.jpg" alt="Benoit Dufumier">
      <h3>Benoit Dufumier</h3>
      <p>NeuroSpin, CEA</p>
    </div>
    <div class="organizer-card">
      <img src="assets/images/organizers/victoria.jpg" alt="Victoria Shevchenko">
      <h3>Victoria Shevchenko</h3>
      <p>INRIA Saclay, Université Paris Cité</p>
    </div>
    <div class="organizer-card">
      <img src="assets/images/organizers/demian.jpg" alt="Demian Wassermann">
      <h3>Demian Wassermann</h3>
      <p>INRIA Saclay</p>
    </div>
  </div>
</section>

<script>
  // Scroll effect for navigation
  window.addEventListener('scroll', function () {
    const nav = document.querySelector('.hero-nav');
    if (window.scrollY > 50) {
      nav.classList.add('scrolled');
    } else {
      nav.classList.remove('scrolled');
    }
  });

  // Mobile menu toggle
  document.addEventListener('DOMContentLoaded', function() {
    const mobileToggle = document.querySelector('.mobile-menu-toggle');
    const navMenu = document.querySelector('.hero-nav ul');
    
    mobileToggle.addEventListener('click', function() {
      mobileToggle.classList.toggle('active');
      navMenu.classList.toggle('active');
    });

    // Close mobile menu when clicking on a link
    const navLinks = document.querySelectorAll('.hero-nav ul li a');
    navLinks.forEach(link => {
      link.addEventListener('click', function() {
        mobileToggle.classList.remove('active');
        navMenu.classList.remove('active');
      });
    });

    // Close mobile menu when clicking outside
    document.addEventListener('click', function(e) {
      if (!mobileToggle.contains(e.target) && !navMenu.contains(e.target)) {
        mobileToggle.classList.remove('active');
        navMenu.classList.remove('active');
      }
    });
  });
</script>