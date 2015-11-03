# Vue Starter Template

A work in progress. Still learning.

## Instructions

1. `npm install`
1. `npm run dev`

## Has

* Myth CSS preprocessor
* Babel
* Bootstrap (TODO: fix this)
* jQuery (TODO: possibly remove this)

## Reference

Useful commands for reference:

* Build once: `browserify -t vueify -e src/jsmain.js -o static/build/bundle.js`
* Or watch: `watchify src/js/main.js -t vueify -e -o '> static/build/bundle.js' -v`
* With compression: `watchify src/js/main.js -t vueify -e -o 'uglifyjs -cm > static/build/bundle.js' -v`
* `npm run dev` does: `watchify -vd -p browserify-hmr -t vueify -e src/js/main.js -o static/build/bundle.js & http-server -c 1 -a localhost`
* `npm run build` does: `NODE_ENV=production ./node_modules/watchify/node_modules/.bin/browserify -t vueify -e src/js/main.js | uglifyjs -c warnings=false -m > static/build/bundle.js`
