---
layout: page
title: CaF lab
subtitle: Building a new platform for quantum simulation, one molecule at a time
---

<style>
/* All styles are scoped to .caf so they only affect this page */
.caf { --caf-accent: #0a6ea8; --caf-soft: #f2f7fb; --caf-line: #dde6ee; }
.caf img { max-width: 100%; height: auto; }
.caf section { margin: 3rem 0; }
.caf h2 { font-size: 1.7rem; font-weight: 700; margin-bottom: 1rem; }
.caf h2::after { content: ""; display: block; width: 3rem; height: 3px; background: var(--caf-accent); margin-top: .5rem; border-radius: 2px; }
.caf .lead { font-size: 1.2rem; line-height: 1.6; }
.caf .figure-cap { font-size: .9rem; color: #6b7680; margin-top: .4rem; line-height: 1.4; }
.caf .rounded-img { border-radius: 10px; box-shadow: 0 4px 14px rgba(0,0,0,.12); }

/* Labels and buttons use the theme's sans-serif font */
.caf .badge-open, .caf .btn-caf, .caf .btn-caf-outline, .caf .timeline .when, .caf .news-list .m, .caf .avatar { font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif; }

/* Hero */
.caf .hero { background: var(--caf-soft); border-radius: 14px; padding: 2rem; margin-top: 1rem; }
.caf .hero h1 { font-size: 1.9rem; font-weight: 800; line-height: 1.25; margin-top: 0; }
.caf .btn-caf { background: var(--caf-accent); color: #fff !important; border-radius: 30px; padding: .55rem 1.3rem; font-weight: 600; text-decoration: none !important; display: inline-block; margin: .3rem .4rem .3rem 0; }
.caf .btn-caf:hover { background: #085683; }
.caf .btn-caf-outline { border: 2px solid var(--caf-accent); color: var(--caf-accent) !important; border-radius: 30px; padding: .45rem 1.2rem; font-weight: 600; text-decoration: none !important; display: inline-block; margin: .3rem .4rem .3rem 0; }
.caf .badge-open { display: inline-block; background: #e6f4ea; color: #1e7b3c; font-weight: 700; font-size: .8rem; letter-spacing: .03em; text-transform: uppercase; padding: .25rem .7rem; border-radius: 20px; margin-bottom: .8rem; }

/* Why molecules cards */
.caf .why-card { background: #fff; border: 1px solid var(--caf-line); border-radius: 10px; padding: 1.1rem 1.2rem; height: 100%; }
.caf .why-card h4 { font-size: 1.05rem; font-weight: 700; margin: 0 0 .4rem; color: var(--caf-accent); }
.caf .why-card p { font-size: .95rem; margin: 0; }

/* Timeline */
.caf .timeline { list-style: none; padding-left: 0; margin: 0; border-left: 3px solid var(--caf-line); }
.caf .timeline li { position: relative; padding: 0 0 1.1rem 1.4rem; }
.caf .timeline li::before { content: ""; position: absolute; left: -9px; top: .35rem; width: 15px; height: 15px; border-radius: 50%; background: var(--caf-accent); border: 3px solid #fff; box-shadow: 0 0 0 1px var(--caf-accent); }
.caf .timeline li.future::before { background: #fff; }
.caf .timeline li.now::before { background: #f0a020; box-shadow: 0 0 0 1px #f0a020; }
.caf .timeline .when { font-size: .8rem; font-weight: 700; text-transform: uppercase; letter-spacing: .04em; color: #6b7680; }
.caf .timeline .what { font-weight: 600; }

/* Join box */
.caf .join { border: 2px solid var(--caf-accent); border-radius: 14px; padding: 1.8rem; }
.caf .join ul { padding-left: 1.2rem; }
.caf .join li { margin-bottom: .3rem; }

/* Team */
.caf .person { display: flex; align-items: center; gap: .8rem; padding: .6rem 0; }
.caf .avatar { flex: 0 0 48px; width: 48px; height: 48px; border-radius: 50%; background: var(--caf-accent); color: #fff; display: flex; align-items: center; justify-content: center; font-weight: 700; font-size: 1rem; }
.caf .avatar.phd { background: #2f9e8f; } .caf .avatar.msci { background: #7a68c4; } .caf .avatar.pdra { background: #d9822b; }
.caf .person .name { font-weight: 700; line-height: 1.2; }
.caf .person .role { font-size: .88rem; color: #6b7680; }

/* Life in the group carousel */
.caf .life-carousel { border-radius: 12px; overflow: hidden; box-shadow: 0 4px 14px rgba(0,0,0,.12); background: #1d2329; }
.caf .life-carousel .slide-frame { aspect-ratio: 3 / 2; display: flex; align-items: center; justify-content: center; background: #1d2329; }
.caf .life-carousel .slide-frame img { width: 100%; height: 100%; object-fit: contain; }
.caf .life-carousel .slide-cap { background: #fff; padding: .9rem 1.2rem 2.4rem; font-size: .98rem; line-height: 1.45; min-height: 5.5rem; }
.caf .life-carousel .slide-cap b { color: var(--caf-accent); margin-right: .3rem; font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif; }
.caf .life-carousel .carousel-indicators { bottom: .2rem; margin-bottom: .4rem; }
.caf .life-carousel .carousel-indicators li { background-color: var(--caf-accent); width: 22px; height: 4px; border-radius: 2px; }
.caf .life-carousel .carousel-control-prev, .caf .life-carousel .carousel-control-next { bottom: 5.5rem; width: 12%; }
.caf .life-carousel .carousel-control-prev-icon, .caf .life-carousel .carousel-control-next-icon { background-color: rgba(0,0,0,.45); border-radius: 50%; width: 2.4rem; height: 2.4rem; background-size: 50%; }

/* Publications and news */
.caf .pubs li { margin-bottom: .8rem; }
.caf details { margin-bottom: .6rem; }
.caf details summary { cursor: pointer; font-weight: 700; font-size: 1.05rem; }
.caf .news-list { list-style: none; padding-left: 0; }
.caf .news-list li { padding: .45rem 0; border-bottom: 1px solid var(--caf-line); }
.caf .news-list .m { display: inline-block; min-width: 5.5rem; font-weight: 700; color: var(--caf-accent); }
.caf .funding { font-size: .9rem; color: #6b7680; border-top: 1px solid var(--caf-line); padding-top: 1rem; }
</style>

<div class="caf">

<!-- ============ HERO ============ -->
<div class="hero">
  <span class="badge-open">PhD position · October 2027</span>
  <h1>Laser cooling molecules for quantum simulation</h1>
  <div class="row align-items-center">
    <div class="col-md-6">
      <p class="lead">Our team is building an experiment to cool calcium monofluoride (CaF) molecules to within a millionth of a degree of absolute zero, trap them with laser beams, and use them to explore quantum physics that is too hard to compute classically.</p>
      <a class="btn-caf" href="#join">Join the team</a>
      <a class="btn-caf-outline" href="#science">Our research</a>
    </div>
    <div class="col-md-6 mt-4 mt-md-0">
      <img class="rounded-img" src="{{ site.url }}{{ site.baseurl }}/research/coldmol/cafcool/img/archie_big_signal.jpg" alt="PhD student Archie with a molecular beam signal">
      <div class="figure-cap">PhD student Archie with a molecular beam signal.</div>
    </div>
  </div>
</div>

<!-- ============ THE SCIENCE ============ -->
<section id="science">
  <h2>Why molecules?</h2>
  <p>The study of ultracold atomic gases extends back around 40 years, and has led to remarkable advances in our understanding of quantum physics. Expanding the ultracold toolkit to molecules promises exciting opportunities to go beyond what is possible with atoms. Molecules possess extra degrees of freedom which span many orders of magnitude in energy, these include vibrational and rotational structure which provide a basis for precision measurement, tests of fundamental physics and the study of quantum chemistry. Polar molecules also experience long-range, anisotropic dipole-dipole interactions which can be used to study many-body physics, or controlled to set up quantum simulations or quantum computation. An optical lattice of ultracold polar molecules is an ideal testbed for many of these applications, and this is the goal of our lab.</p>
    <div class="text-center mb-4">
    <img class="rounded-img" src="{{ site.url }}{{ site.baseurl }}/research/coldmol/cafcool/img/why_molecules.png" alt="Figure showing energy scales, anisotropic dipole-dipole interaction and a drawing of molecules in an optical lattice.">
  </div>
  <div class="row">
    <div class="col-md-4 mb-3"><div class="why-card"><h4>Quantum simulation</h4><p>Arrays of interacting molecules can mimic models of quantum magnetism, helping us understand systems that classical computers struggle to describe.</p></div></div>
    <div class="col-md-4 mb-3"><div class="why-card"><h4>Optical lattice</h4><p>A retro-reflected laser beam sets up a standing intensity wave, ultracold molecules can be pinned to the intensity minima (or maxima).</p></div></div>
    <div class="col-md-4 mb-3"><div class="why-card"><h4>Laser cooling</h4><p>To be trapped, the molecules must be extremely cold (microkelvin), this can only be achieved by using lasers to remove energy.</p></div></div>
  </div>
</section>

<section>
  <h2>How our experiment works</h2>

  <!-- Step 1 + source photo -->
  <div class="row align-items-center mb-4">
    <div class="col-md-7">
      <p><b>1. Making the molecules.</b> Every laser cooling experiment starts by creating molecules. We use a pulsed Nd:YAG laser to ablate a calcium metal target, creating a plasma of Ca ions. Sulfur hexafluoride gas is injected, which reacts with the calcium to form CaF. This happens inside a copper cell cooled to 4&nbsp;K, cold helium gas also flows into the cell and cools the molecules. The cold CaF molecules then leave the cell as a beam travelling at around 150&nbsp;m/s.</p>
    </div>
    <div class="col-md-5">
      <img class="rounded-img" src="{{ site.url }}{{ site.baseurl }}/research/coldmol/cafcool/img/buffer_gas_source.png" alt="Annotated photo of the cryogenic buffer gas source showing the calcium target, helium sorbs, 4 K cryocooler and ablation laser path">
      <div class="figure-cap">Our cryogenic buffer gas source, where the CaF molecules are made.</div>
    </div>
  </div>

  <!-- Step 2 + transitions figure, vertically centred together -->
  <div class="row align-items-center mb-4">
    <div class="col-md-7">
      <p><b>2. Slowing them down.</b> 150&nbsp;m/s is far too fast to trap, so we need to decelerate the molecules. CaF has been chosen because of its nice structure, it has two electronic transitions which are almost closed (X (ground state) to A (1st electronic state) at 606&nbsp;nm and (X to B (2nd electronic state)) at 531&nbsp;nm. We use the X-B transition for laser slowing and counterpropagate a 531&nbsp;nm laser which is detuned to be resonant with fast molecules. We then sweep (chirp) its frequency to stay on resonance with the molecules and they slow down and their Doppler shift changes.</p>
    </div>
    <div class="col-md-5 text-center">
      <img class="rounded-img" src="{{ site.url }}{{ site.baseurl }}/research/coldmol/cafcool/img/CaF_structure.png" alt="Transitions involved in laser cooling CaF">
      <div class="figure-cap">Main transitions involved in slowing and cooling CaF, including vibrational decay probabilities.</div>
    </div>
  </div>

  <!-- Step 3 + coils image, vertically centred together -->
  <div class="row align-items-center mb-4">
    <div class="col-md-7">
      <p><b>3. Trapping and cooling.</b> Next we will capture the slowed molecules in a magneto-optical trap (MOT), cool them further, and load them into optical tweezer arrays and lattices for quantum simulation. We are in the process of building the chamber for the MOT.</p>
    </div>
    <div class="col-md-5 text-center">
      <img class="rounded-img" src="{{ site.url }}{{ site.baseurl }}/research/coldmol/cafcool/img/Lasers.jpeg" alt="Photo of orange and green laser beams">
      <div class="figure-cap">The lasers used for the main cooling transitions.</div>
    </div>
  </div>
</section>

<!-- ============ PROGRESS ============ -->
<section>
  <h2>Our progress so far</h2>
  <div class="row">
    <div class="col-md-6">
      <ul class="timeline">
        <li><div class="when">October 2021</div><div class="what">The group is founded</div>We begin planning our experiment.</li>
        <li><div class="when">September 2022</div><div class="what">New lab completed</div>An office space converted into our lab.</li>
        <li><div class="when">April 2024</div><div class="what">First CaF molecules</div>We see our first molecular signal.</li>
        <li class="now"><div class="when">Now</div><div class="what">Laser slowing the molecular beam</div>Our first slowing signals are in (right).</li>
        <li class="future"><div class="when">Next</div><div class="what">Magneto-optical trap</div>Capturing and cooling the slowed molecules.</li>
        <li class="future"><div class="when">Future</div><div class="what">Molecules in arrays of light</div>Optical lattices and tweezers for quantum simulation.</li>
      </ul>
    </div>
    <div class="col-md-6">
      <img class="rounded-img" src="{{ site.url }}{{ site.baseurl }}/research/coldmol/cafcool/img/first_slowing_signal.png" alt="Graph of molecular beam signal against time with no light, slowing light and slowing plus repump light">
      <div class="figure-cap">Our molecular beam signal with no light (black), slowing light (green), and slowing plus repump light (red). With the repump on, a second peak of later-arriving, slower molecules appears.</div>
    </div>
  </div>
</section>

<!-- ============ JOIN ============ -->
<section id="join">
  <div class="join">
    <span class="badge-open">Now recruiting</span>
    <h2>Join us: PhD starting October 2027</h2>
    <div class="row align-items-center mb-4">
      <div class="col-md-7">
        <p class="lead" style="font-size:1.1rem">We're looking for a PhD student to join the team working towards <b>quantum simulation with a lattice of CaF molecules</b>.</p>
        <p>This is a hands-on experimental project, and you'll be part of a friendly, close-knit team. Along the way you'll learn:</p>
        <ul>
          <li>Laser systems, optics and frequency stabilisation.</li>
          <li>Ultra-high vacuum and cryogenic techniques.</li>
          <li>Electronics, experiment control (Artiq) and data analysis (Python).</li>
          <li>Molecular and atomic physics, and quantum simulation.</li>
        </ul>
        <p>No previous experience with molecules is needed. Curiosity and enthusiasm for experimental physics matter most. Deadline for application:<b>15th December 2026</b></p>
        <a class="btn-caf" href="{{ site.baseurl }}/join/phdrecruit/#Williams">Project details</a>
        <a class="btn-caf-outline" href="{{ site.baseurl }}/join/howtoapply/">How to apply</a>
        <a class="btn-caf-outline" href="{{ site.baseurl }}/join/AboutPhD/">Life as a QLM student</a>
        <p class="mt-3 mb-0">Questions? Email <a href="mailto:hannah.williams4@durham.ac.uk">Dr Hannah Williams</a>. We're happy to chat informally or show you around the lab.</p>
      </div>
      <div class="col-md-5 mt-4 mt-md-0">
        <img class="rounded-img" src="{{ site.url }}{{ site.baseurl }}/research/coldmol/cafcool/img/chamber_lasers.jpg" alt="Vacuum chamber photo with orange and green laser beams">
      </div>
    </div>
  </div>
</section>

<!-- ============ TEAM ============ -->
<section id="team">
  <h2>The team</h2>
  <div class="row">
    <div class="col-md-6 mb-3">
      <img class="rounded-img" src="{{ site.url }}{{ site.baseurl }}/research/coldmol/cafcool/img/team_away_day_2026.jpg" alt="Five members of the CaF team sitting behind a table of Lego models at a team away day">
      <div class="figure-cap">Team away day, 2026.</div>
    </div>
    <div class="col-md-6">
      <div class="person"><div class="avatar">HW</div><div><div class="name"><a href="https://www.durham.ac.uk/staff/hannah-williams4/">Dr Hannah J. Williams</a> <small>(she/her)</small></div><div class="role">Principal Investigator· UKRI Future Leaders Fellow</div></div></div>
      <div class="person"><div class="avatar pdra">BH</div><div><div class="name">Dr Bethan Humphreys <small>(she/her)</small></div><div class="role">Postdoctoral researcher</div></div></div>
      <div class="person"><div class="avatar phd">AB</div><div><div class="name">Archie Baldock <small>(he/him)</small></div><div class="role">PhD student</div></div></div>
      <div class="person"><div class="avatar phd">RH</div><div><div class="name">Becca Hedley <small>(she/her)</small></div><div class="role">PhD student</div></div></div>
      <div class="person"><div class="avatar phd">LR</div><div><div class="name">Lara Rogers <small>(she/her)</small></div><div class="role">PhD student</div></div></div>
      <div class="person"><div class="avatar msci">NS</div><div><div class="name">Nicole Simpson <small>(she/her)</small></div><div class="role">MSci student</div></div></div>
      <div class="person"><div class="avatar msci">AK</div><div><div class="name">Andreas Ktori <small>(he/him)</small></div><div class="role">MSci student</div></div></div>
    </div>
  </div>
  <details class="mt-2">
    <summary>Former members</summary>
    <ul class="mt-2">
      <li>Dr Alex J. Matthies (they/them), PDRA 2023–2026, now a postdoc in Gothenburg</li>
      <li>Tom Philo (he/him), MSci student 2024–2025</li>
      <li>Keelan Sloan and Andrew Elwood, MSci students 2023–2024</li>
      <li>James Crilly, Matthew Page and Yuchao Liu, MSci students 2022–2023</li>
    </ul>
  </details>
</section>

<!-- ============ LIFE IN THE GROUP ============ -->
<section>
  <h2>Life in the group</h2>
  <div id="lifeCarousel" class="carousel slide life-carousel" data-ride="carousel" data-interval="5000" aria-label="Photos from life in the group">
    <ol class="carousel-indicators">
      <li data-target="#lifeCarousel" data-slide-to="0" class="active"></li>
      <li data-target="#lifeCarousel" data-slide-to="1"></li>
      <li data-target="#lifeCarousel" data-slide-to="2"></li>
      <li data-target="#lifeCarousel" data-slide-to="3"></li>
      <li data-target="#lifeCarousel" data-slide-to="4"></li>
      <li data-target="#lifeCarousel" data-slide-to="5"></li>
      <li data-target="#lifeCarousel" data-slide-to="6"></li>
      <li data-target="#lifeCarousel" data-slide-to="7"></li>
      <li data-target="#lifeCarousel" data-slide-to="8"></li>
    </ol>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <div class="slide-frame"><img src="{{ site.url }}{{ site.baseurl }}/research/coldmol/cafcool/img/Team_Seb_June_2026.jpeg" alt="Team members on the swings at a play park while a toddler plays in a toy car in the foreground"></div>
        <div class="slide-cap"><b>Team outing</b> to play park ft. Hannah's baby. May 2026</div>
      </div>
      <div class="carousel-item">
        <div class="slide-frame"><img src="{{ site.url }}{{ site.baseurl }}/research/coldmol/cafcool/img/MOT_coil_winding.jpg" alt="The CaF team winding invacuum MOT coils" loading="lazy"></div>
        <div class="slide-cap"><b>Teamwork</b> Winding MOT coils is a four person job! November 2026.</div>
      </div>
      <div class="carousel-item">
        <div class="slide-frame"><img src="{{ site.url }}{{ site.baseurl }}/research/coldmol/cafcool/img/Escape_the_lab_2025.jpg" alt="The CaF team holding a giant yellow key after completing an escape room" loading="lazy"></div>
        <div class="slide-cap"><b>We escaped!</b> Team escape room, February 2025.</div>
      </div>
      <div class="carousel-item">
        <div class="slide-frame"><img src="{{ site.url }}{{ site.baseurl }}/research/coldmol/cafcool/img/decelerator.jpg" alt="Photo of vacuum chamber" loading="lazy"></div>
        <div class="slide-cap"><b>Teamwork</b> Vacuum chamber for source and slowing, March 2025.</div>
      </div>
      <div class="carousel-item">
        <div class="slide-frame"><img src="{{ site.url }}{{ site.baseurl }}/research/coldmol/cafcool/img/christmas_lunch_2024.jpg" alt="The team sharing pizzas around a table at a Christmas lunch" loading="lazy"></div>
        <div class="slide-cap"><b>Christmas lunch</b> Pizza for the whole team, December 2024.</div>
      </div>
      <div class="carousel-item">
        <div class="slide-frame"><img src="{{ site.url }}{{ site.baseurl }}/research/coldmol/cafcool/img/dipolar_quantum_matter_2024.jpg" alt="Group photo of around sixty participants at the Dipolar Quantum Matter meeting" loading="lazy"></div>
        <div class="slide-cap"><b>Hosting a conference</b> We organised the Dipolar Quantum Matter ICAP satellite meeting in Durham, July 2024.</div>
      </div>
      <div class="carousel-item">
        <div class="slide-frame"><img src="{{ site.url }}{{ site.baseurl }}/research/coldmol/cafcool/img/archie_becca_spooky.jpg" alt="Archie and Becca wearing witch hats while working at the laser table enclosure" loading="lazy"></div>
        <div class="slide-cap"><b>Spooky science</b> Archie and Becca at the laser table. Halloween dress code optional.</div>
      </div>
      <div class="carousel-item">
        <div class="slide-frame"><img src="{{ site.url }}{{ site.baseurl }}/research/coldmol/cafcool/img/inconvenient_package.jpg" alt="Two team members carrying a very long package marked do not bend through the physics building entrance" loading="lazy"></div>
        <div class="slide-cap"><b>Special delivery</b> Some deliveries are more awkward than others.</div>
      </div>
      <div class="carousel-item">
        <div class="slide-frame"><img src="{{ site.url }}{{ site.baseurl }}/research/coldmol/cafcool/img/copper_cell.jpg" alt="Close-up of the copper buffer gas cell mounted inside the vacuum chamber" loading="lazy"></div>
        <div class="slide-cap"><b>Where molecules are born</b> The copper cell of our cryogenic buffer gas source, before it was sealed into the vacuum chamber.</div>
      </div>
    </div>
    <a class="carousel-control-prev" href="#lifeCarousel" role="button" data-slide="prev"><span class="carousel-control-prev-icon" aria-hidden="true"></span><span class="sr-only">Previous photo</span></a>
    <a class="carousel-control-next" href="#lifeCarousel" role="button" data-slide="next"><span class="carousel-control-next-icon" aria-hidden="true"></span><span class="sr-only">Next photo</span></a>
  </div>
</section>

<!-- ============ PUBLICATIONS ============ -->
<section id="publications">
  <h2>Publications</h2>
  <h3>Journal articles</h3>
  <ul class="pubs">
    <li><b>Near-deterministic loading of optical tweezer arrays via repulsive barricade potentials</b> (Preprint), <a href="https://arxiv.org/abs/2604.22406">arXiv:2604.22406</a> (2026).</li>
    <li><b>DiPolMol-Py: A Python package for calculations for <sup>2</sup>Σ ground-state molecules</b>, <i>Computer Physics Communications</i> (2025). <a href="https://doi.org/10.1016/j.cpc.2025.109813">Journal</a> · <a href="https://arxiv.org/abs/2503.21663">arXiv:2503.21663</a></li>
  </ul>
  <h3>Theses</h3>
  <ul class="pubs">
    <li><b>Bethan Humphreys</b> <a href="https://etheses.durham.ac.uk/id/eprint/16227/">Towards Zeeman-Sisyphus Deceleration of CaF Molecules</a> (2025).</li>
    <li><b>Hannah Williams</b> <a href="https://doi.org/10.25560/62635">Producing, trapping and controlling ultracold CaF molecules</a> (2018)</li>
  </ul>
</section>

<!-- ============ NEWS ============ -->
<section id="news">
  <h2>News</h2>
  <ul class="news-list">
    <li><span class="m">Nov 2026</span> We start rebuilding the entire experiment as we change our focus to making a MOT.</li>
    <li><span class="m">Oct 2026</span> Lara joins the lab for her PhD, and Nicole returns along with Andreas for MSci projects. Welcome all!</li>
    <li><span class="m">Sept 2026</span> We see the first signal of laser slowing! </li>
    <li><span class="m">Aug 2026</span> The whole team goes to Imperial for the second UK Laser Cooling Molecules meeting. Nicole finishes her summer internship, having set up environmental monitoring for the lab.</li>
    <li><span class="m">Jul 2026</span> Bethan and Becca attend the <a href="https://www.qsmol.uk/">QSMol</a> kick-off meeting. Nicole joins the team for a summer internship. Welcome Nicole!</li>
    <li><span class="m">Jun 2026</span> Archie presents a poster at <a href="https://www.icap29.com/home.html">ICAP</a> in Wuhan and at the ultracold molecules satellite meeting in Hong Kong. Alex leaves the group to start a postdoc in Gothenburg. Good luck, and thank you!</li>
    <li><span class="m">May 2026</span> We finish the Zeeman-Sisyphus project. Sadly, we saw no deceleration.</li>
    <li><span class="m">Apr 2026</span> Our proposal paper on near-deterministic loading of tweezer arrays is on <a href="https://arxiv.org/abs/2604.22406">arXiv</a>.</li>
  </ul>

  <details>
    <summary>2025</summary>
    <ul class="news-list">
      <li><span class="m">Sep</span> Hannah returns to work. Bethan and Hannah attend the EPSRC Quantum Technologies Future Leaders Event.</li>
      <li><span class="m">Aug</span> Our paper <i>DiPolMol-Py: A Python package for calculations for <sup>2</sup>Σ ground-state molecules</i> is <a href="https://doi.org/10.1016/j.cpc.2025.109813">published</a>.</li>
      <li><span class="m">Jul</span> Archie presents a poster at <a href="https://ecamp15.org/">ECAMP15</a> and Becca presents a poster at <a href="https://yao.iqoqi.at/">YAO</a>, both in Innsbruck.</li>
      <li><span class="m">Jun</span> Tom graduates. Congratulations and best of luck for the future! Bethan presents a poster at <a href="https://www.icols2025.it/">ICOLS2025</a> on the island of Elba, and Alex presents a poster at the <a href="https://www.ultracold-molecules-2025.pl/">Workshop on Ultracold Molecules</a> in Warsaw.</li>
      <li><span class="m">May</span> Bethan passes her viva! Congratulations, and welcome back as a PDRA, Dr Humphreys!</li>
      <li><span class="m">Apr</span> Hannah begins maternity leave.</li>
      <li><span class="m">Mar</span> Becca attends <a href="https://www.nottingham.ac.uk/conference/fac-sci/physics/women-in-physics/">PG Women in Physics</a>. We submit our first <a href="https://arxiv.org/abs/2503.21663">paper</a>, and Bethan submits her PhD thesis.</li>
      <li><span class="m">Jan</span> The whole team heads to Imperial College for the first UK laser cooling molecules workshop.</li>
    </ul>
  </details>

  <details>
    <summary>2024</summary>
    <ul class="news-list">
      <li><span class="m">Oct</span> Rebecca joins the group for her PhD, and Tom starts his Master's project. Welcome to the team, both! Alex spends three weeks visiting cold molecule labs in the USA.</li>
      <li><span class="m">Sep</span> Alex and Hannah attend <a href="https://ccmi2024.ist.ac.at/">CCMI</a> near Vienna, where Alex presents a poster and Hannah gives an invited talk.</li>
      <li><span class="m">Jul</span> We host the <a href="https://durham-qlm.uk/events/conferences/ICAP_satellite/">Dipolar Quantum Matter</a> ICAP satellite meeting, which is a resounding success! Archie presents a poster at the ICAP summer school in Oxford, and Bethan presents a <a href="https://virtual.oxfordabstracts.com/#/event/3520/poster-gallery/grid?sort=program-codes&amp;current=375">poster</a> at <a href="https://icap28.com/">ICAP</a>.</li>
      <li><span class="m">Jun</span> Alex presents a <a href="{{ site.baseurl }}/research/coldmol/cafcool/img/EGAS%202024.pdf" target="_blank">poster</a> at <a href="https://eventos.ugr.es/egas55/">EGAS</a> in Granada. Keelan and Andrew both graduate. Congratulations and good luck in your future endeavours!</li>
      <li><span class="m">Apr</span> We see CaF molecules in the lab for the first time!</li>
    </ul>
  </details>

  <details>
    <summary>2023</summary>
    <ul class="news-list">
      <li><span class="m">Dec</span> Hannah is awarded a UKRI <a href="https://www.durham.ac.uk/departments/academic/physics/news/department-awarded-two-ukri-future-leaders-fellowships/">Future Leaders Fellowship</a> for the project <a href="https://gtr.ukri.org/projects?ref=MR%2FX033430%2F1">Molecules for Quantum Simulation</a>, starting June 2024.</li>
      <li><span class="m">Nov</span> Bethan gives her first academic talk at the <a href="https://quantum.sites.sheffield.ac.uk/about/events/northern-quantum-meeting-ix">Northern Quantum Meeting IX</a> in Sheffield.</li>
      <li><span class="m">Oct</span> The team is growing rapidly! Archie Baldock joins as a PhD student, and two MSci students join: Keelan Sloan, working on background-free imaging of CaF, and Andrew Elwood, building a cooled leader-follower laser system.</li>
      <li><span class="m">Sep</span> Dr Alex Matthies joins the team as a PDRA. Welcome Alex!</li>
      <li><span class="m">Jul</span> James, Yuchao and Matthew all graduate from Durham University. Congratulations all! Keelan Sloan joins for a summer placement to help build our cryogenic buffer gas source. Welcome to the team, Keelan!</li>
      <li><span class="m">Jun</span> Bethan presents her first poster at <a href="https://www.eps-egas.org/302-egas-54.html">EGAS</a> in Strasbourg.</li>
      <li><span class="m">Jan</span> Hannah is awarded an EPSRC <a href="https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/X013758/1">New Investigator Award</a> to test a Zeeman-Sisyphus decelerator for CaF molecules (April 2023 to September 2025).</li>
    </ul>
  </details>

  <details>
    <summary>2022</summary>
    <ul class="news-list">
      <li><span class="m">Oct</span> Three MSci students join the group: James Crilly (co-supervised by Dr Carty, simulating the Zeeman-Sisyphus decelerator), and Matthew Page and Yuchao Liu (co-supervised by Prof. Cornish, working on tweezer simulations and creation using a spatial light modulator).</li>
      <li><span class="m">Sep</span> The lab refurbishment is complete!</li>
      <li><span class="m">Jul</span> Bethan passes her 9-month progression. Congratulations!</li>
      <li><span class="m">Feb</span> Bethan attends the <a href="https://www.erbium.at/UCQG22/">Introductory Course on Ultracold Quantum Gases</a> in Innsbruck.</li>
      <li><span class="m">Jan</span> Work starts on converting office space into our lab.</li>
    </ul>
  </details>

  <details>
    <summary>2021</summary>
    <ul class="news-list">
      <li><span class="m">Oct</span> The group is formed, and Bethan joins as the first PhD student. Welcome Bethan!</li>
    </ul>
  </details>
</section>

<p class="funding">This work is supported by UKRI Future Leaders Fellowship MR/X033430/1. Page design and layout developed with the assistance of Claude (Anthropic), content reviewed by CaF team.</p>

</div>
