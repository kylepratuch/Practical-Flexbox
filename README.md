# Setup:
A quick rundown on how this workflow was setup:
## Sass:
Terminal:
  ```
  gem install Sass
  sass -v
  ```
At this point, you should setup your desired sass file structure. Mine is just an example.
Now, tell Sass to watch an input .scss to compile to an output .css:
`sass --watch scss/styles.scss:css/styles.css`

## Gulp + Autoprefixer:
New Terminal:
  ```
  npm install -g gulp
  npm install gulp --save-dev
  npm install gulp-autoprefixer --save-dev
  touch gulpfile.js
  ```
Refer to gulpfile.js for gulp setup.
Terminal:
  `gulp watch` will watch css/styles.css and output to build/styles.css, according to the task written in gulpfile.js.
