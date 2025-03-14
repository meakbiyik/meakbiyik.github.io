---
layout: page
permalink: /routeformer/
title: Leveraging Driver Field-of-View for Multimodal Ego-Trajectory Prediction
nav: false
---

<style>
  .publication-authors {
    margin-bottom: 1.5rem;
    text-align: center;
    line-height: 1.6;
  }
  
  .author-block {
    display: inline-block;
    margin-right: 0.2rem;
  }
  
  .author-block a {
    font-weight: 500;
    text-decoration: none;
  }
  
  .author-block a:hover {
    text-decoration: underline;
  }
  
  .affiliations {
    margin-top: 0.75rem;
    font-size: 0.9em;
  }
  
  .affiliation-item {
    display: inline-block;
    margin: 0 1rem;
  }
  
  sup {
    font-size: 75%;
    position: relative;
    top: -0.5em;
  }
  
  .conference-info {
    margin-top: 1rem;
    font-weight: bold;
    font-size: 1.1em;
  }

/* Button styles using theme variables */
.publication-links {
  margin-top: 0.8rem;
  margin-bottom: 2rem;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 0.5rem;
}

.link-block {
  display: inline-block;
  margin: 0 0.25rem;
}

.button {
  padding: 0.5rem 1rem;
  border-radius: 4px;
  font-weight: 500;
  display: inline-flex;
  align-items: center;
  transition: all 0.2s ease;
}

.button.is-dark {
  border: 0.5rem var(--global-text-color);
  color: var(--global-bg-color);
}

.button.is-dark:hover {
  background-color: var(--global-theme-color);
  color: var(--global-hover-text-color);
  transform: translateY(-2px);
  box-shadow: 0 2px 5px var(--global-divider-color);
}

.button .icon {
  margin-right: 0.5rem;
}

/* BibTeX styles using theme variables */
#BibTeX {
  margin-top: 2rem;
  padding: 2rem 0;
  border-top: 1px solid var(--global-divider-color);
}

#BibTeX .title {
  color: var(--global-text-color);
}

#BibTeX pre {
  background-color: var(--global-code-bg-color);
  border-radius: 6px;
  padding: 1.25rem;
  overflow-x: auto;
  font-family: 'Courier New', monospace;
  border: 1px solid var(--global-divider-color);
  font-size: 0.9rem;
  line-height: 1.5;
  margin-top: 1rem;
  color: var(--global-text-color);
}

#BibTeX code {
  white-space: pre-wrap;
  color: var(--global-text-color);
}

/* Fix for section layout */
.section {
  padding: 3rem 1.5rem;
  background-color: var(--global-bg-color);
  color: var(--global-text-color);
}

.is-max-desktop {
  max-width: 960px;
  margin: 0 auto;
}

/* Add some spacing to h2 titles */
.title.is-3 {
  margin-bottom: 1.5rem;
  color: var(--global-text-color);
}

/* Style for content */
.content {
  color: var(--global-text-color);
}

.content h2 {
  color: var(--global-text-color);
}

/* Ensure links follow the theme colors */
a {
  color: var(--global-theme-color);
  transition: color 0.2s ease;
}

a:hover {
  color: var(--global-hover-color);
  text-decoration: underline;
}
</style>

<section class="hero">
    <div class="hero-body">
    <div class="is-max-desktop">
        <div class="columns is-centered">
        <div class="column has-text-centered">
        <div class="publication-authors">
            <span class="author-block">
                <a>M. Eren Akbiyik</a><sup>1</sup>,</span>
            <span class="author-block">
                <a>Nedko Savov</a><sup>2</sup>,</span>
            <span class="author-block">
                <a>Danda Pani Paudel</a><sup>2</sup>,</span>
            <span class="author-block">
                <a>Nikola Popovic</a><sup>1,2</sup>,</span> <br/>
            <span class="author-block">
                <a>Christian Vater</a><sup>3</sup>,</span>
            <span class="author-block">
                <a>Otmar Hilliges</a><sup>1</sup>,</span>
            <span class="author-block">
                <a>Luc Van Gool</a><sup>2</sup>,</span>
            <span class="author-block">
                <a>Xi Wang</a><sup>1,4</sup>
            </span>
        </div>

        <div class="publication-authors affiliations">
            <div class="affiliation-item"><sup>1</sup>ETH Zürich</div>
            <div class="affiliation-item"><sup>2</sup>INSAIT, Sofia University "St. Kliment Ohridski"</div>
            <div class="affiliation-item"><sup>3</sup>University of Bern</div>
            <div class="affiliation-item"><sup>4</sup>TU Munich</div>
        </div>

        <div class="publication-authors conference-info">
            ICLR 2025
        </div>

            <div class="column has-text-centered">
            <div class="publication-links">
                <!-- PDF Link. -->
                <span class="link-block">
                <a
                    href="https://arxiv.org/abs/2312.08558"
                    class="external-link button is-normal is-rounded is-dark"
                    target="_blank"
                >
                    <span class="icon">
                    <i class="fas fa-file-pdf"></i>
                    </span>
                    <span>Paper</span>
                </a>
                </span>
                <span class="link-block">
                <a
                    href="https://github.com/meakbiyik/routeformer"
                    class="external-link button is-normal is-rounded is-dark"
                    target="_blank"
                >
                    <span class="icon">
                    <i class="fas fa-file-code"></i>
                    </span>
                    <span>Code</span>
                </a>
                </span>
                <!-- Video Link. -->
                <!--               <span class="link-block">
            <a href="https://youtu.be/YB1_xKlueUI"
                class="external-link button is-normal is-rounded is-dark">
                    target="_blank"
                <span class="icon">
                    <i class="fab fa-youtube"></i>
                </span>
                <span>Video</span>
            </a>
            </span> -->
            </div>
            </div>
        </div>
        </div>
    </div>
    </div>

</section>

<div class="columns is-centered has-text-centered">
    <div class="column is-four-fifths">
    <div class="diagram">
        {% include figure.liquid loading="eager" path="assets/img/framework.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
    </div>
</div>

<section class="section">
    <div class="is-max-desktop">
    <!-- Abstract. -->
    <div class="columns is-centered has-text-centered">
        <div class="column is-four-fifths">
        <h2 class="title is-3">Abstract</h2>
        <div class="content has-text-justified">
            <p>
            Understanding drivers' decision-making is crucial for road safety. Although predicting the ego-vehicle's path is valuable for driver-assistance systems, existing methods mainly focus on external factors like other vehicles' motions, often neglecting the driver's attention and intent. To address this gap, we infer the ego-trajectory by integrating the driver's attention and the surrounding scene. We introduce Routeformer, a novel multimodal ego-trajectory prediction network combining GPS data, environmental context, and driver field-of-view—comprising first-person video and gaze fixations. We also present the Path Complexity Index (PCI), a new metric for trajectory complexity that enables a more nuanced evaluation of challenging scenarios. To tackle data scarcity and enhance diversity, we introduce GEM, a comprehensive dataset of urban driving scenarios enriched with synchronized driver field-of-view and gaze data. Extensive evaluations on GEM and DR(eye)VE demonstrate that Routeformer significantly outperforms state-of-the-art methods, achieving notable improvements in prediction accuracy across diverse conditions. Ablation studies reveal that incorporating driver field-of-view data yields significantly better average displacement error, especially in challenging scenarios with high PCI scores, underscoring the importance of modeling driver attention. All data, code, and models will be made publicly available.
            </p>
        </div>
        </div>
    </div>
    </div>
</section>

<section class="section" id="BibTeX">
    <div class="is-max-desktop content">
    <h2 class="title">BibTeX</h2>
    <pre><code>@inproceedings{akbiyik2023routeformer,
    title={Leveraging Driver Field-of-View for Multimodal Ego-Trajectory Prediction},
    author={M. Eren Akbiyik, Nedko Savov, Danda Pani Paudel, Nikola Popovic, Christian Vater, Otmar Hilliges, Luc Van Gool, Xi Wang},
    booktitle={International Conference on Learning Representations},
    year={2025}
}</code></pre>
    </div>
</section>
