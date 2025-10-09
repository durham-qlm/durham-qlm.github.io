---
layout: page
title: QLM member
subtitle:
---

![Dr Alex Guttridge](/members/current/guttridge/Alex_headshot_s.jpg)

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">

<style>
  .staff-card {
    border: 1px solid #ddd;
    border-radius: 8px;
    padding: 20px;
    margin-bottom: 20px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
  }
  .staff-card h3 {
    margin-top: 0;
  }
  .staff-card p {
    margin-bottom: 10px;
  }
  .staff-links a {
    margin-right: 15px;
    font-size: 1.5em; /* Make icons bigger */
    color: #333;
  }
</style>

<div class="staff-card">
  <h3>Dr Alex Guttridge</h3>
  <p><strong>Royal Society University Research Fellow</strong></p>
  <div class="staff-links">
    <a href="mailto:alexander.guttridge@durham.ac.uk" title="Email"><i class="fas fa-envelope"></i></a>
    <a href="https://www.durham.ac.uk/staff/alexander-guttridge/" title="Staff Page"><i class="fas fa-university"></i></a>
    <a href="https://orcid.org/0000-0001-9886-5739" title="ORCID Profile"><i class="fab fa-orcid"></i></a>
  </div>
</div>

---

## About Me

I am a Royal Society University Research Fellow in the Quantum Light and Matter (QLM) group at Durham University. My research explores how we can assemble and control quantum systems atom by atom.
By controlling individual particles at the quantum level, we can realise next-generation quantum devices — from quantum computers to ultra-sensitive sensors — and explore novel regimes of quantum physics.

In 2025, I established my own research group with the support of an 8-year Royal Society University Research Fellowship. In my group, we are building a new platform that uses arrays of optical tweezers — tightly focused laser beams capable of trapping individual atoms — to trap and control two different atomic species: caesium and ytterbium.
This dual-species approach gives us a versatile new toolbox for investigating the frontiers of quantum science.

Beyond my group’s core research, I contribute to a range of national and international collaborations using individually controlled atoms and molecules for quantum science. I lead an [international collaboration with the University of Waterloo](https://www.durham.ac.uk/news-events/latest-news/2025/01/grant-award-enables-durham-physicists-to-lead-international-quantum-projects-/) focused on quantum sensing, and I am a co-investigator on the EPSRC Programme grant *Quantum many-body physics with ultracold polar molecules* and the project *Enhancing molecular control using Rydberg atoms*.

Outside of research, I co-organise [Quantum on the Clock](https://www.iop.org/physics-community/special-interest-groups/qqq-group/quantum-clock), a UK-wide video competition designed to inspire 16-18 year olds to pursue physics degrees and consider careers in quantum science. Outside of work, I enjoy playing a variety of sports like football, table tennis, and volleyball—though with varying levels of competitiveness!

---

## Research Vision

In my group, we aim to exploit advanced quantum engineering techniques to explore new frontiers in fundamental science and quantum technology. Our approach combines two distinct atomic species in dual-species optical tweezer arrays.
By assigning specialised roles to each species—such as data qubits, ancillas, or sensors—we can realise simplified yet scalable architectures for quantum computing, sensing, and simulation.This strategy allows us to achieve precise control of delicate quantum states while maintaining the flexibility needed to tackle the next generation of challenges in quantum science.

---

## Current Projects

- **[DualQD: Dual-species tweezer arrays for next-generation quantum devices](/projects/current/dualqd.html)**  
  Developing a two-species optical tweezer platform to build programmable quantum systems atom by atom.  
  
- *Enhancing molecular control using Rydberg atoms*  
  EPSRC-funded collaboration to integrate Rydberg physics with ultracold molecule control.  

---

## Opportunities

We are always looking for motivated students and researchers interested in experimental quantum science.  
Interested students see [here](/join/phdrecruit.md) for our current opportunities.
We also welcome approaches from postdoctoral researchers interested in applying for independent research fellowships to be hosted in Durham. For example the [Royal Society Newton International Fellowship](https://royalsociety.org/grants/newton-international/) and the [Marie Skłodowska-Curie Postoctoral Fellowships](https://marie-sklodowska-curie-actions.ec.europa.eu/actions/postdoctoral-fellowships).
Interested applicants should contact [Alex Guttridge](mailto:alexander.guttridge@durham.ac.uk).

---

## Selected Publications

{% assign featured = site.data.guttridge_publist | where: "highlight", 1 %}
{% assign paper_counter = featured.size %}

{% for publi in featured %}
**[{{ paper_counter }}] {{ publi.title }}**  
*{{ publi.authors }}*  
<a href="{{ publi.link.url }}">{{ publi.link.display }}</a>  
{{ publi.description }}  
<br><br>
{% assign paper_counter = paper_counter | minus: 1 %}
{% endfor %}

Full publication list on [Google Scholar](https://scholar.google.com/citations?user=eoAbbbIAAAAJ&hl=en)

---

