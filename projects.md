---
layout: default
title: Projects
---
<style>
/* Projects grid styling */
.projects-container {
  margin-top: 20px;
}
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 30px;
  margin-top: 30px;
}
.project-card {
  background: #fff;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  text-decoration: none;
  color: inherit;
}
.project-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
  text-decoration: none;
  color: inherit;
}
.project-image-container {
  width: 100%;
  height: 200px;
  background: #f8f9fa;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  overflow: hidden;
  padding: 10px;
}
.project-image {
  max-width: 100%;
  max-height: 100%;
  object-fit: contain;
  display: block;
}
.project-content {
  padding: 20px;
}
.project-title {
  font-size: 1.3em;
  font-weight: 600;
  margin: 0 0 10px 0;
  color: #2c3e50;
}
.project-date {
  font-size: 0.9em;
  color: #7f8c8d;
  margin-bottom: 15px;
}
.project-excerpt {
  font-size: 0.95em;
  line-height: 1.5;
  color: #34495e;
  margin: 0;
}
.projects-intro {
  font-size: 1.3em;
  line-height: 1.6;
  color: #2c3e50;
  margin-bottom: 40px;
  margin-top: 30px;
  font-weight: 500;
  text-align: center;
  padding: 0 20px;
}
/* Mobile responsiveness */
@media (max-width: 768px) {
  .projects-grid {
    grid-template-columns: 1fr;
    gap: 20px;
  }
  
  .project-image-container {
    height: 150px;
  }
  
  .project-content {
    padding: 15px;
  }
  
  .project-title {
    font-size: 1.2em;
  }
}
</style>
<div class="projects-container">
  <p class="projects-intro">A selection of my creative projects.</p>
  
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
