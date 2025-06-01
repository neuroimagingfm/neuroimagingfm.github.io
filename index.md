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

  @media (max-width: 600px) {
    .hero h1 {
      font-size: 2em;
    }

    .hero p {
      font-size: 1em;
    }

    .tagline {
      font-size: 1em;
    }

    .hero-nav ul {
      flex-direction: column;
      gap: 10px;
    }
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
</style>

<header class="hero">
  <nav class="hero-nav">
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
    <li>Jean-Rémi King / Charlotte Caucheteux / Hubert Banville (Meta)</li>
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
  window.addEventListener('scroll', function () {
    const nav = document.querySelector('.hero-nav');
    if (window.scrollY > 50) {
      nav.classList.add('scrolled');
    } else {
      nav.classList.remove('scrolled');
    }
  });
</script>
