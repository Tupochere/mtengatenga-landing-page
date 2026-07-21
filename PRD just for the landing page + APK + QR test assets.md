# Mtengatenga Museum AR – Landing Page PRD

## 1. Overview

**Product name:** Mtengatenga Museum AR – Demo Landing Page  
**Type:** Single-page website  
**Goal:** Provide a simple, trusted entry point where people can:
- Understand what the app does in under 10 seconds.
- Watch a short demo video.
- Download the Android APK safely.
- Download QR test assets to try the app.
- Open the existing web/admin app demo (optional link).

This page is for recruiters, supervisors, and potential collaborators who want to quickly see and test the project. [web:6][web:36]

---

## 2. Target Audience & Use Cases

**Target audience:**
- Recruiters and hiring managers reviewing your CV/portfolio.
- FYP supervisors and examiners.
- Developers or collaborators interested in your stack.

**Primary use cases:**
1. A recruiter clicks a link in your CV → lands here → immediately understands the project and can watch a demo without installing anything. [web:6][web:36]  
2. A technically curious visitor wants to try the app → downloads APK and QR pack → follows instructions to run it on their Android phone.  
3. A supervisor wants to see both mobile and web parts → watches demo video and opens the web app link.

---

## 3. Objectives & Success Criteria

**Objectives:**
- Explain the project clearly with a headline, short subheading, and 3–4 bullet features. [web:6][web:36]  
- Make the “Watch Demo” and “Download APK + QR pack” actions extremely obvious. [web:6]  
- Provide instructions that reduce fear about sideloading an APK. [web:39]  
- Link to your live web app demo (even if it’s partial), with context. [web:6][web:36]

**Success criteria (MVP):**
- A first-time visitor can answer “What is this?” and “How do I try it?” within 15 seconds. [web:36]  
- APK and QR pack download work from both desktop and mobile.  
- Page looks good on mobile and loads fast. [web:36][web:39]

---

## 4. Scope

**In scope:**
- Single landing page (no complex navigation).  
- Static content + links/buttons for:
  - Demo video (YouTube).
  - APK download.
  - QR test assets download (ZIP or folder).
  - Web app demo link.
  - Link to GitHub repo.  
- Basic tracking (optional, e.g. simple analytics script).

**Out of scope (for this PRD):**
- Multi-page documentation site.  
- Authentication.  
- Complex blog or news sections.

---

## 5. Content & Structure

### 5.1 Page Sections (Top to Bottom)

1. **Hero Section (Above the Fold)**  
   - Elements:
     - App name: “Mtengatenga Museum AR Experience”  
     - One-sentence value proposition, e.g.  
       “Scan real museum artifacts with your Android phone to unlock AR stories, 3D models, and an AI guide.”  
     - Two primary CTAs:
       - “Watch Demo” (scrolls or opens video section). [web:6][web:36]  
       - “Try the App” (scrolls to download section).  
     - Background: simple image / gradient / museum-themed illustration.  

2. **What This Project Does**  
   - Short paragraph giving context (museum AR app + admin web app).  
   - 3–4 bullets:
     - QR-based artifact scanning. [cite:14][cite:19]  
     - Rich artifact details (text, images, timelines). [cite:19][cite:13]  
     - Optional AR 3D model viewing. [cite:12]  
     - Offline-friendly design & Supabase backend. [cite:16][cite:18]  

3. **Demo Video Section**  
   - Embedded YouTube video (or thumbnail + “Play” button). [web:8][web:6]  
   - Short caption: “1-minute walkthrough of scanning QR codes, viewing artifacts, and using the web dashboard.”  

4. **Try It Yourself – Downloads**  
   - Clear subheading: “Try the Android app in 3 steps”. [web:6][web:36]  
   - Three numbered steps:
     1. Download the APK (button).  
     2. Download the QR test pack (button).  
     3. Follow install & scan instructions below.  
   - Buttons:
     - “Download APK (Android only)”  
       - Points to GitHub Release / Drive / Netlify file. [web:3][web:39]  
     - “Download QR Test Pack”  
       - ZIP of QR images (e.g. `MASK001`, `SHIELD001`, etc.) plus a README. [cite:13][cite:19]  
   - Short note on safety:
     - Explain that it’s a student project APK, not from Play Store.
     - Mention that no personal data is collected (if true).  

5. **How to Install & Test (Instructions)**  
   - A compact, step-by-step list:
     - “On your Android phone, enable installing from ‘unknown sources’ (Settings → Security or Apps → Install unknown apps).” [web:39]  
     - “Download the APK on your phone and tap to install.”  
     - “Open the app, tap ‘Scan Artifact’, and point the camera at one of the QR codes from the test pack (on screen or printed).” [cite:14][cite:13]  
     - “You should see the artifact name and full details. If AR is supported, use the AR button to view the 3D model.” [cite:12]  

6. **Web App / Admin Portal Link**  
   - Short description:
     - “Admin dashboard to manage artifacts, rooms, and analytics (work-in-progress).”  
   - Button:
     - “Open Web Dashboard (Demo)” → link to your React/Vercel deployment.  
   - Note:
     - Mention it’s a demo with sample data and that there’s no login required or provide demo credentials.  

7. **Tech Stack & GitHub**  
   - Brief tech stack line:
     - “Built with Flutter, ARCore, Supabase, and React (web dashboard).” [cite:18][cite:12][cite:20]  
   - Button:
     - “View Source on GitHub” → link to your repo.  

8. **Footer**  
   - Copyright line.  
   - Your name + LinkedIn link.  

---

## 6. Functional Requirements

**FR-1: Hero CTAs**  
- The hero must display “Watch Demo” and “Try the App” buttons, visible without scrolling on desktop and mobile. [web:6][web:36]  
- Clicking “Watch Demo” scrolls to the video section.  
- Clicking “Try the App” scrolls to the download section.

**FR-2: Video Embed**  
- The landing page must embed or link to a YouTube demo video. [web:8][web:6]  
- On mobile, the video must be playable without breaking layout.

**FR-3: APK Download**  
- The page must provide a button that triggers APK download from a stable URL (GitHub release, Drive, or other hosting). [web:3][web:39]  
- The button label must clearly state “Android APK (Sideload)” or similar.

**FR-4: QR Test Pack Download**  
- The page must provide a button that downloads a ZIP containing:
  - QR images (.png). [cite:13]  
  - A README with a list of test artifact codes and instructions.  

**FR-5: Instructions Section**  
- The page must show simple installation and testing instructions in bullet or numbered form. [web:36][web:39]  
- Instructions must mention:
  - Enabling installs from unknown sources.
  - Using QR images to test scanning.
  - Expected behaviour on successful scan.

**FR-6: Web Dashboard Link**  
- The page must include a button/link to open the web app demo in a new tab.  
- Brief explanation: what the dashboard is for and its current completeness level.

**FR-7: Tech Stack & GitHub**  
- The page must list core technologies used. [cite:18][cite:20][cite:12]  
- The page must link to the project’s GitHub repository.

**FR-8: Mobile Responsiveness**  
- Layout must be responsive: hero, video, and buttons readable and usable on small screens. [web:36][web:6]  

---

## 7. Non-Functional Requirements

**NFR-1: Performance**  
- Page should load in under 3 seconds on a typical 3G/4G mobile connection. [web:36][web:39]  
- Images should be optimized (compressed, reasonable resolution).

**NFR-2: Trust & Clarity**  
- Copy must be transparent about:
  - APK not being from Google Play.  
  - Intended use as a demo/student project.  
- No dark patterns or misleading download text. [web:39]

**NFR-3: Accessibility**  
- Button text and headings should be readable with good contrast. [web:36]  
- Video should have a descriptive title and optional captions (handled via YouTube). [web:8]

---

## 8. Design & Style Notes (for Coding Assistant)

- Overall style: modern, clean, with a museum/heritage feel (warm earth tones, subtle patterns).  
- Use one main accent color for CTAs (e.g. deep blue or amber). [web:6]  
- Include at least one screenshot of the app and one image of a QR code being scanned. [web:36]  
- Keep the page **single-column on mobile**, two-column hero on desktop (text + illustrative image/video). [web:36][web:6]

---

## 9. Implementation Notes

- Tech options:
  - Simple React/Next.js or plain HTML + Tailwind; deploy to Vercel/Netlify. [web:6][web:36]  
- APK hosting:
  - Preferred: GitHub Releases or a cloud storage link with stable URL. [web:3][web:39]  
- QR pack hosting:
  - ZIP stored in same project (static file) or on GitHub Releases.

---

