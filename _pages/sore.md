---
layout: page
permalink: /sore/
title: Semantic Outlier Removal with Embedding Models and LLMs
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

  .post-title {
    text-align: center;
    margin-top: -2rem;
  }

/* Button styles using theme variables */
.publication-links {
  margin-top: 0.8rem;
  margin-bottom: 2rem;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 0.5rem;

  @media (max-width: 768px) {
    justify-content: flex-start;
  }
}

.link-block {
  position: relative;
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

.arrow-container {
  position: absolute;
  display: inline-flex;
  flex-direction: row;
  align-items: center;
  min-width: 200px;
  gap: 0.5rem;
}

.curved-arrow {
  margin-bottom: 0.5rem;
}

.arrow-text {
  font-family: 'Comic Sans MS', 'Chalkboard SE', cursive;
  font-size: 0.9rem;
  color: #FF6347;
  text-align: center;
}

</style>

<section class="hero">
    <div class="hero-body">
    <div class="is-max-desktop">
        <div class="columns is-centered">
        <div class="column has-text-centered">
        <div class="publication-authors">
            <span class="author-block">
                <a>Eren Akbiyik</a>,</span>
            <span class="author-block">
                <a>João Almeida</a>,</span>
            <span class="author-block">
                <a>Rik Melis</a>,</span> <br/>
            <span class="author-block">
                <a>Ritu Sriram</a>,</span>
            <span class="author-block">
                <a>Viviana Petrescu</a>,</span>
            <span class="author-block">
                <a>Vilhjálmur Vilhjálmsson</a>,</span>
        </div>

        <div class="publication-authors affiliations">
            <div class="affiliation-item">TripleLift<br/>Zürich, Switzerland</div>
        </div>

        <div class="publication-authors conference-info">
            ACL 2025 Industry Track
        </div>

            <div class="column has-text-centered">
            <div class="publication-links">
                <!-- PDF Link. -->
                <span class="link-block">
                <a
                    href="/assets/pdf/sore.pdf"
                    class="external-link button is-normal is-rounded is-dark"
                    target="_blank"
                >
                    <span class="icon">
                    <i class="fas fa-file-pdf"></i>
                    </span>
                    <span>Paper</span>
                </a>
                </span>
            </div>
            </div>
        </div>
        </div>
    </div>
    </div>

</section>

<section class="section">
    <div class="is-max-desktop">
    <!-- Abstract. -->
    <div class="columns is-centered has-text-centered">
        <div class="column is-four-fifths">
        <h2 class="title is-3">Abstract</h2>
        <div class="content has-text-justified">
            <p>
            Modern text processing pipelines demand robust methods to remove extraneous content while preserving a document's core message. Traditional approaches—such as HTML boilerplate extraction or keyword filters—often fail in multilingual settings and struggle with context-sensitive nuances, whereas Large Language Models (LLMs) offer improved quality at high computational cost. We introduce SORE (Semantic Outlier Removal), a cost-effective, transparent method that leverages multilingual sentence embeddings and approximate nearest-neighbor search to identify and excise unwanted text segments. By first identifying core content via metadata embedding and then flagging segments that either closely match predefined outlier groups or deviate significantly from the core, SORE achieves near-LLM extraction precision at a fraction of the cost. Experiments on HTML datasets demonstrate that SORE outperforms structural methods and yield high precision in diverse scenarios. Our system is currently deployed in production, processing millions of documents daily across multiple languages while maintaining both efficiency and accuracy. To facilitate reproducibility and further research, we release our implementation and evaluation datasets.
            </p>
        </div>
        </div>
    </div>
    </div>
</section>

<div class="columns is-centered has-text-centered">
    <div class="column is-four-fifths">
    <div class="diagram">
        {% include figure.liquid loading="eager" path="assets/img/sore.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
    </div>
</div>

<section class="section" id="BibTeX">
    <div class="is-max-desktop content">
    <h2 class="title">BibTeX</h2>
    <pre><code>@inproceedings{akbiyik2025semantic,
  title={Semantic Outlier Removal with Embedding Models and {LLM}s},
  author={Eren Akbiyik and Jo{\~a}o Almeida and Rik Melis and Ritu Sriram and Viviana Petrescu and Vilhj{\'a}lmur Vilhj{\'a}lmsson},
  booktitle={ACL 2025 Industry Track},
  year={2025}
}</code></pre>
    </div>
</section>
