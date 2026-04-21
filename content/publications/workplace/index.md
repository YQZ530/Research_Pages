---
title: 'Joint Computational Design of Workspaces and Workplans'

# Authors
# If you created a profile for a user (e.g. the default `me` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - me
  - Haikun Huang
  - Erion Plaku
  - Christos Mousas
  - Lap-Fai Yu

# Author notes (optional)
#author_notes:
#  - 'Equal contribution'
#  - 'Equal contribution'

date: '2021-02-28'

# Schedule page publish date (NOT publication's date).
#publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']
# publication_types: ["article-journal"]
# # Publication name and optional abbreviated publication name.
publication: In *ACM Transactions on Graphics (SIGGRAPH Asia 21)*
publication_short: In *SIGGRAPH Asia 21*


header:
  navbar:
    enable: false

image: 
    filename: ""
#   filename: "featured.png"
#   placement: 1
#   caption: ""
#   focal_point: "Smart"
#   preview_only: false
#   resample_filter: "Lanczos"
#   quality: 130
  

abstract: Humans assume different production roles in a workspace. On one hand, humans design workplans to complete tasks as efficiently as possible in order to improve productivity. On the other hand, a nice workspace is essential to facilitate teamwork. In this way, workspace design and workplan design complement each other. Inspired by such observations, we propose an automatic approach to jointly design a workspace and a workplan. Taking staff properties, a space, and work equipment as input, our approach jointly optimizes a workspace and a workplan, considering performance factors such as time efficiency and congestion avoidance, as well as workload factors such as walk effort, turn effort, and workload balances. To enable exploration of design trade-offs, our approach generates a set of Pareto-optimal design solutions with strengths on different objectives, which can be adopted for different work scenarios. We apply our approach to synthesize workspaces and workplans for different workplaces such as a fast food kitchen and a supermarket. We also extend our approach to incorporate other common work considerations such as dynamic work demands and accommodating staff members with different physical capabilities. Evaluation experiments with simulations validate the efficacy of our approach for synthesizing effective workspaces and workplans.


# Summary. An optional shortened abstract.
summary: A computational design tool to synthesize workplaces.

tags:
  - Layout Design
  - Computational Design
  - Personalization
  - Agent Simulation



pager: false
# Display this page in the Featured widget?
#featured: true

# Standard identifiers for auto-linking
hugoblox:
  ids:
    doi: 10.5555/123456

# Custom links

links:
  - type: pdf
    url: "https://yqz530.github.io/paper/workplace.pdf"
  # - type: code
  #   url: https://github.com/HugoBlox/kit
  # - type: dataset
  #   url: https://github.com/HugoBlox/kit
  # - type: slides
  #   url: https://www.slideshare.net/
  # - type: source
  #   url: https://github.com/HugoBlox/kit
  - type: video
    url: https://youtu.be/xP3OhUE8XVs


# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
#   - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""




---
{{< highres src="hiera.png" alt="HieraVisVR System" >}}
  <div>
  <h4>Overview</h4>
  <iframe width="560" height="315" src="https://www.youtube.com/embed/xP3OhUE8XVs " title="PSA Sol1" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
    <style>
  /* Expands the reading text blocks by ~25% (Default is 65ch) */
  .prose, 
  .max-w-prose { max-width: 140ch !important; }
  /* Expands the overarching page container to allow the wider text */
  .max-w-6xl {  max-width: 160rem !important; }
  /* Hides the theme's automatic metadata rows */
  .pub-row { display: none !important; }
</style>
<style>
  .video-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr); /* 3 columns */
    gap: 20px; /* Space between videos */
    margin-top: 20px;
  }
  .video-item {
    width: 100%;
  }
  .video-item iframe {
    width: 100%;
    aspect-ratio: 16 / 9;
    height: auto;
  }
  /* Responsive: stack videos on small screens */
  @media (max-width: 900px) {
    .video-grid { grid-template-columns: repeat(2, 1fr); }
  }
  @media (max-width: 600px) {
    .video-grid { grid-template-columns: 1fr; }
  }
</style>

<div class="video-grid">
  <div class="video-item">
    <h4>Fastfood Restaurant: Solution 1</h4>
    <iframe src="https://www.youtube.com/embed/Z_5wMUSRM7A" title="PSA Sol1" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>

  <div class="video-item">
    <h4>Fastfood Restaurant: Solution 2</h4>
    <iframe src="https://www.youtube.com/embed/uDrBJ_6p8ko" title="PSA Sol2" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>

  <div class="video-item">
    <h4>Fastfood Restaurant: Solution 3</h4>
    <iframe src="https://www.youtube.com/embed/HcHPJ5wVp9o" title="PSA Sol3" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>

  <div class="video-item">
    <h4>Accessibility: Donation Center</h4>
    <iframe src="https://www.youtube.com/embed/BfOOM7BhuEU" title="Donation Center" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>

  <div class="video-item">
    <h4>Supermarket: Morning Strategy</h4>
    <iframe src="https://www.youtube.com/embed/53SJGZB-glI" title="Morning Plan" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>

  <div class="video-item">
    <h4>Supermarket: Afternoon Strategy</h4>
    <iframe src="https://www.youtube.com/embed/Be59z1j9gUE" title="Afternoon Plan" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>
</div>