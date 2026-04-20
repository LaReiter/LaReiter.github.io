---
layout: default
title: Projects
---
<style>
.projects-container {
  margin-top: 20px;
}
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 24px;
  margin-top: 24px;
}
.project-card {
  background: rgba(13, 17, 23, 0.8);
  border: 1px solid rgba(56, 189, 248, 0.12);
  border-radius: 10px;
  overflow: hidden;
  transition: transform 0.25s ease, box-shadow 0.25s ease, border-color 0.25s ease;
  text-decoration: none;
  color: inherit;
}
.project-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 32px rgba(56, 189, 248, 0.12);
  border-color: rgba(56, 189, 248, 0.35);
  text-decoration: none;
  color: inherit;
}
.project-image-container {
  width: 100%;
  height: 190px;
  background: rgba(7, 9, 15, 0.9);
  display: flex;
  align-items: center;
  justify-content: flex-start;
  overflow: hidden;
  padding: 12px;
  border-bottom: 1px solid rgba(56, 189, 248, 0.08);
}
.project-image {
  max-width: 100%;
  max-height: 100%;
  object-fit: contain;
  display: block;
}
.project-content {
  padding: 18px 20px;
}
.project-title {
  font-size: 1.1em;
  font-weight: 600;
  margin: 0 0 8px 0;
  color: #f1f5f9;
  letter-spacing: -0.01em;
}
.project-date {
  font-size: 0.74em;
  font-family: "JetBrains Mono", "Fira Code", monospace;
  color: rgba(56, 189, 248, 0.78);
  margin-bottom: 12px;
  letter-spacing: 0.04em;
}
.project-excerpt {
  font-size: 0.9em;
  line-height: 1.6;
  color: rgba(196, 212, 224, 0.85);
  margin: 0;
}
.projects-intro {
  font-size: 1.05em;
  line-height: 1.65;
  color: rgba(196, 212, 224, 0.8);
  margin-bottom: 32px;
  margin-top: 24px;
  text-align: center;
  padding: 0 20px;
}
.projects-intro a {
  color: #38bdf8;
  text-decoration: none;
  border-bottom: 1px solid rgba(56, 189, 248, 0.3);
  transition: border-color .15s;
}
.projects-intro a:hover {
  border-bottom-color: #38bdf8;
}
@media (max-width: 768px) {
  .projects-grid {
    grid-template-columns: 1fr;
    gap: 16px;
  }
  .project-image-container {
    height: 150px;
  }
  .project-content {
    padding: 14px 16px;
  }
}
</style>
<div class="projects-container">
 <p class="projects-intro">Selected creative projects. A full list can be <a href="https://docs.google.com/document/d/1HXOMjqJpiRDGu4M3EIVrFs6nKMEAouZK_JijJE5TLFg/edit?usp=sharing"> found here.</a></p>
  
  <div class="projects-grid">
    {% for project in site.projects %}
      <a href="{{ project.url }}" class="project-card">
        <div class="project-image-container">
          <img src="{{ project.image }}" alt="{{ project.title }}" class="project-image">
        </div>
        <div class="project-content">
          <h3 class="project-title">{{ project.title }}</h3>
          <p class="project-date">{{ project.date | date: "%B %d, %Y" }}</p>
          <p class="project-excerpt">{{ project.excerpt }}</p>
        </div>
      </a>
    {% endfor %}
  </div>
</div>
