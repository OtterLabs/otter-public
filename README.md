# Otter #

This is a lightweight custom website template, built for Otter. It uses the Landkit theme by GoodThemes with custom additions for increased speed and better SEO searchability.

For docs, visit http://landkit.goodthemes.co/docs/index.html.

### Get Started ###

To get started, follow the instructions below:

1. Make sure you have Node installed since Landkit uses npm to manage dependencies.
3. Run `npm install gulp-cli -g`: If you don't have the Gulp command line interface, you need to install it.
4. Run `npm install`: Open your command line to the root directory of your unzipped theme and run to install all of Landkit's dependencies.

### File Includes ###

The `gulp-file-include` package is used to make partials easier to use for initial development (on your Node server) before you deploy the HTML. We will use these to make components around the site and optimize for SEO purposes and general architecture. Easily create new `.html` partials inside the `/partials` folder and point to them from any file by specifying the path to the partial file and using the `@@include` keyword.

*Header*: `@@include("partials/header.html")`\
*Navbar*: `@@include("partials/navbar.html")`\
*Footer*: `@@include("partials/footer.html")`

You can also pass parameters to the partials, but this will be deployed as static HTML (not dynamic).

`@@include("partials/head.html",{"type": "website"})`

### Compiling ###

Gulp is used to manage Landkit development. For docs on Gulp, visit https://gulpjs.com.

Open your command line to the root directory of the theme to use the following commands:

1. `gulp`: Compile and watch the SCSS/JS/HTML, use Live Reload to update browsers instantly, start a server, and pop a tab in your default browser. Any changes made to the source files will be compiled as soon as you save the file.
2. `gulp build`: Generates a /dist directory with all the production files.

### Javascript ###

The following Javascript packages are pre-installed:

1. Bootstrap https://getbootstrap.com/docs
2. JQuery: https://api.jquery.com/

### Styling ###

The following CSS packages are pre-installed:

1. Tachyons: https://tachyons.io/docs/
2. FontAwesome: https://fontawesome.com/icons

### Fonts ###

The following open-source fonts are pre-installed:

2. Feather: `fonts/Feather`\
2. HK Grotesk Pro: `fonts/HK%20Grotesk%20Pro`

For custom CSS, you can use the default files below or create your own and reference them in `/partials/head.html`.

1. Theme: `css/theme.css`
2. Custom: `css/custom.css`

### Deployment ###

Once you've compiled, point your server to `docs/docs/index.html` or `docs/docs/index.html`.

### Support ###

For support go to hireotter.com or email kyle@hireotter.com.