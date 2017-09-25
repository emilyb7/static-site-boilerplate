## Static site boilerplate

This is a boilerplate for making simple multi-page websites with static content.

I'm using pug for templating, and building using gulp.

CSS is done (mostly) with tachyons.

Linter + prettier already set up.

### How to use

- Clone this repo, remove git history and rename
- Ensure you have Gulp and ESlint installed globally
- `npm install`
- Run `gulp watch` to spin up a local dev server and watch for changes

All changes to files, styling, content etc. need to be made within the `/src` directory.

Gulp watches for changes to templates and CSS, but not new images or fonts. So if adding new images you need to `gulp clean && gulp build`.

To build for production run `gulp build`.

This is ideal for hosting on github pages or similar.


### Things to improve

- Prevent dev server from crashing whenever pug process throws an error
- Be able to view files in the browser with or without their `.html` extension
- Better way of rebuilding tachyons files
- Better linting for pug
