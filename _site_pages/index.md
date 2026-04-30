---
layout: home
title: About
description: "About Gaeun Ji, M.S. student in Computer Science at Kyung Hee University."
permalink: /
---

<div class="container">
  <section id="news">
    <div class="section-title">News</div>
    <ul class="news-list">
      <li class="news-item">
        <span class="news-date">2026</span>
        <span class="news-content">Started M.S. research focused on robustness and reliability in language models.</span>
        <span class="news-tag career">Research</span>
      </li>
      <li class="news-item">
        <span class="news-date">2025</span>
        <span class="news-content">Participated in team projects on practical machine learning and data-driven problem solving.</span>
        <span class="news-tag award">Project</span>
      </li>
    </ul>
    <div style="margin-top:12px;">
      <button class="more-news-btn" id="moreNewsBtn" onclick="toggleMoreNews()">
        <span class="more-news-arrow">▸</span> More News
      </button>
      <div class="more-news-body" id="moreNewsBody">
        <ul class="news-list" style="margin-top:4px;">
          <li class="news-item">
            <span class="news-date">2001</span>
            <span class="news-content">Birth</span>
            <span class="news-tag paper">Event</span>
          </li>
        </ul>
      </div>
    </div>
  </section>

  <section id="research">
    <div class="section-title">Research</div>
    <div class="honor-list">
      <div class="honor-entry">
        <div>
          <div class="honor-title">Trustworthy AI</div>
          <div class="honor-sub">Reliability, uncertainty estimation, and evaluation methodology for real-world usage.</div>
        </div>
        <div class="honor-date">Current</div>
      </div>
      <div class="honor-entry">
        <div>
          <div class="honor-title">LLM Safety</div>
          <div class="honor-sub">Prompt-risk analysis, safety behaviors, and robust testing protocols.</div>
        </div>
        <div class="honor-date">Current</div>
      </div>
      <div class="honor-entry">
        <div>
          <div class="honor-title">Multi-Modal AI</div>
          <div class="honor-sub">Text-image reasoning reliability and consistency checks.</div>
        </div>
        <div class="honor-date">Current</div>
      </div>
    </div>

    <div class="section-title section-title--sub">Publications</div>
    <div class="pub-list">
      <div class="pub-entry">
        <img class="pub-thumb" src="https://placehold.co/120x72" alt="publication template">
        <div class="pub-body">
          <div class="pub-title">[PLACEHOLDER: Paper Title]</div>
          <div class="pub-authors">[PLACEHOLDER: Authors]</div>
          <div class="pub-meta">
            <span class="venue-badge preprint">[PLACEHOLDER: Venue / Status]</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="projects">
    <div class="section-title">Projects</div>
    <div class="projects-grid">
      {% assign sorted_projects = site.projects | sort: "date" | reverse %}
      {% for project in sorted_projects %}
        <div class="project-card">
          <div class="project-header">
            <div class="project-title">{{ project.title }}</div>
            <span class="project-org">{{ project.status }}</span>
          </div>
          <div class="project-subtitle">{{ project.date | date: "%Y-%m" }}</div>
          <ul class="project-bullets">
            <li>{{ project.summary }}</li>
          </ul>
        </div>
      {% endfor %}
    </div>
  </section>

  <section>
    <div class="section-title">Education</div>
    <div class="edu-list">
      <div class="edu-entry">
        <div class="edu-school">Kyung Hee University</div>
        <div class="edu-degree">M.S. in Computer Science</div>
        <div class="edu-meta"> 2026.03 – Present</div>
      </div>  
      <div class="edu-entry">
        <div class="edu-school">Kyung Hee University</div>
        <div class="edu-degree">B.S. in Economics and Computer Science </div>
        <div class="edu-meta"> 2020.03 – 2026.02 </div>
      </div>
    </div>
  </section>

  <section>
    <div class="section-title">Honors &amp; Awards</div>
    <div class="honor-list">
      <div class="honor-entry">
        <div>
          <div class="honor-title">Academic Excellence Award</div>
          <div class="honor-sub">Awarded by Kyung Hee University for top academic performance</div>
        </div>
        <div class="honor-date">Nov. 2022</div>
      </div>

    </div>

  </section>
</div>
