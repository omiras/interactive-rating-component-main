# Frontend Mentor - Interactive rating component solution using TailWind CSS

This is a solution to the [Interactive rating component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/interactive-rating-component-koxpeBUmI). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I liked about Tailwind](#What-I-liked-about-using-Tailwind-😊)
  - [Continued development](#What-I-did-NOT-like-about-using-Tailwind-😢)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the app depending on their device's screen size
- See hover states for all interactive elements on the page
- Select and submit a number rating
- See the "Thank you" card state after submitting a rating

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## Built with

- Tailwind CSS
- Custom Tailwind classes
- Flexbox
- Mobile-first workflow

## Why Tailwind

I wanted to use Tailwind for a simple component and use some of his features such as custom classes using the [`@apply`](https://tailwindcss.com/docs/reusing-styles#extracting-classes-with-apply) directive.

### What I liked about using Tailwind 😊

- I love using Tailwind to teach CSS to my students. It really forces you to understand deeply CSS instead of just relying on a CSS framework (which is not a bad thing at all!)
- The relative units of Tailwind (p-1, p-2) lets you you to build things around relative mesures. For people who is not a designer, it really helps to think this way: "I need something closer to that other thing" rather than "the elements in this flex container should be splitted with a gap of exactly **7 px**.
- You can configure your default styles and custom colors in **talwind.config.js**

### What I did NOT like about using Tailwind 😢

- To be honest, the section title should be "What I did not like about Tailwind in **this project**
- Yeah, it's kind overkill to use custom configuration (tailwind.config.js) in this project. I could have use very similar colors or [arbitrary values](https://tailwindcss.com/docs/adding-custom-styles#using-arbitrary-values).
- Tailwind is really component focused. It encourages you to [extract components](https://tailwindcss.com/docs/reusing-styles#extracting-components-and-partials) rather than using the `@apply` directive. That's why it fits really well for frameworks such as React or Vue, but for this project. I ended up copying to many classes (luckly, [multi-cursor helped](https://tailwindcss.com/docs/reusing-styles#multi-cursor-editing)).

```
          class="bg-primary py-2 px-4  hover:cursor-pointer hover:bg-medium-grey hover:text-black hover:font-bold"
          data-rating="1">1</span> <span
          class="bg-primary py-2 px-4 hover:cursor-pointer hover:bg-medium-grey hover:text-black hover:font-bold"
          data-rating="2">2</span> <span
          class="bg-primary py-2 px-4 hover:cursor-pointer hover:bg-medium-grey hover:text-black hover:font-bold"
          data-rating="3">3</span>
```

### How to compile and modify this project

1. You will need to [install Talwind](https://tailwindcss.com/docs/installation)
2. Then just execute:

```
npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```

**Importat note on using Tailwind for Front End Mentor Challanges**

Be sure to modify **tailwind.config.js** so it takes into account **index.html** file to recompile src/input.css

```
module.exports = {
  content: ["./src/**/*.{html,js}", "index.html"],
```

### Useful resources

- [Install and compile Tailwind](https://tailwindcss.com/docs/installation) - Just follow the steps to install properly Tailwind and also to be able to modify tailwind.config.js.
- [Extracting classes using @apply](hhttps://tailwindcss.com/docs/reusing-styles#extracting-classes-with-apply) - I created a custom class `bg-primary`

## Author

- [GitHub](https://github.com/omiras)
- [@Frontend Mentor profile](https://www.frontendmentor.io/profile/omiras)
- [Linkedin](https://www.linkedin.com/in/mirasortiz/)
