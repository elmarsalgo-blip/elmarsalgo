<h1 align="center">Hi 👋, I'm Vincent Elmar</h1>
<h3 align="center">A passionate frontend developer from namek</h3>

- 🔭 I’m currently a student **Vincent**

<h3 align="left">Connect with me:</h3>
<p align="left">
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://reactjs.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="40" height="40"/> </a> </p>



<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="theme-color" content="#08090d">
    <title>Welcome to the SYNK</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500;600;700;800&family=Space+Grotesk:wght@400;500;600&display=swap" rel="stylesheet">
    <style>
        :root {
            color-scheme: dark;
            --ink: #08090d;
            --cyan: #54f5f2;
            --pink: #ff4bc8;
            --white: #f4f5f8;
        }

        * {
            box-sizing: border-box;
        }

        body {
            min-height: 100vh;
            margin: 0;
            display: grid;
            place-items: center;
            overflow: hidden;
            color: var(--white);
            background:
                radial-gradient(ellipse at 18% 82%, rgb(255 75 200 / 17%), transparent 34%),
                radial-gradient(ellipse at 84% 20%, rgb(84 245 242 / 16%), transparent 35%),
                linear-gradient(135deg, #090a0f 0%, #11131a 48%, #08090d 100%);
            font-family: "Space Grotesk", sans-serif;
        }

        body::before {
            position: fixed;
            inset: 0;
            background-image:
                linear-gradient(rgb(255 255 255 / 4%) 1px, transparent 1px),
                linear-gradient(90deg, rgb(255 255 255 / 4%) 1px, transparent 1px);
            background-size: 52px 52px;
            mask-image: linear-gradient(transparent, #000 18%, #000 82%, transparent);
            content: "";
            pointer-events: none;
        }

        main {
            position: relative;
            width: min(900px, calc(100% - 40px));
            padding: clamp(44px, 10vw, 112px) 24px;
            text-align: center;
            animation: arrive 900ms cubic-bezier(.2, .8, .2, 1) both;
        }

        .eyebrow {
            display: inline-flex;
            align-items: center;
            gap: 12px;
            margin: 0 0 28px;
            color: var(--cyan);
            font-size: 11px;
            font-weight: 600;
            letter-spacing: 0.24em;
            text-transform: uppercase;
        }

        .eyebrow::before,
        .eyebrow::after {
            width: 30px;
            height: 1px;
            background: currentColor;
            content: "";
            box-shadow: 0 0 12px currentColor;
        }

        h1 {
            margin: 0;
            font-family: "Orbitron", sans-serif;
            font-size: clamp(40px, 9.5vw, 100px);
            font-weight: 800;
            line-height: 1.08;
            letter-spacing: 0.02em;
            text-shadow: 0 0 32px rgb(84 245 242 / 18%);
        }

        h1 span {
            display: block;
            color: transparent;
            background: linear-gradient(100deg, var(--cyan) 4%, var(--white) 48%, var(--pink) 96%);
            background-clip: text;
            -webkit-background-clip: text;
        }

        .tagline {
            margin: 26px 0 0;
            color: rgb(244 245 248 / 65%);
            font-size: 13px;
            letter-spacing: 0.2em;
            text-transform: uppercase;
        }

        .orbit {
            position: absolute;
            z-index: -1;
            top: 50%;
            left: 50%;
            width: min(65vw, 520px);
            aspect-ratio: 1;
            border: 1px solid rgb(84 245 242 / 12%);
            border-radius: 50%;
            box-shadow: 0 0 80px rgb(84 245 242 / 5%), inset 0 0 80px rgb(255 75 200 / 4%);
            transform: translate(-50%, -50%) rotate(-24deg) scaleY(.42);
            pointer-events: none;
        }

        .orbit::before,
        .orbit::after {
            position: absolute;
            inset: 12%;
            border: 1px solid rgb(255 75 200 / 16%);
            border-radius: 50%;
            content: "";
        }

        .orbit::after {
            inset: 24%;
            border-color: rgb(84 245 242 / 18%);
        }

        @keyframes arrive {
            from { opacity: 0; transform: translateY(18px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @media (max-width: 520px) {
            .tagline { font-size: 10px; }
            .orbit { width: 88vw; }
        }

        @media (prefers-reduced-motion: reduce) {
            *, *::before, *::after {
                animation-duration: 0.01ms !important;
                animation-iteration-count: 1 !important;
                scroll-behavior: auto !important;
            }
        }
    </style>
</head>
<body>
    <main>
        <div class="orbit" aria-hidden="true"></div>
        <p class="eyebrow">A new dimension awaits</p>
        <h1>WELCOME <span>GUYS!</span></h1>
        <p class="tagline">Welcome to the SYNK</p>
    </main>
</body>
</html>
