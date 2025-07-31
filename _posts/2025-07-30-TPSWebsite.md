---
title: "TPS Website"
date: 2025-07-30
categories: [TPS Website]
---

# Introduction

For the past month, I worked on creating a new website for the Technology Policy Society at JHU to better capture the scope and impact of the organization's work.

# Development Notes

Since this is purely a frontend project, I started out with bootstrapping Create React App.
```bash
npm install react-bootstrap bootstrap
```

Then, I created a basic structure for my multipage website that utilizes react-router-dom. 

```bash
components/
├── Navigation.tsx
├── MainPage.tsx
├── ProjectPage.tsx
├── ResourcePage.tsx
├── TeamPage.tsx
├── TeamCards.tsx
├── Footer.tsx
└── and CSS files for all components
```

**Navigation Bar**

I created a sticky navigation bar with a simple menu list that contains "HOME," "PROJECTS," "RESOURCES," "TEAM"

<img width="1493" height="143" alt="Screenshot 2025-07-31 at 4 29 50 PM" src="https://github.com/user-attachments/assets/8eb41d82-a308-437d-9cea-b8c7636738bf" />


**Main Page**

- Main landing section with a tagline and I added animated through CSS
- Section with a blurb about TPS
- Project section that highlights Hackathon and Fellowship
- Impact section with countup function coded on JS
- Partner section with automatically moving caurosel
- Contact us section with team photo

**Projects Page**

- Section on AI Security Hackathon with information blurbs, caurosel with image highlights, cards for project features
- Section on AI Security Frontiers Fellowship

**Resources Page**

- Cards on featured articles on JHU CS and Apart Research

**Team Page**

- Cards on each members utilizing TeamCards.tsx (image, name, affiliation, position, email, and linkedin)

**Footer**

- Simple copyright note
- Mini menu bar


*The website is currently deployed through vercel*

**Feel free to check it out: https://tps-jhu.vercel.app**







