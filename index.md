---
layout: default
title: Kyungmin Kang | Data Scientist & Economist
---

<!-- Hero Section -->
<section class="hero">
  <div class="hero-wrapper">
    <div class="hero-left">
      <img src="/assets/img/headshot.jpg" alt="KM Kang Headshot">
    </div>
    <div class="hero-right">
      <h1>Kyungmin Kang</h1>
      <h2>Economist & Data Scientist</h2>
      <p>Ph.D. in Economics, Johns Hopkins University</p>
     <a href="mailto:kyungmin.kang@outlook.com"><i class="fas fa-envelope"></i> kyungmin.kang@outlook.com</a>

      <ul class="hero-skills">
        <li>Causal Inference & Machine Learning</li>
        <li>Dynamic Modeling & Structural Estimation</li>
        <li>LangChain · HuggingFace · D3.js · SQL · Python</li>
        <li>10+ Years Data-Driven Research & 5+ Years Teaching</li>
      </ul>
      <div class="hero-buttons">
        <a href="/resume.pdf" class="resume-btn">Resume</a>
        <!-- <a href="#contact" class="btn secondary">Contact Me</a> -->
      </div>
    </div>
  </div>
</section>




<!-- About Section -->
<section class="about" id="about">
  <h3>About Me</h3>
<p>
Hi. I’m <strong>Kyungmin Kang</strong>, a Ph.D. economist with 10+ years of experience bridging economic theory and statistical modeling with data to drive real-world impact. I specialize in causal inference, machine learning, and dynamic decision models—building tools that support product, policy, and research decisions across domains.
</p>

<p>
On the industry-facing side, I’m currently developing an AI-powered investment recommendation system that interprets SEC filings using LangChain, HuggingFace Transformers, SQL, and D3.js. It is aimed at providing insights to novice and professional users through chat and dashboard interfaces. Earlier, I worked at a startup where I collaborated cross-functionally with engineers and UI/UX designers to prioritize features and streamline product design for a consumer-facing app.
</p>

<p>
My academic research focuses on causal evaluations of federal policies and dynamic modeling of teacher effectiveness in education. This work has been published in journals such as the <em>Review of Economics and Statistics</em> and the <em>Southern Economic Journal</em>, and has informed real-world human capital development. I’ve mentored undergraduate researchers—-many of whom were later admitted to Ph.D. programs at institutions like UCLA and Rochester—-and I’ve taught 90+ student classes while presenting findings to both academic and government stakeholders. I value clarity, rigor, and real-world relevance in every stage of the data lifecycle.
</p>
</section>

<!-- Latest Writing Section -->
<!-- <section class="recent-posts">
  <h3>Recent Writing</h3>
  <ul class="post-snippets">
    {% for post in site.posts limit:3 %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
        <p>{{ post.excerpt | strip_html | truncate: 140 }}</p>
        <p>{{ post.tags | strip_html | truncate: 100}}</p>
      </li>
    {% endfor %}
  </ul>
  <a href="/blog" class="btn">View All Posts</a>
</section> -->


<!-- Projects Section -->
<section class="projects" id="projects">
  <h3>Projects</h3>
  <div class="project-grid">
    <div class="project-card">
      <h4>Stock Price Visualizer</h4>
      <p>Interactive D3.js chart showing prices across timeframes.</p>
      <div class="tags"><span>D3.js</span><span>JavaScript</span><span>Finance</span></div>
      <a href="https://github.com/kyungmin-kang/stock-price-visualizer" class="btn project-link" target="_blank">View Project</a>
    </div>
    <div class="project-card private">
      <h4>InvestGPT</h4>
      <p>LLM-powered chatbot surfacing investment insights from SEC filings.</p>
      <div class="tags"><span>LangChain</span><span>PostgreSQL</span><span>Finance</span></div>
      <div class="private-label">Code private</div>
    </div>
    <div class="project-card private">
      <h4>RL vs Structural Modeling</h4>
      <p>Comparing reinforcement learning vs structural models in economic environments.</p>
      <div class="tags"><span>Python</span><span>RL</span><span>Dynamic Models</span></div>
      <div class="private-label">Code private</div>
    </div>
    <!-- <div class="project-card private">
      <h4>PronounceGPT</h4>
      <p>Personalized Chinese pronunciation tutor with scoring and feedback.</p>
      <div class="tags"><span>React</span><span>Edge AI</span><span>Docker</span></div>
      <div class="private-label">Code private</div>
    </div> -->
  </div>
</section>


<!-- Recent Writing Section -->
<section class="recent-posts" id="writing">
  <h3>Recent Writing</h3>
  <div class="writing-grid">
    {% for post in site.posts limit:3 %}
    <div class="writing-card">
      <h4><a href="{{ post.url }}">{{ post.title }}</a></h4>
      <p>{{ post.excerpt | strip_html | truncate: 100 }}</p>
      <div class="tags">
        {% for tag in post.tags %}
        <span>{{ tag }}</span>
        {% endfor %}
      </div>
    </div>
    {% endfor %}
  </div>  
  <div style="margin-top: 1rem; text-align: center;">
    <a href="/blog" class="btn">View All Writing</a>
  </div>
</section>

<!-- Contact Section -->
<!-- <section class="contact" id="contact">
  <h3>Contact</h3>
  <p>If you're working at the intersection of AI, economics, and data — I'd love to connect.</p>
  <p>Email: <a href="mailto:kyungmin.kang@outlook.com">kyungmin.kang@outlook.com</a></p>
  <div class="socials">
    <a href="https://github.com/kyungmin-kang">GitHub</a> |
    <a href="https://linkedin.com/in/kmkang">LinkedIn</a>
  </div>
</section> -->

<link rel="stylesheet" href="/assets/css/style.css">
