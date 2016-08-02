# cleverbiscuit.com

The company website for Clever Biscuit, built using [jekyllized](https://github.com/sondr3/generator-jekyllized)

# Installtion

- Add the repo to your local machine
- CD to the root folder
- Run `npm install` from terminal
- Run `bower install` from terminal

## Developing locally

Run `gulp` in terminal. This will fire up localhost and display the site. Gulp will be watching for any Jekyll/CSS/JS changes.

## Build

To create a build run `gulp build`. This will build the site in the `/dist/` folder and can be used as a dev site for debuggin.

### Build - Production

To create a build for the live site run `gulp build --prod`. This will minify CSS/JS/HTML, cache bust, optimise images, GZIP assets.

## Deploy

Run `gulp deploy` in terminal. This will push the contents of `/dist/` folder to the 'master' branch. Which will push to the live site instantly-ish.
