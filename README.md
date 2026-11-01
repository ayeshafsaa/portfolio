# Ayesha Naveed | Portfolio

A personal portfolio website for **Ayesha Naveed**, a frontend developer who builds interactive, animated web experiences with React, Three.js and Framer Motion.

**Live site:** [portfolio-six-ashen-58.vercel.app](https://portfolio-six-ashen-58.vercel.app)

## Features

- 3D hero with a floating avatar that tilts toward the mouse (React Three Fiber)
- Animated full-page background with a moving constellation and glowing nebulas
- Floating pill-style navbar, section dots and a side icon menu that follow the scroll position
- Smooth scroll between sections, plus a top scroll-progress bar
- About section with expertise cards and animated skill bars
- Projects section with live-demo and GitHub buttons on every card
- Working contact form (sends messages through Formspree) with success and error states
- Fully responsive for mobile, tablet and desktop

## Tech stack

- React 19 (Create React App)
- Three.js, @react-three/fiber and @react-three/drei
- Framer Motion
- Tailwind CSS 3
- Formspree for the contact form

## Project structure

```
portfolio/
├── public/
│   ├── index.html
│   └── avatar.png            # hero image
└── src/
    ├── App.js
    ├── index.css             # fonts, colours, background animations
    └── components/
        ├── Background.jsx    # animated constellation and nebulas
        ├── Navbar.jsx
        ├── SectionNav.jsx    # side dots and icon menu
        ├── HeroScene.jsx     # 3D hero
        ├── About.jsx
        ├── Projects.jsx
        ├── Contact.jsx
        ├── ScrollIndicator.jsx
        ├── Icons.jsx
        └── useActiveSection.js
```

## Getting started

Make sure Node.js (version 18 or newer) is installed, then:

```bash
# 1. Clone the repository
git clone https://github.com/ayeshafsaa/portfolio.git

# 2. Go into the project folder
cd portfolio

# 3. Install dependencies
npm install

# 4. Start the development server
npm start
```

The site opens at [http://localhost:3000](http://localhost:3000).

## Scripts

| Command | What it does |
| --- | --- |
| `npm start` | Runs the app in development mode |
| `npm run build` | Creates an optimized production build in the `build` folder |
| `npm test` | Runs the test runner |

## Customizing

- **Hero image:** replace `public/avatar.png` (a transparent PNG works best).
- **Projects:** edit the `projects` array at the top of `src/components/Projects.jsx`. Each project has a title, description, tags, features, a live link and a GitHub link. Use `'#'` for a link that does not exist yet and its button is hidden.
- **Skills and stats:** edit the `skills` array in `About.jsx` and the `stats` array in `HeroScene.jsx`.
- **Contact form:** create a free form at [formspree.io](https://formspree.io), then replace the `FORMSPREE_URL` value in `Contact.jsx`.
- **Social links and email:** update them in `Navbar.jsx` and `Contact.jsx`.
- **Colours and fonts:** `src/index.css` (Bebas Neue and Outfit from Google Fonts).

## Deployment

The project deploys directly to Vercel or Netlify:

1. Push the code to GitHub.
2. Import the repository in Vercel (the Create React App preset is detected automatically).
3. Click **Deploy**. Every later push to the main branch redeploys the site.

## Contact

- GitHub: [@ayeshafsaa](https://github.com/ayeshafsaa)
- LinkedIn: [Ayesha Naveed](https://www.linkedin.com/in/ayesha-naveed-871591284)
- Fiverr: [ayeshaskitchen](https://www.fiverr.com/ayeshaskitchen)
