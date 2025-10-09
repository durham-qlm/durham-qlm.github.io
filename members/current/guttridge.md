---
layout: page
title: QLM member
subtitle:
---

<div style="text-align: center;">

  <h3>Dr. Alex Guttridge (he/him)</h3>

  <img src="/members/current/guttridge/Alex_headshot_s.jpg" alt="Dr Alex Guttridge" width="250" />

  <p>
    <a href="mailto:alexander.guttridge@durham.ac.uk">Email</a> | 
    <a href="https://www.durham.ac.uk/staff/alexander-guttridge/">Staff Page</a> | 
    <a href="https://scholar.google.com/citations?user=eoAbbbIAAAAJ&hl=en">Google Scholar</a> | 
    <a href="https://orcid.org/0000-0001-9886-5739">ORCID</a>
  </p>

</div>



---

## About Me

I am a Royal Society University Research Fellow in the Quantum Light and Matter (QLM) group at Durham University. My research explores how we can assemble and control quantum systems atom by atom.
By controlling individual particles at the quantum level, we can realise next-generation quantum devices — from quantum computers to ultra-sensitive sensors — and explore novel regimes of quantum physics.

In 2025, I established my own research group with the support of an 8-year Royal Society University Research Fellowship. In my group, we are building a new platform that uses arrays of optical tweezers — tightly focused laser beams capable of trapping individual atoms — to trap and control two different atomic species: caesium and ytterbium.
<!--This dual-species approach gives us a versatile new toolbox for investigating the frontiers of quantum science.-->

Outside of research, I co-organise [Quantum on the Clock](https://www.iop.org/physics-community/special-interest-groups/qqq-group/quantum-clock), a UK-wide video competition designed to inspire 16-18 year olds to pursue physics degrees and consider careers in quantum science. Outside of work, I enjoy playing a variety of sports like football, table tennis, and volleyball—though with varying levels of competitiveness!

---

## Research Vision

In my group, we aim to exploit advanced quantum engineering techniques to explore new frontiers in both fundamental science and emerging quantum technologies. Using optical tweezer arrays, we trap and control individual atoms and molecules, building quantum matter one particle at a time. This approach enables scalable, programmable control over quantum matter, allowing us to explore new quantum phenomena and establish the foundations for future quantum devices.

---

## Current Projects

- **[DualQD: Dual-species tweezer arrays for next-generation quantum devices](/research/tech/dualqd)**

    Developing a two-species optical tweezer platform to build programmable quantum systems atom by atom.
  
Beyond my group’s core research, I contribute to a range of national and international collaborations using individually controlled atoms and molecules for quantum science. I lead an [international collaboration with the University of Waterloo](https://www.durham.ac.uk/news-events/latest-news/2025/01/grant-award-enables-durham-physicists-to-lead-international-quantum-projects-/) focused on developing "generation after next" quantum sensor arrays using atoms and molecules in optical tweezers. I am also co-investigator on the EPSRC Programme grant *Quantum many-body physics with ultracold polar molecules* and the project *Enhancing molecular control using Rydberg atoms*. The project below is in collaboration with Prof. Simon Cornish:

- [Enhancing molecular control using Rydberg atoms](https://www.cornishlabs.uk/tweezers) (with Prof. Simon Cornish)

    Exploring how to use Rydberg atoms to enhance the control of ultracold polar molecules in optical tweezers.
    
---

## Opportunities

We are always looking for motivated students and researchers interested in experimental quantum science. 

**We are currently recruiting for my DualQD project**. Interested students please see [here](/join/phdrecruit) for our current opportunities.

We also welcome approaches from postdoctoral researchers interested in applying for independent research fellowships to be hosted in Durham. For example the [Royal Society Newton International Fellowship](https://royalsociety.org/grants/newton-international/) and the [Marie Skłodowska-Curie Postoctoral Fellowships](https://marie-sklodowska-curie-actions.ec.europa.eu/actions/postdoctoral-fellowships).

Interested applicants should contact [Dr. Alex Guttridge](mailto:alexander.guttridge@durham.ac.uk).

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

