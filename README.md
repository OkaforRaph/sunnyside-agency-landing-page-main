# Frontend Mentor - Sunnyside agency landing page solution

This is a solution to the [Sunnyside agency landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/sunnyside-agency-landing-page-7yVs3B6ef). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![](./design/desktop-preview.jpg)

### Links

- Solution URL: [https://github.com/OkaforRaph/sunnyside-agency-landing-page-main.git](https://github.com/OkaforRaph/sunnyside-agency-landing-page-main.git)
- Live Site URL: [https://okaforraph.github.io/sunnyside-agency-landing-page-main/](https://okaforraph.github.io/sunnyside-agency-landing-page-main/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Desktop first workflow
- CSS Absolute positioning

### What I learned

I really challenged myself to get the header/ Hero section right... Tried all to make the Hero look exactly like the design, so i ended up using absolute positioning... Really enjoyed the challenge tho

```html
<header class="header">
	<a href="#">
		<img src="./images/logo.svg" alt="Sunnyside logo" class="logo" />
	</a>

	<nav class="main-nav">
		<ul class="main-nav-list">
			<li><a class="main-nav-link" href="#">About</a></li>
			<li><a class="main-nav-link" href="#">Services</a></li>
			<li><a class="main-nav-link" href="#">Projects</a></li>
			<li><a class="main-nav-link nav-cta" href="#cta">Contact</a></li>
		</ul>
	</nav>

	<!-- Mobile menu  -->
	<button class="btn-mobile-nav">
		<ion-icon class="icon-mobile-nav" name="menu-outline"></ion-icon>
		<ion-icon class="icon-mobile-nav" name="close-outline"></ion-icon>
	</button>
</header>
```

```css
.header {
	display: flex;
	justify-content: space-between;
	align-items: center;
	padding: 2.4rem 4.8rem;

	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	z-index: 20;
}

.main-nav-list {
	list-style: none;
	display: flex;
	align-items: center;
	gap: 4.8rem;
}

.main-nav-link:link,
.main-nav-link:visited {
	display: inline-block;
	text-decoration: none;
	color: var(--White);
	font-weight: 500;
	transition: all 0.3s;
}

.main-nav-link.nav-cta:link,
.main-nav-link.nav-cta:visited {
	padding: 1.2rem 2.4rem;
	border-radius: 9px;
	color: var(--Very-dark-grayish-blue);
	background-color: var(--White);
	text-transform: uppercase;
	font-family: "Fraunces", serif;
	font-size: 1.6rem;
	font-weight: 700;
}

.main-nav-link.nav-cta:hover,
.main-nav-link.nav-cta:active {
	background-color: #63b8e2;
	color: var(--White);
}
```

### Continued development

I will continue to learn how to integrate Javascript to websites to make it more functional

### Useful resources

- [Example resource 1](https://www.youtube.com/kepowob) - Found Kevin Powell's videos helpful when using absolute positioning.
- [Example resource 2](https://github.com/codewithsadee/) - I also found this Github repository helpful.

## Author

- LinkedIn - [Okafor Raphael](https://www.linkedin.com/in/okafor-raphael-6b29a017b/)
- Frontend Mentor - [@OkaforRaph](https://www.frontendmentor.io/profile/OkaforRaph)
- Twitter - [@RaphOkafor\_](https://www.twitter.com/Raphokafor_)
