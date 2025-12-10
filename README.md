# Hi there, I'm Yassin 👋

<!-- Hero SVG with animated gradient + waving hand -->
<svg width="100%" height="180" viewBox="0 0 1200 180" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Animated hero banner">
  <defs>
    <linearGradient id="g" x1="0" x2="1" y1="0" y2="1">
      <stop offset="0%" stop-color="#7b2ff7">
        <animate attributeName="stop-color" dur="6s" repeatCount="indefinite" values="#7b2ff7;#00c6ff;#7b2ff7" />
      </stop>
      <stop offset="100%" stop-color="#00c6ff">
        <animate attributeName="stop-color" dur="6s" repeatCount="indefinite" values="#00c6ff;#7b2ff7;#00c6ff" />
      </stop>
    </linearGradient>

    <!-- waving hand path reused -->
    <g id="hand">
      <path fill="#fff" d="M22 2c-1 0-4 1-6 4-2 2-4 6-4 9s2 9 7 11 10 1 13-1 4-6 3-9c-1-3-4-6-7-9s-5-5-6-5z"/>
    </g>

    <!-- moving mask for the typing/shimmer -->
    <mask id="m">
      <rect x="0" y="0" width="1200" height="160" fill="white"/>
      <rect id="maskRect" x="-300" y="0" width="300" height="160" fill="black">
        <animate attributeName="x" from="-300" to="1200" dur="4s" repeatCount="indefinite" />
      </rect>
    </mask>
  </defs>

  <!-- background -->
  <rect width="1200" height="160" rx="12" fill="url(#g)" />

  <!-- Soft floating blobs -->
  <g opacity="0.15">
    <ellipse cx="100" cy="60" rx="120" ry="40" fill="#fff">
      <animate attributeName="cx" dur="8s" values="100;300;100" repeatCount="indefinite"/>
    </ellipse>
    <ellipse cx="900" cy="120" rx="140" ry="50" fill="#000">
      <animate attributeName="cy" dur="10s" values="120;40;120" repeatCount="indefinite"/>
    </ellipse>
  </g>

  <!-- Text -->
  <g transform="translate(40,40)" fill="#fff" font-family="'Segoe UI', Roboto, Helvetica, Arial, sans-serif">
    <text x="0" y="40" font-size="32" font-weight="700">Yassin Sabek</text>

    <!-- Subtitle with shimmer (mask) -->
    <g mask="url(#m)">
      <text x="0" y="80" font-size="18" font-weight="500" fill="#e6f7ff">Software engineer • Web & Open Source</text>
    </g>
  </g>

  <!-- Waving hand (animated rotation) -->
  <g transform="translate(1120,36) scale(2.5)">
    <use href="#hand" transform="rotate(0 10 10)">
      <animateTransform attributeName="transform" attributeType="XML" type="rotate" dur="1.2s" values="0 10 10;18 10 10;0 10 10" repeatCount="indefinite" />
    </use>
  </g>
</svg>

---

A few quick links
- 🔭 Currently working on: cool web animations, tooling, and open-source utilities
- 🌱 Learning: advanced SVG motion, WebGPU experiments
- 💬 Ask me about: JavaScript, TypeScript, React, and deployment pipelines
- 📫 How to reach me: find me on GitHub (this profile) — link to social badges below

<!-- Animated status/pulse badge -->
<svg width="220" height="40" viewBox="0 0 220 40" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="status badge">
  <defs>
    <linearGradient id="b" x1="0" x2="1">
      <stop offset="0%" stop-color="#00ffd5"/><stop offset="100%" stop-color="#00a0ff"/>
    </linearGradient>
  </defs>
  <rect rx="8" width="220" height="40" fill="#0b1220"/>
  <g transform="translate(12,8)">
    <circle cx="10" cy="10" r="6" fill="url(#b)">
      <animate attributeName="r" dur="1.5s" values="6;10;6" repeatCount="indefinite"/>
      <animate attributeName="opacity" dur="1.5s" values="1;0.4;1" repeatCount="indefinite"/>
    </circle>
    <text x="28" y="15" font-family="Inter, Arial" font-size="13" fill="#dbeafe">Open to collaborations</text>
  </g>
</svg>

---

Technologies I use
- JavaScript / TypeScript
- React / Next.js
- Node.js / Deno
- CSS / SVG animations

Show me your language stats
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=YassinSabek2k05&layout=compact&theme=vision-friendly-dark)

Want to use this README?
1. Create a repository named exactly YassinSabek2k05 (your GitHub username).
2. Add this README.md to the repo root and push.
3. Visit your profile page and enjoy the animated header.

Notes & compatibility
- GitHub strips some SVG features in certain contexts (especially external SVGs and some CSS). Inline SVGs inside README.md usually work, but animation support can vary by browser and the GitHub UI.
- If an animation is not visible, try viewing the raw README or opening your profile in another browser.

Customize it
- Replace my name and links.
- Tweak colors in the gradient stops.
- Swap or extend SVGs — remove or add shapes, or ask me to generate a dark-mode alternative.

If you'd like, I can:
- produce a pure-dark-mode variant,
- create multiple small animated badges for skills,
- or build a lightweight JS-powered profile card that you can host and embed.

Would you like a dark-mode version or a set of small animated skill badges next?
