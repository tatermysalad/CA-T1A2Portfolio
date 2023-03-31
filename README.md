# T1A2 - Project: Plan and Develop a Portfolio Website

## Links

-   [Portfolio website](https://edoughertyportfolio.netlify.app)
-   [GitHub repo](https://github.com/tatermysalad/T1A2Portfolio)
-   [Presentation](https://youtube.com)

## Purpose

This is a portfolio website for displaying myself as a developer and IT professional. I have listed my skills, interests, professional knowledge and showcase of my abilities with HTML and CSS.

## Functionality/ features

### Every viewport:

-   Scalable elements using clamp, min/max, vw/vh, percentages, and rem values for text.
-   Animations on each page for fluid look and feel
-   Blog features grid which resizes on viewport

```scss
.blog-parent {
            display: grid;
            gap: 1.5rem;
            grid-auto-columns: 1fr;
            grid-template-areas:
                "one"
                "two"
                "three"
                "four"
                "five";
            @media screen and (min-width: $medium) {
                grid-template-areas:
                    "two two"
                    "one three"
                    "four three"
                    "five five";
            }
            @media screen and (min-width: $large) {
                grid-template-areas:
                    "two two one three"
                    "five four four three";
            }
```

-   Home page words 'Ed', 'simplicity','design' and 'function' change with mouse hover (not as noticable on phones with no mouse though)

```scss
.about-me-sub {
    /* Changes the headings for specific words to show user they are links */
    font-family: $heading;
    font-size: 2rem;
    text-decoration: none;
    color: black;
    &:hover {
        text-shadow: 2px 2px black;
        color: white;
    }
}
```

### Small/ mobile views:

-   'Hamburger' menu
    -   Menu slides in from the right of the screen checkbox which triggers
    ```scss
     {
        transform: translateX(-100vw);
    }
    ```
    -   Font and heading changes for each page to let user know which page they are on.

### Medium/ tablet view and Large/ Desktop view

-   Always visible header
-   The social media elements are based on the footer
    -   To the left for medium
    -   Centre for large/desktop.

## Sitemap

The following is a png file created on [draw.io](https://draw.io)
![Site Map](./docs/Site%20Map.png)

## Screenshots

### Below are screenshots of the Small/ Mobile viewport

![Home Page Small Home View](./docs/Small%20-%20Home.png)
![Home Page Small Home Menu View](./docs/Small%20-%20Home%20Menu.png)
![Home Page Small About View](./docs/Small%20-%20About.png)
![Home Page Small About Menu View](./docs/Small%20-%20About%20Menu.png)
![Home Page Small Blog View](./docs/Small%20-%20Blog.png)
![Home Page Small Blog Menu View](./docs/Small%20-%20Blog%20Menu.png)
![Home Page Small Contact View](./docs/Small%20-%20Contact.png)
![Home Page Small Contact Menu View](./docs/Small%20-%20Contact%20Menu.png)

### Below are screenshots of the Medium/ Tablet viewport

![Home Page Medium Home View](./docs/Medium%20-%20Home.png)
![Home Page Medium About View](./docs/Medium%20-%20About.png)
![Home Page Medium Blog View](./docs/Medium%20-%20Blog.png)
![Home Page Medium Contact View](./docs/Medium%20-%20Contact.png)

### Below are screenshots of the Large/ Desktop viewport

![Home Page Large Home View](./docs/Large%20-%20Home.png)
![Home Page Large About View](./docs/Large%20-%20About.png)
![Home Page Large Blog View](./docs/Large%20-%20Blog.png)
![Home Page Large Contact View](./docs/Large%20-%20Contact.png)

## Target Audience

The target audience of this portfolio is anyone who is interested in learning about myself, including my skills and what my interests are through my blog entries.

## Tech Stack

-   Sitemap created from [draw.io](https://draw.io)
-   Site plan created on [figma.com](https://www.figma.com/file/UKrFoOnXShVvHg3sVTMrJC/Portfolio-Website?node-id=14%3A395&t=FxBhUNpIrxp7jS8J-1)
-   Colour palette 'Rosettes and Cream' from [canva.com](https://www.canva.com/colors/color-palettes/rosettes-and-cream/)
-   Colour contrast checked on [webaim.org](https://webaim.org/resources/contrastchecker/)
-   HTML
-   CSS
    -   SCSS
-   Netlify
-   Written with Visual Studio Code
