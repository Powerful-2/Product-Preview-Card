# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)


### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## 1. The Development Process

To ensure a high-end "luxury" look, I followed a Mobile-First workflow:
Deconstruction: I analyzed the Figma design to identify the "Auto Layout" containers (Image vs. Content).

Semantic HTML: I built a clean structure using <main> for the card, <img> for responsive images, and <article> for the product details.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

- Global Styling: Set up CSS variables for the signature "Dark Cyan" (#3D8168) and "Cream" (#F2EAE2) backgrounds.
- Layout Engine: Used Flexbox on the body to keep the card perfectly centered and Media Queries to switch from a vertical stack (Mobile) to a horizontal row (Desktop).

### What I Learned
- Figma-to-Code Translation: I mastered converting Figma "Auto Layout" properties like gap: 24px and padding: 32px into precise CSS.
- Responsive Images: Implemented the <img> element to automatically swap the portrait mobile image for the landscape desktop version.
- Typography Hierarchy: Learned how to use Fraunces (700 weight) and Montserrat (500/700) with specific letter-spacing (5px) to achieve a premium brand aesthetic.
- Box Model Mastery: Used box-sizing: border-box to ensure padding didn't break the card's fixed dimensions (350px mobile / 600px desktop).


To see how you can add code snippets, see below:
```html
<h1>Some HTML code I'm proud of</h1>
<main class="card-container">
  <div class="card-image">
    <picture>
      <source srcset="images/image-product-desktop.jpg" media="(min-width: 600px)">
      <img src="images/image-product-mobile.jpg" alt="Gabrielle Essence Perfume">
    </picture>
  </div>
  <article class="card-content">
    <div class="title-container">
      <p class="category-label">Perfume</p>
      <h1 class="product-title">Gabrielle Essence Eau De Parfum</h1>
      <p class="description">A floral, solar and voluptuous interpretation...</p>
    </div>
  </article>
</main>

```css
proud-of-this-css:
<!-- /* Mobile */ -->
.card-container {
    display: flex;
    flex-direction: column;
    width: 350px;
}

<!-- /* Desktop Side-by-Side */ -->
@media (min-width: 600px) {
    .card-container {
        flex-direction: row;
        width: 600px;
        height: 450px;
    }
}

```JS
-- I will add Javascripts to this projects once I have learnt enough, and I have the confidents to do JS projects. 

<!-- ### Future Project Strategy -->
For my next projects, I will continue to:
- Map out the Box Model before writing a single line of code.
- Stick to Semantic Tags for better SEO and Accessibility (Aria-labels).
- Use Relative Units (like 100vh and rem) to ensure the design scales on all monitor sizes.

<!-- ### Useful resources -->
- CSS-Tricks Guide to Flexbox - Essential for centering the component.
- MDN Docs on the Picture Element - Helped me understand how to swap desktop and mobile assets.
- Anima Blog: Figma to Web - Explained how to translate absolute positions into flex containers.

<!-- ## Author -->
- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - (https://www.frontendmentor.io/profile/Powerful-2)
- Twitter - (https://x.com/Koolprince0)

<!-- ## Acknowledgments -->
- I want to thank Bro. Tobi, who supported me with internet connection and also guided me in using MDN docs and CSS tricks for Flexbox to build my project. 

- The use of Claude & ChatGPT to guide me on how to read my Figma measurements.