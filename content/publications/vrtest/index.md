---
title: 'HieraVisVR: Hierarchical Visual Analytics for Motion-Centric VR Playtesting'

# Authors
# If you created a profile for a user (e.g. the default `me` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - me
  - Erdem Murat
  - Liuchuan Yu
  - Haikun Huang
  - Minsoo Choi
  - Christos Mousas
  - Lap-Fai Yu

# Author notes (optional)
#author_notes:
#  - 'Equal contribution'
#  - 'Equal contribution'

date: '2026-02-28'

# Schedule page publish date (NOT publication's date).
#publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']
# publication_types: ["article-journal"]
# # Publication name and optional abbreviated publication name.
publication: In *Proceedings of the ACM Conference on Human Factors in Computing Systems (CHI'26)*
publication_short: In *CHI*


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
  

abstract: Playtesting is widely used in the game industry to identify design flaws and evaluate player experience, yet little research explores how to effectively visualize and analyze playtesting data. This challenge is particularly pronounced in motion-based VR games, which involve physical movements and interactions tracked through multimodal inputs, resulting in complex multidimensional data. To better understand the challenges designers face, we conducted a formative study with 30 practitioners in the VR domain to characterize playtesting workflows and associated tasks. Based on these findings, we present HieraVisVR, a hierarchical visual analytics framework that incorporates body-motion-related data to help designers identify player behaviors and critical game moments, simplifying their workflow. We demonstrate the applicability of HieraVisVR in three different applications and evaluate our system with playtesting experts through an analysis of motion-based game data. The study results suggest that our system enhances playtesters' understanding of the gameplay and improves their data analysis workflow.


# Summary. An optional shortened abstract.
summary: A visual analytics tool to streamline the VR game playtesting process..

tags:
  - Visual analytic 
  - VR Playtesting workflow
  - Clustering



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
    url: "https://yqz530.github.io/paper/vrtest.pdf"
  # - type: code
  #   url: https://github.com/HugoBlox/kit
  # - type: dataset
  #   url: https://github.com/HugoBlox/kit
  # - type: slides
  #   url: https://www.slideshare.net/
  # - type: source
  #   url: https://github.com/HugoBlox/kit
  - type: video
    url: https://youtu.be/mFpQj-F7muU




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

<div class="not-prose max-w-prose grid grid-cols-1 md:grid-cols-[220px_auto] gap-4 my-6 text-base" style="line-height: 1.5;">

  <div class="font-bold text-2xl">Abstract</div>
  <div class="mb-4">
    Playtesting is widely used in the game industry to identify design flaws and evaluate player experience, yet little research explores how to effectively visualize and analyze playtesting data. This challenge is particularly pronounced in motion-based VR games, which involve physical movements and interactions tracked through multimodal inputs, resulting in complex multidimensional data. To better understand the challenges designers face, we conducted a formative study with 30 practitioners in the VR domain to characterize playtesting workflows and associated tasks. Based on these findings, we present HieraVisVR, a hierarchical visual analytics framework that incorporates body-motion-related data to help designers identify player behaviors and critical game moments, simplifying their workflow. We demonstrate the applicability of HieraVisVR in three different applications and evaluate our system with playtesting experts through an analysis of motion-based game data. The study results suggest that our system enhances playtesters' understanding of the gameplay and improves their data analysis workflow.
  </div>

  <div class="font-bold text-2xl">Publication</div>
  <div>
    In <em>Proceedings of the ACM Conference on Human Factors in Computing Systems (CHI'26)</em>
  </div>

  <div class="font-bold text-2xl mt-4">Video</div>
  <div class="video-container mt-4" style="margin-bottom: 2rem;">
    <iframe width="100%" height="350" src="https://www.youtube.com/embed/mFpQj-F7muU" title="HieraVisVR" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="border-radius: 8px;"></iframe>
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
  .max-w-prose { 
    max-width: 85ch !important; 
  }

  /* Expands the overarching page container to allow the wider text */
  .max-w-6xl { 
    max-width: 90rem !important; 
  }
  
  /* Hides the theme's automatic metadata rows */
  .pub-row { 
    display: none !important; 
  }
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