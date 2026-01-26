# Design Document
## Abhimanyu Dudeja Portfolio Website

**Author:** Abhimanyu Dudeja  
**Course:** CS5610 - Web Development  
**Date:** January 2025  
**Version:** 1.0

---

## Table of Contents

1. [Project Description](#1-project-description)
2. [User Personas](#2-user-personas)
3. [User Stories](#3-user-stories)
4. [Design Mockups](#4-design-mockups)
5. [Technical Architecture](#5-technical-architecture)
6. [Accessibility Considerations](#6-accessibility-considerations)

---

## 1. Project Description

### 1.1 Overview

This project is a personal portfolio website designed to showcase my professional profile, technical skills, projects, and career journey. The website serves as a digital resume and professional presence for potential employers, recruiters, and collaborators.

### 1.2 Goals

- **Primary Goal:** Create a compelling online presence that effectively communicates my skills and experience to potential employers seeking Software Engineers, Data Engineers, or ML Engineers for co-op positions.

- **Secondary Goals:**
  - Demonstrate proficiency in modern web development (HTML5, CSS3, ES6+)
  - Showcase my projects and published research
  - Provide easy ways for visitors to contact me
  - Meet all CS5610 assignment requirements

### 1.3 Target Audience

1. **Recruiters and HR Professionals** - Looking for co-op candidates
2. **Technical Hiring Managers** - Evaluating technical skills
3. **Fellow Students and Researchers** - Interested in collaboration
4. **Academic Evaluators** - Assessing coursework

### 1.4 Key Features

| Feature | Description | Priority |
|---------|-------------|----------|
| Responsive Design | Works on desktop, tablet, mobile | High |
| Typing Animation | Dynamic role display | High |
| Project Showcase | Filterable project gallery | High |
| Career Timeline | Interactive journey visualization | Medium |
| Contact Information | Easy access to contact methods | High |

---

## 2. User Personas

### Persona 1: Sarah Chen - Technical Recruiter

**Demographics:**
- Age: 32
- Location: Boston, MA
- Occupation: Senior Technical Recruiter at a Fortune 500 company
- Education: Bachelor's in Human Resources

**Background:**
Sarah has 8 years of experience recruiting software engineers. She reviews 50+ portfolios per week and has limited time per candidate. She uses LinkedIn, job boards, and university career fairs to find talent.

**Goals:**
- Quickly assess candidate qualifications
- Find candidates matching specific technical requirements
- Verify skills mentioned on resumes
- Gather contact information efficiently

**Pain Points:**
- Portfolios that are slow to load
- Missing contact information
- Unclear technical skill levels
- Portfolios without project examples

**Tech Savviness:** Intermediate - comfortable with standard web browsing, uses multiple devices

**Quote:** "I need to see what you can actually build, not just what you say you can do."

**How This Site Helps:**
- Clear skills section with specific technologies
- Project gallery with detailed descriptions
- Prominent contact information
- Fast-loading, clean design

---

### Persona 2: David Martinez - Engineering Manager

**Demographics:**
- Age: 41
- Location: San Francisco, CA (Remote Hiring)
- Occupation: Engineering Manager at a Data/ML Startup
- Education: MS in Computer Science

**Background:**
David leads a team of 12 engineers and is actively hiring for a Data Engineering Co-op. He has strong technical knowledge and evaluates candidates' code quality and problem-solving approach.

**Goals:**
- Evaluate technical depth and breadth
- Assess code quality and best practices
- Understand candidate's project experience
- Find candidates interested in data engineering/ML

**Pain Points:**
- Portfolios with no code samples
- Vague project descriptions
- Candidates without relevant domain experience
- Poor documentation practices

**Tech Savviness:** Expert - examines source code, checks GitHub

**Quote:** "Show me your thought process and how you approach problems."

**How This Site Helps:**
- Links to published research papers
- Detailed project descriptions with tech stacks
- Clean, well-documented code in GitHub
- Clear demonstration of data/ML expertise

---

### Persona 3: Maya Patel - Computer Science Student

**Demographics:**
- Age: 23
- Location: Boston, MA
- Occupation: MS CS Student at Northeastern
- Education: Currently pursuing Master's

**Background:**
Maya is a fellow graduate student interested in machine learning. She's looking for inspiration for her own portfolio and potential research collaboration opportunities.

**Goals:**
- Get inspiration for portfolio design
- Learn about peer projects and research
- Find potential collaboration opportunities
- Understand career paths in the field

**Pain Points:**
- Overly complex or overwhelming designs
- No way to contact the person
- Unclear about their specializations

**Tech Savviness:** Advanced - familiar with web technologies

**Quote:** "I want to see what's possible and get ideas for my own work."

**How This Site Helps:**
- Modern, clean design as inspiration
- Research publications listed
- Journey page showing career progression
- Open source code on GitHub

---

## 3. User Stories

### Epic 1: First Impression & Navigation

**Story 1.1: Landing Experience**
> As a **recruiter**, I want to **immediately understand who this person is and what they do** so that I can **quickly decide if they're relevant for my open positions**.

**Acceptance Criteria:**
- [ ] Name prominently displayed
- [ ] Role/title visible above the fold
- [ ] Professional photo included
- [ ] Page loads in under 3 seconds

**Story 1.2: Easy Navigation**
> As a **visitor**, I want to **easily navigate between different sections** so that I can **find the information I'm looking for without confusion**.

**Acceptance Criteria:**
- [ ] Navigation menu visible on all pages
- [ ] Current page indicated in navigation
- [ ] Mobile-responsive navigation menu
- [ ] All links work correctly

---

### Epic 2: Skills Assessment

**Story 2.1: Technical Skills Overview**
> As a **hiring manager**, I want to **see a clear breakdown of technical skills** so that I can **assess if the candidate matches our tech stack**.

**Acceptance Criteria:**
- [ ] Skills organized by category
- [ ] Specific technologies listed (not just "coding")
- [ ] Visual presentation (icons/cards)
- [ ] No exaggerated or unclear claims

**Story 2.2: Experience Validation**
> As a **technical evaluator**, I want to **see evidence of skills through projects** so that I can **verify the candidate can apply these skills**.

**Acceptance Criteria:**
- [ ] Each skill connected to at least one project
- [ ] Projects include technology tags
- [ ] Links to code repositories where applicable

---

### Epic 3: Project Exploration

**Story 3.1: Project Browsing**
> As a **visitor**, I want to **browse through projects by category** so that I can **focus on areas most relevant to me**.

**Acceptance Criteria:**
- [ ] Filter buttons for project categories
- [ ] Smooth filtering animation
- [ ] All projects visible with "All" filter
- [ ] Filter state persists during session

**Story 3.2: Project Details**
> As a **hiring manager**, I want to **understand what each project does and how it was built** so that I can **assess technical problem-solving abilities**.

**Acceptance Criteria:**
- [ ] Project description explains the problem solved
- [ ] Technologies used clearly listed
- [ ] Date/timeline provided
- [ ] Links to demo or code (where available)

**Story 3.3: Research Access**
> As a **researcher**, I want to **access published papers** so that I can **read the full research work**.

**Acceptance Criteria:**
- [ ] Published papers prominently featured
- [ ] Direct links to publications
- [ ] Brief summary of research

---

### Epic 4: Career Journey

**Story 4.1: Career Progression**
> As a **recruiter**, I want to **understand the candidate's career trajectory** so that I can **assess growth and commitment**.

**Acceptance Criteria:**
- [ ] Timeline of education and work
- [ ] Key achievements highlighted
- [ ] Logical progression shown
- [ ] Future goals indicated

**Story 4.2: Personal Touch**
> As a **fellow student**, I want to **learn personal facts beyond just technical info** so that I can **connect on a human level**.

**Acceptance Criteria:**
- [ ] Interests/hobbies section
- [ ] Professional but personable tone
- [ ] Photos that show personality

---

### Epic 5: Contact & Connection

**Story 5.1: Easy Contact**
> As a **recruiter**, I want to **quickly find contact information** so that I can **reach out about opportunities**.

**Acceptance Criteria:**
- [ ] Email prominently displayed
- [ ] Phone number available
- [ ] LinkedIn profile linked
- [ ] Contact info on every page (footer)

**Story 5.2: Professional Networks**
> As a **visitor**, I want to **connect on professional platforms** so that I can **follow their work or network**.

**Acceptance Criteria:**
- [ ] GitHub link visible
- [ ] LinkedIn link visible
- [ ] Links open in new tabs
- [ ] Icons clearly indicate platform

---

## 4. Design Mockups

### 4.1 Design Inspiration

The design is inspired by modern portfolio templates with a clean, professional aesthetic. Key design decisions:

- **Color Scheme:** Coral/pink (#ff6b6b) as primary accent color for warmth and memorability, paired with neutral grays for professionalism
- **Typography:** Poppins (sans-serif) for readability, Playfair Display (serif) for elegant headings
- **Layout:** Clean hero section with image, card-based content sections

### 4.2 Homepage Wireframe

```
+----------------------------------------------------------+
|  [AD Logo]              Home | Projects | Journey        |
+----------------------------------------------------------+
|                                                          |
|  WELCOME TO MY WORLD                                     |
|                                                          |
|  Hi, I'm Abhimanyu Dudeja                 [Profile      |
|  a Data Engineer.|                         Photo]        |
|                                                          |
|  MS Computer Science student...                          |
|                                                          |
|  [View My Work]  [Read Research]                         |
|                                                          |
|  FIND ME ON                                              |
|  [GitHub] [LinkedIn] [Email]                             |
|                                                          |
+----------------------------------------------------------+
|                                                          |
|              Technical Expertise                         |
|  +----------+ +----------+ +----------+ +----------+     |
|  | Data     | | Machine  | | Full     | | Database |     |
|  | Engineer | | Learning | | Stack    | | Systems  |     |
|  +----------+ +----------+ +----------+ +----------+     |
|                                                          |
+----------------------------------------------------------+
|        Research Highlight (Dark Background)              |
|  [Published Research]                                    |
|  Brain Tumor Detection...                                |
|  97% Accuracy | 94% Precision                            |
|  [Read Publication]                                      |
+----------------------------------------------------------+
|  Footer: Copyright | Contact Info                        |
+----------------------------------------------------------+
```

### 4.3 Projects Page Wireframe

```
+----------------------------------------------------------+
|  [AD Logo]              Home | Projects | Journey        |
+----------------------------------------------------------+
|                                                          |
|                    My Projects                           |
|         A collection of my work in ML...                 |
|                                                          |
|   [All] [Machine Learning] [Data Engineering] [Web]      |
|                                                          |
+----------------------------------------------------------+
|                                                          |
|  +------------------+  +------------------+              |
|  | [Project Image]  |  | [Project Image]  |              |
|  | Brain Tumor CNN  |  | Diabetic Retino  |              |
|  | Jan 2025         |  | May 2024         |              |
|  | Description...   |  | Description...   |              |
|  | [TF] [Keras]     |  | [CNN] [OpenCV]   |              |
|  | [Read Paper]     |  | [View Code]      |              |
|  +------------------+  +------------------+              |
|                                                          |
|  +------------------+  +------------------+              |
|  | [Project Image]  |  | [Project Image]  |              |
|  | Music Database   |  | AWS ETL Pipeline |              |
|  | ...              |  | ...              |              |
|  +------------------+  +------------------+              |
|                                                          |
+----------------------------------------------------------+
```

### 4.4 Journey Page Wireframe

```
+----------------------------------------------------------+
| [AI Generated Notice Banner]                             |
+----------------------------------------------------------+
|  [AD Logo]              Home | Projects | Journey        |
+----------------------------------------------------------+
|                                                          |
|                    My Journey                            |
|         From Chennai to Boston...                        |
|                                                          |
|     (Chennai) -------- ✈ -------- (Boston)              |
|                                                          |
+----------------------------------------------------------+
|                      |                                   |
|  [2021]              |                                   |
|  The Beginning       |                                   |
|  SRM Institute...   [2021]                               |
|                      |                                   |
|                      |        [2023]                     |
|                     [2023]    First Industry             |
|                      |        Experience                 |
|                      |        Deloitte...                |
|  [2024]              |                                   |
|  Deep Dive into ML   |                                   |
|  Healthcare AI...   [2024]                               |
|                      |                                   |
|                      |        [2025]                     |
|                     [2025]    Published Researcher       |
|                      |        Springer...                |
|                      |                                   |
+----------------------------------------------------------+
|              Quick Facts About Me                        |
|  [🏀 Basketball] [🧮 Math] [📚 Research] [🌏 Travel]     |
+----------------------------------------------------------+
```

### 4.5 Mobile Responsive Design

All pages follow a mobile-first approach with:
- Hamburger menu for navigation
- Single-column layouts on small screens
- Touch-friendly button sizes (min 44px)
- Reduced font sizes and spacing
- Timeline shifts to single-column layout

---

## 5. Technical Architecture

### 5.1 File Structure

```
abhimanyu-portfolio/
├── index.html           # Homepage
├── projects.html        # Projects listing
├── journey.html         # AI-generated timeline
├── css/
│   ├── main.css        # Shared styles, variables
│   ├── home.css        # Homepage-specific
│   ├── projects.css    # Projects page
│   └── journey.css     # Journey page
├── js/
│   ├── main.js         # Navigation, shared
│   ├── typing.js       # TypeWriter class
│   ├── projects.js     # Project filtering
│   └── journey.js      # Timeline animations
└── images/
    ├── profile.png
    └── favicon.png
```

### 5.2 CSS Architecture

- **CSS Custom Properties** for theming
- **BEM-like naming** for components
- **Mobile-first** media queries
- **No !important** declarations
- **Flexbox/Grid** for layouts

### 5.3 JavaScript Modules

All JavaScript uses ES6 modules with `type="module"`:

| Module | Responsibility |
|--------|---------------|
| main.js | Navigation, scroll effects |
| typing.js | TypeWriter animation class |
| projects.js | ProjectFilter class |
| journey.js | TimelineAnimator class |

---

## 6. Accessibility Considerations

### 6.1 WCAG 2.1 Compliance

- **Perceivable:** Alt text on images, sufficient color contrast
- **Operable:** Keyboard navigation, no time limits
- **Understandable:** Consistent navigation, clear labels
- **Robust:** Valid HTML, works across browsers

### 6.2 Implementation Details

| Feature | Implementation |
|---------|---------------|
| Images | All images have descriptive alt text |
| Navigation | Keyboard accessible, visible focus states |
| Color | Contrast ratio ≥ 4.5:1 for text |
| Motion | Respects prefers-reduced-motion |
| Semantics | Proper heading hierarchy, landmarks |

---

## Document History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | Jan 2025 | Abhimanyu Dudeja | Initial document |

---

*This design document was created as part of CS5610 Web Development at Northeastern University.*
