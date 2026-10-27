## 1. Aim

To design and develop a complete responsive landing page using HTML5, CSS3, and Flexbox.

## 2. Objectives

- Create a responsive navigation bar.
- Design an attractive hero section with text, buttons, and an image.
- Create three feature cards using Flexbox.
- Add a call-to-action (CTA) section.
- Design a consistent footer.
- Use `gap`, `justify-content`, `align-items`, and `flex-wrap`.
- Make the website responsive for desktop, tablet, and mobile screens.
- Upload the project to a GitHub repository.

## 3. Technologies Used

- HTML5
- CSS3
- Flexbox
- Media Queries
- Google Fonts
- Git and GitHub

## 4. Project Structure

Create a folder named `assignment-7.5` with these files:

```text
assignment-7.5/
│
├── index.html
└── style.css
```

## 5. Complete HTML Code

Create a file named `index.html` and paste this code:

### index.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <meta
        name="description"
        content="Discover creative digital solutions with BrightSpace."
    >

    <title>BrightSpace | Build Something Amazing</title>

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

    <link
        href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700;800&display=swap"
        rel="stylesheet"
    >

    <link rel="stylesheet" href="style.css">
</head>

<body>

    <!-- Navigation Bar -->

    <header class="header" id="home">
        <nav class="navbar container">

            <a href="#home" class="logo">
                <span class="logo-icon">B</span>
                BrightSpace
            </a>

            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#features">Features</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>

            <a href="#contact" class="nav-button">Get Started</a>

        </nav>
    </header>

    <main>

        <!-- Hero Section -->

        <section class="hero" id="about">
            <div class="container hero-content">

                <div class="hero-text">
                    <span class="hero-label">
                        YOUR IDEAS, OUR INNOVATION
                    </span>

                    <h1>
                        Build Something
                        <span>Amazing.</span>
                    </h1>

                    <p>
                        Bring your ideas to life with creative digital
                        solutions. Discover new possibilities, simplify
                        your work, and create something extraordinary
                        with BrightSpace.
                    </p>

                    <div class="hero-buttons">
                        <a href="#contact" class="button primary-button">
                            Get Started &rarr;
                        </a>

                        <a href="#features" class="button secondary-button">
                            Explore Features
                        </a>
                    </div>

                    <div class="hero-note">
                        <span class="check-icon">✓</span>
                        Simple, smart, and built for everyone.
                    </div>
                </div>

                <div class="hero-image">
                    <img
                        src="https://images.unsplash.com/photo-1497366754035-f200968a6e72?auto=format&fit=crop&w=1000&q=85"
                        alt="Modern workspace with desks and computers"
                    >

                    <div class="image-badge">
                        <span class="badge-icon">✦</span>
                        <div>
                            <strong>Think Creative</strong>
                            <p>Make ideas happen</p>
                        </div>
                    </div>
                </div>

            </div>
        </section>

        <!-- Features Section -->

        <section class="features section-padding" id="features">
            <div class="container">

                <div class="section-heading">
                    <span class="section-label">OUR FEATURES</span>

                    <h2>Everything You Need to Grow</h2>

                    <p>
                        Explore simple and powerful features designed
                        to help you turn ideas into results.
                    </p>
                </div>

                <div class="feature-cards">

                    <!-- Feature Card 1 -->

                    <article class="feature-card">
                        <div class="feature-icon purple-icon">✦</div>

                        <h3>Creative Design</h3>

                        <p>
                            Enjoy a clean, modern, and attractive design
                            that makes every interaction memorable.
                        </p>

                        <a href="#contact" class="feature-link">
                            Learn more &rarr;
                        </a>
                    </article>

                    <!-- Feature Card 2 -->

                    <article class="feature-card">
                        <div class="feature-icon blue-icon">⚡</div>

                        <h3>Fast Performance</h3>

                        <p>
                            Experience a smooth and simple interface
                            designed to help you work more efficiently.
                        </p>

                        <a href="#contact" class="feature-link">
                            Learn more &rarr;
                        </a>
                    </article>

                    <!-- Feature Card 3 -->

                    <article class="feature-card">
                        <div class="feature-icon green-icon">◎</div>

                        <h3>Fully Responsive</h3>

                        <p>
                            Access the website on desktops, tablets,
                            and smartphones without layout issues.
                        </p>

                        <a href="#contact" class="feature-link">
                            Learn more &rarr;
                        </a>
                    </article>

                </div>
            </div>
        </section>

        <!-- Call-to-Action Section -->

        <section class="cta-section" id="contact">
            <div class="container cta-content">

                <div class="cta-text">
                    <span class="cta-label">READY TO BEGIN?</span>

                    <h2>Let's Build Something Great Together.</h2>

                    <p>
                        Take the first step toward your next big idea.
                        Start exploring what you can create today.
                    </p>
                </div>

                <a href="mailto:hello@example.com" class="button cta-button">
                    Let's Get Started &rarr;
                </a>

            </div>
        </section>

    </main>

    <!-- Footer Section -->

    <footer class="footer">
        <div class="container footer-content">

            <a href="#home" class="footer-logo">
                <span class="logo-icon">B</span>
                BrightSpace
            </a>

            <p>
                &copy; 2026 BrightSpace. All rights reserved.
            </p>

            <a href="#home" class="back-to-top">
                Back to top ↑
            </a>

        </div>
    </footer>

</body>
</html>
```

## 6. Complete CSS Code

Create a file named `style.css` in the same folder and paste this code:

### style.css

```css
/* ==============================
   1. Global Styles
================================= */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
    scroll-padding-top: 90px;
}

body {
    font-family: "Poppins", sans-serif;
    color: #172554;
    background-color: #ffffff;
    line-height: 1.7;
    overflow-wrap: break-word;
}

img {
    display: block;
    max-width: 100%;
}

a {
    text-decoration: none;
    color: inherit;
}

.container {
    width: 90%;
    max-width: 1200px;
    margin: 0 auto;
}

.section-padding {
    padding: 90px 0;
}

/* ==============================
   2. Navigation Bar
================================= */

.header {
    position: sticky;
    top: 0;
    z-index: 1000;
    background-color: #ffffff;
    border-bottom: 1px solid #e8edf5;
}

.navbar {
    min-height: 82px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 25px;
}

.logo,
.footer-logo {
    display: flex;
    align-items: center;
    gap: 10px;
    color: #172554;
    font-size: 23px;
    font-weight: 800;
    white-space: nowrap;
}

.logo-icon {
    width: 42px;
    height: 42px;
    display: inline-flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
    border-radius: 12px;
    color: #ffffff;
    background: linear-gradient(135deg, #4f46e5, #8b5cf6);
    font-size: 22px;
}

.nav-links {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    gap: 28px;
    list-style: none;
}

.nav-links a {
    color: #64748b;
    font-size: 14px;
    font-weight: 500;
    transition: color 0.3s ease;
}

.nav-links a:hover {
    color: #4f46e5;
}

.nav-button {
    display: inline-block;
    padding: 11px 20px;
    border-radius: 9px;
    background-color: #4f46e5;
    color: #ffffff;
    font-size: 14px;
    font-weight: 600;
    white-space: nowrap;
    transition: background-color 0.3s ease;
}

.nav-button:hover {
    background-color: #3730a3;
}

/* ==============================
   3. Hero Section
================================= */

.hero {
    padding: 85px 0;
    background:
        radial-gradient(
            circle at 90% 10%,
            #ede9fe 0,
            transparent 35%
        ),
        #f8faff;
}

.hero-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 60px;
}

.hero-text {
    flex: 1 1 50%;
    min-width: 0;
}

.hero-label,
.section-label,
.cta-label {
    display: inline-block;
    color: #4f46e5;
    font-size: 12px;
    font-weight: 700;
    letter-spacing: 1.5px;
}

.hero-label {
    padding: 8px 14px;
    margin-bottom: 20px;
    border: 1px solid #ddd6fe;
    border-radius: 30px;
    background-color: #f5f3ff;
}

.hero-text h1 {
    margin-bottom: 22px;
    font-size: clamp(36px, 5vw, 60px);
    font-weight: 800;
    line-height: 1.2;
    letter-spacing: -1.5px;
}

.hero-text h1 span {
    display: block;
    color: #4f46e5;
}

.hero-text > p {
    max-width: 520px;
    margin-bottom: 28px;
    color: #64748b;
    font-size: 16px;
    line-height: 1.9;
}

.hero-buttons {
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    gap: 14px;
}

.button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 8px;
    padding: 14px 22px;
    border: 2px solid transparent;
    border-radius: 9px;
    font-size: 14px;
    font-weight: 600;
    text-align: center;
    transition:
        background-color 0.3s ease,
        color 0.3s ease,
        transform 0.3s ease;
}

.primary-button {
    background-color: #4f46e5;
    color: #ffffff;
}

.primary-button:hover {
    background-color: #3730a3;
    transform: translateY(-2px);
}

.secondary-button {
    border-color: #dbe3f0;
    background-color: #ffffff;
    color: #172554;
}

.secondary-button:hover {
    border-color: #4f46e5;
    color: #4f46e5;
    transform: translateY(-2px);
}

.hero-note {
    display: flex;
    align-items: center;
    gap: 9px;
    margin-top: 25px;
    color: #64748b;
    font-size: 13px;
}

.check-icon {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 22px;
    height: 22px;
    border-radius: 50%;
    background-color: #dcfce7;
    color: #15803d;
    font-weight: 700;
}

/* Hero Image */

.hero-image {
    position: relative;
    flex: 1 1 50%;
    min-width: 0;
}

.hero-image > img {
    width: 100%;
    height: 430px;
    object-fit: cover;
    border-radius: 24px;
    box-shadow: 0 25px 60px rgba(79, 70, 229, 0.15);
}

.image-badge {
    position: absolute;
    bottom: 22px;
    left: -20px;
    display: flex;
    align-items: center;
    gap: 12px;
    max-width: calc(100% - 20px);
    padding: 15px 18px;
    border: 1px solid #eef2f7;
    border-radius: 14px;
    background-color: #ffffff;
    box-shadow: 0 12px 30px rgba(15, 23, 42, 0.12);
}

.badge-icon {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 40px;
    height: 40px;
    flex-shrink: 0;
    border-radius: 10px;
    background-color: #ede9fe;
    color: #4f46e5;
    font-size: 22px;
}

.image-badge strong {
    display: block;
    font-size: 13px;
}

.image-badge p {
    color: #64748b;
    font-size: 11px;
}

/* ==============================
   4. Features Section
================================= */

.features {
    background-color: #ffffff;
}

.section-heading {
    max-width: 650px;
    margin: 0 auto 45px;
    text-align: center;
}

.section-heading h2 {
    margin: 12px 0;
    font-size: clamp(27px, 3.5vw, 40px);
    line-height: 1.3;
    letter-spacing: -0.8px;
}

.section-heading > p {
    color: #64748b;
    font-size: 15px;
}

.feature-cards {
    display: flex;
    justify-content: center;
    align-items: stretch;
    flex-wrap: wrap;
    gap: 25px;
}

.feature-card {
    display: flex;
    flex: 1 1 280px;
    flex-direction: column;
    min-width: 0;
    max-width: 380px;
    padding: 30px;
    border: 1px solid #e8edf5;
    border-radius: 18px;
    background-color: #ffffff;
    box-shadow: 0 8px 30px rgba(15, 23, 42, 0.04);
    transition:
        transform 0.3s ease,
        box-shadow 0.3s ease;
}

.feature-card:hover {
    transform: translateY(-6px);
    box-shadow: 0 18px 40px rgba(15, 23, 42, 0.09);
}

.feature-icon {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 54px;
    height: 54px;
    margin-bottom: 22px;
    border-radius: 15px;
    font-size: 25px;
    font-weight: 700;
}

.purple-icon {
    background-color: #ede9fe;
    color: #6d28d9;
}

.blue-icon {
    background-color: #dbeafe;
    color: #1d4ed8;
}

.green-icon {
    background-color: #dcfce7;
    color: #15803d;
}

.feature-card h3 {
    margin-bottom: 12px;
    font-size: 20px;
}

.feature-card > p {
    flex-grow: 1;
    margin-bottom: 22px;
    color: #64748b;
    font-size: 14px;
    line-height: 1.9;
}

.feature-link {
    align-self: flex-start;
    color: #4f46e5;
    font-size: 14px;
    font-weight: 600;
}

.feature-link:hover {
    color: #3730a3;
}

/* ==============================
   5. Call-to-Action Section
================================= */

.cta-section {
    padding: 65px 0;
    background: linear-gradient(135deg, #3730a3, #6d28d9);
    color: #ffffff;
}

.cta-content {
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
    gap: 35px;
}

.cta-text {
    flex: 1 1 450px;
    min-width: 0;
}

.cta-label {
    color: #c4b5fd;
}

.cta-text h2 {
    max-width: 600px;
    margin: 12px 0;
    font-size: clamp(27px, 4vw, 40px);
    line-height: 1.3;
}

.cta-text p {
    max-width: 550px;
    color: #e0e7ff;
    font-size: 14px;
}

.cta-button {
    flex-shrink: 0;
    background-color: #ffffff;
    color: #3730a3;
}

.cta-button:hover {
    background-color: #ede9fe;
    transform: translateY(-2px);
}

/* ==============================
   6. Footer
================================= */

.footer {
    padding: 25px 0;
    background-color: #111c3d;
    color: #cbd5e1;
}

.footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 18px;
}

.footer-logo {
    color: #ffffff;
    font-size: 18px;
}

.footer-logo .logo-icon {
    width: 34px;
    height: 34px;
    font-size: 18px;
}

.footer-content > p {
    font-size: 12px;
    text-align: center;
}

.back-to-top {
    color: #c4b5fd;
    font-size: 13px;
    font-weight: 500;
}

.back-to-top:hover {
    color: #ffffff;
}

/* ==============================
   7. Tablet Responsive Design
================================= */

@media (max-width: 900px) {
    .navbar {
        gap: 16px;
    }

    .nav-links {
        gap: 16px;
    }

    .logo {
        font-size: 20px;
    }

    .hero {
        padding: 65px 0;
    }

    .hero-content {
        gap: 30px;
    }

    .hero-image > img {
        height: 350px;
    }

    .feature-card {
        flex-basis: 260px;
        padding: 25px;
    }
}

/* ==============================
   8. Mobile Responsive Design
================================= */

@media (max-width: 650px) {
    .container {
        width: 92%;
    }

    .section-padding {
        padding: 60px 0;
    }

    .navbar {
        justify-content: space-between;
        flex-wrap: wrap;
        padding: 15px 0;
    }

    .logo {
        font-size: 21px;
    }

    .logo-icon {
        width: 36px;
        height: 36px;
        font-size: 19px;
    }

    .nav-button {
        padding: 9px 12px;
        font-size: 12px;
    }

    .nav-links {
        order: 3;
        width: 100%;
        justify-content: center;
        gap: 12px 22px;
    }

    .nav-links a {
        font-size: 12px;
    }

    .hero {
        padding: 50px 0 60px;
    }

    .hero-content {
        flex-direction: column;
        align-items: stretch;
        gap: 38px;
    }

    .hero-text h1 {
        font-size: clamp(34px, 9vw, 46px);
        letter-spacing: -1px;
    }

    .hero-text > p {
        font-size: 14px;
    }

    .hero-buttons {
        gap: 10px;
    }

    .button {
        padding: 12px 16px;
        font-size: 13px;
    }

    .hero-image > img {
        height: 290px;
        border-radius: 18px;
    }

    .image-badge {
        left: 12px;
        bottom: 12px;
        padding: 11px 13px;
    }

    .section-heading {
        margin-bottom: 30px;
    }

    .section-heading > p {
        font-size: 14px;
    }

    .feature-cards {
        flex-direction: column;
        align-items: stretch;
        gap: 18px;
    }

    .feature-card {
        flex: 1 1 auto;
        width: 100%;
        max-width: none;
    }

    .cta-section {
        padding: 50px 0;
    }

    .cta-content {
        flex-direction: column;
        align-items: flex-start;
        gap: 25px;
    }

    .cta-text {
        flex-basis: auto;
        width: 100%;
    }

    .cta-button {
        max-width: 100%;
    }

    .footer-content {
        flex-direction: column;
        justify-content: center;
        text-align: center;
    }
}

/* ==============================
   9. Extra Small Screens
================================= */

@media (max-width: 380px) {
    .logo {
        gap: 6px;
        font-size: 18px;
    }

    .nav-button {
        padding: 8px 9px;
        font-size: 11px;
    }

    .nav-links {
        gap: 10px 15px;
    }

    .hero-label {
        font-size: 10px;
        letter-spacing: 0.8px;
    }

    .hero-text h1 {
        font-size: 32px;
    }

    .hero-buttons {
        flex-direction: column;
        align-items: stretch;
    }

    .hero-buttons .button {
        width: 100%;
    }

    .hero-image > img {
        height: 230px;
    }

    .feature-card {
        padding: 22px;
    }

    .cta-text h2 {
        font-size: 27px;
    }

    .footer-content > p {
        font-size: 11px;
    }
}
```

## 7. How to Run the Project

1. Open Visual Studio Code.
2. Create a folder named `assignment-7.5`.
3. Create `index.html` and `style.css` inside the folder.
4. Paste the respective code into each file.
5. Save both files.
6. Right-click `index.html` and select **Open with Live Server**. If Live Server is not installed, install the VS Code Live Server extension or open `index.html` directly in a browser.
7. Resize the browser window or use Chrome DevTools to test mobile responsiveness.

## 8. Flexbox Properties Used

| CSS Property | Purpose |
|---|---|
| `display: flex` | Arranges elements using Flexbox |
| `justify-content: space-between` | Distributes elements horizontally |
| `align-items: center` | Aligns elements along the cross-axis |
| `gap` | Adds spacing between elements |
| `flex-wrap: wrap` | Allows elements to move to another row |
| `flex-direction: column` | Stacks elements vertically on mobile |
| `flex: 1 1 280px` | Allows feature cards to grow and wrap responsively |

## 9. Responsive Design Testing

Test the website at these viewport widths:

- **1440px:** Desktop layout with navigation and three feature cards in a row.
- **768px:** Tablet layout with flexible spacing and wrapping cards.
- **390px:** Mobile layout with stacked hero content and feature cards.
- **320px:** Extra-small screen layout with reduced font sizes and vertically arranged buttons.

Check that text, images, buttons, and cards remain within the viewport without unwanted horizontal scrolling.

## 10. Expected Output

The completed landing page contains:

1. A navigation bar with the BrightSpace logo, navigation links, and Get Started button.
2. A hero section with a heading, description, CTA buttons, and image.
3. Three feature cards for Creative Design, Fast Performance, and Fully Responsive.
4. A call-to-action section encouraging visitors to get started.
5. A footer containing the logo, copyright notice, and Back to Top link.
6. A responsive design that adjusts to desktop, tablet, and mobile screens.

## 11. GitHub Repository Submission

### Step 1: Initialize Git

Open the terminal in the `assignment-7.5` folder and run:

```bash
git init
git add index.html style.css
git commit -m "Create responsive Flexbox landing page"
```

### Step 2: Create a GitHub Repository

1. Visit https://github.com/
2. Sign in to your GitHub account.
3. Click the **New repository** option.
4. Enter the repository name: `assignment-7.5`
5. Select **Public** if your assignment requires a public repository.
6. Create the repository without adding a README, license, or `.gitignore` if you have already created the local project.

### Step 3: Connect and Push the Project

Replace `YOUR_USERNAME` with your actual GitHub username and run:

```bash
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/assignment-7.5.git
git push -u origin main
```

If Git reports that `origin` already exists, use `git remote set-url origin https://github.com/YOUR_USERNAME/assignment-7.5.git` before pushing.

### Step 4: Verify the Submission

Open your GitHub repository and confirm that these files are present:

- `index.html`
- `style.css`

Copy the repository URL for your assignment submission.

**GitHub Repository Link:** `https://github.com/YOUR_USERNAME/assignment-7.5`

Replace `YOUR_USERNAME` with your actual username. The link above is a template, not a created or verified repository.

## 12. Result

Successfully designed and developed a complete responsive landing page using HTML5, CSS3, and Flexbox. The project includes a navigation bar, hero section, three feature cards, a call-to-action section, and a footer. Flexbox properties and media queries ensure consistent spacing, alignment, and responsive behavior across different screen sizes.
