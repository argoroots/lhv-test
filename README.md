# LHV test for frontend developer

Some key points how all this is done:
- Base CSS framework is [Bootstrap](http://getbootstrap.com) - The wheel is already invented!
- HTML is written in [Jade](http://jade-lang.com) and CSS is in [Stylus](https://learnboost.github.io/stylus/) - Life is too short to write extra </> and {}.
- External frameworks are installed and managed with [Bower](http://bower.io) - A package manager for the web.
- Everything is processed, converted and minified into one index.html with [Grunt](http://gruntjs.com) -  I'm too lazy to not automate everything.

## Some development tips
First we need to install Bower, Grunt (with its components) and download web frameworks with Bower (you need [Node.js](https://nodejs.org) and npm for this). Inside project folder do some shell magic:
```
npm install -g grunt-cli bower
npm install
bower install
```

To build index.html use the following shell command:
```
grunt build
```

Grunt can also track file changes, automatically rebuild index.html and serve this site in [localhost:4000](). All for dead easy development. Just use the following shell command:
```
grunt
```
