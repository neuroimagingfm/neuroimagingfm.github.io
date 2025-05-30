---
layout: default
title: Foundation Models for Neuroimaging @ NeurIPS 2025
---

<style>
  body {
    font-family: 'Segoe UI', sans-serif;
    background: #f9f9fc;
    color: #333;
    line-height: 1.6;
    margin: 0;
    padding: 0;
  }

  footer {
    display: none;
  }

  .site-header {
    padding-left: 30px;
    padding-right: 30px;
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
    background: linear-gradient(to right, #1e3c72, #2a5298);
    color: white;
    padding: 4rem 1rem;
    text-align: center;

    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
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
  <h1>Foundation Models for Neuroimaging</h1>
  <p class="tagline">Promises, pitfalls, and the imperative need for domain knowledge from cognitive and clinical neuroscience</p>
  <p>Submitted at NeurIPS 2025</p>
</header>

<section class="section">
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

<section class="section">
  <h2>Objectives</h2>
  <ul>
    <li>Develop scalable, generalizable brain models across diverse populations</li>
    <li>Integrate multimodal neuroimaging to build unified brain representations</li>
    <li>Enable clinical applications such as biomarker discovery and diagnosis</li>
    <li>Advance cognitive neuroscience via brain decoding and representation learning</li>
  </ul>
</section>

<section class="section">
  <h2>Topics</h2>
  <ul>
    <li>Foundation models for structural, functional, and diffusion imaging</li>
    <li>Large-scale and multimodal neuroimaging datasets</li>
    <li>Biomarker discovery and model interpretability</li>
    <li>Brain decoding across modalities (fMRI, EEG, MEG)</li>
    <li>Multimodal representation learning and structure-function alignment</li>
  </ul>
</section>

<section class="section">
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

<section class="section">
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

<section class="section">
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

