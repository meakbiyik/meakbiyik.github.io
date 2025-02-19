---
layout: page
permalink: /routeformer/
title: Leveraging Driver Field-of-View for Multimodal Ego-Trajectory Prediction
nav: false
---

<section class="hero">
    <div class="hero-body">
    <div class="is-max-desktop">
        <div class="columns is-centered">
        <div class="column has-text-centered">
            <div class="is-size-5 publication-authors">
            <span class="author-block">
                <a href="https://github.com/meakbiyik">M. Eren Akbiyik</a
                ><sup>1</sup>,</span
            >
            <span class="author-block">
                <a>Nedko Savov</a><sup>2</sup>,</span
            >
            <span class="author-block">
                <a>Danda Pani Paudel</a><sup>1,2</sup>,</span
            >
            <span class="author-block">
                <a>Nikola Popovic</a><sup>1,2</sup>,</span
            >
            <span class="author-block">
                <a>Christian Vater</a><sup>1</sup>,</span
            >
            <span class="author-block">
                <a href="https://ait.ethz.ch/people/hilliges"
                >Otmar Hilliges</a
                ><sup>1</sup>,</span
            >
            <span class="author-block">
                <a
                href="https://ee.ethz.ch/the-department/faculty/professors/person-detail.OTAyMzM=.TGlzdC80MTEsMTA1ODA0MjU5.html/"
                >Luc Van Gool</a
                ><sup>1,2</sup>,</span
            >
            <span class="author-block">
                <a href="https://ait.ethz.ch/people/xiwang">Xi Wang</a
                ><sup>1</sup>
            </span>
            </div>

            <div class="is-size-5 publication-authors">
            <span class="author-block"
                ><sup>1</sup>ETH Zurich, Switzerland</span
            >
            <br />
            <span class="author-block"
                ><sup>2</sup>INSAIT, Sofia University</span
            >
            <br />
            <span class="author-block"> <b>ICLR 2025</b></span>
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
