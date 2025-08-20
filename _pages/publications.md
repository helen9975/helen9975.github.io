---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

## Research Publications

My research focuses on **perception, representation, and planning for robot manipulation**. I work at the intersection of computer vision, machine learning, and robotics to develop systems that can better understand and interact with their environment.

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

<style>
.publications-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 2rem;
  margin: 2rem 0;
}

.publication-card {
  background: white;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  overflow: hidden;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  border: 1px solid #e1e5e9;
}

.publication-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 25px rgba(0,0,0,0.15);
}

.publication-thumbnail {
  width: 100%;
  height: 200px;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  font-size: 3rem;
  font-weight: bold;
  position: relative;
}

.publication-thumbnail::before {
  content: attr(data-initial);
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.publication-content {
  padding: 1.5rem;
}

.publication-title {
  font-size: 1.1rem;
  font-weight: 600;
  color: #2c3e50;
  margin-bottom: 0.5rem;
  line-height: 1.4;
}

.publication-authors {
  font-size: 0.9rem;
  color: #7f8c8d;
  margin-bottom: 0.5rem;
  line-height: 1.3;
}

.publication-venue {
  font-size: 0.85rem;
  color: #e74c3c;
  font-weight: 500;
  margin-bottom: 0.75rem;
}

.publication-excerpt {
  font-size: 0.9rem;
  color: #555;
  line-height: 1.5;
  margin-bottom: 1rem;
}

.publication-links {
  display: flex;
  gap: 0.75rem;
  flex-wrap: wrap;
}

.publication-link {
  display: inline-flex;
  align-items: center;
  gap: 0.25rem;
  padding: 0.4rem 0.8rem;
  background: #f8f9fa;
  border: 1px solid #e9ecef;
  border-radius: 6px;
  text-decoration: none;
  color: #495057;
  font-size: 0.8rem;
  font-weight: 500;
  transition: all 0.2s ease;
}

.publication-link:hover {
  background: #e9ecef;
  color: #212529;
  text-decoration: none;
}

.publication-link.primary {
  background: #667eea;
  color: white;
  border-color: #667eea;
}

.publication-link.primary:hover {
  background: #5a6fd8;
  color: white;
}

.publication-link.secondary {
  background: #28a745;
  color: white;
  border-color: #28a745;
}

.publication-link.secondary:hover {
  background: #218838;
  color: white;
}

.publication-link.tertiary {
  background: #ffc107;
  color: #212529;
  border-color: #ffc107;
}

.publication-link.tertiary:hover {
  background: #e0a800;
  color: #212529;
}

.stats-section {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 2rem;
  border-radius: 12px;
  margin: 2rem 0;
  text-align: center;
}

.stats-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 1.5rem;
  margin-top: 1.5rem;
}

.stat-item {
  text-align: center;
}

.stat-number {
  font-size: 2.5rem;
  font-weight: bold;
  display: block;
}

.stat-label {
  font-size: 0.9rem;
  opacity: 0.9;
}

.research-areas {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  margin: 2rem 0;
}

.research-card {
  background: white;
  padding: 1.5rem;
  border-radius: 8px;
  border-left: 4px solid #667eea;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}

.research-card h4 {
  color: #2c3e50;
  margin-bottom: 0.5rem;
}

.research-card p {
  color: #7f8c8d;
  margin: 0;
  line-height: 1.5;
}
</style>

<div class="stats-section">
  <h3>Publication Statistics</h3>
  <div class="stats-grid">
    <div class="stat-item">
      <span class="stat-number">12</span>
      <span class="stat-label">Total Publications</span>
    </div>
    <div class="stat-item">
      <span class="stat-number">5</span>
      <span class="stat-label">Conference Papers</span>
    </div>
    <div class="stat-item">
      <span class="stat-number">3</span>
      <span class="stat-label">Oral Presentations</span>
    </div>
    <div class="stat-item">
      <span class="stat-number">4</span>
      <span class="stat-label">In Submission</span>
    </div>
  </div>
</div>

<div class="publications-grid">
{% for post in site.publications reversed %}
  <div class="publication-card">
    <div class="publication-thumbnail" data-initial="{{ post.title | slice: 0, 1 }}">
    </div>
    <div class="publication-content">
      <h3 class="publication-title">{{ post.title }}</h3>
      <div class="publication-authors">{{ post.citation | split: '.' | first }}</div>
      <div class="publication-venue">{{ post.venue }}</div>
      <div class="publication-excerpt">{{ post.excerpt }}</div>
      <div class="publication-links">
        {% if post.paperurl %}
        <a href="{{ post.paperurl }}" class="publication-link primary" target="_blank">
          📄 Paper
        </a>
        {% endif %}
        {% if post.website %}
        <a href="{{ post.website }}" class="publication-link secondary" target="_blank">
          🌐 Website
        </a>
        {% endif %}
        {% if post.code %}
        <a href="{{ post.code }}" class="publication-link tertiary" target="_blank">
          💻 Code
        </a>
        {% endif %}
      </div>
    </div>
  </div>
{% endfor %}
</div>

## Research Areas

<div class="research-areas">
  <div class="research-card">
    <h4>🤖 Robot Manipulation</h4>
    <p>Developing algorithms for precise and robust robotic manipulation tasks</p>
  </div>
  <div class="research-card">
    <h4>👁️ Computer Vision</h4>
    <p>Novel approaches for visual perception and scene understanding</p>
  </div>
  <div class="research-card">
    <h4>🧠 Representation Learning</h4>
    <p>Learning effective representations for robotic tasks</p>
  </div>
  <div class="research-card">
    <h4>📊 Machine Learning</h4>
    <p>Applying deep learning and reinforcement learning to robotics</p>
  </div>
  <div class="research-card">
    <h4>🎯 Motion Planning</h4>
    <p>Algorithms for safe and efficient robot motion</p>
  </div>
</div>
