---
title: 'PoseVEC: Authoring Adaptive Pose-aware Effects using Visual Programming and Demonstrations'

# Authors
# If you created a profile for a user (e.g. the default `me` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - me
  - Cuong Nguyen
  - Rubaiat Habib Kazi
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
publication:  The 36th Annual ACM Symposium on User Interface Software and Technology (UIST ’23)
publication_short: In *UIST*


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
  

abstract: Pose-aware visual effects where graphics assets and animations are rendered reactively to the human pose have become increasingly popular, appearing on mobile devices, the web, or even headmounted displays like AR glasses. Yet, creating such effects still remains difficult for novices. In a traditional video editing workflow, a creator could utilize keyframes to create expressive but non-adaptive results which cannot be reused for other videos. Alternatively, programming-based approaches allow users to develop interactive effects, but are cumbersome for users to quickly express their creative intents. In this work, we propose a lightweight visual programming workflow for authoring adaptive and expressive pose effects. By combining a programming by demonstration paradigm with visual programming, we simplify three key tasks in the authoring process creating pose triggers, designing animation parameters, and rendering. We evaluated our system with a qualitative user study and a replicated example study, finding that all participants can create effects efficiently.


# Summary. An optional shortened abstract.
summary: Toolkit for authoring Adaptive Pose-aware Effects.

tags:
  - Visual Effects Authoring
  - Motion Graphics
  - Programming by Demonstration
  - Machine Learning



pager: false
# Display this page in the Featured widget?
#featured: true

# Standard identifiers for auto-linking
hugoblox:
  ids:
    doi: 10.1145/3586183.3606788

# Custom links

links:
  - type: pdf
    url: "https://yqz530.github.io/paper/UIST23.pdf"
  # - type: code
  #   url: https://github.com/HugoBlox/kit
  # - type: dataset
  #   url: https://github.com/HugoBlox/kit
  # - type: slides
  #   url: https://www.slideshare.net/
  # - type: source
  #   url: https://github.com/HugoBlox/kit
  - type: video
    url: https://youtu.be/5Od8u77GEYs




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
{{< highres src="sample.png" alt="PoseVEC System" >}}

<div class="not-prose max-w-prose grid grid-cols-1 md:grid-cols-[200px_auto] gap-4 my-6 text-base" style="line-height: 1.5;">

  <div class="font-bold text-2xl">Abstract</div>
  <div class="mb-4">
   Pose-aware visual effects where graphics assets and animations are rendered reactively to the human pose have become increasingly popular, appearing on mobile devices, the web, or even headmounted displays like AR glasses. Yet, creating such effects still remains difficult for novices. In a traditional video editing workflow, a creator could utilize keyframes to create expressive but non-adaptive results which cannot be reused for other videos. Alternatively, programming-based approaches allow users to develop interactive effects, but are cumbersome for users to quickly express their creative intents. In this work, we propose a lightweight visual programming workflow for authoring adaptive and expressive pose effects. By combining a programming by demonstration paradigm with visual programming, we simplify three key tasks in the authoring process: creating pose triggers, designing animation parameters, and rendering. We evaluated our system with a qualitative user study and a replicated example study, finding that all participants can create effects efficiently.
  </div>

  <div class="font-bold text-2xl">Publication</div>
  <div>
    In <em>Proceedings of the 36th Annual ACM Symposium on User Interface Software and Technology (UIST ’23)</em>
  </div>

  <div class="font-bold text-2xl mt-4">Video</div>
  <div class="video-container mt-4" style="margin-bottom: 2rem;">
    <iframe width="100%" height="250" src="https://www.youtube.com/embed/5Od8u77GEYs" title="Arlens" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="border-radius: 8px;"></iframe>
  </div>

</div>



<style>
  /* Expands the reading text blocks by ~25% (Default is 65ch) */
  .prose, 
  .max-w-prose { max-width: 120ch !important; }
  /* Expands the overarching page container to allow the wider text */
  .max-w-6xl {  max-width: 140rem !important; }
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