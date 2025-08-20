---
permalink: /
title: "About Me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
/* Hero Section */
.hero-section {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  color: white;
  padding: 4rem 0;
  text-align: center;
  margin: -2rem -2rem 3rem -2rem;
  position: relative;
  overflow: hidden;
}

.hero-section::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><defs><pattern id="grain" width="100" height="100" patternUnits="userSpaceOnUse"><circle cx="25" cy="25" r="1" fill="rgba(255,255,255,0.1)"/><circle cx="75" cy="75" r="1" fill="rgba(255,255,255,0.1)"/><circle cx="50" cy="10" r="0.5" fill="rgba(255,255,255,0.1)"/></pattern></defs><rect width="100" height="100" fill="url(%23grain)"/></svg>');
  opacity: 0.3;
}

.hero-content {
  position: relative;
  z-index: 2;
}

.hero-avatar {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  border: 4px solid rgba(255,255,255,0.3);
  margin: 0 auto 2rem;
  display: block;
  box-shadow: 0 8px 32px rgba(0,0,0,0.2);
}

.hero-title {
  font-size: 3rem;
  font-weight: 700;
  margin-bottom: 1rem;
  text-shadow: 0 2px 4px rgba(0,0,0,0.3);
}

.hero-subtitle {
  font-size: 1.3rem;
  margin-bottom: 1.5rem;
  opacity: 0.95;
  font-weight: 300;
}

.hero-description {
  font-size: 1.1rem;
  max-width: 600px;
  margin: 0 auto;
  line-height: 1.6;
  opacity: 0.9;
}

/* Research Focus Section */
.research-focus {
  background: white;
  padding: 3rem 2rem;
  border-radius: 16px;
  box-shadow: 0 4px 20px rgba(0,0,0,0.08);
  margin: 2rem 0;
  text-align: center;
}

.research-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
  margin: 2rem 0;
}

.research-card {
  background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
  padding: 2rem 1.5rem;
  border-radius: 12px;
  border-left: 4px solid #667eea;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.research-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 25px rgba(0,0,0,0.15);
}

.research-card h3 {
  color: #2c3e50;
  margin-bottom: 1rem;
  font-size: 1.3rem;
}

.research-card p {
  color: #6c757d;
  line-height: 1.6;
  margin: 0;
}

/* Main Content */
.main-content {
  background: white;
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.05);
  margin: 2rem 0;
}

.content-section {
  margin-bottom: 2.5rem;
}

.content-section h2 {
  color: #2c3e50;
  border-bottom: 3px solid #667eea;
  padding-bottom: 0.5rem;
  margin-bottom: 1.5rem;
  font-size: 1.8rem;
}

.content-section p {
  line-height: 1.7;
  color: #555;
  margin-bottom: 1rem;
}

/* Awards Section */
.awards-section {
  background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
  padding: 2rem;
  border-radius: 12px;
  margin: 2rem 0;
}

.awards-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1.5rem;
  margin-top: 1.5rem;
}

.award-item {
  background: white;
  padding: 1.5rem;
  border-radius: 8px;
  border-left: 4px solid #28a745;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}

.award-item h4 {
  color: #2c3e50;
  margin-bottom: 0.5rem;
}

.award-item p {
  color: #6c757d;
  margin: 0;
  font-size: 0.9rem;
}

/* News Section */
.news-section {
  background: white;
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.05);
  margin: 2rem 0;
}

.news-item {
  padding: 1rem 0;
  border-bottom: 1px solid #e9ecef;
  transition: background-color 0.2s ease;
}

.news-item:last-child {
  border-bottom: none;
}

.news-item:hover {
  background-color: #f8f9fa;
  margin: 0 -1rem;
  padding: 1rem;
  border-radius: 8px;
}

.news-date {
  color: #667eea;
  font-weight: 600;
  font-size: 0.9rem;
  margin-bottom: 0.5rem;
}

.news-content {
  color: #2c3e50;
  line-height: 1.6;
}

.news-content a {
  color: #667eea;
  text-decoration: none;
  font-weight: 500;
}

.news-content a:hover {
  text-decoration: underline;
}

/* Responsive Design */
@media (max-width: 768px) {
  .hero-section {
    padding: 3rem 1rem;
    margin: -1rem -1rem 2rem -1rem;
  }
  
  .hero-title {
    font-size: 2.5rem;
  }
  
  .hero-subtitle {
    font-size: 1.1rem;
  }
  
  .research-grid {
    grid-template-columns: 1fr;
  }
  
  .main-content, .awards-section, .news-section {
    padding: 1.5rem;
  }
}
</style>

<!-- Hero Section -->
<div class="hero-section">
  <div class="hero-content">
    <img src="{{ site.url }}{{ site.baseurl }}/images/profile.jpg" alt="Helen Wang" class="hero-avatar">
    <h1 class="hero-title">Yi Ru (Helen) Wang</h1>
    <p class="hero-subtitle">Ph.D. Student in Computer Science</p>
    <p class="hero-description">University of Washington Paul G. Allen School of Computer Science and Engineering</p>
  </div>
</div>

<!-- Research Focus Section -->
<div class="research-focus">
  <h2>Research Focus</h2>
  <p style="font-size: 1.1rem; color: #6c757d; margin-bottom: 2rem;">
    My work focuses on developing comprehensive frameworks and methodologies to assess, understand, and enhance robotic manipulation capabilities.
  </p>
  <div class="research-grid">
    <div class="research-card">
      <h3>🤖 Evaluation</h3>
      <p>Developing frameworks to assess robotic manipulation systems more effectively and comprehensively</p>
    </div>
    <div class="research-card">
      <h3>🧠 Representation</h3>
      <p>Learning better representations for manipulation tasks and robotic understanding</p>
    </div>
    <div class="research-card">
      <h3>💭 Reasoning</h3>
      <p>Enabling robots to reason about their actions, failures, and decision-making processes</p>
    </div>
  </div>
</div>

<!-- Main Content -->
<div class="main-content">
  <div class="content-section">
    <h2>About Me</h2>
    <p>I am a Ph.D. student in the **Paul G. Allen School of Computer Science and Engineering at the University of Washington**, advised by Professor [Siddhartha Srinivasa](https://goodrobot.ai) ([Personal Robotics Lab](https://personalrobotics.cs.washington.edu/)) and Professor [Dieter Fox](https://homes.cs.washington.edu/~fox/) ([Robotics and State Estimation Lab](https://rse-lab.cs.washington.edu/people/)).</p>
    
    <p>Before my Ph.D., I completed my Bachelor of Applied Science in [Engineering Science](https://engsci.utoronto.ca/program/what-is-engsci/) with a specialization in Robotics and a minor in AI at the University of Toronto. There, I conducted research on Learning-based Perception for Transparent Objects, advised by [Prof. Animesh Garg](https://animesh.garg.tech/) ([People AI and Robotics Lab](https://www.pair.toronto.edu)) and [Prof. Florian Shkurti](http://www.cs.toronto.edu/~florian/) ([Robot Vision and Learning Lab](https://rvl.cs.toronto.edu/#/)).</p>
    
    <p>Apart from my academic pursuits, I have worked as a research intern at Huawei Technologies R&D Canada, computer vision intern at EATLAB, and undergraduate research assistant at the National University of Singapore.</p>
  </div>

  <div class="content-section">
    <h2>Fellowship & Awards</h2>
    <p>I have been honored to receive several prestigious awards and fellowships:</p>
    <ul>
      <li><strong>[CRA Outstanding Undergraduate Research Award](https://cra.org/about/awards/outstanding-undergraduate-researcher-award/#2022)</strong> - Honourable Mention (2022)</li>
      <li><strong>[National Undergraduate Research Award (NSERC USRA)](https://www.nserc-crsng.gc.ca/students-etudiants/ug-pc/usra-brpc_eng.asp)</strong> (2021, 2022)</li>
      <li><strong>[NSERC Postgraduate Scholarships-Doctoral Program](https://www.nserc-crsng.gc.ca/Students-Etudiants/PG-CS/cgrsd-besrd_eng.asp)</strong> - Currently supported by this prestigious fellowship</li>
    </ul>
  </div>

  <div class="content-section">
    <h2>Collaboration & Opportunities</h2>
    <p>I have had the privilege to work with some amazing collaborators, and am always looking for motivated students and new collaborations. Drop me an email if you are interested!</p>
  </div>
</div>

<!-- Recent News Section -->
<div class="news-section">
  <h2>Recent News</h2>
  
  <div class="news-item">
    <div class="news-date">January 2025</div>
    <div class="news-content">Our work [AHA](https://aha-vlm.github.io), a VLM for failure detection and reasoning in robot manipulation, has been accepted to ICLR.</div>
  </div>
  
  <div class="news-item">
    <div class="news-date">September 2024</div>
    <div class="news-content">Our work [Manipulate-Anything](https://robot-ma.github.io), a method for automated data-collection and verification for robotic manipulation has been accepted to CoRL.</div>
  </div>
  
  <div class="news-item">
    <div class="news-date">January 2024</div>
    <div class="news-content">Started my internship at [Nvidia Seattle Robotics Lab](https://research.nvidia.com/labs/srl/).</div>
  </div>
  
  <div class="news-item">
    <div class="news-date">January 2024</div>
    <div class="news-content">Started my 2-year term as the Chair of the [Student Activities Committee](https://www.ieee-ras.org/about-ras/governance/member-activities-board/student-activities-committee) for the Robotics and Automation Society (RAS).</div>
  </div>
  
  <div class="news-item">
    <div class="news-date">October 2023</div>
    <div class="news-content">Our work, [NEWTON](https://arxiv.org/abs/2310.07018), a dataset and benchmark to evaluate LLMs' physical reasoning capabilities, accepted at EMNLP 2023, see you in Singapore!</div>
  </div>
  
  <div class="news-item">
    <div class="news-date">September 2023</div>
    <div class="news-content">Our work, [AR2D2](https://arxiv.org/abs/2306.13818), a AR-based method for collecting robot demonstrations, accepted at CoRL 2023, see you in Atlanta!</div>
  </div>
  
  <div class="news-item">
    <div class="news-date">April 2023</div>
    <div class="news-content">Awarded the [NSERC PGSD Fellowship](https://www.nserc-crsng.gc.ca/students-etudiants/pg-cs/bellandpostgrad-belletsuperieures_eng.asp) for my Graduate Studies</div>
  </div>
  
  <div class="news-item">
    <div class="news-date">March 2023</div>
    <div class="news-content">Our work, [MVTrans](https://arxiv.org/abs/2302.11683), a novel multi-task perception framework & photorealistic dataset, accepted at ICRA 2023</div>
  </div>
  
  <div class="news-item">
    <div class="news-date">September 2021</div>
    <div class="news-content">Our work, [TranspareNet](https://arxiv.org/abs/2110.00087), a encoder-decoder based depth estimation method and real-world data-collection and annotation pipeline, accepted at CoRL 2021 for Oral Presentation</div>
  </div>
</div>



