<svg width="100%" viewBox="0 0 1000 400" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid slice">
  <defs>
    <style>
      @keyframes twinkle {
        0%, 100% { opacity: 0.3; }
        50% { opacity: 1; }
      }
      @keyframes fadeInUp {
        0% { opacity: 0; transform: translateY(20px); }
        100% { opacity: 1; transform: translateY(0); }
      }
      @keyframes slideInLeft {
        0% { opacity: 0; transform: translateX(-30px); }
        100% { opacity: 1; transform: translateX(0); }
      }
      @keyframes glow {
        0%, 100% { filter: drop-shadow(0 0 5px rgba(0, 212, 255, 0.5)); }
        50% { filter: drop-shadow(0 0 20px rgba(124, 58, 237, 1)); }
      }
    </style>
    <linearGradient id="textGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#00d4ff;stop-opacity:1" />
      <stop offset="50%" style="stop-color:#7c3aed;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#ec4899;stop-opacity:1" />
    </linearGradient>
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#0a0e27;stop-opacity:1" />
      <stop offset="50%" style="stop-color:#1a1f3a;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#0f1629;stop-opacity:1" />
    </linearGradient>
  </defs>
  
  <!-- Dark background -->
  <rect width="1000" height="400" fill="url(#bgGrad)"/>
  
  <!-- Twinkling stars background -->
  <circle cx="50" cy="40" r="1.5" fill="white" opacity="0.4">
    <animate attributeName="opacity" from="0.3" to="1" dur="2.5s" repeatCount="indefinite" begin="0s"/>
  </circle>
  <circle cx="150" cy="60" r="1" fill="white" opacity="0.4">
    <animate attributeName="opacity" from="0.3" to="1" dur="2s" repeatCount="indefinite" begin="0.5s"/>
  </circle>
  <circle cx="300" cy="35" r="1.5" fill="white" opacity="0.4">
    <animate attributeName="opacity" from="0.3" to="1" dur="2.2s" repeatCount="indefinite" begin="1s"/>
  </circle>
  <circle cx="450" cy="50" r="1" fill="white" opacity="0.4">
    <animate attributeName="opacity" from="0.3" to="1" dur="2.8s" repeatCount="indefinite" begin="0.3s"/>
  </circle>
  <circle cx="600" cy="30" r="1.5" fill="white" opacity="0.4">
    <animate attributeName="opacity" from="0.3" to="1" dur="2.4s" repeatCount="indefinite" begin="0.8s"/>
  </circle>
  <circle cx="750" cy="55" r="1" fill="white" opacity="0.4">
    <animate attributeName="opacity" from="0.3" to="1" dur="2.6s" repeatCount="indefinite" begin="1.2s"/>
  </circle>
  <circle cx="900" cy="40" r="1.5" fill="white" opacity="0.4">
    <animate attributeName="opacity" from="0.3" to="1" dur="2.3s" repeatCount="indefinite" begin="0.6s"/>
  </circle>
  <circle cx="100" cy="350" r="1" fill="white" opacity="0.4">
    <animate attributeName="opacity" from="0.3" to="1" dur="2.5s" repeatCount="indefinite" begin="0.2s"/>
  </circle>
  <circle cx="400" cy="370" r="1.5" fill="white" opacity="0.4">
    <animate attributeName="opacity" from="0.3" to="1" dur="2.1s" repeatCount="indefinite" begin="0.9s"/>
  </circle>
  <circle cx="800" cy="360" r="1" fill="white" opacity="0.4">
    <animate attributeName="opacity" from="0.3" to="1" dur="2.7s" repeatCount="indefinite" begin="1.1s"/>
  </circle>
  
  <!-- Shooting stars -->
  <g>
    <!-- Shooting star 1 -->
    <line x1="0" y1="120" x2="60" y2="120" stroke="white" stroke-width="2.5" stroke-linecap="round">
      <animate attributeName="x1" from="-100" to="1100" dur="4s" repeatCount="indefinite" begin="0s"/>
      <animate attributeName="x2" from="0" to="1200" dur="4s" repeatCount="indefinite" begin="0s"/>
      <animate attributeName="opacity" from="0" to="1" dur="4s" repeatCount="indefinite" begin="0s" values="0;1;1;0"/>
    </line>
    
    <!-- Shooting star 2 -->
    <line x1="0" y1="200" x2="60" y2="200" stroke="white" stroke-width="2.5" stroke-linecap="round">
      <animate attributeName="x1" from="-100" to="1100" dur="4s" repeatCount="indefinite" begin="1.2s"/>
      <animate attributeName="x2" from="0" to="1200" dur="4s" repeatCount="indefinite" begin="1.2s"/>
      <animate attributeName="opacity" from="0" to="1" dur="4s" repeatCount="indefinite" begin="1.2s" values="0;1;1;0"/>
    </line>
    
    <!-- Shooting star 3 -->
    <line x1="0" y1="280" x2="60" y2="280" stroke="white" stroke-width="2.5" stroke-linecap="round">
      <animate attributeName="x1" from="-100" to="1100" dur="4s" repeatCount="indefinite" begin="2.4s"/>
      <animate attributeName="x2" from="0" to="1200" dur="4s" repeatCount="indefinite" begin="2.4s"/>
      <animate attributeName="opacity" from="0" to="1" dur="4s" repeatCount="indefinite" begin="2.4s" values="0;1;1;0"/>
    </line>
  </g>
  
  <!-- Main title with gradient and glow -->
  <text x="500" y="170" font-size="56" font-weight="bold" fill="url(#textGrad)" text-anchor="middle" letter-spacing="2">
    Yassin Sabek
    <animate attributeName="opacity" from="0" to="1" dur="1s" begin="0s"/>
  </text>
  
  <!-- Subtitle with fade animation -->
  <text x="500" y="230" font-size="24" fill="white" text-anchor="middle" opacity="0.9">
    Full Stack Developer
    <animate attributeName="opacity" from="0" to="0.9" dur="1.2s" begin="0.3s"/>
  </text>
  
  <!-- Description with delayed fade -->
  <text x="500" y="270" font-size="16" fill="white" text-anchor="middle" opacity="0.7">
    Building elegant solutions with code
    <animate attributeName="opacity" from="0" to="0.7" dur="1.2s" begin="0.6s"/>
  </text>
  
  <!-- Decorative line accent -->
  <line x1="250" y1="310" x2="750" y2="310" stroke="url(#textGrad)" stroke-width="2" opacity="0.6">
    <animate attributeName="opacity" from="0" to="0.6" dur="1.2s" begin="0.9s"/>
  </line>
</svg>

<div align="center">

# Hi there, I'm Yassin Sabek! 👋

**Welcome to my GitHub profile!** I'm passionate about building innovative solutions and contributing to open source projects.

[Portfolio](#portfolio) • [Projects](#projects) • [Skills](#skills) • [Connect](#connect-with-me)

</div>

---

## 📋 Table of Contents
- [About Me](#about-me)
- [Skills](#skills)
- [Featured Projects](#featured-projects)
- [GitHub Statistics](#github-statistics)
- [Experience & Education](#experience--education)
- [Certifications](#certifications)
- [Blog & Articles](#blog--articles)
- [Connect With Me](#connect-with-me)

---

## About Me

👨‍💻 **Full Stack Developer** with passion for creating elegant solutions to complex problems.

- 🎯 **Focus**: Web Development, Software Architecture, Clean Code
- 🌱 **Currently Learning**: Advanced System Design, Cloud Technologies
- 💡 **Interested In**: Open Source Contribution, Technical Mentoring
- 🎓 **Philosophy**: Continuous learning and growth mindset

---

## 🛠️ Skills

### Programming Languages
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![HTML5](https://img.shields.io/badge/-HTML5-E34C26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/-CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

### Frontend Technologies
![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Vue.js](https://img.shields.io/badge/-Vue.js-4FC08D?style=flat-square&logo=vue.js&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/-Tailwind%20CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)

### Backend & Databases
![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)

### Tools & Platforms
![GitHub](https://img.shields.io/badge/-GitHub-181717?style=flat-square&logo=github)
![Git](https://img.shields.io/badge/-Git-F05032?style=flat-square&logo=git&logoColor=white)
![VS Code](https://img.shields.io/badge/-VS%20Code-007ACC?style=flat-square&logo=visual-studio-code)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/-AWS-232F3E?style=flat-square&logo=amazon-aws&logoColor=white)

---

## Featured Projects

### 🚀 [Project Name 1](https://github.com/YassinSabek2k05/project1)
**Description**: Brief description of what this project does and why it's awesome.
- **Tech Stack**: React, Node.js, MongoDB
- **Features**: Key feature 1, Key feature 2, Key feature 3
- **Status**: Active

### 🎨 [Project Name 2](https://github.com/YassinSabek2k05/project2)
**Description**: Another amazing project that showcases your skills.
- **Tech Stack**: Vue.js, Express, PostgreSQL
- **Features**: Feature highlight 1, Feature highlight 2
- **Status**: Maintained

### 📊 [Project Name 3](https://github.com/YassinSabek2k05/project3)
**Description**: Community-driven project with excellent documentation.
- **Tech Stack**: TypeScript, Next.js, GraphQL
- **Contributors**: 5+
- **Downloads**: 1000+

---

## GitHub Statistics

<div align="center">

![Yassin's GitHub stats](https://github-readme-stats.vercel.app/api?username=YassinSabek2k05&show_icons=true&theme=radical&include_all_commits=true&count_private=true)

</div>

<div align="center">

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=YassinSabek2k05&layout=compact&theme=radical)

</div>

<div align="center">

![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=YassinSabek2k05&theme=radical)

</div>

---

## Experience & Education

### 💼 Professional Experience

**Senior Developer** @ Tech Company (2023 - Present)
- Led development of full-stack web applications
- Mentored junior developers
- Improved system performance by 40%

**Full Stack Developer** @ Startup XYZ (2021 - 2023)
- Built scalable REST APIs
- Implemented responsive UI components
- Deployed applications to AWS

### 🎓 Education

**Bachelor of Science in Computer Science**
- University Name (Graduation: Year)
- GPA: X.XX/4.0

---

## Certifications

- ✅ AWS Certified Solutions Architect
- ✅ MongoDB Certified Associate
- ✅ Google Cloud Professional Developer
- 🔄 In Progress: Kubernetes for Developers

---

## Blog & Articles

📝 **Recent Articles**:
- [Article Title 1](https://medium.com/@username/article1) - Published on Medium
- [Article Title 2](https://dev.to/@username/article2) - Published on Dev.to
- [Tutorial: Building a REST API](https://example.com) - Personal Blog

---

## 📊 Activity Graph

![Activity Graph](https://activity-graph.herokuapp.com/graph?username=YassinSabek2k05&theme=radical)

---

## 🎯 2024 Goals

- [ ] Contribute to 5+ open source projects
- [ ] Publish 12 blog articles
- [ ] Build 3 production-ready applications
- [ ] Learn Rust and WebAssembly

---

## Support & Contributions

If you find my work helpful, consider:
- ⭐ Starring my repositories
- 🔗 Contributing to open source projects
- 💬 Sharing feedback and suggestions
- 📢 Recommending me to others

---

## 📫 Connect With Me

<div align="center">

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/YassinSabek)
[![Twitter](https://img.shields.io/badge/-Twitter-1DA1F2?style=flat-square&logo=twitter&logoColor=white)](https://twitter.com/YassinSabek)
[![Email](https://img.shields.io/badge/-Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:your.email@example.com)
[![Portfolio](https://img.shields.io/badge/-Portfolio-000000?style=flat-square&logo=netlify&logoColor=white)](https://yourportfolio.com)
[![Dev.to](https://img.shields.io/badge/-Dev.to-0A0A0A?style=flat-square&logo=dev.to&logoColor=white)](https://dev.to/username)

Feel free to reach out if you want to collaborate on a project or just chat about technology! 💬

</div>

---

<div align="center">

### ⭐️ If you found this profile helpful, consider giving it a star!

**Last Updated**: December 2024

</div>

⭐️ From [YassinSabek2k05](https://github.com/YassinSabek2k05)
