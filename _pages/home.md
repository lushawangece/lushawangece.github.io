---
layout: archive
permalink: /
title: "Home"
excerpt: "Home"
author_profile: true
redirect_from: 
  - /home/
  - /home.html
---



PhD Positions Available  
======
I'm seeking self-motivated students who are passionate about research and have strong background in mathematical and electrical engineering to join my group. My research interests include modeling, optimization and machine learning for power distribution systems. If you are passionate about advancing research in these fields, please send your resume to [lusha.wang@ua.edu](mailto:lusha.wang@ua.edu) with subject line "PhD Application + Name". Detailed information can be found on the [PhD application details]({{ '/team/#join-the-team' | relative_url }}) page.


<!-- Biography
======
Dr. Lusha Wang is a tenure-track Assistant Professor with the [Department of Electrical and Computer Engineering](https://ece.eng.ua.edu/) at the [University of Alabama](https://www.ua.edu/). She was a Postdoctoral Appointee in the Energy System Division, [Argonne National Laboratory](https://www.anl.gov/) during 2022-2023. She received the B.E. degree in Electrical Engineering from Wuhan University, Wuhan, China in 2016 and the Ph.D. degree in Electrical Engineering at the School of Electrical Engineering and Computer Science, [Washington State University](https://wsu.edu/), Pullman, WA, USA in 2022, advised by [Prof. Noel Schulz](https://president.wsu.edu/noel-schulz-bio/) and [Prof. Anamika Dubey](https://eecs.wsu.edu/~adubey/). She has been a research aide with the Energy System Division, [Argonne National Laboratory](https://www.anl.gov/) in 2019 and 2020.  -->

Education
======

- Ph.D. in Electrical Engineering (Minor: Computer Science), Washington State University, Pullman, USA, 2022.
- B.E. in Electrical Engineering, Wuhan University, Wuhan, China, 2016.



Work Experience
======

- Assistant Professor, The University of Alabama, Alabama, United States, 2023–present.
- Post-doctoral Appointee, Argonne National Laboratory, Illinois, United States, 2022–2023.
- Research Aide, Argonne National Laboratory, Illinois, United States, May–Dec 2019; May–Aug 2020.
- Graduate Research Assistant, Washington State University, Pullman, United States, 2017–2022.
- Software Developer, Virtue Intelligent Network Co., Ltd., Wuhan, China, 2016–2017.


Research Interests
======
My research focuses on analyzing and managing electric vehicles (EVs) and distributed energy resources (DERs) in emerging power distribution and transportation systems for improved grid resilience. The goal of my research is to develop practically efficient tools for utilities that lead to intelligent and sustainable power and energy systems and facilitate electrification.
1. Power distribution systems modeling and analysis
1. Transportation electrification
1. Power system resilience and protection
1. Power system optimization and control
1. Distributed renewable integration


Awards
=======
* IEEE PES General Meeting Best Paper Award 2025: _Smart_ _charging_ _impact_ _analysis_ _using_ _clustering_ _methods_ _and_ _real-world_ _distribution_ _feeders_
* iREDEFINE Professional Development Award:   _Awarded_ _to_ _12_ _PhD_ _students_ _and_ _Post-doc_ _in_ _the_ _US_ _and_ _Canada_ _selected_ _by_ _ECE_ _department_ _chairs_, 2023 
* IEEE PES Grid Edge Technologies 3-Minute Ph.D. Dissertation Challenge Finalist, 2023

CV
======

<p class="cv-line">
  <a href="{{ '/files/cv.pdf' | relative_url }}">Download CV (PDF)</a>
  <small id="cv-updated" class="cv-muted"> · Checking…</small>
</p>

<script>
(async () => {
  const el = document.getElementById('cv-updated');
  if (!el) return;

  const owner = 'lushawangece';
  const repo  = 'lushawangece.github.io';
  const path  = 'files/cv.pdf';        // repo-relative path to your PDF
  const branch = 'master';             // change if your default branch differs

  try {
    const url = `https://api.github.com/repos/${owner}/${repo}/commits?sha=${branch}&path=${encodeURIComponent(path)}&per_page=1`;
    const res = await fetch(url);
    if (!res.ok) throw new Error('HTTP ' + res.status);
    const data = await res.json();
    const iso  = data?.[0]?.commit?.committer?.date || data?.[0]?.commit?.author?.date;
    if (!iso) { el.remove(); return; }

    // Show in your local timezone
    const d = new Date(iso);
    const opts = { year:'numeric', month:'short', day:'2-digit', timeZone:'America/Chicago' };
    el.textContent = ' · Updated ' + d.toLocaleDateString(undefined, opts);
  } catch (e) {
    // if the API fails, hide the placeholder
    el.remove();
  }
})();
</script>

<style>
  .cv-line { margin:.25rem 0 1rem; }
  .cv-muted { color:#444; font-weight:400; }
</style>



Contact
======

**Email:**  
lusha.wang[AT]ua.edu  
lwang115[AT]ua.edu  
lushawang06[AT]gmail.com  

**Address:**  
3018 SERC  
Tuscaloosa, AL 35487  
United States
