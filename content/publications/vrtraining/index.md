---
title: 'Mixed-Integer Programming for Adaptive VR Workflow Training'

# Authors
# If you created a profile for a user (e.g. the default `me` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - me
  - Chuan Yan
  - Haikun Huang
  - Simon Su
  - Lap-Fai Yu


date: '2023-10-28'

# Schedule page publish date (NOT publication's date).
#publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']
# publication_types: ["article-journal"]
# # Publication name and optional abbreviated publication name.
publication:  HCII
publication_short: In *HCII*


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
  

abstract: ...


# Summary. An optional shortened abstract.
summary: Generate adaptive training content for VR.

tags:
  - Adaptive training
  - Optimizatin 
  - Game design
  - Mixed-Integer Programming



pager: false
# Display this page in the Featured widget?
#featured: true

# Standard identifiers for auto-linking
hugoblox:
  ids:
    doi: 10.1007/978-3-031-61047-9_21

# Custom links

links:
  - type: pdf
    url: "https://yqz530.github.io/paper/vrtraining.pdf"
  # - type: code
  #   url: https://github.com/HugoBlox/kit
  # - type: dataset
  #   url: https://github.com/HugoBlox/kit
  # - type: slides
  #   url: https://www.slideshare.net/
  - type: pdf
    url: https://yqz530.github.io/paper/vrtraining_supp.pdf
  - type: video
    url: https://youtu.be/ZmRH4Bv5xWU



# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""




---
{{< highres src="sample.png" alt="VR Training" >}}

<div class="not-prose max-w-prose grid grid-cols-1 md:grid-cols-[300px_auto] gap-4 my-6 text-base" style="line-height: 1.5;">

  <div class="font-bold text-2xl">Abstract</div>
  <div class="mb-4">
   With advances in consumer-grade virtual reality (VR) devices, VR training gains unprecedented attention in research and industries. Although the nature of VR training encourages trainees to actively learn through exploring and gathering information in a simulated virtual environment, designing effective virtual training environments is non-trivial. We propose an adaptive approach that guides trainees to develop psychomotor skills in a simulated virtual environment. As a showcase, we demonstrate our novel approach for restaurant service using a game-based VR application. By incorporating the trainee’s performance and learning progress into optimization objectives, our approach uses mixed integer programming (MIP) to generate VR training sessions iteratively. Through collecting the trainee’s performance in VR training, our approach adapts the VR training sessions by considering the trainee’s strengths and weaknesses, guiding the trainee to improve over training sessions. We validated our approach through two experimental studies. In the first study, we compared our approach with a random training task assignment approach and a performance-only MIP approach through performing simulated restaurant service training. In the second study, we compared our approach with the random assignment approach by evaluating trainees’ skill developments in restaurant services. The results show that our skill-driven adaptive training approach outperforms the random assignment approach.
  </div>

  <div class="font-bold text-2xl">Publication</div>
  <div>
    In <em>Proceedings of the 26th HCI International Conference, HCII 2024</em>
  </div>

  <div class="font-bold text-2xl mt-4">Video</div>
  <div class="video-container mt-4" style="margin-bottom: 2rem;">
    <iframe width="100%" height="450" src="https://www.youtube.com/embed/ZmRH4Bv5xWU" title="Arlens" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="border-radius: 8px;"></iframe>
  </div>

</div>


<!-- <style>
  /* Expands the body text width */
  .prose { max-width: 110% !important; }
  .max-w-prose { max-width: 120% !important; }
  .max-w-6xl { max-width: 100rem !important; }
  .pub-row { display: none !important; }
</style> -->
<style>
  /* Expands the reading text blocks by ~25% (Default is 65ch) */
  .prose, 
  .max-w-prose { max-width: 100ch !important; }
  /* Expands the overarching page container to allow the wider text */
  .max-w-6xl {  max-width: 100rem !important; }
  /* Hides the theme's automatic metadata rows */
  .pub-row { display: none !important; }
</style>

<script>
  document.addEventListener('DOMContentLoaded', function() {
    // 1. Fix Bio Links
    const bioLinks = document.querySelectorAll('a[href*="/authors/"], a[href*="localhost:1313"]');
    bioLinks.forEach(link => {
      if (link.textContent.trim().includes('Yongqi Zhang')) {
        link.href = 'https://yqz530.github.io/';
      }
    });

    // 2. Hide Theme Metadata (FIXED: Now ignores your custom HTML block)
    const labels = document.querySelectorAll('div');
    labels.forEach(label => {
      const text = label.textContent.trim();
      if (text === 'Type' || text === 'Publication') {
        // Ensure we are NOT hiding our new custom 'not-prose' grid
        if (label.parentElement && !label.closest('.not-prose')) {
          label.parentElement.style.display = 'none';
        }
      }
    });
  });
</script>