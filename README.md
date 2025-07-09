[![deploy](https://github.com/wexcommerce/wexcommerce.github.io/actions/workflows/deploy.yml/badge.svg)](https://github.com/wexcommerce/wexcommerce.github.io/actions/workflows/deploy.yml) [![lighthouse](https://github.com/wexcommerce/wexcommerce.github.io/actions/workflows/lighthouse.yml/badge.svg)](https://github.com/wexcommerce/wexcommerce.github.io/actions/workflows/lighthouse.yml)

# wexCommerce Website

This repository contains the source code for the [wexCommerce](https://wexcommerce.github.io/) official landing page.

The website is built using [Vite](https://vitejs.dev/) with plain HTML, CSS, and JavaScript.

## About

wexCommerce is an open-source and cross-platform single-vendor marketplace offering an SEO-optimized web storefront and a powerful admin panel for managing your online store.  

This website presents the main features, demo, support, and contact sections to introduce wexCommerce to users and developers.

## Features

- Multilingual support (English, French, Spanish, Portuguese, Japanese, Chinese)
- Responsive and accessible design  
- Language switcher and dark mode toggle  
- Demo links and contact form integration  
- Simple, clean, and modern UI built with Vite

## Separation of Concerns (SoC)

Each file/module has a single responsibility, helping keep the codebase clean and maintainable:

| File / Module        | Responsibility (Concern)                                      | Description                                                                 |
|----------------------|---------------------------------------------------------------|-----------------------------------------------------------------------------|
| `index.html`         | Structure / Content                                           | Defines the HTML structure and semantic layout of the page.                |
| `style.css`          | Presentation (Styling)                                        | Handles layout, colors, fonts, and responsive design using CSS.            |
| `i18n.js`            | Internationalization (i18n)                                   | Manages language loading, switching, and translation key resolution.       |
| `ui.js`              | UI Behavior / Interactivity                                   | Manages dynamic UI features like header/footer loading, scroll effects, hamburger menu, theme toggle, etc. |
| `main.js`            | Application Initialization / Coordination                     | Initializes the app, connects modules together, and runs on DOM ready.     |
| `vite.config.js`     | Build Tool Configuration                                      | Configures how files are served and built using Vite.                      |
| `public/` folder     | Static Assets                                                 | Contains images, icons, and static resources directly served as-is.        |

By keeping each concern isolated in its own file, the project becomes easier to understand, test, and extend.

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v14+ recommended)  
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)

### Installation

Clone the repository:

```bash
git clone https://github.com/aelassas/wexcommerce.github.io.git
cd wexcommerce.github.io
```

Install dependencies:

```bash
npm install
```

### Development

Start the local development server with hot module replacement:

```bash
npm run dev
```

### Build

Build the static site for production:

```bash
npm run build
```

The built files will be in the dist folder, ready to be deployed.

### Preview Production Build

To preview the production build locally:

```bash
npm run preview
```

## Deployment

This project is configured to be deployed on [GitHub Pages](https://pages.github.com/).

After building, push the `dist` contents to the gh-pages branch or use GitHub Actions for automated deployment.

## Contributing

Contributions and suggestions are welcome. Feel free to open issues or pull requests.

Please keep changes focused and provide clear descriptions.

## License

This project is licensed under the MIT License.

## Links

* [wexCommerce GitHub](https://github.com/aelassas/wexcommerce)
* [wexCommerce Live Demo](https://wexcommerce.github.io/#demo)
* [Documentation](https://github.com/aelassas/wexcommerce/wiki)
