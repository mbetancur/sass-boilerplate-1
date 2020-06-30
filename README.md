# Sass Boilerplate

## Sass Case Study
### Use of the 7-1 architecture pattern boilerplate in order to improve my Sass skills.
#### check ``` index.html ``` to see improved topics 

## My particular use:

### Npm sass compiler and server

```bash
npm install live-server
npm install node-sass
```
### Scripts for package.json

```bash
"server": "live-server"
"compile-sass": "node-sass stylesheets/main.scss main.css",
"compile-sass-w": "node-sass stylesheets/main.scss main.css  --watch",
```
------

This is a sample project using the [7-1 architecture pattern](http://sass-guidelin.es/#architecture) and sticking to [Sass Guidelines](http://sass-guidelin.es) writing conventions.

Each folder of this project has its own `README.md` file to explain the purpose and add extra information. Be sure to browse the repository to see how it works.

## Using the indented syntax

### Sass conversion

This boilerplate does not provide a `.sass` version as it would be painful to maintain both versions without an appropriate build process. However, it is very easy to convert this boilerplate to Sass indented syntax.

Clone it, head into the project and then run:

```
sass-convert -F scss -T sass -i -R ./  && find . -iname “*.scss” -exec bash -c 'mv "$0" “${0%\.scss}.sass"' {} \;
```

### Use with Node-sass

When using `node-sass` - in order to build that boilerplate, one needs to:

- install `node-sass` if not yet installed:

```bash
npm install -g node-sass
```

- run build command from command line:

```bash
node-sass stylesheets/main.scss dist/main.css
```
