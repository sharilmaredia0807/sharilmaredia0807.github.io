Build me a complete personal portfolio website as a single-page HTML/CSS/JS file. This is a cooler, more personable alternative to my LinkedIn — same information, but tells a story and shows personality.
---
## IDENTITY
Name: Sharil Maredia
Current role: Incoming Mechanical Engineer @ Sunday Robotics | MS Candidate, MIT
Email: sharilmaredia@gmail.com
LinkedIn: https://linkedin.com/in/sharilmaredia
Twitter: https://twitter.com/sharilmaredia
Instagram: https://instagram.com/sharilmaredia
---
## AESTHETIC & DESIGN DIRECTION
**Vibe:** Modern minimalist + techy. Think monokai.com — confident, typography-first, generous whitespace, nothing decorative that doesn't earn its place.
**Color palette:**
- Background: #0a0a0a
- Surface/cards: #111111 and #1a1a1a
- Primary accent: #E31E24 (red — use sparingly)
- Text primary: #f0f0f0
- Text secondary: #888888
- Borders: #222222
**Typography:**
- Headings: "Syne" (Google Fonts) — 400, 700, 800
- Body: "Space Grotesk" (Google Fonts) — 300, 400, 500
- Labels/tags/code: "JetBrains Mono" (Google Fonts) — 400, 500
- Do NOT use Inter, Roboto, or system fonts.
**Motion & interaction:**
- Page load: staggered fade-up on hero elements via animation-delay
- Scroll reveal: sections fade in on viewport entry (IntersectionObserver)
- Hover: red underline slides in on nav links; cards lift subtly (translateY -3px)
- Custom cursor: small red circle, lerp-follows mouse, scales up on hover over interactive elements. Set cursor: none on body.
- Scroll progress indicator: 2px red line fixed at very top of viewport, grows left to right as user scrolls
- No gratuitous animation — everything intentional
**Layout:**
- Full-bleed dark sections
- Asymmetric grid moments — photos offset, not centered
- Generous whitespace
- Thin 1px red accent lines used sparingly
- Fully mobile responsive, hamburger nav on mobile
---
## SECTIONS
### 1. NAV
- Fixed top, backdrop-blur on scroll
- Logo: "SM" in JetBrains Mono, red
- Links: About, Experience, Education, Projects, Skills, Contact
- Mobile: hamburger slides down
---
### 2. HERO
- Large Syne heading: "Sharil Maredia"
- Subtitle with staggered word animation: "Engineer. Builder. Incoming @ Sunday Robotics."
- Bio: "I build things that move, last, and matter. From Tesla to SpaceX to MIT — I've spent my career designing hardware at the edge of what's possible."
- "Currently" line below bio in JetBrains Mono, muted, with a small pulsing red dot:
  `● Currently: finishing my MS at MIT. Next up: Sunday Robotics.`
- Two CTA buttons: "See My Work" (→ #projects) | "Download Resume" (→ SMarediaResume.pdf)
- Photo: `SMarediaHeadshot.jpg` — right of text, slightly offset/cropped asymmetrically. Subtle desaturation or dark red duotone treatment. Not a boring centered headshot.
- Company badges row below bio — label: "Where I've worked:" in small JetBrains Mono. Logo files: `mit-logo.png`, `nasa-logo.png`, `spacex-logo.png`, `tesla-logo.png`, `sunday-logo.png`. Display at ~32px height, single-color white (filter: brightness(0) invert(1)), opacity 0.4, brighten to full on hover. Fallback to monospace text badge if file missing.
---
### 3. ABOUT
- Section header: "About"
- First-person copy — warm, confident, like describing yourself to someone cool at a party:
  - Engineer who loves making things actually exist in the world, not just on a screen
  - At the MIT Self-Assembly Lab building systems to help restore coastlines
  - Heading to Sunday Robotics after MIT
  - Has built lathes, yoyos, airplanes, PCBs, and a 5-meter ocean simulator
  - "Builder" is the core identity word
  - Short sentences. Real. Not stuffy.
- Two photos, editorial asymmetric layout:
  1. `mefun.JPG` — caption: "In the shop (safety glasses mandatory, apparently)"
  2. `smaredia.jpg` — no caption
- Captions in small JetBrains Mono, muted
---
### 4. EXPERIENCE
- Section header: "Experience"
- Vertical timeline: dates on left, content on right, 1px red vertical spine
- Work experience ONLY — no personal or academic projects here
- Each entry: Company in Syne (large, bold), Role, Date + Location in JetBrains Mono, bullets in Space Grotesk
**Sunday Robotics** | Mechanical Engineer | Incoming
- Joining full-time post-MIT
**MIT Self-Assembly Lab** | Researcher | Aug 2024 – Present | Cambridge, MA
- Constructed a 5m × 5m × 3m gantry system to simulate oceanic forcing on atolls for coastal regrowth research
- Designed a precision motion control system replicating real-world hydrodynamic conditions
**Tesla** | New Programs Engineering Intern | Jun 2024 – Aug 2024 & May 2025 – Aug 2025 | Hawthorne, CA
- Led HVAC system development for the Tesla Robovan and a critical Roadster system as Responsible Engineer
- Supported Cybercab prototype builds — designed parts to resolve assembly issues and optimize processes
- Developed a LIDAR-based ground truth test rig for Model 3 used for Cybercab calibration
**Tesla** | Mechanical Design Engineering Intern | May 2023 – Aug 2023 | Palo Alto, CA
- Designed and validated Model S/X battery pack changes to reduce thermal event propagation, cut costs, improve assembly
- Developed HV distribution structural parts for Model 3/Y battery pack to minimize headcount and BOM costs
**SpaceX** | Mechanical Engineering Intern | May 2022 – Aug 2022 | Redmond, WA
- Designed automated tooling for Starlink v2.0 solar module production line — significant rate and yield improvements
- Aided in design, manufacturing, and assembly of onboard power systems for v2.0 Starlink satellite
**NASA – Johnson Space Center** | Mechanical Engineer | Aug 2019 – Mar 2020 | Houston, TX
- Designed a more efficient water capture and recirculation device for the ISS with NASA Crew and Thermal Systems
- Presented project updates to senior engineers for review
Group the two Tesla entries with a subtle visual connector (bracket or "3 internships" badge).
---
### 5. EDUCATION
- Section header: "Education"
- Two bold cards:
**MIT — M.S. Mechanical Engineering** | Sep 2024 – May 2026
Specialization: Machine Design | GPA: 5.0 / 5.0
**MIT — B.S. Mechanical Engineering** | Sep 2020 – May 2024
GPA: 5.0 / 5.0
- Use `mitgrad.jpg` editorially — full-bleed background with dark overlay, or asymmetric photo beside cards. Caption in JetBrains Mono: "MIT Commencement, 2024"
- Publications callout (small card within section):
  "Development of a Millimeter-Scale Laminar Flow Mixer for Rapid Iteration of Sustainable Energy Materials"
  Link: "Read paper →" href="#" (I will fill in the URL)
---
### 6. PROJECTS
- Section header: "Projects"
- Personal and academic projects only — no overlap with Experience
- 2-column grid desktop, 1 column mobile
- Each card: Title (Syne), context line (JetBrains Mono), 2–3 sentence description, tag badges, image slot, video slot where noted
- Image slot: use matching file if present (ontrack.jpg, lathe.jpg, yoyo.jpg, robot.jpg, nimbus.jpg, airplane.jpg, printer.jpg). If missing, show placeholder: dashed 1px red border, `// photo coming soon` in JetBrains Mono.
- Comment every slot: `<!-- PROJECT IMAGE: replace with <img src="filename.jpg" alt="..."> -->`
**OnTrack** | MIT 2.009 · 2023
Led a team to design an automated rail-cleaning system for commuter trains, preventing traction failures that cause trains to miss their braking zone. Enables more frequent maintenance while cutting operating costs.
Tags: [Product Design] [Team Lead] [Mechanical Systems] [MIT 2.009]
Image: `micd.JPG`
**Desktop Lathe** | MIT 2.72 · 2023
Designed and built a precision desktop lathe capable of machining aluminum to 50 micron accuracy and 40 micron repeatability.
Tags: [Machining] [Precision Engineering] [Manufacturing] [MIT 2.72]
Image: placeholder
Video slot: `<!-- PROJECT VIDEO: replace with <video src="lathe.mp4" controls></video> -->` — show styled placeholder with `// video coming soon`
**Mass-Manufactured Yoyo** | MIT 2.008 · 2022
Designed and produced 50 injection-molded yoyos through MIT's manufacturing class — full lifecycle from DFM to tooling to production run.
Tags: [DFM] [Injection Molding] [Product Design] [MIT 2.008]
Image: placeholder
**Line-Following Robot (Custom PCB)** | MIT 2.679 · 2024
Designed a custom PCB from scratch for a computer vision line-following robot — schematic design, board layout, and bring-up.
Tags: [PCB Design] [Computer Vision] [Embedded Systems] [Robotics]
Image: placeholder
**Solar Electric Vehicle — Nimbus** | MIT SEVT · 2020–2022
Member of MIT's Solar Electric Vehicle Team. Built CAD for the suspension and steering system and collaborated with the Aerospace Team on energy optimization. Raced and won the 2021 American Solar Challenge.
Tags: [CAD] [Suspension] [Solar Vehicle] [2021 ASC Winner]
Image: `nimbus.jpg`
**RV-12 Airplane** | High School · 2019
Led construction of the avionics and inner wing structure for a fully functional, flyable Van's RV-12 aircraft — built in high school.
Tags: [Avionics] [Aerospace] [Structures]
Image: placeholder
**Resin 3D Printer** | Personal Project
Built a DLP resin 3D printer with friends. Designed the print bed system: leveling, movement, and resin distribution.
Tags: [3D Printing] [DLP] [Hardware]
Image: placeholder
---
### 7. SKILLS
- Section header: "Skills"
- One flat cluster of equal tag badges — no categories, no headers
- Skills: SolidWorks, Siemens NX, CATIA, PTC Creo, FEA, CFD, GD&T, DFM, Python, MATLAB, PCB Design, Robotics, Precision Manufacturing
- Tags: #1a1a1a bg, 1px #2a2a2a border, JetBrains Mono, subtle red border on hover
---
### 8. CONTACT
- No section header. No dividers. Clean centered content on dark background.
- One line: "Always down to talk engineering, collaborate, or just geek out."
- Large email as plain link: sharilmaredia@gmail.com
- Row of minimal icon links: Email, LinkedIn, Twitter/X, Instagram, Resume
- Inline SVG icons only — no icon library. Keep it sparse.
---
## COPY NOTES
- Concise everywhere. If it can be said in 5 words, don't use 10.
- No filler. No "passionate about" language.
- Let credentials speak — don't over-explain them.
---
## TECHNICAL REQUIREMENTS
- Single HTML file — all CSS and JS inline. Vanilla JS only, no frameworks.
- All assets in the same folder as the HTML file:
  - Photos: `SMarediaHeadshot.jpg`, `micd.JPG`, `smaredia.jpg`, `mefun.JPG`, `mitgrad.jpg`, `nimbus.jpg`
  - Logos: `mit-logo.png`, `nasa-logo.png`, `spacex-logo.png`, `tesla-logo.png`, `sunday-logo.png`
  - Resume: `SMarediaResume.pdf`
  - Video (to be added): `lathe.mp4`
- Scroll progress bar: 2px, #E31E24, fixed at very top of viewport, width driven by scroll position
- Custom cursor: red dot, lerp follow, scales on hover. cursor: none on body.
- Google Fonts via CDN: Syne, Space Grotesk, JetBrains Mono
- Favicon: "SM" text or red square
- Every project image/video slot has a clear HTML comment even when an image is present
- Clean, well-commented code throughout
- Asset discovery: Before building, scan the project folder for any image, video, 
  or PDF files not explicitly listed above. Use your judgment to place them where 
  they fit — project cards, the About section, or the gallery. If the filename 
  suggests a project (e.g. "lathe.jpg", "yoyo.png"), drop it into the matching 
  project card. If it looks like a candid or action photo, consider adding it to 
  the About section as an additional photo. If unsure, add it to a commented-out 
  block at the bottom of the HTML so it's easy to place later:
  <!-- UNUSED ASSET: filename.jpg — place manually where appropriate -->