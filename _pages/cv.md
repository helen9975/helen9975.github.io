---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<style>
.cv-container {
  width: 100%;
  height: 80vh;
  border: 1px solid #e1e5e9;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}

.cv-pdf {
  width: 100%;
  height: 100%;
  border: none;
}

.cv-download {
  margin-top: 1rem;
  text-align: center;
}

.cv-download a {
  display: inline-block;
  padding: 0.75rem 1.5rem;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  text-decoration: none;
  border-radius: 6px;
  font-weight: 500;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.cv-download a:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(102, 126, 234, 0.4);
  text-decoration: none;
  color: white;
}

.cv-download i {
  margin-right: 0.5rem;
}
</style>

<div class="cv-container">
  <iframe 
    src="/files/YiRuWang_CV-1.pdf" 
    class="cv-pdf"
    title="Yi Ru Wang CV"
    allowfullscreen>
  </iframe>
</div>

<div class="cv-download">
  <a href="/files/YiRuWang_CV-1.pdf" target="_blank">
    <i class="fa fa-download"></i>
    Download CV (PDF)
  </a>
</div>
