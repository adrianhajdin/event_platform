<div align="center">
  <br />
    <a href="https://www.youtube.com/watch?v=FkowOdMjvYo" target="_blank">
      <img src="https://github.com/sujatagunale/EasyRead/assets/151519281/65ff8e7a-9167-4761-bb89-59b6b3ba8307" alt="Project Banner">
    </a>
  <br />

  <div>
    <img src="https://img.shields.io/badge/-React_JS-black?style=for-the-badge&logoColor=white&logo=react&color=61DAFB" alt="react.js" />
    <img src="https://img.shields.io/badge/-Three_JS-black?style=for-the-badge&logoColor=white&logo=threedotjs&color=000000" alt="three.js" />
    <img src="https://img.shields.io/badge/-Tailwind_CSS-black?style=for-the-badge&logoColor=white&logo=tailwindcss&color=06B6D4" alt="tailwindcss" />
  </div>

  <h3 align="center">A 3D Dev Portfolio</h3>

   <div align="center">
     Build this project step by step with our detailed tutorial on <a href="https://www.youtube.com/@javascriptmastery/videos" target="_blank"><b>JavaScript Mastery</b></a> YouTube. Join the JSM family!
    </div>
</div>

## 📋 <a name="table">Table of Contents</a>

1. 🤖 [Introduction](#introduction)
2. ⚙️ [Tech Stack](#tech-stack)
3. 🔋 [Features](#features)
4. 🤸 [Quick Start](#quick-start)
5. 🕸️ [Snippets](#snippets)
6. 🔗 [Links](#links)
7. 🚀 [More](#more)

## 🚨 Tutorial

This repository contains the code corresponding to an in-depth tutorial available on our YouTube channel, <a href="https://www.youtube.com/@javascriptmastery/videos" target="_blank"><b>JavaScript Mastery</b></a>. 

If you prefer visual learning, this is the perfect resource for you. Follow our tutorial to learn how to build projects like these step-by-step in a beginner-friendly manner!

<a href="https://www.youtube.com/watch?v=FkowOdMjvYo" target="_blank"><img src="https://github.com/sujatagunale/EasyRead/assets/151519281/1736fca5-a031-4854-8c09-bc110e3bc16d" /></a>

## <a name="introduction">🤖 Introduction</a>

Built with React.js for handling the user interface, Three.js for rendering 3D elements, and styled with TailwindCSS, 3D Island is a website project. The primary goal is to demonstrate the developer's skills in a unique manner that creates a lasting impact.

If you're getting started and need assistance or face any bugs, join our active Discord community with over 27k+ members. It's a place where people help each other out.

<a href="https://discord.com/invite/n6EdbFJ" target="_blank"><img src="https://github.com/sujatagunale/EasyRead/assets/151519281/618f4872-1e10-42da-8213-1d69e486d02e" /></a>

## <a name="tech-stack">⚙️ Tech Stack</a>

- Node.js
- React.js
- Three.js
- React Three Fiber
- React Three Drei
- Email JS
- Vite
- Tailwind CSS

## <a name="features">🔋 Features</a>

👉 **Engaging 3D Floating Fox Island**: Rotate and explore using drag-and-drop or arrow keys.

👉 **Dynamic Sky Movement**: Sky adapts to Island motion, enhancing the immersive experience.

👉 **Soaring 3D Bird**: Responds dynamically to camera positions, adding a lively touch.

👉 **Informative Island Sections**: Each island part shares details about the individual.

👉 **Comprehensive About Page**: Dive into detailed information, skills, and education.

👉 **Project Showcase**: Explore a curated list of projects created by the individual.

👉 **Contact Page with EmailJS Integration**: Easily send emails directly from the contact form.

👉 **Interactive Fox on Contact Page**: A playful fox reacts to user interactions with the form.

👉 **Seamless Animations**: Enjoy fluid and captivating visual transitions.

👉 **Lofi Music Integration**: Delight in smooth music that adapts to user interactions.

👉 **Responsive Design**: Optimized for a seamless experience across all devices.

👉 **Aesthetic Glassmorphism and Neobrutalism Effects**: Elevate the visual appeal with modern design trends.

and many more, including code architecture and reusability 

## <a name="quick-start">🤸 Quick Start</a>

Follow these steps to set up the project locally on your machine.

**Prerequisites**

Make sure you have the following installed on your machine:

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/en)
- [npm](https://www.npmjs.com/) (Node Package Manager)

**Cloning the Repository**

```bash
git clone https://github.com/your-username/your-project.git
cd your-project
```

**Installation**

Install the project dependencies using npm:

```bash
npm install
```

**Set Up Environment Variables**

Create a new file named `.env` in the root of your project and add the following content:

```env
#NEXT
NEXT_PUBLIC_SERVER_URL=

#CLERK
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_CLERK_WEBHOOK_SECRET=

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

#MONGODB
MONGODB_URI=

#UPLOADTHING
UPLOADTHING_SECRET=
UPLOADTHING_APP_ID=

#STRIPE
STRIPE_SECRET_KEY=
STRIPE_WEBHOOK_SECRET=
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=
```

Replace the placeholder values with your actual EmailJS credentials. You can obtain these credentials by signing up on the [EmailJS website](https://www.emailjs.com/).

**Running the Project**

```bash
npm start
```

Open [http://localhost:3000](http://localhost:3000) in your browser to view the project.

## <a name="snippets">🕸️ Snippets</a>

<details>
<summary><code>index.css</code></summary>

```css
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600;700;800;900&family=Work+Sans:wght@100;200;300;400;500;600;700;800;900&display=swap");

@tailwind base;
@tailwind components;
@tailwind utilities;

:root {
  --blue-rgb: 237 245 255;
  --green-rgb: 125 161 35;
}

body {
  font-family: "Work Sans", sans-serif;
}

body:has(.card[data-color="blue"]:hover) {
  background-color: rgb(var(--blue-rgb) / 25%);
}

body:has(.card[data-color="green"]:hover) {
  background-color: rgb(var(--green-rgb) / 25%);
}

@layer utilities {
  .max-container {
    @apply max-w-5xl mx-auto sm:p-16 pb-12 !pt-[126px] px-8 min-h-[calc(100vh-80px)];
  }

  .head-text {
    @apply sm:text-5xl text-3xl font-semibold sm:leading-snug font-poppins;
  }

  .subhead-text {
    @apply font-semibold sm:text-3xl text-xl relative font-poppins;
  }

  .blue-gradient_text {
    @apply bg-gradient-to-r from-[#00c6ff] to-[#0072ff] bg-clip-text text-transparent;
  }

  .input {
    @apply bg-white border border-gray-200 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5 mt-2.5 font-normal shadow-card;
  }

  .textarea {
    @apply block p-2.5 w-full text-sm text-gray-900 bg-white rounded-lg border border-gray-200 focus:ring-blue-500 focus:border-blue-500 mt-2.5 font-normal shadow-card;
  }

  .btn {
    @apply text-white bg-gradient-to-r from-[#00c6ff] to-[#0072ff] focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm w-full sm:w-auto px-5 py-2.5 text-center;
  }

  .header {
    @apply flex justify-between items-center sm:px-16 px-8 py-4 max-w-5xl mx-auto absolute top-0 bg-transparent z-10 right-0 left-0;
  }

  .footer {
    @apply max-w-5xl mx-auto sm:px-16 pb-6 px-8 flex flex-col gap-7;
  }

  .footer-container {
    @apply flex flex-wrap gap-7 items-center justify-between;
  }

  .info-box {
    @apply mx-5 relative flex text-white flex-col gap-3 max-w-2xl neo-brutalism-blue pt-4 pb-12 px-8;
  }

  .neo-btn {
    @apply py-3 px-6 rounded-lg text-blue-500 text-center font-semibold sm:w-1/2 w-[90%] -bottom-5 absolute mx-auto right-0 left-0 flex justify-center items-center gap-3;
  }

  .cta {
    @apply w-full flex items-center md:flex-row flex-col sm:mt-16 mt-8 gap-7;
  }

  .cta-text {
    @apply text-black-500 font-extrabold flex-1 text-3xl max-md:text-center;
  }
}

.glassmorphism {
  background: rgba(8, 116, 239, 0.07);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border-radius: 10px;
  border: 1px solid rgba(255, 255, 255, 0.18);
}

.logo {
  border-radius: 8.889px;
  background: #fff;
  box-shadow: 0px 10px 35px -4px rgba(67, 83, 255, 0.15),
    0px 1.5px 4px -1px rgba(67, 83, 255, 0.2);
}

.block-container {
  position: relative;
  transition: 250ms;
  perspective: 500px;
}

.block-container .btn-back {
  position: absolute;
  inset: 0;
  z-index: -1;
  width: inherit;
  height: inherit;
  transition: 250ms;
  transform-style: preserve-3d;
  transform-origin: bottom right;
  transform: rotateZ(15deg);
  will-change: transform;
  box-shadow: 16px 0 40px #e4e4e4;
}

.block-container .btn-back-red {
  background: linear-gradient(135deg, #ff4b1f -20%, #ff9068 120%);
}

.block-container .btn-back-green {
  background: linear-gradient(135deg, #adfda2 -20%, #11d3f3 120%);
}

.block-container .btn-back-yellow {
  background: linear-gradient(135deg, #f7971e -20%, #ffd200 120%);
}

.block-container .btn-back-blue {
  background: linear-gradient(135deg, #0061ff -20%, #60efff 120%);
}

.block-container .btn-back-orange {
  background: linear-gradient(135deg, #ff0f7b -20%, #f89b29 120%);
}

.block-container .btn-back-pink {
  background: linear-gradient(135deg, #e81cff -20%, #40c9ff 120%);
}

.block-container .btn-back-black {
  background: linear-gradient(135deg, #0a1647 -20%, #e4e7e4 120%);
}

.block-container .btn-front {
  position: absolute;
  inset: 0;
  z-index: 1;
  width: inherit;
  height: inherit;
  background-color: #ffffff33;
  -webkit-backdrop-filter: blur(20px);
  backdrop-filter: blur(20px);
  transition: 250ms;
  transform-style: preserve-3d;
  transform-origin: top left;
  overflow: hidden;
}

.block-container:hover > .btn-back {
  transform: translateZ(20px) rotateZ(15deg) rotateX(-20deg) rotateY(-20deg);
}

.block-container:hover > .btn-front {
  transform: translateZ(80px) translateY(-5px) rotateX(15deg) rotateY(15deg);
}

/* Neo Brutalism */
.neo-brutalism-blue {
  background: #2b77e7;
  position: relative;
  border-radius: 10px;
  border: #2b77e7;
  box-shadow: 0.6vmin 0.6vmin #336cc1, 1vmin 1vmin #0092db, 1vmin 1vmin #0092db,
    0.65vmin 1vmin #0092db, 1vmin 0.65vmin #0092db;
}

.neo-brutalism-white {
  background: #fff;
  border: #fff;
  box-shadow: 0.6vmin 0.6vmin #fff, 1vmin 1vmin #d2e4ff, 1vmin 1vmin #d2e4ff,
    0.65vmin 1vmin #d2e4ff, 1vmin 0.65vmin #d2e4ff;
}
```
</details>

<details>
<summary><code>constants/index.js</code></summary>

```javascript
import { meta, shopify, starbucks, tesla } from "../assets/images";
import {
    car,
    contact,
    css,
    estate,
    express,
    git,
    github,
    html,
    javascript,
    linkedin,
    mongodb,
    motion,
    mui,
    nextjs,
    nodejs,
    pricewise,
    react,
    redux,
    sass,
    snapgram,
    summiz,
    tailwindcss,
    threads,
    typescript
} from "../assets/icons";

export const skills = [
    {
        imageUrl: css,
        name: "CSS",
        type: "Frontend",
    },
    {
        imageUrl: express,
        name: "Express",
        type: "Backend",
    },
    {
        imageUrl: git,
        name: "Git",
        type: "Version Control",
    },
    {
        imageUrl: github,
        name: "GitHub",
        type: "Version Control",
    },
    {
        imageUrl: html,
        name: "HTML",
        type: "Frontend",
    },
    {
        imageUrl: javascript,
        name: "JavaScript",
        type: "Frontend",
    },
    {
        imageUrl: mongodb,
        name: "MongoDB",
        type: "Database",
    },
    {
        imageUrl: motion,
        name: "Motion",
        type: "Animation",
    },
    {
        imageUrl: mui,
        name: "Material-UI",
        type: "Frontend",
    },
    {
        imageUrl: nextjs,
        name: "Next.js",
        type: "Frontend",
    },
    {
        imageUrl: nodejs,
        name: "Node.js",
        type: "Backend",
    },
    {
        imageUrl: react,
        name: "React",
        type: "Frontend",
    },
    {
        imageUrl: redux,
        name: "Redux",
        type: "State Management",
    },
    {
        imageUrl: sass,
        name: "Sass",
        type: "Frontend",
    },
    {
        imageUrl: tailwindcss,
        name: "Tailwind CSS",
        type: "Frontend",
    },
    {
        imageUrl: typescript,
        name: "TypeScript",
        type: "Frontend",
    }
];

export const experiences = [
    {
        title: "React.js Developer",
        company_name: "Starbucks",
        icon: starbucks,
        iconBg: "#accbe1",
        date: "March 2020 - April 2021",
        points: [
            "Developing and maintaining web applications using React.js and other related technologies.",
            "Collaborating with cross-functional teams including designers, product managers, and other developers to create high-quality products.",
            "Implementing responsive design and ensuring cross-browser compatibility.",
            "Participating in code reviews and providing constructive feedback to other developers.",
        ],
    },
    {
        title: "React Native Developer",
        company_name: "Tesla",
        icon: tesla,
        iconBg: "#fbc3bc",
        date: "Jan 2021 - Feb 2022",
        points: [
            "Developing and maintaining web applications using React.js and other related technologies.",
            "Collaborating with cross-functional teams including designers, product managers, and other developers to create high-quality products.",
            "Implementing responsive design and ensuring cross-browser compatibility.",
            "Participating in code reviews and providing constructive feedback to other developers.",
        ],
    },
    {
        title: "Web Developer",
        company_name: "Shopify",
        icon: shopify,
        iconBg: "#b7e4c7",
        date: "Jan 2022 - Jan 2023",
        points: [
            "Developing and maintaining web applications using React.js and other related technologies.",
            "Collaborating with cross-functional teams including designers, product managers, and other developers to create high-quality products.",
            "Implementing responsive design and ensuring cross-browser compatibility.",
            "Participating in code reviews and providing constructive feedback to other developers.",
        ],
    },
    {
        title: "Full stack Developer",
        company_name: "Meta",
        icon: meta,
        iconBg: "#a2d2ff",
        date: "Jan 2023 - Present",
        points: [
            "Developing and maintaining web applications using React.js and other related technologies.",
            "Collaborating with cross-functional teams including designers, product managers, and other developers to create high-quality products.",
            "Implementing responsive design and ensuring cross-browser compatibility.",
            "Participating in code reviews and providing constructive feedback to other developers.",
        ],
    },
];

export const socialLinks = [
    {
        name: 'Contact',
        iconUrl: contact,
        link: '/contact',
    },
    {
        name: 'GitHub',
        iconUrl: github,
        link: 'https://github.com/YourGitHubUsername',
    },
    {
        name: 'LinkedIn',
        iconUrl: linkedin,
        link: 'https://www.linkedin.com/in/YourLinkedInUsername',
    }
];

export const projects = [
    {
        iconUrl: pricewise,
        theme: 'btn-back-red',
        name: 'Amazon Price Tracker',
        description: 'Developed a web application that tracks and notifies users of price changes for products on Amazon, helping users find the best deals.',
        link: 'https://github.com/adrianhajdin/pricewise',
    },
    {
        iconUrl: threads,
        theme: 'btn-back-green',
        name: 'Full Stack Threads Clone',
        description: 'Created a full-stack replica of the popular discussion platform "Threads," enabling users to post and engage in threaded conversations.',
        link: 'https://github.com/adrianhajdin/threads',
    },
    {
        iconUrl: car,
        theme: 'btn-back-blue',
        name: 'Car Finding App',
        description: 'Designed and built a mobile app for finding and comparing cars on the market, streamlining the car-buying process.',
        link: 'https://github.com/adrianhajdin/project_next13_car_showcase',
    },
    {
        iconUrl: snapgram,
        theme: 'btn-back-pink',
        name: 'Full Stack Instagram Clone',
        description: 'Built a complete clone of Instagram, allowing users to share photos and connect with friends in a familiar social media environment.',
        link: 'https://github.com/adrianhajdin/social_media_app',
    },
    {
        iconUrl: estate,
        theme: 'btn-back-black',
        name: 'Real-Estate Application',
        description: 'Developed a web application for real estate listings, facilitating property searches and connecting buyers with sellers.',
        link: 'https://github.com/adrianhajdin/projects_realestate',
    },
    {
        iconUrl: summiz,
        theme: 'btn-back-yellow',
        name: 'AI Summarizer Application',
        description: 'App that leverages AI to automatically generate concise & informative summaries from lengthy text content, or blogs.',
        link: 'https://github.com/adrianhajdin/project_ai_summarizer',
    }
];
```
</details>

<details>
<summary><code>tailwind.config.js</code></summary>

```javascript
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {
      colors: {
        gray: {
          200: "#D5DAE1"
        },
        black: {
          DEFAULT: "#000",
          500: "#1D2235"
        },
        blue: {
          500: "#2b77e7"
        }
      },
      fontFamily: {
        worksans: ["Work Sans", "sans-serif"],
        poppins: ['Poppins', "sans-serif"]
      },
      boxShadow: {
        card: '0px 1px 2px 0px rgba(0, 0, 0, 0.05)'
      }
    },
  },
  plugins: [],
}
```
</details>

<details>
<summary>Normalized Rotation Algorithm</summary>

```javascript
const normalizedRotation =
  ((rotation % (2 * Math.PI)) + 2 * Math.PI) % (2 * Math.PI);

// Set the current stage based on the island's orientation
switch (true) {
  case normalizedRotation >= 5.45 && normalizedRotation <= 5.85:
    setCurrentStage(4);
    break;
  case normalizedRotation >= 0.85 && normalizedRotation <= 1.3:
    setCurrentStage(3);
    break;
  case normalizedRotation >= 2.4 && normalizedRotation <= 2.6:
    setCurrentStage(2);
    break;
  case normalizedRotation >= 4.25 && normalizedRotation <= 4.75:
    setCurrentStage(1);
    break;
  default:
    setCurrentStage(null);
}
```
</details>

## <a name="links">🔗 Links</a>

Models and Assets used in the project can be found [here](https://drive.google.com/file/d/1TACDN8qFpi_NW66I4p48R9_MUmx-JT3P/edit)

## <a name="more">🚀 More</a>

**Advance your skills with Next.js 14 Pro Course**

Enjoyed creating this project? Dive deeper into our PRO courses for a richer learning adventure. They're packed with detailed explanations, cool features, and exercises to boost your skills. Give it a go!

<a href="https://jsmastery.pro/next14" target="_blank">
<img src="https://github.com/sujatagunale/EasyRead/assets/151519281/557837ce-f612-4530-ab24-189e75133c71" alt="Project Banner">
</a>

<br />
<br />

**Accelerate your professional journey with Expert Training program**

And if you're hungry for more than just a course and want to understand how we learn and tackle tech challenges, hop into our personalized masterclass. We cover best practices, different web skills, and offer mentorship to boost your confidence. Let's learn and grow together!

<a href="https://www.jsmastery.pro/masterclass" target="_blank">
<img src="https://github.com/sujatagunale/EasyRead/assets/151519281/fed352ad-f27b-400d-9b8f-c7fe628acb84" alt="Project Banner">
</a>

#
