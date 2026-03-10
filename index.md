---
Welcome to Q CONS! Click on any section below to learn more about me and what I offer to support your business growth.

<div class="section-grid">

  <div class="section-card" onclick="toggleSection('about')">
    <div class="card-icon">👤</div>
    <h3>About Me</h3>
    <p class="preview-text">Who I am and what I do</p>
  </div>

  <div class="section-card" onclick="toggleSection('cv')">
    <div class="card-icon">📄</div>
    <h3>My CV</h3>
    <p class="preview-text">Experience & qualifications</p>
  </div>

  <div class="section-card" onclick="toggleSection('services')">
    <div class="card-icon">⚡</div>
    <h3>My Services</h3>
    <p class="preview-text">How I can help you</p>
  </div>

  <div class="section-card" onclick="toggleSection('contact')">
    <div class="card-icon">📫</div>
    <h3>My Contacts</h3>
    <p class="preview-text">Get in touch with me</p>
  </div>

</div>

<!-- About Me Expanded Section -->
<div id="about" class="expanded-content">
  <button class="close-btn" onclick="toggleSection('about')">×</button>
  <h2>👤 About Me</h2>
  
  <div class="content-grid">
    <div class="info-card">
      <h4>📌 Background</h4>
      <p>I'm a [your profession] based in [your location] with [X] years of experience.</p>
    </div>
    
    <div class="info-card">
      <h4>🎯 Interests</h4>
      <ul>
        <li>Interest 1</li>
        <li>Interest 2</li>
        <li>Interest 3</li>
      </ul>
    </div>
    
    <div class="info-card">
      <h4>🎓 Education</h4>
      <p><strong>Degree</strong> - University (Year)</p>
      <p><strong>Certification</strong> - Institution (Year)</p>
    </div>
  </div>
</div>

<!-- My CV Expanded Section -->
<div id="cv" class="expanded-content">
  <button class="close-btn" onclick="toggleSection('cv')">×</button>
  <h2>📄 My CV</h2>
  
  <div class="content-grid">
    <div class="info-card">
      <h4>💼 Work Experience</h4>
      <div class="timeline-item">
        <div class="timeline-date">2022 - Present</div>
        <strong>Job Title</strong> at Company
        <p>• Responsibility 1<br>• Responsibility 2</p>
      </div>
      
      <div class="timeline-item">
        <div class="timeline-date">2020 - 2022</div>
        <strong>Previous Job</strong> at Previous Company
        <p>• Responsibility 1<br>• Responsibility 2</p>
      </div>
    </div>
    
    <div class="info-card">
      <h4>🔧 Skills</h4>
      <div class="skills-tags">
        <span class="skill-tag">Skill 1</span>
        <span class="skill-tag">Skill 2</span>
        <span class="skill-tag">Skill 3</span>
        <span class="skill-tag">Skill 4</span>
      </div>
      
      <div class="skills-tags">
        <span class="skill-tag">English (Fluent)</span>
        <span class="skill-tag">Spanish (Intermediate)</span>
      </div>
    </div>
  </div>
</div>

<!-- My Services Expanded Section -->
<div id="services" class="expanded-content">
  <button class="close-btn" onclick="toggleSection('services')">×</button>
  <h2>⚡ My Services</h2>
  
  <div class="content-grid">
    <div class="service-card">
      <div style="font-size: 2.5em;">💻</div>
      <h3>Service 1</h3>
      <p>Description of service 1</p>
      <div class="price-tag">$XXX</div>
    </div>
    
    <div class="service-card">
      <div style="font-size: 2.5em;">🎨</div>
      <h3>Service 2</h3>
      <p>Description of service 2</p>
      <div class="price-tag">$XXX</div>
    </div>
    
    <div class="service-card">
      <div style="font-size: 2.5em;">📊</div>
      <h3>Service 3</h3>
      <p>Description of service 3</p>
      <div class="price-tag">$XXX</div>
    </div>
  </div>
</div>

<!-- My Contacts Expanded Section -->
<div id="contact" class="expanded-content">
  <button class="close-btn" onclick="toggleSection('contact')">×</button>
  <h2>📫 My Contacts</h2>
  
  <div class="content-grid">
    <div class="info-card">
      <h4>📧 Email</h4>
      <div class="contact-item">
        <span class="contact-icon">📧</span>
        <a href="mailto:your.email@example.com">your.email@example.com</a>
      </div>
      
      <h4>📱 Phone</h4>
      <div class="contact-item">
        <span class="contact-icon">📱</span>
        <a href="tel:+1234567890">+1 (234) 567-890</a>
      </div>
      
      <h4>📍 Location</h4>
      <div class="contact-item">
        <span class="contact-icon">📍</span>
        <span>City, Country</span>
      </div>
    </div>
    
    <div class="info-card">
      <h4>🌐 Social Media</h4>
      <div class="social-links">
        <a href="#" class="social-link">LinkedIn</a>
        <a href="#" class="social-link">Twitter</a>
        <a href="#" class="social-link">GitHub</a>
      </div>
    </div>
  </div>
</div>

<!-- JavaScript for Toggle Function -->
<script>
function toggleSection(sectionId) {
  const section = document.getElementById(sectionId);
  const allSections = document.querySelectorAll('.expanded-content');
  
  // Close all other sections
  allSections.forEach(s => {
    if (s.id !== sectionId) {
      s.classList.remove('active');
    }
  });
  
  // Toggle the clicked section
  section.classList.toggle('active');
  
  // Scroll to section if opened
  if (section.classList.contains('active')) {
    setTimeout(() => {
      section.scrollIntoView({ behavior: 'smooth', block: 'start' });
    }, 100);
  }
}

// Click outside to close (optional)
document.addEventListener('click', function(event) {
  if (!event.target.closest('.section-card') && 
      !event.target.closest('.expanded-content') && 
      !event.target.closest('.close-btn')) {
    document.querySelectorAll('.expanded-content').forEach(s => {
      s.classList.remove('active');
    });
  }
});
</script>

---

*Last updated: March 2026*
