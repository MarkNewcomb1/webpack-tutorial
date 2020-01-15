# webpack-tutorial
getting started with webpack

## What's happening
Instead of referencing lodash in a script tag in the head of the
HTML document, and then referencing another script in the bottom of the body tag,
using webpack allows you to use import/export statements of your dependencies 
(and convert them to older-than-ES6) and then spit out one single js file. 

Where this file is output is dependent on your `webpack.config.js` file, which also
determines where the "entry point" is (which js file to call first, which then calls perhaps other files in a project).
It also determines the directory of the output - in this case, 'dist'.

From there, we can either use the webpack cli by typing `npx webpack` or leverage
our package.json and include a script. In the script:

```
 "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "build": "webpack"
  },
```

'build' means 'webpack' - so when we type `npm run build`, it's short for
`npm run webpack` - which is usually a longer command line. 

### Conclusion

Webpack is a module bundler - you can have modules and webpack will make a dependency graph
of these and spit out a single js file. 

