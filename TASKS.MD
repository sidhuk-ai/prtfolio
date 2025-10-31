# 🧭 Portfolio – Improvement Task List

This document outlines enhancement tasks for the **Portfolio** project.  
Tasks are categorized into **Basic**, **Intermediate**, and **Advanced** levels to help contributors choose issues that match their skill set.

Each task includes a **Description**, **Requirements**, and **Acceptance Criteria**.

---

## 🟢 Basic Tasks

### 1\. Add “Back to Top” Button

**Description:**  


Add floating button to scroll smoothly back to top.

**Requirements:**

 - Add a **floating button** (bottom‑right corner) that is hidden by default.

 - Button should appear after scrolling down a certain distance (e.g., 200–300px).

 - On click, the page should **smoothly scroll** back to the top.

 - Use **vanilla JavaScript** for scroll detection and smooth scrolling.

 - Style the button to match the site’s theme (colors, typography, hover effects).

 - Ensure the button is **accessible** (ARIA label, keyboard focusable).

 - Responsive: should not overlap with footer or other floating elements on small screens.
    

**Acceptance Criteria:**

 - A “Back to Top” button is present but hid**den on initial load**.

 - Button **appears after scrolling down** the page.

 - Clicking the button **smoothly scrolls** the page to the top.

 - Button styling is consistent with the portfolio’s design system.

 - Works across modern browsers (Chrome, Firefox, Edge, Safari).

 - Fully accessible (screen readers announce it, keyboard users can activate it).

 - Responsive on all screen sizes without overlapping important content.
    

### 2\. Create a Responsive Contact Form (No JS Implementation)

**Description:**  

Create simple responsive contact form using only HTML and CSS.


**Requirements:**
 - Create a **new Contact Form** section (or enhance the existing one if present).

 - Include the following fields:

    - **Name** (text input)

    - **Email** (email input)

    - **Message** (textarea)

    - **Submit button**

 - Use semantic HTML (`<form>`, `<label>`, `<input>`, `<textarea>`, `<button>`).

 - Ensure all inputs have **associated labels** (visible or visually hidden).

 - Style the form with CSS to match the portfolio’s design system (colors, fonts, spacing).

 - Make the form **responsive**:

    - Full‑width on small screens.

    - Nicely aligned layout on larger screens (e.g., side‑by‑side fields or centered form).

 - No JavaScript is required - this is purely structural and visual.

**Acceptance Criteria:**

 - A **Contact Form section** is present on the site.

 - Form includes **Name, Email, Message, and Submit button**.

 - All inputs have **labels** for accessibility.

 - Form styling is consistent with the portfolio’s theme.

 - Layout is **responsive**: adapts to mobile, tablet, and desktop.

 - No JavaScript is used - only HTML and CSS.

 - Tested across modern browsers (Chrome, Firefox, Edge, Safari).


### 3\. Refactor Hardcoded Colors into CSS Variables


**Description:**  
Colors in `assets/css/style.css` are hardcoded, which makes theme changes harder to manage.

**Requirements:**

-   Define color variables in the `:root` selector.
    
-   Replace all hardcoded color values with the defined CSS variables.
    

**Acceptance Criteria:**

-   All colors reference CSS variables.
    
-   Updating a variable reflects the color change across the entire theme.

---    

## 🟡 Intermediate Tasks

### 4\. Animated Skill Bars on Scroll

**Description:**  
Animate skill bars filling when scrolled into viewport.

**Requirements:**

 - Detect when the **Skills section** enters the viewport (using `IntersectionObserver` or scroll events).

 - Animate each skill bar from **0% width to its target** percentage (e.g., 80%, 95%).

 - Ensure animation **runs only once per page load** (not every time the user scrolls back).

 - Use **CSS transitions/animations** combined with vanilla JS for triggering.

 - Keep the animation **smooth and performant** (no layout shifts).

 - Maintain **responsiveness**: bars should animate correctly on all screen sizes.

 - Ensure **accessibility**: skill values should still be readable as text (not only visual).
    

**Acceptance Criteria:**

 - Skill bars start at **0% width** on initial load.

 - Bars **animate to their defined percentage** when scrolled into view.

 - Animation triggers **only once per session** (no repeated animations on scroll back).

 - Animation is **smooth and consistent** across browsers.

 - Skill percentages remain **visible as text** for accessibility.

 - Works on desktop, tablet, and mobile screen sizes.

 - No external libraries used - only HTML, CSS, and vanilla JS.
    

### 5\. Add Dark Mode Toggle

**Description:**  
The portfolio currently lacks theme customization options.

**Requirements:**

-   Add a dark mode toggle button.
    
-   Use CSS variables to switch between light and dark themes.
    
-   Store the user’s theme preference in `localStorage`.
    

**Acceptance Criteria:**

-   Clicking the toggle switches between light and dark themes.
    
-   User preference persists on reload.
    
-   All sections adapt correctly to both themes.

  

### 6\. Create a Hamburger Menu Functionality with Smooth Animations

**Description:**  

Implement responsive hamburger menu toggle with smooth animations.


**Requirements:**

 - Implement **toggle functionality** for the hamburger button:

    - Clicking the button should **open/close** the navigation menu.

    - Menu should slide in/out or fade in/out with smooth CSS transitions.

 - Add **animated transformation** of the hamburger icon:

    - Three lines morph into an “X” when active, and back to hamburger when closed.

 - Ensure **ARIA attributes** update dynamically (`aria-expanded="true/false"`) for accessibility.

 - Navigation menu should **close automatically** when:

    - A nav link is clicked.

    - The user clicks outside the menu area.

 - Keep the design consistent with the site’s theme (colors, spacing, typography).

 - Ensure responsiveness across screen sizes (desktop, tablet, mobile).

 - Use **only HTML, CSS, and vanilla JS** (no external libraries).
    

**Acceptance Criteria:**

 - Hamburger button toggles the navigation menu open/closed.

 - Menu opens/closes with **smooth animations** (slide/fade).

 - Hamburger icon **animates into an “X”** when active.

 - aria-expanded attribute updates correctly for screen readers.

 - Clicking a nav link or outside the menu closes the menu.

 - Works across modern browsers (Chrome, Firefox, Edge, Safari).

 - Fully responsive and accessible on all screen sizes.
    
---

## 🔴 Advanced Tasks

### 7\. Add Spam Protection to Contact Form

**Description:**  
The contact form is currently susceptible to spam submissions.

**Requirements:**

-   Implement **Google reCAPTCHA** or a honeypot field for spam prevention.
    
-   Ensure legitimate users can still submit easily.
    

**Acceptance Criteria:**

-   Spam bots are effectively blocked.
    
-   Human users can submit without friction.
    

### 8\. Implement AJAX Form Submission

**Description:**  
The contact form reloads the page upon submission.

**Requirements:**

-   Use JavaScript `fetch()` or `XMLHttpRequest` to handle asynchronous submission.
    
-   Display success/error messages dynamically.
    

**Acceptance Criteria:**

-   Form submission happens without page reload.
    
-   Success message appears for valid inputs.
    
-   Error message appears for failed submissions.
    

### 9\. News Section Auto‑Slider

**Description:**  

Make the News section auto‑scroll horizontally with smooth sliding.


**Requirements:**

 - Implement auto‑sliding for the News section cards.

 - Cards should scroll horizontally every few seconds.

 - Add pause on hover so users can read without interruption.

 - Include next/prev controls for manual navigation.

 - Ensure smooth CSS transitions for sliding.

 - Use vanilla JavaScript only (no external libraries).

 - Keep the design consistent with the portfolio’s theme.

 - Ensure responsiveness across devices (desktop, tablet, mobile).


**Acceptance Criteria:**

 - News cards auto‑slide horizontally at a set interval.

 - Hovering over the section pauses auto‑scroll.

 - Next/Prev buttons manually control the slider.

 - Sliding is smooth and performant.

 - Works across modern browsers (Chrome, Firefox, Edge, Safari).

 - Fully responsive on all screen sizes.

 - No external libraries used - only HTML, CSS, and vanilla JS.


### 10\. Interactive Vertical Timeline with Scroll Reveal

**Description:**

Transform static timeline into **vertical layout with scroll‑triggered animations**.


**Requirements:**


 - Add a central vertical line to represent the timeline axis.

 - Position timeline items alternating left/right of the line on desktop.

 - On smaller screens, items should stack vertically for readability.

 - Implement scroll reveal animations (fade/slide in) when items enter the viewport.

 - Use CSS transitions/animations and vanilla JS (`IntersectionObserver` preferred).

 - Ensure accessibility: animations should not block content visibility for screen readers.

 - Keep the design consistent with the existing portfolio theme (colors, typography, spacing).


**Acceptance Criteria:**


 - Timeline displays with a central vertical line.

 - Items alternate left/right on desktop, stack vertically on mobile.

 - Each item animates into view only when scrolled into the viewport.

 - Animations are smooth and performant (no jank).

 - Works across modern browsers (Chrome, Firefox, Edge, Safari).

 - No external libraries used - only HTML, CSS, and vanilla JS.

 - Responsive and accessible (keyboard navigation and screen readers unaffected).

---
## 📦 Contribution Guidelines

To contribute, please follow these steps carefully:

1.  **Fork the Repository**  
    Create your personal fork of the project.
    
2.  **Create a Feature Branch**
    
    ```bash
    git checkout -b feature/task-name
    ```
    
3.  **Implement the Task**  
    Follow the listed requirements and keep your changes modular.
    
4.  **Test Your Changes**  
    Verify responsiveness, accessibility, and overall functionality.  
    Run **Lighthouse** or similar audits if applicable.
    
5.  **Commit with a Clear Message**
    
    ```bash
    git commit -m "Added real-time form validation to contact section"
    ```
    
6.  **Push and Open a Pull Request**  
    Push your branch to your fork, then open a PR to the main repository.  
    Mention the related task number in your PR description (e.g., “Fixes Task #5”).
    
7.  **Code Review**  
    Be open to feedback and make updates if requested.
    

